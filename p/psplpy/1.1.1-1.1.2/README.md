# Comparing `tmp/psplpy-1.1.1.tar.gz` & `tmp/psplpy-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psplpy-1.1.1.tar", last modified: Sun May 12 15:22:54 2024, max compression
+gzip compressed data, was "psplpy-1.1.2.tar", last modified: Sun May 12 23:19:33 2024, max compression
```

## Comparing `psplpy-1.1.1.tar` & `psplpy-1.1.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 a         (1000) a         (1000)        0 2024-05-12 15:22:54.723680 psplpy-1.1.1/
--rw-r--r--   0 a         (1000) a         (1000)      530 2024-05-12 15:22:54.723680 psplpy-1.1.1/PKG-INFO
--rwxr-xr-x   0 a         (1000) a         (1000)      213 2024-04-30 14:21:49.000000 psplpy-1.1.1/README.md
-drwxr-xr-x   0 a         (1000) a         (1000)        0 2024-05-12 15:22:54.719680 psplpy-1.1.1/psplpy/
--rwxr-xr-x   0 a         (1000) a         (1000)       80 2024-04-30 14:21:49.000000 psplpy-1.1.1/psplpy/__init__.py
--rwxr-xr-x   0 a         (1000) a         (1000)     2339 2024-04-30 14:21:49.000000 psplpy-1.1.1/psplpy/concurrency_utils.py
--rwxr-xr-x   0 a         (1000) a         (1000)     4387 2024-05-12 15:18:12.000000 psplpy-1.1.1/psplpy/dynamic_compose.py
--rwxr-xr-x   0 a         (1000) a         (1000)      932 2024-04-30 14:21:49.000000 psplpy-1.1.1/psplpy/file_utils.py
--rwxr-xr-x   0 a         (1000) a         (1000)    16862 2024-04-30 14:21:49.000000 psplpy-1.1.1/psplpy/image_utils.py
--rwxr-xr-x   0 a         (1000) a         (1000)     3579 2024-04-30 14:21:49.000000 psplpy-1.1.1/psplpy/middleware_utils.py
--rwxr-xr-x   0 a         (1000) a         (1000)     3984 2024-05-12 14:43:27.000000 psplpy-1.1.1/psplpy/network_utils.py
--rwxr-xr-x   0 a         (1000) a         (1000)      959 2024-04-30 14:21:49.000000 psplpy-1.1.1/psplpy/other_utils.py
-drwxr-xr-x   0 a         (1000) a         (1000)        0 2024-05-12 15:22:54.719680 psplpy-1.1.1/psplpy/scripts/
--rwxr-xr-x   0 a         (1000) a         (1000)     4316 2024-04-30 14:21:49.000000 psplpy-1.1.1/psplpy/scripts/block_jetbrains.py
--rwxr-xr-x   0 a         (1000) a         (1000)     1194 2024-04-30 14:21:49.000000 psplpy-1.1.1/psplpy/scripts/upload_pypi_project.py
--rwxr-xr-x   0 a         (1000) a         (1000)     8500 2024-04-30 14:21:49.000000 psplpy-1.1.1/psplpy/serialization_utils.py
-drwxr-xr-x   0 a         (1000) a         (1000)        0 2024-05-12 15:22:54.723680 psplpy-1.1.1/psplpy.egg-info/
--rw-r--r--   0 a         (1000) a         (1000)      530 2024-05-12 15:22:54.000000 psplpy-1.1.1/psplpy.egg-info/PKG-INFO
--rwxr-xr-x   0 a         (1000) a         (1000)      681 2024-05-12 15:22:54.000000 psplpy-1.1.1/psplpy.egg-info/SOURCES.txt
--rwxr-xr-x   0 a         (1000) a         (1000)        1 2024-05-12 15:22:54.000000 psplpy-1.1.1/psplpy.egg-info/dependency_links.txt
--rwxr-xr-x   0 a         (1000) a         (1000)        7 2024-05-12 15:22:54.000000 psplpy-1.1.1/psplpy.egg-info/top_level.txt
--rwxr-xr-x   0 a         (1000) a         (1000)      423 2024-05-12 15:21:15.000000 psplpy-1.1.1/pyproject.toml
--rw-r--r--   0 a         (1000) a         (1000)       38 2024-05-12 15:22:54.723680 psplpy-1.1.1/setup.cfg
-drwxr-xr-x   0 a         (1000) a         (1000)        0 2024-05-12 15:22:54.723680 psplpy-1.1.1/tests/
--rwxr-xr-x   0 a         (1000) a         (1000)      909 2024-04-30 14:21:49.000000 psplpy-1.1.1/tests/test.py
--rwxr-xr-x   0 a         (1000) a         (1000)      873 2024-04-30 14:21:49.000000 psplpy-1.1.1/tests/test_concurrency_utils.py
--rwxr-xr-x   0 a         (1000) a         (1000)      830 2024-05-12 15:16:14.000000 psplpy-1.1.1/tests/test_dynamic_compose.py
--rwxr-xr-x   0 a         (1000) a         (1000)      464 2024-04-30 14:21:49.000000 psplpy-1.1.1/tests/test_file_utils.py
--rwxr-xr-x   0 a         (1000) a         (1000)     4448 2024-04-30 14:21:49.000000 psplpy-1.1.1/tests/test_image_utils.py
--rwxr-xr-x   0 a         (1000) a         (1000)     3001 2024-04-30 14:21:49.000000 psplpy-1.1.1/tests/test_middleware_utils.py
--rwxr-xr-x   0 a         (1000) a         (1000)     1659 2024-05-12 14:34:29.000000 psplpy-1.1.1/tests/test_network_utils.py
--rwxr-xr-x   0 a         (1000) a         (1000)      478 2024-04-30 14:21:49.000000 psplpy-1.1.1/tests/test_other_utils.py
--rwxr-xr-x   0 a         (1000) a         (1000)     5480 2024-04-30 14:21:49.000000 psplpy-1.1.1/tests/test_serialization_utils.py
+drwxr-xr-x   0 a         (1000) a         (1000)        0 2024-05-12 23:19:33.689577 psplpy-1.1.2/
+-rw-r--r--   0 a         (1000) a         (1000)      530 2024-05-12 23:19:33.689577 psplpy-1.1.2/PKG-INFO
+-rwxr-xr-x   0 a         (1000) a         (1000)      213 2024-04-30 14:21:49.000000 psplpy-1.1.2/README.md
+drwxr-xr-x   0 a         (1000) a         (1000)        0 2024-05-12 23:19:33.689577 psplpy-1.1.2/psplpy/
+-rwxr-xr-x   0 a         (1000) a         (1000)       80 2024-04-30 14:21:49.000000 psplpy-1.1.2/psplpy/__init__.py
+-rwxr-xr-x   0 a         (1000) a         (1000)     2339 2024-04-30 14:21:49.000000 psplpy-1.1.2/psplpy/concurrency_utils.py
+-rwxr-xr-x   0 a         (1000) a         (1000)     4399 2024-05-12 19:22:53.000000 psplpy-1.1.2/psplpy/dynamic_compose.py
+-rwxr-xr-x   0 a         (1000) a         (1000)      932 2024-04-30 14:21:49.000000 psplpy-1.1.2/psplpy/file_utils.py
+-rwxr-xr-x   0 a         (1000) a         (1000)    16862 2024-04-30 14:21:49.000000 psplpy-1.1.2/psplpy/image_utils.py
+-rwxr-xr-x   0 a         (1000) a         (1000)     3579 2024-04-30 14:21:49.000000 psplpy-1.1.2/psplpy/middleware_utils.py
+-rwxr-xr-x   0 a         (1000) a         (1000)     3984 2024-05-12 14:43:27.000000 psplpy-1.1.2/psplpy/network_utils.py
+-rwxr-xr-x   0 a         (1000) a         (1000)      959 2024-04-30 14:21:49.000000 psplpy-1.1.2/psplpy/other_utils.py
+drwxr-xr-x   0 a         (1000) a         (1000)        0 2024-05-12 23:19:33.689577 psplpy-1.1.2/psplpy/scripts/
+-rwxr-xr-x   0 a         (1000) a         (1000)     4316 2024-04-30 14:21:49.000000 psplpy-1.1.2/psplpy/scripts/block_jetbrains.py
+-rwxr-xr-x   0 a         (1000) a         (1000)     1194 2024-04-30 14:21:49.000000 psplpy-1.1.2/psplpy/scripts/upload_pypi_project.py
+-rwxr-xr-x   0 a         (1000) a         (1000)     8500 2024-04-30 14:21:49.000000 psplpy-1.1.2/psplpy/serialization_utils.py
+drwxr-xr-x   0 a         (1000) a         (1000)        0 2024-05-12 23:19:33.689577 psplpy-1.1.2/psplpy.egg-info/
+-rw-r--r--   0 a         (1000) a         (1000)      530 2024-05-12 23:19:33.000000 psplpy-1.1.2/psplpy.egg-info/PKG-INFO
+-rwxr-xr-x   0 a         (1000) a         (1000)      681 2024-05-12 23:19:33.000000 psplpy-1.1.2/psplpy.egg-info/SOURCES.txt
+-rwxr-xr-x   0 a         (1000) a         (1000)        1 2024-05-12 23:19:33.000000 psplpy-1.1.2/psplpy.egg-info/dependency_links.txt
+-rwxr-xr-x   0 a         (1000) a         (1000)        7 2024-05-12 23:19:33.000000 psplpy-1.1.2/psplpy.egg-info/top_level.txt
+-rwxr-xr-x   0 a         (1000) a         (1000)      423 2024-05-12 19:20:29.000000 psplpy-1.1.2/pyproject.toml
+-rw-r--r--   0 a         (1000) a         (1000)       38 2024-05-12 23:19:33.689577 psplpy-1.1.2/setup.cfg
+drwxr-xr-x   0 a         (1000) a         (1000)        0 2024-05-12 23:19:33.689577 psplpy-1.1.2/tests/
+-rwxr-xr-x   0 a         (1000) a         (1000)      909 2024-04-30 14:21:49.000000 psplpy-1.1.2/tests/test.py
+-rwxr-xr-x   0 a         (1000) a         (1000)      873 2024-04-30 14:21:49.000000 psplpy-1.1.2/tests/test_concurrency_utils.py
+-rwxr-xr-x   0 a         (1000) a         (1000)      848 2024-05-12 19:23:08.000000 psplpy-1.1.2/tests/test_dynamic_compose.py
+-rwxr-xr-x   0 a         (1000) a         (1000)      464 2024-04-30 14:21:49.000000 psplpy-1.1.2/tests/test_file_utils.py
+-rwxr-xr-x   0 a         (1000) a         (1000)     4448 2024-04-30 14:21:49.000000 psplpy-1.1.2/tests/test_image_utils.py
+-rwxr-xr-x   0 a         (1000) a         (1000)     3001 2024-04-30 14:21:49.000000 psplpy-1.1.2/tests/test_middleware_utils.py
+-rwxr-xr-x   0 a         (1000) a         (1000)     1659 2024-05-12 14:34:29.000000 psplpy-1.1.2/tests/test_network_utils.py
+-rwxr-xr-x   0 a         (1000) a         (1000)      478 2024-04-30 14:21:49.000000 psplpy-1.1.2/tests/test_other_utils.py
+-rwxr-xr-x   0 a         (1000) a         (1000)     5480 2024-04-30 14:21:49.000000 psplpy-1.1.2/tests/test_serialization_utils.py
```

### Comparing `psplpy-1.1.1/PKG-INFO` & `psplpy-1.1.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psplpy
-Version: 1.1.1
+Version: 1.1.2
 Summary: The Personal Study Purposes Library of PYthon.
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `psplpy-1.1.1/psplpy/concurrency_utils.py` & `psplpy-1.1.2/psplpy/concurrency_utils.py`

 * *Files identical despite different names*

### Comparing `psplpy-1.1.1/psplpy/dynamic_compose.py` & `psplpy-1.1.2/psplpy/dynamic_compose.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
         self.env = self._get_env()
         args, self.extra_args = self._get_args()
         self.env.update(dict(args.e or ()))
 
     @staticmethod
     def _parse_key_value(arg_string: str):
-        key, value = arg_string.strip().split('=')
+        key, value = arg_string.strip().split('=', maxsplit=1)
         return key, value
 
     def _get_env(self):
         env_dict = {}
         if self.env_file.exists():
             with open(self.env_file) as f:
                 for line in f.readlines():
```

### Comparing `psplpy-1.1.1/psplpy/file_utils.py` & `psplpy-1.1.2/psplpy/file_utils.py`

 * *Files identical despite different names*

### Comparing `psplpy-1.1.1/psplpy/image_utils.py` & `psplpy-1.1.2/psplpy/image_utils.py`

 * *Files identical despite different names*

### Comparing `psplpy-1.1.1/psplpy/middleware_utils.py` & `psplpy-1.1.2/psplpy/middleware_utils.py`

 * *Files identical despite different names*

### Comparing `psplpy-1.1.1/psplpy/network_utils.py` & `psplpy-1.1.2/psplpy/network_utils.py`

 * *Files identical despite different names*

### Comparing `psplpy-1.1.1/psplpy/other_utils.py` & `psplpy-1.1.2/psplpy/other_utils.py`

 * *Files identical despite different names*

### Comparing `psplpy-1.1.1/psplpy/scripts/block_jetbrains.py` & `psplpy-1.1.2/psplpy/scripts/block_jetbrains.py`

 * *Files identical despite different names*

### Comparing `psplpy-1.1.1/psplpy/scripts/upload_pypi_project.py` & `psplpy-1.1.2/psplpy/scripts/upload_pypi_project.py`

 * *Files identical despite different names*

### Comparing `psplpy-1.1.1/psplpy/serialization_utils.py` & `psplpy-1.1.2/psplpy/serialization_utils.py`

 * *Files identical despite different names*

### Comparing `psplpy-1.1.1/psplpy.egg-info/PKG-INFO` & `psplpy-1.1.2/psplpy.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psplpy
-Version: 1.1.1
+Version: 1.1.2
 Summary: The Personal Study Purposes Library of PYthon.
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `psplpy-1.1.1/psplpy.egg-info/SOURCES.txt` & `psplpy-1.1.2/psplpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `psplpy-1.1.1/tests/test.py` & `psplpy-1.1.2/tests/test.py`

 * *Files identical despite different names*

### Comparing `psplpy-1.1.1/tests/test_concurrency_utils.py` & `psplpy-1.1.2/tests/test_concurrency_utils.py`

 * *Files identical despite different names*

### Comparing `psplpy-1.1.1/tests/test_dynamic_compose.py` & `psplpy-1.1.2/tests/test_dynamic_compose.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 compose_dumped_file = dc_compose_dir / 'compose-dumped.yml'
 dockerfile_dumped_file = dc_compose_dir / 'Dockerfile-dumped'
 
 
 def tests():
     DynamicCompose.CWD = dc_rc_dir
     dc = DynamicCompose()
+    print(dc.env)
     dc.compose_dir = dc_compose_dir
 
     dc.format_compose()
     dc.format_dockerfile()
     dc.dump()
 
     assert compose_dumped_file.read_text().strip() == dc.compose_file.read_text().strip()
```

### Comparing `psplpy-1.1.1/tests/test_image_utils.py` & `psplpy-1.1.2/tests/test_image_utils.py`

 * *Files identical despite different names*

### Comparing `psplpy-1.1.1/tests/test_middleware_utils.py` & `psplpy-1.1.2/tests/test_middleware_utils.py`

 * *Files identical despite different names*

### Comparing `psplpy-1.1.1/tests/test_network_utils.py` & `psplpy-1.1.2/tests/test_network_utils.py`

 * *Files identical despite different names*

### Comparing `psplpy-1.1.1/tests/test_serialization_utils.py` & `psplpy-1.1.2/tests/test_serialization_utils.py`

 * *Files identical despite different names*

