# Comparing `tmp/socketbee-0.0.3.tar.gz` & `tmp/socketbee-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socketbee-0.0.3.tar", last modified: Mon May 13 05:48:26 2024, max compression
+gzip compressed data, was "socketbee-0.0.4.tar", last modified: Mon May 13 05:49:21 2024, max compression
```

## Comparing `socketbee-0.0.3.tar` & `socketbee-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 boulamakandine   (501) staff       (20)        0 2024-05-13 05:48:26.639528 socketbee-0.0.3/
--rw-r--r--   0 boulamakandine   (501) staff       (20)     1053 2024-05-13 04:59:24.000000 socketbee-0.0.3/LICENSE.md
--rw-r--r--   0 boulamakandine   (501) staff       (20)      641 2024-05-13 05:48:26.639339 socketbee-0.0.3/PKG-INFO
--rw-r--r--   0 boulamakandine   (501) staff       (20)       32 2024-05-13 05:00:53.000000 socketbee-0.0.3/README.md
--rw-r--r--   0 boulamakandine   (501) staff       (20)      704 2024-05-13 05:48:25.000000 socketbee-0.0.3/pyproject.toml
--rw-r--r--   0 boulamakandine   (501) staff       (20)       38 2024-05-13 05:48:26.639567 socketbee-0.0.3/setup.cfg
--rw-r--r--   0 boulamakandine   (501) staff       (20)      121 2024-05-13 04:56:07.000000 socketbee-0.0.3/setup.py
-drwxr-xr-x   0 boulamakandine   (501) staff       (20)        0 2024-05-13 05:48:26.638442 socketbee-0.0.3/socketbee/
--rw-r--r--   0 boulamakandine   (501) staff       (20)        0 2024-05-13 04:42:01.000000 socketbee-0.0.3/socketbee/__init__.py
--rw-r--r--   0 boulamakandine   (501) staff       (20)     1559 2024-05-13 04:55:43.000000 socketbee-0.0.3/socketbee/client.py
--rw-r--r--   0 boulamakandine   (501) staff       (20)        0 2024-05-13 04:42:14.000000 socketbee-0.0.3/socketbee/settings.py
-drwxr-xr-x   0 boulamakandine   (501) staff       (20)        0 2024-05-13 05:48:26.639153 socketbee-0.0.3/socketbee.egg-info/
--rw-r--r--   0 boulamakandine   (501) staff       (20)      641 2024-05-13 05:48:26.000000 socketbee-0.0.3/socketbee.egg-info/PKG-INFO
--rw-r--r--   0 boulamakandine   (501) staff       (20)      272 2024-05-13 05:48:26.000000 socketbee-0.0.3/socketbee.egg-info/SOURCES.txt
--rw-r--r--   0 boulamakandine   (501) staff       (20)        1 2024-05-13 05:48:26.000000 socketbee-0.0.3/socketbee.egg-info/dependency_links.txt
--rw-r--r--   0 boulamakandine   (501) staff       (20)       24 2024-05-13 05:48:26.000000 socketbee-0.0.3/socketbee.egg-info/requires.txt
--rw-r--r--   0 boulamakandine   (501) staff       (20)       10 2024-05-13 05:48:26.000000 socketbee-0.0.3/socketbee.egg-info/top_level.txt
+drwxr-xr-x   0 boulamakandine   (501) staff       (20)        0 2024-05-13 05:49:21.821529 socketbee-0.0.4/
+-rw-r--r--   0 boulamakandine   (501) staff       (20)     1053 2024-05-13 04:59:24.000000 socketbee-0.0.4/LICENSE.md
+-rw-r--r--   0 boulamakandine   (501) staff       (20)      665 2024-05-13 05:49:21.821354 socketbee-0.0.4/PKG-INFO
+-rw-r--r--   0 boulamakandine   (501) staff       (20)       32 2024-05-13 05:00:53.000000 socketbee-0.0.4/README.md
+-rw-r--r--   0 boulamakandine   (501) staff       (20)      716 2024-05-13 05:49:20.000000 socketbee-0.0.4/pyproject.toml
+-rw-r--r--   0 boulamakandine   (501) staff       (20)       38 2024-05-13 05:49:21.821572 socketbee-0.0.4/setup.cfg
+-rw-r--r--   0 boulamakandine   (501) staff       (20)      121 2024-05-13 04:56:07.000000 socketbee-0.0.4/setup.py
+drwxr-xr-x   0 boulamakandine   (501) staff       (20)        0 2024-05-13 05:49:21.820460 socketbee-0.0.4/socketbee/
+-rw-r--r--   0 boulamakandine   (501) staff       (20)        0 2024-05-13 04:42:01.000000 socketbee-0.0.4/socketbee/__init__.py
+-rw-r--r--   0 boulamakandine   (501) staff       (20)     1559 2024-05-13 04:55:43.000000 socketbee-0.0.4/socketbee/client.py
+-rw-r--r--   0 boulamakandine   (501) staff       (20)        0 2024-05-13 04:42:14.000000 socketbee-0.0.4/socketbee/settings.py
+drwxr-xr-x   0 boulamakandine   (501) staff       (20)        0 2024-05-13 05:49:21.821170 socketbee-0.0.4/socketbee.egg-info/
+-rw-r--r--   0 boulamakandine   (501) staff       (20)      665 2024-05-13 05:49:21.000000 socketbee-0.0.4/socketbee.egg-info/PKG-INFO
+-rw-r--r--   0 boulamakandine   (501) staff       (20)      272 2024-05-13 05:49:21.000000 socketbee-0.0.4/socketbee.egg-info/SOURCES.txt
+-rw-r--r--   0 boulamakandine   (501) staff       (20)        1 2024-05-13 05:49:21.000000 socketbee-0.0.4/socketbee.egg-info/dependency_links.txt
+-rw-r--r--   0 boulamakandine   (501) staff       (20)       33 2024-05-13 05:49:21.000000 socketbee-0.0.4/socketbee.egg-info/requires.txt
+-rw-r--r--   0 boulamakandine   (501) staff       (20)       10 2024-05-13 05:49:21.000000 socketbee-0.0.4/socketbee.egg-info/top_level.txt
```

### Comparing `socketbee-0.0.3/LICENSE.md` & `socketbee-0.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `socketbee-0.0.3/PKG-INFO` & `socketbee-0.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: socketbee
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Python wrapper for the SocketBee.
 Author-email: "Boulama K." <boulama@otimbi.com>
 Project-URL: Homepage, https://github.com/socketbee/socketbee.py
 Project-URL: Bug Tracker, https://github.com/socketbee/socketbee.py/issues
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: python-socketio[client]
+Requires-Dist: requests
 
 ## SocketBee Python client
 
 WIP.
```

### Comparing `socketbee-0.0.3/pyproject.toml` & `socketbee-0.0.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "socketbee"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Boulama K.", email="boulama@otimbi.com" },
 ]
 description = "A Python wrapper for the SocketBee."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
-dependencies = ["python-socketio[client]"]
+dependencies = ["python-socketio[client]", "requests"]
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `socketbee-0.0.3/socketbee/client.py` & `socketbee-0.0.4/socketbee/client.py`

 * *Files identical despite different names*

### Comparing `socketbee-0.0.3/socketbee.egg-info/PKG-INFO` & `socketbee-0.0.4/socketbee.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: socketbee
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Python wrapper for the SocketBee.
 Author-email: "Boulama K." <boulama@otimbi.com>
 Project-URL: Homepage, https://github.com/socketbee/socketbee.py
 Project-URL: Bug Tracker, https://github.com/socketbee/socketbee.py/issues
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: python-socketio[client]
+Requires-Dist: requests
 
 ## SocketBee Python client
 
 WIP.
```

