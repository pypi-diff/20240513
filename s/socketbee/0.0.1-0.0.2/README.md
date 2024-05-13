# Comparing `tmp/socketbee-0.0.1.tar.gz` & `tmp/socketbee-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socketbee-0.0.1.tar", last modified: Mon May 13 05:08:29 2024, max compression
+gzip compressed data, was "socketbee-0.0.2.tar", last modified: Mon May 13 05:37:10 2024, max compression
```

## Comparing `socketbee-0.0.1.tar` & `socketbee-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 boulamakandine   (501) staff       (20)        0 2024-05-13 05:08:29.062337 socketbee-0.0.1/
--rw-r--r--   0 boulamakandine   (501) staff       (20)     1053 2024-05-13 04:59:24.000000 socketbee-0.0.1/LICENSE.md
--rw-r--r--   0 boulamakandine   (501) staff       (20)      641 2024-05-13 05:08:29.062151 socketbee-0.0.1/PKG-INFO
--rw-r--r--   0 boulamakandine   (501) staff       (20)       32 2024-05-13 05:00:53.000000 socketbee-0.0.1/README.md
--rw-r--r--   0 boulamakandine   (501) staff       (20)      703 2024-05-13 04:58:16.000000 socketbee-0.0.1/pyproject.toml
--rw-r--r--   0 boulamakandine   (501) staff       (20)       38 2024-05-13 05:08:29.062383 socketbee-0.0.1/setup.cfg
--rw-r--r--   0 boulamakandine   (501) staff       (20)      121 2024-05-13 04:56:07.000000 socketbee-0.0.1/setup.py
-drwxr-xr-x   0 boulamakandine   (501) staff       (20)        0 2024-05-13 05:08:29.061241 socketbee-0.0.1/socketbee/
--rw-r--r--   0 boulamakandine   (501) staff       (20)        0 2024-05-13 04:42:01.000000 socketbee-0.0.1/socketbee/__init__.py
--rw-r--r--   0 boulamakandine   (501) staff       (20)     1559 2024-05-13 04:55:43.000000 socketbee-0.0.1/socketbee/client.py
--rw-r--r--   0 boulamakandine   (501) staff       (20)        0 2024-05-13 04:42:14.000000 socketbee-0.0.1/socketbee/settings.py
-drwxr-xr-x   0 boulamakandine   (501) staff       (20)        0 2024-05-13 05:08:29.061966 socketbee-0.0.1/socketbee.egg-info/
--rw-r--r--   0 boulamakandine   (501) staff       (20)      641 2024-05-13 05:08:29.000000 socketbee-0.0.1/socketbee.egg-info/PKG-INFO
--rw-r--r--   0 boulamakandine   (501) staff       (20)      272 2024-05-13 05:08:29.000000 socketbee-0.0.1/socketbee.egg-info/SOURCES.txt
--rw-r--r--   0 boulamakandine   (501) staff       (20)        1 2024-05-13 05:08:29.000000 socketbee-0.0.1/socketbee.egg-info/dependency_links.txt
--rw-r--r--   0 boulamakandine   (501) staff       (20)       16 2024-05-13 05:08:29.000000 socketbee-0.0.1/socketbee.egg-info/requires.txt
--rw-r--r--   0 boulamakandine   (501) staff       (20)       10 2024-05-13 05:08:29.000000 socketbee-0.0.1/socketbee.egg-info/top_level.txt
+drwxr-xr-x   0 boulamakandine   (501) staff       (20)        0 2024-05-13 05:37:10.109727 socketbee-0.0.2/
+-rw-r--r--   0 boulamakandine   (501) staff       (20)     1053 2024-05-13 04:59:24.000000 socketbee-0.0.2/LICENSE.md
+-rw-r--r--   0 boulamakandine   (501) staff       (20)      641 2024-05-13 05:37:10.109549 socketbee-0.0.2/PKG-INFO
+-rw-r--r--   0 boulamakandine   (501) staff       (20)       32 2024-05-13 05:00:53.000000 socketbee-0.0.2/README.md
+-rw-r--r--   0 boulamakandine   (501) staff       (20)      703 2024-05-13 05:30:19.000000 socketbee-0.0.2/pyproject.toml
+-rw-r--r--   0 boulamakandine   (501) staff       (20)       38 2024-05-13 05:37:10.109767 socketbee-0.0.2/setup.cfg
+-rw-r--r--   0 boulamakandine   (501) staff       (20)      121 2024-05-13 04:56:07.000000 socketbee-0.0.2/setup.py
+drwxr-xr-x   0 boulamakandine   (501) staff       (20)        0 2024-05-13 05:37:10.108655 socketbee-0.0.2/socketbee/
+-rw-r--r--   0 boulamakandine   (501) staff       (20)        0 2024-05-13 04:42:01.000000 socketbee-0.0.2/socketbee/__init__.py
+-rw-r--r--   0 boulamakandine   (501) staff       (20)     1559 2024-05-13 04:55:43.000000 socketbee-0.0.2/socketbee/client.py
+-rw-r--r--   0 boulamakandine   (501) staff       (20)        0 2024-05-13 04:42:14.000000 socketbee-0.0.2/socketbee/settings.py
+drwxr-xr-x   0 boulamakandine   (501) staff       (20)        0 2024-05-13 05:37:10.109381 socketbee-0.0.2/socketbee.egg-info/
+-rw-r--r--   0 boulamakandine   (501) staff       (20)      641 2024-05-13 05:37:10.000000 socketbee-0.0.2/socketbee.egg-info/PKG-INFO
+-rw-r--r--   0 boulamakandine   (501) staff       (20)      272 2024-05-13 05:37:10.000000 socketbee-0.0.2/socketbee.egg-info/SOURCES.txt
+-rw-r--r--   0 boulamakandine   (501) staff       (20)        1 2024-05-13 05:37:10.000000 socketbee-0.0.2/socketbee.egg-info/dependency_links.txt
+-rw-r--r--   0 boulamakandine   (501) staff       (20)       24 2024-05-13 05:37:10.000000 socketbee-0.0.2/socketbee.egg-info/requires.txt
+-rw-r--r--   0 boulamakandine   (501) staff       (20)       10 2024-05-13 05:37:10.000000 socketbee-0.0.2/socketbee.egg-info/top_level.txt
```

### Comparing `socketbee-0.0.1/LICENSE.md` & `socketbee-0.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `socketbee-0.0.1/PKG-INFO` & `socketbee-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: socketbee
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python wrapper for the SocketBee.
 Author-email: "Boulama K." <boulama@otimbi.com>
-Project-URL: Homepage, https://github.com/socketbee/socketbee-python
-Project-URL: Bug Tracker, https://github.com/socketbee/socketbee-python/issues
+Project-URL: Homepage, https://github.com/socketbee/socketbee.py
+Project-URL: Bug Tracker, https://github.com/socketbee/socketbee.py/issues
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
-Requires-Dist: python-socketio
+Requires-Dist: python-socketio[client]
 
 ## SocketBee Python client
 
 WIP.
```

### Comparing `socketbee-0.0.1/pyproject.toml` & `socketbee-0.0.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "socketbee"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Boulama K.", email="boulama@otimbi.com" },
 ]
 description = "A Python wrapper for the SocketBee."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
-dependencies = ["python-socketio"]
+dependencies = ["python-socketio[client]"]
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/socketbee/socketbee-python"
-"Bug Tracker" = "https://github.com/socketbee/socketbee-python/issues"
+"Homepage" = "https://github.com/socketbee/socketbee.py"
+"Bug Tracker" = "https://github.com/socketbee/socketbee.py/issues"
```

### Comparing `socketbee-0.0.1/socketbee/client.py` & `socketbee-0.0.2/socketbee/client.py`

 * *Files identical despite different names*

### Comparing `socketbee-0.0.1/socketbee.egg-info/PKG-INFO` & `socketbee-0.0.2/socketbee.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: socketbee
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python wrapper for the SocketBee.
 Author-email: "Boulama K." <boulama@otimbi.com>
-Project-URL: Homepage, https://github.com/socketbee/socketbee-python
-Project-URL: Bug Tracker, https://github.com/socketbee/socketbee-python/issues
+Project-URL: Homepage, https://github.com/socketbee/socketbee.py
+Project-URL: Bug Tracker, https://github.com/socketbee/socketbee.py/issues
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
-Requires-Dist: python-socketio
+Requires-Dist: python-socketio[client]
 
 ## SocketBee Python client
 
 WIP.
```

