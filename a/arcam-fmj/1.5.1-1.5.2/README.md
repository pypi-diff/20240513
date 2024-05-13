# Comparing `tmp/arcam_fmj-1.5.1.tar.gz` & `tmp/arcam_fmj-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcam_fmj-1.5.1.tar", last modified: Fri May 10 15:21:47 2024, max compression
+gzip compressed data, was "arcam_fmj-1.5.2.tar", last modified: Mon May 13 18:35:28 2024, max compression
```

## Comparing `arcam_fmj-1.5.1.tar` & `arcam_fmj-1.5.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:21:47.137612 arcam_fmj-1.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-10 15:21:39.000000 arcam_fmj-1.5.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-05-10 15:21:47.137612 arcam_fmj-1.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-10 15:21:39.000000 arcam_fmj-1.5.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-10 15:21:47.137612 arcam_fmj-1.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-10 15:21:39.000000 arcam_fmj-1.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:21:47.133612 arcam_fmj-1.5.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:21:47.129612 arcam_fmj-1.5.1/src/arcam/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:21:47.133612 arcam_fmj-1.5.1/src/arcam/fmj/
--rw-r--r--   0 runner    (1001) docker     (127)    38139 2024-05-10 15:21:39.000000 arcam_fmj-1.5.1/src/arcam/fmj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7355 2024-05-10 15:21:39.000000 arcam_fmj-1.5.1/src/arcam/fmj/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    10656 2024-05-10 15:21:39.000000 arcam_fmj-1.5.1/src/arcam/fmj/console.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 15:21:39.000000 arcam_fmj-1.5.1/src/arcam/fmj/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-05-10 15:21:39.000000 arcam_fmj-1.5.1/src/arcam/fmj/server.py
--rw-r--r--   0 runner    (1001) docker     (127)    16212 2024-05-10 15:21:39.000000 arcam_fmj-1.5.1/src/arcam/fmj/state.py
--rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-05-10 15:21:39.000000 arcam_fmj-1.5.1/src/arcam/fmj/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:21:47.133612 arcam_fmj-1.5.1/src/arcam_fmj.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-05-10 15:21:47.000000 arcam_fmj-1.5.1/src/arcam_fmj.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-10 15:21:47.000000 arcam_fmj-1.5.1/src/arcam_fmj.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 15:21:47.000000 arcam_fmj-1.5.1/src/arcam_fmj.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-10 15:21:47.000000 arcam_fmj-1.5.1/src/arcam_fmj.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-10 15:21:47.000000 arcam_fmj-1.5.1/src/arcam_fmj.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-10 15:21:47.000000 arcam_fmj-1.5.1/src/arcam_fmj.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:21:47.133612 arcam_fmj-1.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-05-10 15:21:39.000000 arcam_fmj-1.5.1/tests/test_fake.py
--rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-05-10 15:21:39.000000 arcam_fmj-1.5.1/tests/test_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-05-10 15:21:39.000000 arcam_fmj-1.5.1/tests/test_standard.py
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-05-10 15:21:39.000000 arcam_fmj-1.5.1/tests/test_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     5154 2024-05-10 15:21:39.000000 arcam_fmj-1.5.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:35:28.809664 arcam_fmj-1.5.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-13 18:35:16.000000 arcam_fmj-1.5.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-05-13 18:35:28.809664 arcam_fmj-1.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-13 18:35:16.000000 arcam_fmj-1.5.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-13 18:35:28.809664 arcam_fmj-1.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-13 18:35:16.000000 arcam_fmj-1.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:35:28.801664 arcam_fmj-1.5.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:35:28.801664 arcam_fmj-1.5.2/src/arcam/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:35:28.805664 arcam_fmj-1.5.2/src/arcam/fmj/
+-rw-r--r--   0 runner    (1001) docker     (127)    38139 2024-05-13 18:35:16.000000 arcam_fmj-1.5.2/src/arcam/fmj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7355 2024-05-13 18:35:16.000000 arcam_fmj-1.5.2/src/arcam/fmj/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10656 2024-05-13 18:35:16.000000 arcam_fmj-1.5.2/src/arcam/fmj/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 18:35:16.000000 arcam_fmj-1.5.2/src/arcam/fmj/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-05-13 18:35:16.000000 arcam_fmj-1.5.2/src/arcam/fmj/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16212 2024-05-13 18:35:16.000000 arcam_fmj-1.5.2/src/arcam/fmj/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-05-13 18:35:16.000000 arcam_fmj-1.5.2/src/arcam/fmj/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:35:28.809664 arcam_fmj-1.5.2/src/arcam_fmj.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-05-13 18:35:28.000000 arcam_fmj-1.5.2/src/arcam_fmj.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-13 18:35:28.000000 arcam_fmj-1.5.2/src/arcam_fmj.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 18:35:28.000000 arcam_fmj-1.5.2/src/arcam_fmj.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-13 18:35:28.000000 arcam_fmj-1.5.2/src/arcam_fmj.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-13 18:35:28.000000 arcam_fmj-1.5.2/src/arcam_fmj.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-13 18:35:28.000000 arcam_fmj-1.5.2/src/arcam_fmj.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:35:28.809664 arcam_fmj-1.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-05-13 18:35:16.000000 arcam_fmj-1.5.2/tests/test_fake.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-05-13 18:35:16.000000 arcam_fmj-1.5.2/tests/test_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-05-13 18:35:16.000000 arcam_fmj-1.5.2/tests/test_standard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-05-13 18:35:16.000000 arcam_fmj-1.5.2/tests/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5154 2024-05-13 18:35:16.000000 arcam_fmj-1.5.2/tests/test_utils.py
```

### Comparing `arcam_fmj-1.5.1/LICENSE.txt` & `arcam_fmj-1.5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `arcam_fmj-1.5.1/PKG-INFO` & `arcam_fmj-1.5.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: arcam-fmj
-Version: 1.5.1
+Version: 1.5.2
 Summary: A python library for speaking to Arcam receivers
 Home-page: https://github.com/elupus/arcam_fmj
 Author: Joakim Plate
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Environment :: Plugins
 Classifier: Framework :: AsyncIO
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 Requires-Dist: attrs>18.1
-Requires-Dist: async
 Provides-Extra: tests
 Requires-Dist: pytest>3.6.4; extra == "tests"
 Requires-Dist: pytest-asyncio==0.21.2; extra == "tests"
 Requires-Dist: pytest-aiohttp>=1.0.0; extra == "tests"
 Requires-Dist: pytest-cov>=3.0.0; extra == "tests"
 Requires-Dist: coveralls; extra == "tests"
 Requires-Dist: pytest-mock; extra == "tests"
```

### Comparing `arcam_fmj-1.5.1/README.rst` & `arcam_fmj-1.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `arcam_fmj-1.5.1/setup.py` & `arcam_fmj-1.5.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,27 +5,27 @@
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.rst"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="arcam-fmj",
-    version="1.5.1",
+    version="1.5.2",
     description="A python library for speaking to Arcam receivers",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     license="MIT",
     packages=["arcam.fmj"],
     package_dir={"": "src"},
     package_data = {
         'arcam.fmj': ['py.typed'],
     },
     python_requires=">=3.8",
     author="Joakim Plate",
-    install_requires=["attrs>18.1", "async"],
+    install_requires=["attrs>18.1"],
     extras_require={
         "tests": [
             "pytest>3.6.4",
             "pytest-asyncio==0.21.2",
             "pytest-aiohttp>=1.0.0",
             "pytest-cov>=3.0.0",
             "coveralls",
```

### Comparing `arcam_fmj-1.5.1/src/arcam/fmj/__init__.py` & `arcam_fmj-1.5.2/src/arcam/fmj/__init__.py`

 * *Files identical despite different names*

### Comparing `arcam_fmj-1.5.1/src/arcam/fmj/client.py` & `arcam_fmj-1.5.2/src/arcam/fmj/client.py`

 * *Files identical despite different names*

### Comparing `arcam_fmj-1.5.1/src/arcam/fmj/console.py` & `arcam_fmj-1.5.2/src/arcam/fmj/console.py`

 * *Files identical despite different names*

### Comparing `arcam_fmj-1.5.1/src/arcam/fmj/server.py` & `arcam_fmj-1.5.2/src/arcam/fmj/server.py`

 * *Files identical despite different names*

### Comparing `arcam_fmj-1.5.1/src/arcam/fmj/state.py` & `arcam_fmj-1.5.2/src/arcam/fmj/state.py`

 * *Files identical despite different names*

### Comparing `arcam_fmj-1.5.1/src/arcam/fmj/utils.py` & `arcam_fmj-1.5.2/src/arcam/fmj/utils.py`

 * *Files identical despite different names*

### Comparing `arcam_fmj-1.5.1/src/arcam_fmj.egg-info/PKG-INFO` & `arcam_fmj-1.5.2/src/arcam_fmj.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: arcam-fmj
-Version: 1.5.1
+Version: 1.5.2
 Summary: A python library for speaking to Arcam receivers
 Home-page: https://github.com/elupus/arcam_fmj
 Author: Joakim Plate
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Environment :: Plugins
 Classifier: Framework :: AsyncIO
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 Requires-Dist: attrs>18.1
-Requires-Dist: async
 Provides-Extra: tests
 Requires-Dist: pytest>3.6.4; extra == "tests"
 Requires-Dist: pytest-asyncio==0.21.2; extra == "tests"
 Requires-Dist: pytest-aiohttp>=1.0.0; extra == "tests"
 Requires-Dist: pytest-cov>=3.0.0; extra == "tests"
 Requires-Dist: coveralls; extra == "tests"
 Requires-Dist: pytest-mock; extra == "tests"
```

### Comparing `arcam_fmj-1.5.1/src/arcam_fmj.egg-info/SOURCES.txt` & `arcam_fmj-1.5.2/src/arcam_fmj.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arcam_fmj-1.5.1/tests/test_fake.py` & `arcam_fmj-1.5.2/tests/test_fake.py`

 * *Files identical despite different names*

### Comparing `arcam_fmj-1.5.1/tests/test_source.py` & `arcam_fmj-1.5.2/tests/test_source.py`

 * *Files identical despite different names*

### Comparing `arcam_fmj-1.5.1/tests/test_standard.py` & `arcam_fmj-1.5.2/tests/test_standard.py`

 * *Files identical despite different names*

### Comparing `arcam_fmj-1.5.1/tests/test_state.py` & `arcam_fmj-1.5.2/tests/test_state.py`

 * *Files identical despite different names*

### Comparing `arcam_fmj-1.5.1/tests/test_utils.py` & `arcam_fmj-1.5.2/tests/test_utils.py`

 * *Files identical despite different names*

