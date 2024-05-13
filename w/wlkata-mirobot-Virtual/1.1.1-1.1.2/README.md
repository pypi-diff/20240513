# Comparing `tmp/wlkata_mirobot_Virtual-1.1.1.tar.gz` & `tmp/wlkata_mirobot_Virtual-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wlkata_mirobot_Virtual-1.1.1.tar", last modified: Sun May 12 09:34:49 2024, max compression
+gzip compressed data, was "wlkata_mirobot_Virtual-1.1.2.tar", last modified: Mon May 13 01:09:17 2024, max compression
```

## Comparing `wlkata_mirobot_Virtual-1.1.1.tar` & `wlkata_mirobot_Virtual-1.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 09:34:49.053572 wlkata_mirobot_Virtual-1.1.1/
--rw-rw-rw-   0        0        0      110 2024-05-12 09:34:49.051577 wlkata_mirobot_Virtual-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      592 2024-05-11 10:00:37.000000 wlkata_mirobot_Virtual-1.1.1/license.txt
--rw-rw-rw-   0        0        0       42 2024-05-12 09:34:49.053572 wlkata_mirobot_Virtual-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0      236 2024-05-12 09:34:36.000000 wlkata_mirobot_Virtual-1.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-12 09:34:49.047588 wlkata_mirobot_Virtual-1.1.1/wlkata_mirobot_Virtual/
--rw-rw-rw-   0        0        0       83 2024-05-12 02:38:37.000000 wlkata_mirobot_Virtual-1.1.1/wlkata_mirobot_Virtual/__init__.py
--rw-rw-rw-   0        0        0    15592 2024-05-12 09:34:01.000000 wlkata_mirobot_Virtual-1.1.1/wlkata_mirobot_Virtual/wlkata_mirobot_Virtual.py
-drwxrwxrwx   0        0        0        0 2024-05-12 09:34:49.051577 wlkata_mirobot_Virtual-1.1.1/wlkata_mirobot_Virtual.egg-info/
--rw-rw-rw-   0        0        0      110 2024-05-12 09:34:48.000000 wlkata_mirobot_Virtual-1.1.1/wlkata_mirobot_Virtual.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      288 2024-05-12 09:34:48.000000 wlkata_mirobot_Virtual-1.1.1/wlkata_mirobot_Virtual.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 09:34:48.000000 wlkata_mirobot_Virtual-1.1.1/wlkata_mirobot_Virtual.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2024-05-12 09:34:48.000000 wlkata_mirobot_Virtual-1.1.1/wlkata_mirobot_Virtual.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-13 01:09:17.901435 wlkata_mirobot_Virtual-1.1.2/
+-rw-rw-rw-   0        0        0      110 2024-05-13 01:09:17.899439 wlkata_mirobot_Virtual-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      592 2024-05-11 10:00:37.000000 wlkata_mirobot_Virtual-1.1.2/license.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 01:09:17.901435 wlkata_mirobot_Virtual-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      236 2024-05-13 01:04:28.000000 wlkata_mirobot_Virtual-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 01:09:17.895450 wlkata_mirobot_Virtual-1.1.2/wlkata_mirobot_Virtual/
+-rw-rw-rw-   0        0        0       83 2024-05-12 02:38:37.000000 wlkata_mirobot_Virtual-1.1.2/wlkata_mirobot_Virtual/__init__.py
+-rw-rw-rw-   0        0        0    15615 2024-05-13 01:08:43.000000 wlkata_mirobot_Virtual-1.1.2/wlkata_mirobot_Virtual/wlkata_mirobot_Virtual.py
+drwxrwxrwx   0        0        0        0 2024-05-13 01:09:17.899439 wlkata_mirobot_Virtual-1.1.2/wlkata_mirobot_Virtual.egg-info/
+-rw-rw-rw-   0        0        0      110 2024-05-13 01:09:17.000000 wlkata_mirobot_Virtual-1.1.2/wlkata_mirobot_Virtual.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      288 2024-05-13 01:09:17.000000 wlkata_mirobot_Virtual-1.1.2/wlkata_mirobot_Virtual.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 01:09:17.000000 wlkata_mirobot_Virtual-1.1.2/wlkata_mirobot_Virtual.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2024-05-13 01:09:17.000000 wlkata_mirobot_Virtual-1.1.2/wlkata_mirobot_Virtual.egg-info/top_level.txt
```

### Comparing `wlkata_mirobot_Virtual-1.1.1/license.txt` & `wlkata_mirobot_Virtual-1.1.2/license.txt`

 * *Files identical despite different names*

### Comparing `wlkata_mirobot_Virtual-1.1.1/wlkata_mirobot_Virtual/wlkata_mirobot_Virtual.py` & `wlkata_mirobot_Virtual-1.1.2/wlkata_mirobot_Virtual/wlkata_mirobot_Virtual.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         self.invalid_IP_Port_Connect()
         self.status_state = None
         self.robot_type = 1
         self.global_state = [1,1,1]
         self.IO = [0,0,0,0,0,0,0,0]
         self.default_speed = 1000
         ### 第七轴/滑轨
-        self.angles_6 = 0
+        self.angles_7 = 0
   
     ### 作为client 连接服务端--Start
     def invalid_IP_Port_Connect(self,):
         self.flag = False
         self.client_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         #### 更改IP/PORT连接服务端 
         if self.server_IP == '':
@@ -106,23 +106,18 @@
             # pattern = r'"com1State":"(\w+)"'
             pattern = r'"com1State":"(\w+)","com2State":"(\w+)"'
             
             match = re.search(pattern, msg)
             if match:
                 state = match.group(1)
                 state2 = match.group(2)
-                # self.status_state = state
-                print(f"robot state is {state}")
-                print(f"robot2 state is {state2}")
 
             else:
                 state = None
-                # self.status_state = self.status_state
                 print("No match found state")
-                # pass
 
         except Exception as e:
             print(e)
         
         if state is not None and state2 is not None:
             self._set_status(state, state2)
         elif state is not None and state2 is None:
@@ -141,16 +136,16 @@
 
     def send_msg(self,com1_data=None, com2_data = None, wait_idle=False):
         robot_type = self.robot_type
         state = self.global_state
         com1 = com1_data
         com2 = com2_data ### if com2_data is not None else com1_data
         rs485 = ""
-        com1Float = self.angles_6 
-        com2Float = self.angles_6 
+        com1Float = self.angles_7 
+        com2Float = self.angles_7 
         io = self.IO
         
         ### 消息体
         message_body = self.create_message_body(robot_type, state, com1, com2, rs485, com1Float, com2Float, io)
         ### 消息体长度
         data_size = len(message_body)
         ### 控制器类型：虚拟控制器
@@ -166,22 +161,28 @@
         
         if com2_data is not None:
             self.status_state2 = None
         
         if wait_idle:
             self.wait_until_idle()
 	
-    def _set_status(self, state, state2 = None):
+    def _set_status(self, state= None, state2 = None):
         self.status_state = state
         self.status_state2 = state2 
     
     def wait_until_idle(self, refresh_rate = 0.1):
-        while self.status_state != "Idle" or self.status_state is None:
-            time.sleep(refresh_rate)
-            self.get_status_state()
+        if self.status_state2 is not None:
+            while self.status_state2 != "Idle" and  self.status_state != "Idle":
+                time.sleep(refresh_rate)
+                self.get_status_state()
+        
+        else:
+            while self.status_state != "Idle" or self.status_state is None:
+                time.sleep(refresh_rate)
+                self.get_status_state()
 
     ### G代码指令转换
     ### API函数
     ### IO输出设置
     def set_Output(self, output_id, value):
         self.IO[output_id] = value
         return self.IO
```

