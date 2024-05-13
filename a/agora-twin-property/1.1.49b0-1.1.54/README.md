# Comparing `tmp/agora_twin_property-1.1.49b0-py2.py3-none-any.whl.zip` & `tmp/agora_twin_property-1.1.54-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,10 @@
-Zip file size: 3819 bytes, number of entries: 7
--rw-r--r--  2.0 fat       39 b- defN 24-Mar-12 15:43 agora_twin_property/__init__.py
--rw-r--r--  2.0 fat     6879 b- defN 24-Mar-12 15:43 agora_twin_property/twin_property.py
--rw-r--r--  2.0 fat       27 b- defN 24-Mar-13 18:40 agora_twin_property/version.py
--rw-r--r--  2.0 fat      131 b- defN 24-Mar-12 15:43 agora_twin_property-1.1.49b0.dist-info/LICENSE
--rw-r--r--  2.0 fat       99 b- defN 16-Jan-01 00:00 agora_twin_property-1.1.49b0.dist-info/WHEEL
--rw-r--r--  2.0 fat      846 b- defN 16-Jan-01 00:00 agora_twin_property-1.1.49b0.dist-info/METADATA
--rw-r--r--  2.0 fat      616 b- defN 16-Jan-01 00:00 agora_twin_property-1.1.49b0.dist-info/RECORD
-7 files, 8637 bytes uncompressed, 2707 bytes compressed:  68.7%
+Zip file size: 4838 bytes, number of entries: 8
+-rw-r--r--  2.0 fat       31 b- defN 24-May-13 16:50 agora_twin_property/__init__.py
+-rw-r--r--  2.0 fat     7931 b- defN 24-May-13 16:50 agora_twin_property/twin_property.py
+-rw-r--r--  2.0 fat     2092 b- defN 24-May-13 16:50 agora_twin_property/twin_property_observer.py
+-rw-r--r--  2.0 fat       25 b- defN 24-May-13 17:00 agora_twin_property/version.py
+-rw-r--r--  2.0 fat      131 b- defN 24-May-13 16:50 agora_twin_property-1.1.54.dist-info/LICENSE
+-rw-r--r--  2.0 fat       99 b- defN 16-Jan-01 00:00 agora_twin_property-1.1.54.dist-info/WHEEL
+-rw-r--r--  2.0 fat      893 b- defN 16-Jan-01 00:00 agora_twin_property-1.1.54.dist-info/METADATA
+-rw-r--r--  2.0 fat      710 b- defN 16-Jan-01 00:00 agora_twin_property-1.1.54.dist-info/RECORD
+8 files, 11912 bytes uncompressed, 3576 bytes compressed:  70.0%
```

## zipnote {}

```diff
@@ -1,22 +1,25 @@
 Filename: agora_twin_property/__init__.py
 Comment: 
 
 Filename: agora_twin_property/twin_property.py
 Comment: 
 
+Filename: agora_twin_property/twin_property_observer.py
+Comment: 
+
 Filename: agora_twin_property/version.py
 Comment: 
 
-Filename: agora_twin_property-1.1.49b0.dist-info/LICENSE
+Filename: agora_twin_property-1.1.54.dist-info/LICENSE
 Comment: 
 
-Filename: agora_twin_property-1.1.49b0.dist-info/WHEEL
+Filename: agora_twin_property-1.1.54.dist-info/WHEEL
 Comment: 
 
-Filename: agora_twin_property-1.1.49b0.dist-info/METADATA
+Filename: agora_twin_property-1.1.54.dist-info/METADATA
 Comment: 
 
-Filename: agora_twin_property-1.1.49b0.dist-info/RECORD
+Filename: agora_twin_property-1.1.54.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## agora_twin_property/__init__.py

```diff
@@ -1 +1 @@
-from .twin_property import TwinProperty
+from .twin_property import Twin
```

## agora_twin_property/twin_property.py

```diff
@@ -1,123 +1,121 @@
 from agora_redis_client import redis
 from agora_logging import logger
 from agora_config import config
+from .twin_property_observer import TwinPropertyObserver
 from enum import Enum
 
 class RedisPattern(Enum):
     DESIRED = "desired"
-    REPORTED = "reported"    
+    REPORTED = "reported" 
 
 class TwinPropertySingleton(): 
     _instance = None
 
     def __init__(self) -> None:
-        self.__sub_devices = dict()
+        super().__init__()
+        if not redis.is_connected():
+            redis.connect()
+        self.pubsub = redis.pubsub()
+        redis.config_set('notify-keyspace-events', 'KEA')
         self.__sleep_time = 0.01
-
+        self.observer_callbacks = {}    
+        self.__twin_property_running = 0
+ 
+            
     def __new__(cls, *args, **kwargs):
         if not cls._instance:
             cls._instance = super().__new__(cls, *args, **kwargs)
-        return cls._instance
+        return cls._instance     
 
-    class __Device:
-        def __init__(self, tp_id,  pattern, callback_method): 
-            self.tp_id = tp_id
-            self.pattern = pattern
-            self.callback_method = callback_method
-
-    class CallbackResponse(__Device):
-        def __init__(self, tp_id, key, value):
-            self.tp_id = tp_id
-            self.key = key
-            self.value = value
-
-    def set_property_change_callback(self, method_to_callback:any, tp_ids:list=None):
-        try:
-            self.__clear_all_device()
-            if not callable(method_to_callback):
-                raise TypeError("Required Call-back method")
-                    
-            if tp_ids is None:
-                device_id = get_device_id()
-                tp_ids = [device_id]
-            
-            for device_id in tp_ids:
-                pattern = f"twin_properties/{device_id}/{RedisPattern.DESIRED.value}/"
-                obj_device = self.__Device(tp_id = str(device_id), pattern = pattern, callback_method = method_to_callback)
-                self.__sub_devices[str(device_id)] = obj_device
-                self.__subscribe_patterns(obj_device)
+    def observe(self, app_callback: callable, tp_group_id: str, property_name :str = None) -> None:    
+        """
+        Create Observable and add to list and start the subscription to the pattern
+        """    
+        if tp_group_id is None: raise ValueError("tp_group_id cannot be None")
+        if not callable(app_callback): raise TypeError("app_callback is not callable method")
+        if tp_group_id not in self.observer_callbacks:
+            observer = TwinPropertyObserver(tp_group_id,property_name)
+            observer.attach(app_callback)
+            self.__add_observer(observer,None)    
+        else:
+            callbacks = self.observer_callbacks[tp_group_id]
+            if property_name not in callbacks:
+                observer = TwinPropertyObserver(tp_group_id,property_name)
+                observer.attach(app_callback)
+                self.__add_observer(observer,callbacks)
+            else:
+                logger.warn(f"Duplicate request for subscription to same group{tp_group_id} and property {property_name}")
+
+    def stop_observe(self, tp_group_id: str, property_name :str = None) -> None:        
+        if tp_group_id is None: raise ValueError("tp_group_id cannot be None")
+        if property_name is None: property_name = "*"
+        if tp_group_id in self.observer_callbacks and property_name in self.observer_callbacks[tp_group_id]:
+            self.__remove_observer(tp_group_id,property_name)                
+        else:
+            logger.info(f"No Observer found for the group {tp_group_id}, property{property_name}")
                 
+    def __add_observer(self, observer: TwinPropertyObserver, callbacks:dict=None):
+        """
+        Add Observable to dictionary and start subscription
+        """
+        if callbacks is None: 
+            callbacks = {}
+        callbacks[observer.property_name] = observer
+        self.observer_callbacks[observer.tp_id] = callbacks
+        self.__subscribe_patterns(observer)
+      
+    def __remove_observer(self, tp_group_id:str,property_name:str = None):
+        """
+        Remove Observable from dictionary and stop subscription
+        """        
+        observer = self.observer_callbacks[tp_group_id][property_name]
+        self.__unsubscribe_patterns(observer)        
+        del self.observer_callbacks[tp_group_id][property_name]
+        
+        
+    def __subscribe_patterns(self, observer:TwinPropertyObserver):
+        """
+        Subscribe to pattern in Redis
+        """
+        try:            
+            self.pubsub.psubscribe(**{"__key*__:"+ observer.pattern : observer.subscription_callback})
+            if not self.__twin_property_running :
+                self.pubsub.run_in_thread(sleep_time=float(self.__sleep_time))
+                self.__twin_property_running = 1
+            logger.info("Running : {0} redis event subscriber ...".format(observer.pattern))
+        except Exception as error:
+            logger.exception(error, "Error while suscribing to pattern {0} ".format(observer.pattern))
+
+    def __unsubscribe_patterns(self, observer:TwinPropertyObserver):
+        """
+        Unsubscribe pattern in Redis
+        """
+        try:               
+            self.pubsub.punsubscribe("__key*__:"+ observer.pattern ) 
+            logger.info(" {0} twin property unsubscribe ...".format(observer.pattern))
         except Exception as error:
-            logger.exception(error, "Error while set property change callback ")
-
-        return self.__sub_devices    
-
-    def __clear_all_device(self):
-        self.__sub_devices.clear()
-
-    def __subscribe_patterns(self, device:__Device):
-        try:
-            if not redis.is_connected():
-                redis.connect()
-
-            pubsub = redis.pubsub()
-            redis.config_set('notify-keyspace-events', 'KEA')
-            pubsub.psubscribe(**{"__key*__:"+ device.pattern +"*": self.__subscription_callback})
-            pubsub.run_in_thread(sleep_time=float(self.__sleep_time))
-
-            logger.info("Running : {0} redis event subscriber ...".format(device.pattern))
-
-
-        except Exception as error:
-            logger.exception(error, "Error while suscribing to pattern {0} ".format(device.pattern))
-
-    def __subscription_callback(self, msg):
-        try:
-            channel = msg["channel"]
-            keys = channel.split(":")
-            prop_value = redis.get(keys[1])
-            logger.debug(f"Desired Key : {keys[1]}, value : {prop_value}")
-            prop = str(keys[1]).split(sep="/")
-            prop_name_value = str(keys[1]).split(sep=f"/{RedisPattern.DESIRED.value}/")
-            device_id= prop[1]
-            prop_name =  prop_name_value[1].rstrip("/") if len(prop_name_value) > 0 else ''
-            is_valid, error = is_valid_prop_name(prop_name)
-            if (is_valid == False): raise error
-
-            is_valid, error = is_valid_prop_value(prop_value)
-            if (is_valid == False): raise error
-
-
-            robj =  self.CallbackResponse(
-                tp_id= device_id,
-                key= prop_name,
-                value= prop_value
-            )
-
-            obj_device = self.__sub_devices.get(device_id)
-            obj_device.callback_method(robj)
-
-        except Exception as error:
-            logger.exception(error, "Error while executing callback method")
-        return None
+            logger.exception(error, "Error while unsubscriber to pattern {0} ".format(observer.pattern))
     
     @staticmethod
-    def set_reported_property( prop_name:str, prop_value:any, tp_id =None):
+    def set_reported_property( prop_name:str, prop_value:any, tp_group_id):
+        """
+        Set reported property in Redis key 'set twin_properties/{tp_group_id}/reported/{propname} {propvalue}'
+        """
         try:
-            if tp_id is None : tp_id = get_device_id()
+            if tp_group_id is None : raise AttributeError("Error 'tp_group_id' cannot be null")
             
             is_valid, error = is_valid_prop_name(prop_name)
             if (is_valid == False): raise error
 
             if prop_value is None:
                 raise ValueError("Property Value is not set")
 
-            key = f'twin_properties/{tp_id}/{RedisPattern.REPORTED.value}/{prop_name}'
-            appname = f"twin_properties/{tp_id}/reported/__appname"
+            key = f'twin_properties/{tp_group_id}/{RedisPattern.REPORTED.value}/{prop_name}'
+            appname = f"twin_properties/{tp_group_id}/reported/__appname"
             if not redis.is_connected():
                redis.connect()            
             if type(prop_value) ==bool:
                 if prop_value:
                      prop_value = "1"
                 else:
                     prop_value = "0"
@@ -126,68 +124,69 @@
             redis.set(key, prop_value)
             
 
         except Exception as error:
             logger.exception(error, 'Exception occurred while setting the set reported property')
             
     @staticmethod        
-    def get_desired_property(prop_name:str, tp_id = None):
+    def get_desired_property(prop_name:str, tp_group_id:str):
+        """
+        Get desired property in Redis key 'get twin_properties/{tp_group_id}/desired/{propname}'
+        """
         try:
-            if tp_id is None : tp_id = get_device_id()
+            if tp_group_id is None : raise AttributeError("Error 'tp_group_id' cannot be null")
             
             is_valid, error = is_valid_prop_name(prop_name)
             if (is_valid == False): raise error            
 
-            key = f'twin_properties/{tp_id}/{RedisPattern.DESIRED.value}/{prop_name}'
+            key = f'twin_properties/{tp_group_id}/{RedisPattern.DESIRED.value}/{prop_name}'
 
             if not redis.is_connected():
                redis.connect()            
 
             if redis.exists(key) <= 0:
                 logger.info("Property Name - {} does not exists".format(key))
 
             return redis.get(key)
 
         except Exception as error:
             logger.exception(error, 'Exception occurred while setting the get desired property')
 
     @staticmethod        
-    def get_reported_property(prop_name:str, tp_id = None):
+    def get_reported_property(prop_name:str, tp_group_id:str):
+        """
+        Get reported property in Redis key 'get twin_properties/{tp_group_id}/reported/{propname}'
+        """
         try:
-            if tp_id is None : tp_id = get_device_id()
+            if tp_group_id is None : raise AttributeError("Error 'tp_group_id' cannot be null")
 
             is_valid, error = is_valid_prop_name(prop_name)
             if (is_valid == False): raise error
 
-            key = f'twin_properties/{tp_id}/{RedisPattern.REPORTED.value}/{prop_name}'
+            key = f'twin_properties/{tp_group_id}/{RedisPattern.REPORTED.value}/{prop_name}'
 
             if not redis.is_connected():
                redis.connect()  
 
             if redis.exists(key) <= 0:
                 logger.info("Property Name - {} does not exists".format(key))
 
             return redis.get(key)
 
         except Exception as error:
             logger.exception(error, 'Exception occurred while setting the get reported property')
 
 
 @staticmethod
-def get_device_id():
-    device_id=config.get("AEA2:BusClient:DeviceId", "999")
-    return device_id
-
-@staticmethod
 def is_valid_prop_name(prop_name:str):
     if prop_name is None:
         return (False, ValueError("Property Name is not set"))
     return (True, None)       
 
 @staticmethod
 def is_valid_prop_value(prop_value:str):
     if prop_value is None:
         return (False, ValueError("Property value is not set"))
     return (True, None)       
 
 
-TwinProperty = TwinPropertySingleton()
+Twin = TwinPropertySingleton()
```

## agora_twin_property/version.py

```diff
@@ -1 +1 @@
-__version__ = '1.1.49b0'
+__version__ = '1.1.54'
```

## Comparing `agora_twin_property-1.1.49b0.dist-info/METADATA` & `agora_twin_property-1.1.54.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 Metadata-Version: 2.1
 Name: agora_twin_property
-Version: 1.1.49b0
+Version: 1.1.54
 Summary: Agora twin property for the Agora Edge Apps SDK 2.0 (Python)
 Author-email: AgoraIoT <agoraiot@slb.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Dist: agora_logging == 1.1.49b0
-Requires-Dist: agora_config == 1.1.49b0
+Requires-Dist: agora_logging == 1.1.54
+Requires-Dist: agora_config == 1.1.54
 Requires-Dist: redis
 Project-URL: Home, https://slb-edge.github.io
 
 
 # agora_twin_property
 
 This package is the twin property library for the Agora Edge Apps SDK (Python) developed by SLB.
 
 Use this SDK to construct an edge application, and then containerize it for the running on the edge with AgoraIoT.  Documentation on using the entire SDK can be found at: [AgoraIoT SDK Documentation](https://slb-edge.github.io).
 
 ## Release Notes
 
+### v1.1.53
+- Make versions of all modules the same
+
 ### v1.0.46 - Beta
 
 - Initial test release.
```

