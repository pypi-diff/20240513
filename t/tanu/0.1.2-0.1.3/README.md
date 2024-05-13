# Comparing `tmp/tanu-0.1.2.tar.gz` & `tmp/tanu-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tanu-0.1.2.tar", last modified: Sun May 12 01:51:47 2024, max compression
+gzip compressed data, was "tanu-0.1.3.tar", last modified: Mon May 13 10:25:24 2024, max compression
```

## Comparing `tanu-0.1.2.tar` & `tanu-0.1.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2024-05-12 01:51:47.824319 tanu-0.1.2/
--rw-r--r--   0 shuntaro   (501) staff       (20)    35149 2024-05-11 14:48:01.000000 tanu-0.1.2/LICENSE.txt
--rw-r--r--   0 shuntaro   (501) staff       (20)        0 2024-05-11 15:14:35.000000 tanu-0.1.2/MANIFEST.in
--rw-r--r--   0 shuntaro   (501) staff       (20)      692 2024-05-12 01:51:47.824259 tanu-0.1.2/PKG-INFO
--rw-r--r--   0 shuntaro   (501) staff       (20)      101 2024-05-11 15:12:10.000000 tanu-0.1.2/README.md
--rw-r--r--   0 shuntaro   (501) staff       (20)       94 2023-01-22 06:54:48.000000 tanu-0.1.2/pyproject.toml
--rw-r--r--   0 shuntaro   (501) staff       (20)      701 2024-05-12 01:51:47.824556 tanu-0.1.2/setup.cfg
--rw-r--r--   0 shuntaro   (501) staff       (20)       37 2022-12-09 19:04:39.000000 tanu-0.1.2/setup.py
-drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2024-05-12 01:51:47.820852 tanu-0.1.2/src/
-drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2024-05-12 01:51:47.822659 tanu-0.1.2/src/tanu/
--rw-r--r--   0 shuntaro   (501) staff       (20)       38 2024-05-11 14:04:14.000000 tanu-0.1.2/src/tanu/__init__.py
--rw-r--r--   0 shuntaro   (501) staff       (20)    17016 2024-05-12 01:51:20.000000 tanu-0.1.2/src/tanu/tanu.py
-drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2024-05-12 01:51:47.823770 tanu-0.1.2/src/tanu/utils/
--rw-r--r--   0 shuntaro   (501) staff       (20)        0 2024-05-11 15:36:56.000000 tanu-0.1.2/src/tanu/utils/__init__.py
--rw-r--r--   0 shuntaro   (501) staff       (20)     1339 2024-05-11 15:28:52.000000 tanu-0.1.2/src/tanu/utils/object_encoder_decoder.py
-drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2024-05-12 01:51:47.824053 tanu-0.1.2/src/tanu.egg-info/
--rw-r--r--   0 shuntaro   (501) staff       (20)      692 2024-05-12 01:51:47.000000 tanu-0.1.2/src/tanu.egg-info/PKG-INFO
--rw-r--r--   0 shuntaro   (501) staff       (20)      332 2024-05-12 01:51:47.000000 tanu-0.1.2/src/tanu.egg-info/SOURCES.txt
--rw-r--r--   0 shuntaro   (501) staff       (20)        1 2024-05-12 01:51:47.000000 tanu-0.1.2/src/tanu.egg-info/dependency_links.txt
--rw-r--r--   0 shuntaro   (501) staff       (20)       33 2024-05-12 01:51:47.000000 tanu-0.1.2/src/tanu.egg-info/requires.txt
--rw-r--r--   0 shuntaro   (501) staff       (20)        5 2024-05-12 01:51:47.000000 tanu-0.1.2/src/tanu.egg-info/top_level.txt
+drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2024-05-13 10:25:24.060119 tanu-0.1.3/
+-rw-r--r--   0 shuntaro   (501) staff       (20)    35149 2024-05-11 14:48:01.000000 tanu-0.1.3/LICENSE.txt
+-rw-r--r--   0 shuntaro   (501) staff       (20)        0 2024-05-11 15:14:35.000000 tanu-0.1.3/MANIFEST.in
+-rw-r--r--   0 shuntaro   (501) staff       (20)      692 2024-05-13 10:25:24.060057 tanu-0.1.3/PKG-INFO
+-rw-r--r--   0 shuntaro   (501) staff       (20)      101 2024-05-11 15:12:10.000000 tanu-0.1.3/README.md
+-rw-r--r--   0 shuntaro   (501) staff       (20)       94 2023-01-22 06:54:48.000000 tanu-0.1.3/pyproject.toml
+-rw-r--r--   0 shuntaro   (501) staff       (20)      701 2024-05-13 10:25:24.060404 tanu-0.1.3/setup.cfg
+-rw-r--r--   0 shuntaro   (501) staff       (20)       37 2022-12-09 19:04:39.000000 tanu-0.1.3/setup.py
+drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2024-05-13 10:25:24.056361 tanu-0.1.3/src/
+drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2024-05-13 10:25:24.058280 tanu-0.1.3/src/tanu/
+-rw-r--r--   0 shuntaro   (501) staff       (20)       38 2024-05-11 14:04:14.000000 tanu-0.1.3/src/tanu/__init__.py
+-rw-r--r--   0 shuntaro   (501) staff       (20)    17312 2024-05-13 10:24:40.000000 tanu-0.1.3/src/tanu/tanu.py
+drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2024-05-13 10:25:24.059406 tanu-0.1.3/src/tanu/utils/
+-rw-r--r--   0 shuntaro   (501) staff       (20)        0 2024-05-11 15:36:56.000000 tanu-0.1.3/src/tanu/utils/__init__.py
+-rw-r--r--   0 shuntaro   (501) staff       (20)     1339 2024-05-11 15:28:52.000000 tanu-0.1.3/src/tanu/utils/object_encoder_decoder.py
+drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2024-05-13 10:25:24.059810 tanu-0.1.3/src/tanu.egg-info/
+-rw-r--r--   0 shuntaro   (501) staff       (20)      692 2024-05-13 10:25:24.000000 tanu-0.1.3/src/tanu.egg-info/PKG-INFO
+-rw-r--r--   0 shuntaro   (501) staff       (20)      332 2024-05-13 10:25:24.000000 tanu-0.1.3/src/tanu.egg-info/SOURCES.txt
+-rw-r--r--   0 shuntaro   (501) staff       (20)        1 2024-05-13 10:25:24.000000 tanu-0.1.3/src/tanu.egg-info/dependency_links.txt
+-rw-r--r--   0 shuntaro   (501) staff       (20)       33 2024-05-13 10:25:24.000000 tanu-0.1.3/src/tanu.egg-info/requires.txt
+-rw-r--r--   0 shuntaro   (501) staff       (20)        5 2024-05-13 10:25:24.000000 tanu-0.1.3/src/tanu.egg-info/top_level.txt
```

### Comparing `tanu-0.1.2/LICENSE.txt` & `tanu-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tanu-0.1.2/PKG-INFO` & `tanu-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tanu
-Version: 0.1.2
+Version: 0.1.3
 Summary: Message passing between Python programs via RabbitMQ.
 Author: chocolate-icecream
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `tanu-0.1.2/setup.cfg` & `tanu-0.1.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = tanu
-version = 0.1.2
+version = 0.1.3
 author = chocolate-icecream
 description = Message passing between Python programs via RabbitMQ.
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
```

### Comparing `tanu-0.1.2/src/tanu/tanu.py` & `tanu-0.1.3/src/tanu/tanu.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,30 +89,39 @@
             keys = serialized_key.split("/")
             target_dict = getattr(letter, keys[0])
             for key in keys[1:-1]:
                 target_dict = target_dict[key]
             target_dict[keys[-1]] = decoder(target_dict[keys[-1]])
 
 class Tanuki:
-    def __init__(self, worker_name, host="localhost", port=5672, callback_func=None, accept_previous_job=True):
+    def __init__(self, worker_name, host=None, port=None, callback_func=None, accept_previous_job=True):
         """Initialize the Tanuki worker with basic configurations."""
         self.worker_name = worker_name
-        self.host = host
-        self.port = port
+        if host is None:
+            url = os.getenv("TANU_RABBITMQ_URL")
+            if len(url) == 0:
+                self.host = "localhost"
+                self.port = port if port else 5672
+            else:
+                self.host = url.split(":")[:-1]
+                self.port = port if port else 5672
+        else:
+            self.host = host
+            self.port = port if port else 5672
         self.callback_func = callback_func
         self.accept_previous_job = accept_previous_job
         self.result_queues = {}
         self.units = {}
         self.unique_identifier = self.generate_unique_identifier()
         self.prepare_task_queue()
         self.start_result_retrieve_thread()
 
     def prepare_task_queue(self):
         """Prepare the task queue by connecting to the message broker."""
-        self.task_connection = pika.BlockingConnection(pika.ConnectionParameters(self.host))
+        self.task_connection = pika.BlockingConnection(pika.ConnectionParameters(host=self.host, port=self.port))
         self.task_channel = self.task_connection.channel()
         self.task_channel.queue_declare(queue=self.task_queue_name, durable=True)
 
     def start_result_retrieve_thread(self):
         """Start a separate thread to handle result retrieval."""
         t = threading.Thread(target=self.start_consumer)
         t.daemon = True
@@ -141,15 +150,15 @@
             logger.error(f"Error processing result: {traceback.format_exc()}")
 
     def send(self, payload):
         """Send a task payload to the task queue."""
         payload = payload.copy()
         job_id = uuid.uuid4().hex
         payload["job_id"] = job_id
-        payload["units"] = self.units.copy()
+        payload["units"] = self.units
         payload["result_queue_name"] = self.result_queue_name
         payload["encoded"] = {}
         apply_encoder(payload["encoded"], payload["params"], "params")
         request = RequestLetter(**payload)
         message = request.json()
         try:
             self.task_channel.basic_publish(exchange="", routing_key=self.task_queue_name, body=message, properties=pika.BasicProperties(delivery_mode=pika.DeliveryMode.Persistent))
@@ -226,15 +235,15 @@
         while True:
             self.response = self.queue.get()
             if self.response.status in [StatusEnum.DONE, StatusEnum.ERROR]:
                 break
         del self.parent.result_queues[self.job_id]
         del self.queue
         if self.response.status == StatusEnum.ERROR:
-            raise Exception(f"Job did not complete successfully: {self.response.result['msg'] if 'msg' in self.response.result else '---'}")
+            raise Exception(self.response.result["msg"])
 
         return self.response.result
 
 class TanukiResponseConnection:
     """Manages the communication of results back to the requester."""
 
     def __init__(self, request: RequestLetter = None, units=None):
@@ -255,34 +264,34 @@
         self.connection = pika.BlockingConnection(pika.ConnectionParameters('localhost'))
         self.channel = self.connection.channel()
     
     def set_request(self, request: RequestLetter):
         """Set the request details for sending responses."""
         self.request = request
     
-    def send(self, status: StatusEnum, result: dict, _retry_count: int = 0):
+    def send(self, status: StatusEnum, result: dict):
         """Send a status update or result back to the requester."""
         assert self.request, "Request must be set before sending data."
-        try:
-            request_dict = {"command": self.request.command, "params": self.request.params}
-            encoded_dict = {}
-            apply_encoder(encoded_dict, self.request.params, "request/params")
-            apply_encoder(encoded_dict, result, "result")
-            response = ResponseLetter(job_id=self.request.job_id, status=status, request=request_dict, result=result, units=self.units)
-            message = response.json()
+        
+        request_dict = {"command": self.request.command, "params": self.request.params}
+        encoded_dict = {}
+        apply_encoder(encoded_dict, self.request.params, "request/params")
+        apply_encoder(encoded_dict, result, "result")
+        response = ResponseLetter(job_id=self.request.job_id, status=status, request=request_dict, result=result, units=self.units)
+        message = response.json()
 
+        try:
             self.channel.queue_declare(queue=self.request.result_queue_name)
             self.channel.basic_publish(exchange="", routing_key=self.request.result_queue_name, body=message)
-
         except pika.exceptions.StreamLostError:
-            if _retry_count < 1:
-                logger.warning("Stream Lost Error. Try reconnection...")
-                self.close()
-                self.connect()
-                self.send(status, result=result, _retry_count=_retry_count + 1)
+            logger.debug("Stream Lost Error. Try reconnection...")
+            self.close()
+            self.connect()
+            self.channel.queue_declare(queue=self.request.result_queue_name)
+            self.channel.basic_publish(exchange="", routing_key=self.request.result_queue_name, body=message)
 
     def send_status(self, status: StatusEnum, msg: str):
         """Send a simple status message."""
         self.send(status, {"msg": msg})
             
     def close(self):
         """Close the messaging connections gracefully."""
```

### Comparing `tanu-0.1.2/src/tanu/utils/object_encoder_decoder.py` & `tanu-0.1.3/src/tanu/utils/object_encoder_decoder.py`

 * *Files identical despite different names*

### Comparing `tanu-0.1.2/src/tanu.egg-info/PKG-INFO` & `tanu-0.1.3/src/tanu.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tanu
-Version: 0.1.2
+Version: 0.1.3
 Summary: Message passing between Python programs via RabbitMQ.
 Author: chocolate-icecream
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

