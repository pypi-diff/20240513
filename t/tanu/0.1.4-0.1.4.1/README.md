# Comparing `tmp/tanu-0.1.4.tar.gz` & `tmp/tanu-0.1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tanu-0.1.4.tar", last modified: Mon May 13 10:30:04 2024, max compression
+gzip compressed data, was "tanu-0.1.4.1.tar", last modified: Mon May 13 10:36:08 2024, max compression
```

## Comparing `tanu-0.1.4.tar` & `tanu-0.1.4.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2024-05-13 10:30:04.156176 tanu-0.1.4/
--rw-r--r--   0 shuntaro   (501) staff       (20)    35149 2024-05-11 14:48:01.000000 tanu-0.1.4/LICENSE.txt
--rw-r--r--   0 shuntaro   (501) staff       (20)        0 2024-05-11 15:14:35.000000 tanu-0.1.4/MANIFEST.in
--rw-r--r--   0 shuntaro   (501) staff       (20)      692 2024-05-13 10:30:04.156111 tanu-0.1.4/PKG-INFO
--rw-r--r--   0 shuntaro   (501) staff       (20)      101 2024-05-11 15:12:10.000000 tanu-0.1.4/README.md
--rw-r--r--   0 shuntaro   (501) staff       (20)       94 2023-01-22 06:54:48.000000 tanu-0.1.4/pyproject.toml
--rw-r--r--   0 shuntaro   (501) staff       (20)      701 2024-05-13 10:30:04.156432 tanu-0.1.4/setup.cfg
--rw-r--r--   0 shuntaro   (501) staff       (20)       37 2022-12-09 19:04:39.000000 tanu-0.1.4/setup.py
-drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2024-05-13 10:30:04.153587 tanu-0.1.4/src/
-drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2024-05-13 10:30:04.154807 tanu-0.1.4/src/tanu/
--rw-r--r--   0 shuntaro   (501) staff       (20)       38 2024-05-11 14:04:14.000000 tanu-0.1.4/src/tanu/__init__.py
--rw-r--r--   0 shuntaro   (501) staff       (20)    17341 2024-05-13 10:29:40.000000 tanu-0.1.4/src/tanu/tanu.py
-drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2024-05-13 10:30:04.155727 tanu-0.1.4/src/tanu/utils/
--rw-r--r--   0 shuntaro   (501) staff       (20)        0 2024-05-11 15:36:56.000000 tanu-0.1.4/src/tanu/utils/__init__.py
--rw-r--r--   0 shuntaro   (501) staff       (20)     1339 2024-05-11 15:28:52.000000 tanu-0.1.4/src/tanu/utils/object_encoder_decoder.py
-drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2024-05-13 10:30:04.155894 tanu-0.1.4/src/tanu.egg-info/
--rw-r--r--   0 shuntaro   (501) staff       (20)      692 2024-05-13 10:30:04.000000 tanu-0.1.4/src/tanu.egg-info/PKG-INFO
--rw-r--r--   0 shuntaro   (501) staff       (20)      332 2024-05-13 10:30:04.000000 tanu-0.1.4/src/tanu.egg-info/SOURCES.txt
--rw-r--r--   0 shuntaro   (501) staff       (20)        1 2024-05-13 10:30:04.000000 tanu-0.1.4/src/tanu.egg-info/dependency_links.txt
--rw-r--r--   0 shuntaro   (501) staff       (20)       33 2024-05-13 10:30:04.000000 tanu-0.1.4/src/tanu.egg-info/requires.txt
--rw-r--r--   0 shuntaro   (501) staff       (20)        5 2024-05-13 10:30:04.000000 tanu-0.1.4/src/tanu.egg-info/top_level.txt
+drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2024-05-13 10:36:08.980911 tanu-0.1.4.1/
+-rw-r--r--   0 shuntaro   (501) staff       (20)    35149 2024-05-11 14:48:01.000000 tanu-0.1.4.1/LICENSE.txt
+-rw-r--r--   0 shuntaro   (501) staff       (20)        0 2024-05-11 15:14:35.000000 tanu-0.1.4.1/MANIFEST.in
+-rw-r--r--   0 shuntaro   (501) staff       (20)      723 2024-05-13 10:36:08.980831 tanu-0.1.4.1/PKG-INFO
+-rw-r--r--   0 shuntaro   (501) staff       (20)      101 2024-05-11 15:12:10.000000 tanu-0.1.4.1/README.md
+-rw-r--r--   0 shuntaro   (501) staff       (20)       94 2023-01-22 06:54:48.000000 tanu-0.1.4.1/pyproject.toml
+-rw-r--r--   0 shuntaro   (501) staff       (20)      720 2024-05-13 10:36:08.981400 tanu-0.1.4.1/setup.cfg
+-rw-r--r--   0 shuntaro   (501) staff       (20)       37 2022-12-09 19:04:39.000000 tanu-0.1.4.1/setup.py
+drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2024-05-13 10:36:08.933713 tanu-0.1.4.1/src/
+drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2024-05-13 10:36:08.974218 tanu-0.1.4.1/src/tanu/
+-rw-r--r--   0 shuntaro   (501) staff       (20)       38 2024-05-11 14:04:14.000000 tanu-0.1.4.1/src/tanu/__init__.py
+-rw-r--r--   0 shuntaro   (501) staff       (20)    17945 2024-05-13 10:35:50.000000 tanu-0.1.4.1/src/tanu/tanu.py
+drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2024-05-13 10:36:08.980044 tanu-0.1.4.1/src/tanu/utils/
+-rw-r--r--   0 shuntaro   (501) staff       (20)        0 2024-05-11 15:36:56.000000 tanu-0.1.4.1/src/tanu/utils/__init__.py
+-rw-r--r--   0 shuntaro   (501) staff       (20)     1339 2024-05-11 15:28:52.000000 tanu-0.1.4.1/src/tanu/utils/object_encoder_decoder.py
+drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2024-05-13 10:36:08.980539 tanu-0.1.4.1/src/tanu.egg-info/
+-rw-r--r--   0 shuntaro   (501) staff       (20)      723 2024-05-13 10:36:08.000000 tanu-0.1.4.1/src/tanu.egg-info/PKG-INFO
+-rw-r--r--   0 shuntaro   (501) staff       (20)      332 2024-05-13 10:36:08.000000 tanu-0.1.4.1/src/tanu.egg-info/SOURCES.txt
+-rw-r--r--   0 shuntaro   (501) staff       (20)        1 2024-05-13 10:36:08.000000 tanu-0.1.4.1/src/tanu.egg-info/dependency_links.txt
+-rw-r--r--   0 shuntaro   (501) staff       (20)       47 2024-05-13 10:36:08.000000 tanu-0.1.4.1/src/tanu.egg-info/requires.txt
+-rw-r--r--   0 shuntaro   (501) staff       (20)        5 2024-05-13 10:36:08.000000 tanu-0.1.4.1/src/tanu.egg-info/top_level.txt
```

### Comparing `tanu-0.1.4/LICENSE.txt` & `tanu-0.1.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tanu-0.1.4/PKG-INFO` & `tanu-0.1.4.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: tanu
-Version: 0.1.4
+Version: 0.1.4.1
 Summary: Message passing between Python programs via RabbitMQ.
 Author: chocolate-icecream
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: pika>=1.0
 Requires-Dist: pandas>=1.0
 Requires-Dist: numpy>=1.0
+Requires-Dist: pydantic>=2.7
 
 # Tanu
 
 Tanuki serves as a tool to facilitates message passing between Python programs via RabbitMQ.
```

### Comparing `tanu-0.1.4/setup.cfg` & `tanu-0.1.4.1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = tanu
-version = 0.1.4
+version = 0.1.4.1
 author = chocolate-icecream
 description = Message passing between Python programs via RabbitMQ.
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
@@ -18,14 +18,15 @@
 packages = find:
 include_package_data = True
 python_requires = >=3.6
 install_requires = 
 	pika >= 1.0
 	pandas >= 1.0
 	numpy >= 1.0
+	pydantic >= 2.7
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `tanu-0.1.4/src/tanu/tanu.py` & `tanu-0.1.4.1/src/tanu/tanu.py`

 * *Files 3% similar despite different names*

```diff
@@ -125,15 +125,15 @@
         """Start a separate thread to handle result retrieval."""
         t = threading.Thread(target=self.start_consumer)
         t.daemon = True
         t.start()
 
     def start_consumer(self):
         """Continuously consume results from the result queue."""
-        connection = pika.BlockingConnection(pika.ConnectionParameters(self.host))
+        connection = pika.BlockingConnection(pika.ConnectionParameters(host=self.host, port=self.port))
         channel = connection.channel()
         channel.queue_declare(queue=self.result_queue_name)
         channel.basic_consume(queue=self.result_queue_name, auto_ack=True, on_message_callback=self.on_result_received)
         channel.start_consuming()
 
     def on_result_received(self, ch, method, properties, body):
         """Handle received results and trigger callback if set."""
@@ -242,30 +242,31 @@
             raise Exception(self.response.result["msg"])
 
         return self.response.result
 
 class TanukiResponseConnection:
     """Manages the communication of results back to the requester."""
 
-    def __init__(self, request: RequestLetter = None, units=None):
+    def __init__(self, parent, request: RequestLetter = None, units=None):
+        self.parent = parent
         self.request = request
         self.units = units if units else {}
         self.connect()
 
     @classmethod
-    def send_error(cls, request: RequestLetter, msg: str):
+    def send_error(cls, parent, request: RequestLetter, msg: str):
         """Send an error message back to the requester."""
         logger.error(msg)
-        connection = TanukiResponseConnection(request)
+        connection = TanukiResponseConnection(parent, request)
         connection.send_status(StatusEnum.ERROR, msg)
         connection.close()
     
     def connect(self):
         """Establish a connection to the message broker."""
-        self.connection = pika.BlockingConnection(pika.ConnectionParameters('localhost'))
+        self.connection = pika.BlockingConnection(pika.ConnectionParameters(host=self.parent.host, port=self.parent.port))
         self.channel = self.connection.channel()
     
     def set_request(self, request: RequestLetter):
         """Set the request details for sending responses."""
         self.request = request
     
     def send(self, status: StatusEnum, result: dict):
@@ -303,38 +304,50 @@
             self.connection.close()
         except pika.exceptions.ConnectionWrongStateError:
             pass
 
 class TanukiWorker:
     """Defines a worker that can execute commands based on requests received through a message queue."""
 
-    def __init__(self, name: str, auth: str = ""):
+    def __init__(self, name: str, auth: str = "", host=None, port=None):
         self.name = name
         self.auth = auth
+        if host is None:
+            url = os.getenv("TANU_RABBITMQ_URL")
+            if len(url) == 0:
+                self.host = "localhost"
+                self.port = port if port else 5672
+            else:
+                self.host = ":".join(url.split(":")[:-1])
+                self.port = port if port else int(url.split(":")[-1])
+        else:
+            self.host = host
+            self.port = port if port else 5672
+
         self.command_dict = {}
         self.units = {}
     
     def run(self):
         """Start consuming tasks from the queue."""
         queue_name = f"task_{self.name}"
-        self.connection_for_task_queue = pika.BlockingConnection(pika.ConnectionParameters('localhost'))
-        self.base_response_connection = TanukiResponseConnection(units=self.units)
+        self.connection_for_task_queue = pika.BlockingConnection(pika.ConnectionParameters(host=self.host, port=self.port))
+        self.base_response_connection = TanukiResponseConnection(self, units=self.units)
         channel = self.connection_for_task_queue.channel()
         channel.queue_declare(queue=queue_name, durable=True)
         channel.basic_qos(prefetch_count=1)
         channel.basic_consume(queue=queue_name, on_message_callback=self._call_command)
         logger.info(f"{self.name} starts running...")
         channel.start_consuming()
 
     def _call_command(self, ch_req, method, properties, body):
         """Process incoming command requests."""
         try:
             request = RequestLetter.parse_raw(body)
             if request.command not in self.command_dict:
-                TanukiResponseConnection.send_error(request, f"Tanuki Worker {self.name} cannot recognize '{request.command}'.")
+                TanukiResponseConnection.send_error(self, request, f"Tanuki Worker {self.name} cannot recognize '{request.command}'.")
                 ch_req.basic_ack(delivery_tag=method.delivery_tag)
                 return
         except Exception as e:
             logger.error(traceback.format_exc())
             ch_req.basic_ack(delivery_tag=method.delivery_tag)
             return
 
@@ -346,15 +359,15 @@
                                             "ch_req": ch_req,
                                             "delivery_tag": method.delivery_tag})
                 t.daemon = True
                 t.start()
             else:
                 self._perform_registered_command(self.base_response_connection, request)
         except Exception as e:
-            TanukiResponseConnection.send_error(request, traceback.format_exc())
+            TanukiResponseConnection.send_error(self, request, traceback.format_exc())
         finally:
             if not self.command_dict[request.command]["multi_threading"]:
                 ch_req.basic_ack(delivery_tag=method.delivery_tag)
 
     def _perform_registered_command(self, connection: TanukiResponseConnection, request: RequestLetter):
         """Execute a registered command."""
         apply_decoder(request)
@@ -369,15 +382,15 @@
         else:
             logger.error(f"{request.command} on {self.name} returns an incorrect result {result} with type {type(result)}.")
             connection.send_status(StatusEnum.ERROR, f"{request.command} on {self.name} returns an incorrect result {result} with type {type(result)}.")
             
 
     def _perform_registered_command_for_multi_threading(self, request: RequestLetter, ch_req, delivery_tag):
         """Execute a registered command in a separate thread."""
-        connection = TanukiResponseConnection(request, units=self.units)
+        connection = TanukiResponseConnection(self, request, units=self.units)
         try:
             self._perform_registered_command(request)
         finally:
             connection.close()
             self._ack_message(ch_req, delivery_tag)
 
     def _ack_message(self, channel, delivery_tag):
```

### Comparing `tanu-0.1.4/src/tanu/utils/object_encoder_decoder.py` & `tanu-0.1.4.1/src/tanu/utils/object_encoder_decoder.py`

 * *Files identical despite different names*

### Comparing `tanu-0.1.4/src/tanu.egg-info/PKG-INFO` & `tanu-0.1.4.1/src/tanu.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: tanu
-Version: 0.1.4
+Version: 0.1.4.1
 Summary: Message passing between Python programs via RabbitMQ.
 Author: chocolate-icecream
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: pika>=1.0
 Requires-Dist: pandas>=1.0
 Requires-Dist: numpy>=1.0
+Requires-Dist: pydantic>=2.7
 
 # Tanu
 
 Tanuki serves as a tool to facilitates message passing between Python programs via RabbitMQ.
```

