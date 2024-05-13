# Comparing `tmp/tanu-0.1.3.tar.gz` & `tmp/tanu-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tanu-0.1.3.tar", last modified: Mon May 13 10:25:24 2024, max compression
+gzip compressed data, was "tanu-0.1.4.tar", last modified: Mon May 13 10:30:04 2024, max compression
```

## Comparing `tanu-0.1.3.tar` & `tanu-0.1.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2024-05-13 10:25:24.060119 tanu-0.1.3/
--rw-r--r--   0 shuntaro   (501) staff       (20)    35149 2024-05-11 14:48:01.000000 tanu-0.1.3/LICENSE.txt
--rw-r--r--   0 shuntaro   (501) staff       (20)        0 2024-05-11 15:14:35.000000 tanu-0.1.3/MANIFEST.in
--rw-r--r--   0 shuntaro   (501) staff       (20)      692 2024-05-13 10:25:24.060057 tanu-0.1.3/PKG-INFO
--rw-r--r--   0 shuntaro   (501) staff       (20)      101 2024-05-11 15:12:10.000000 tanu-0.1.3/README.md
--rw-r--r--   0 shuntaro   (501) staff       (20)       94 2023-01-22 06:54:48.000000 tanu-0.1.3/pyproject.toml
--rw-r--r--   0 shuntaro   (501) staff       (20)      701 2024-05-13 10:25:24.060404 tanu-0.1.3/setup.cfg
--rw-r--r--   0 shuntaro   (501) staff       (20)       37 2022-12-09 19:04:39.000000 tanu-0.1.3/setup.py
-drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2024-05-13 10:25:24.056361 tanu-0.1.3/src/
-drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2024-05-13 10:25:24.058280 tanu-0.1.3/src/tanu/
--rw-r--r--   0 shuntaro   (501) staff       (20)       38 2024-05-11 14:04:14.000000 tanu-0.1.3/src/tanu/__init__.py
--rw-r--r--   0 shuntaro   (501) staff       (20)    17312 2024-05-13 10:24:40.000000 tanu-0.1.3/src/tanu/tanu.py
-drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2024-05-13 10:25:24.059406 tanu-0.1.3/src/tanu/utils/
--rw-r--r--   0 shuntaro   (501) staff       (20)        0 2024-05-11 15:36:56.000000 tanu-0.1.3/src/tanu/utils/__init__.py
--rw-r--r--   0 shuntaro   (501) staff       (20)     1339 2024-05-11 15:28:52.000000 tanu-0.1.3/src/tanu/utils/object_encoder_decoder.py
-drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2024-05-13 10:25:24.059810 tanu-0.1.3/src/tanu.egg-info/
--rw-r--r--   0 shuntaro   (501) staff       (20)      692 2024-05-13 10:25:24.000000 tanu-0.1.3/src/tanu.egg-info/PKG-INFO
--rw-r--r--   0 shuntaro   (501) staff       (20)      332 2024-05-13 10:25:24.000000 tanu-0.1.3/src/tanu.egg-info/SOURCES.txt
--rw-r--r--   0 shuntaro   (501) staff       (20)        1 2024-05-13 10:25:24.000000 tanu-0.1.3/src/tanu.egg-info/dependency_links.txt
--rw-r--r--   0 shuntaro   (501) staff       (20)       33 2024-05-13 10:25:24.000000 tanu-0.1.3/src/tanu.egg-info/requires.txt
--rw-r--r--   0 shuntaro   (501) staff       (20)        5 2024-05-13 10:25:24.000000 tanu-0.1.3/src/tanu.egg-info/top_level.txt
+drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2024-05-13 10:30:04.156176 tanu-0.1.4/
+-rw-r--r--   0 shuntaro   (501) staff       (20)    35149 2024-05-11 14:48:01.000000 tanu-0.1.4/LICENSE.txt
+-rw-r--r--   0 shuntaro   (501) staff       (20)        0 2024-05-11 15:14:35.000000 tanu-0.1.4/MANIFEST.in
+-rw-r--r--   0 shuntaro   (501) staff       (20)      692 2024-05-13 10:30:04.156111 tanu-0.1.4/PKG-INFO
+-rw-r--r--   0 shuntaro   (501) staff       (20)      101 2024-05-11 15:12:10.000000 tanu-0.1.4/README.md
+-rw-r--r--   0 shuntaro   (501) staff       (20)       94 2023-01-22 06:54:48.000000 tanu-0.1.4/pyproject.toml
+-rw-r--r--   0 shuntaro   (501) staff       (20)      701 2024-05-13 10:30:04.156432 tanu-0.1.4/setup.cfg
+-rw-r--r--   0 shuntaro   (501) staff       (20)       37 2022-12-09 19:04:39.000000 tanu-0.1.4/setup.py
+drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2024-05-13 10:30:04.153587 tanu-0.1.4/src/
+drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2024-05-13 10:30:04.154807 tanu-0.1.4/src/tanu/
+-rw-r--r--   0 shuntaro   (501) staff       (20)       38 2024-05-11 14:04:14.000000 tanu-0.1.4/src/tanu/__init__.py
+-rw-r--r--   0 shuntaro   (501) staff       (20)    17341 2024-05-13 10:29:40.000000 tanu-0.1.4/src/tanu/tanu.py
+drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2024-05-13 10:30:04.155727 tanu-0.1.4/src/tanu/utils/
+-rw-r--r--   0 shuntaro   (501) staff       (20)        0 2024-05-11 15:36:56.000000 tanu-0.1.4/src/tanu/utils/__init__.py
+-rw-r--r--   0 shuntaro   (501) staff       (20)     1339 2024-05-11 15:28:52.000000 tanu-0.1.4/src/tanu/utils/object_encoder_decoder.py
+drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2024-05-13 10:30:04.155894 tanu-0.1.4/src/tanu.egg-info/
+-rw-r--r--   0 shuntaro   (501) staff       (20)      692 2024-05-13 10:30:04.000000 tanu-0.1.4/src/tanu.egg-info/PKG-INFO
+-rw-r--r--   0 shuntaro   (501) staff       (20)      332 2024-05-13 10:30:04.000000 tanu-0.1.4/src/tanu.egg-info/SOURCES.txt
+-rw-r--r--   0 shuntaro   (501) staff       (20)        1 2024-05-13 10:30:04.000000 tanu-0.1.4/src/tanu.egg-info/dependency_links.txt
+-rw-r--r--   0 shuntaro   (501) staff       (20)       33 2024-05-13 10:30:04.000000 tanu-0.1.4/src/tanu.egg-info/requires.txt
+-rw-r--r--   0 shuntaro   (501) staff       (20)        5 2024-05-13 10:30:04.000000 tanu-0.1.4/src/tanu.egg-info/top_level.txt
```

### Comparing `tanu-0.1.3/LICENSE.txt` & `tanu-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tanu-0.1.3/PKG-INFO` & `tanu-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tanu
-Version: 0.1.3
+Version: 0.1.4
 Summary: Message passing between Python programs via RabbitMQ.
 Author: chocolate-icecream
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `tanu-0.1.3/setup.cfg` & `tanu-0.1.4/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = tanu
-version = 0.1.3
+version = 0.1.4
 author = chocolate-icecream
 description = Message passing between Python programs via RabbitMQ.
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
```

### Comparing `tanu-0.1.3/src/tanu/tanu.py` & `tanu-0.1.4/src/tanu/tanu.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,16 +98,16 @@
         self.worker_name = worker_name
         if host is None:
             url = os.getenv("TANU_RABBITMQ_URL")
             if len(url) == 0:
                 self.host = "localhost"
                 self.port = port if port else 5672
             else:
-                self.host = url.split(":")[:-1]
-                self.port = port if port else 5672
+                self.host = ":".join(url.split(":")[:-1])
+                self.port = port if port else int(url.split(":")[-1])
         else:
             self.host = host
             self.port = port if port else 5672
         self.callback_func = callback_func
         self.accept_previous_job = accept_previous_job
         self.result_queues = {}
         self.units = {}
```

### Comparing `tanu-0.1.3/src/tanu/utils/object_encoder_decoder.py` & `tanu-0.1.4/src/tanu/utils/object_encoder_decoder.py`

 * *Files identical despite different names*

### Comparing `tanu-0.1.3/src/tanu.egg-info/PKG-INFO` & `tanu-0.1.4/src/tanu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tanu
-Version: 0.1.3
+Version: 0.1.4
 Summary: Message passing between Python programs via RabbitMQ.
 Author: chocolate-icecream
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

