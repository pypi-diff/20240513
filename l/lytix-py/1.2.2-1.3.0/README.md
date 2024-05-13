# Comparing `tmp/lytix_py-1.2.2.tar.gz` & `tmp/lytix_py-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lytix_py-1.2.2.tar", last modified: Sat May 11 21:32:09 2024, max compression
+gzip compressed data, was "lytix_py-1.3.0.tar", last modified: Mon May 13 18:40:10 2024, max compression
```

## Comparing `lytix_py-1.2.2.tar` & `lytix_py-1.3.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-11 21:32:09.736040 lytix_py-1.2.2/
--rw-r--r--   0 sidpremkumar   (501) staff       (20)     1081 2024-05-05 21:16:18.000000 lytix_py-1.2.2/LICENSE.md
--rw-r--r--   0 sidpremkumar   (501) staff       (20)     1008 2024-05-11 21:32:09.735719 lytix_py-1.2.2/PKG-INFO
--rw-r--r--   0 sidpremkumar   (501) staff       (20)      450 2024-05-05 21:16:53.000000 lytix_py-1.2.2/README.md
--rw-r--r--   0 sidpremkumar   (501) staff       (20)      625 2024-05-11 21:32:04.000000 lytix_py-1.2.2/pyproject.toml
--rw-r--r--   0 sidpremkumar   (501) staff       (20)       38 2024-05-11 21:32:09.736104 lytix_py-1.2.2/setup.cfg
-drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-11 21:32:09.732923 lytix_py-1.2.2/src/
-drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-11 21:32:09.734058 lytix_py-1.2.2/src/lytix_py/
-drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-11 21:32:09.734800 lytix_py-1.2.2/src/lytix_py/LLLogger/
--rw-r--r--   0 sidpremkumar   (501) staff       (20)      886 2024-05-06 00:20:17.000000 lytix_py-1.2.2/src/lytix_py/LLLogger/LLLogger.py
-drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-11 21:32:09.734953 lytix_py-1.2.2/src/lytix_py/MetricCollector/
--rw-r--r--   0 sidpremkumar   (501) staff       (20)     2643 2024-05-11 21:29:45.000000 lytix_py-1.2.2/src/lytix_py/MetricCollector/MetricCollector.py
--rw-r--r--   0 sidpremkumar   (501) staff       (20)      102 2024-05-07 21:15:04.000000 lytix_py-1.2.2/src/lytix_py/__init__.py
--rw-r--r--   0 sidpremkumar   (501) staff       (20)      403 2024-05-05 21:48:37.000000 lytix_py-1.2.2/src/lytix_py/envVars.py
-drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-11 21:32:09.735419 lytix_py-1.2.2/src/lytix_py.egg-info/
--rw-r--r--   0 sidpremkumar   (501) staff       (20)     1008 2024-05-11 21:32:09.000000 lytix_py-1.2.2/src/lytix_py.egg-info/PKG-INFO
--rw-r--r--   0 sidpremkumar   (501) staff       (20)      345 2024-05-11 21:32:09.000000 lytix_py-1.2.2/src/lytix_py.egg-info/SOURCES.txt
--rw-r--r--   0 sidpremkumar   (501) staff       (20)        1 2024-05-11 21:32:09.000000 lytix_py-1.2.2/src/lytix_py.egg-info/dependency_links.txt
--rw-r--r--   0 sidpremkumar   (501) staff       (20)       32 2024-05-11 21:32:09.000000 lytix_py-1.2.2/src/lytix_py.egg-info/requires.txt
--rw-r--r--   0 sidpremkumar   (501) staff       (20)        9 2024-05-11 21:32:09.000000 lytix_py-1.2.2/src/lytix_py.egg-info/top_level.txt
+drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-13 18:40:10.096819 lytix_py-1.3.0/
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)     1081 2024-05-05 21:16:18.000000 lytix_py-1.3.0/LICENSE.md
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)     1008 2024-05-13 18:40:10.096591 lytix_py-1.3.0/PKG-INFO
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)      450 2024-05-05 21:16:53.000000 lytix_py-1.3.0/README.md
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)      625 2024-05-13 18:39:59.000000 lytix_py-1.3.0/pyproject.toml
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)       38 2024-05-13 18:40:10.096861 lytix_py-1.3.0/setup.cfg
+drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-13 18:40:10.094345 lytix_py-1.3.0/src/
+drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-13 18:40:10.095116 lytix_py-1.3.0/src/lytix_py/
+drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-13 18:40:10.095993 lytix_py-1.3.0/src/lytix_py/LLLogger/
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)      886 2024-05-06 00:20:17.000000 lytix_py-1.3.0/src/lytix_py/LLLogger/LLLogger.py
+drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-13 18:40:10.096131 lytix_py-1.3.0/src/lytix_py/MetricCollector/
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)     2652 2024-05-13 18:39:50.000000 lytix_py-1.3.0/src/lytix_py/MetricCollector/MetricCollector.py
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)      133 2024-05-13 18:39:31.000000 lytix_py-1.3.0/src/lytix_py/__init__.py
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)      575 2024-05-13 18:39:42.000000 lytix_py-1.3.0/src/lytix_py/envVars.py
+drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-13 18:40:10.096323 lytix_py-1.3.0/src/lytix_py.egg-info/
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)     1008 2024-05-13 18:40:10.000000 lytix_py-1.3.0/src/lytix_py.egg-info/PKG-INFO
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)      345 2024-05-13 18:40:10.000000 lytix_py-1.3.0/src/lytix_py.egg-info/SOURCES.txt
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)        1 2024-05-13 18:40:10.000000 lytix_py-1.3.0/src/lytix_py.egg-info/dependency_links.txt
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)       32 2024-05-13 18:40:10.000000 lytix_py-1.3.0/src/lytix_py.egg-info/requires.txt
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)        9 2024-05-13 18:40:10.000000 lytix_py-1.3.0/src/lytix_py.egg-info/top_level.txt
```

### Comparing `lytix_py-1.2.2/LICENSE.md` & `lytix_py-1.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lytix_py-1.2.2/PKG-INFO` & `lytix_py-1.3.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lytix-py
-Version: 1.2.2
+Version: 1.3.0
 Summary: Official Lytix Client Packages
 Author-email: Lytix <support@lytix.com>
 Project-URL: Homepage, https://github.com/Lytix-Labs/lytix-py
 Project-URL: Issues, https://github.com/Lytix-Labs/lytix-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lytix_py-1.2.2/pyproject.toml` & `lytix_py-1.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lytix-py"
-version = "1.2.2"
+version = "1.3.0"
 authors = [
   { name="Lytix", email="support@lytix.com" },
 ]
 description = "Official Lytix Client Packages"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `lytix_py-1.2.2/src/lytix_py/LLLogger/LLLogger.py` & `lytix_py-1.3.0/src/lytix_py/LLLogger/LLLogger.py`

 * *Files identical despite different names*

### Comparing `lytix_py-1.2.2/src/lytix_py/MetricCollector/MetricCollector.py` & `lytix_py-1.3.0/src/lytix_py/MetricCollector/MetricCollector.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import requests
 from urllib.parse import urljoin
-from lytix_py.envVars import LX_API_KEY, LX_BASE_URL
 import os.path
 import time
+from lytix_py.envVars import LytixCreds
 
 """
  Main class to collect and report metrics
  back to HQ
 """
 class _MetricCollector:
     _apiKey: str = None
     _baseURL: str = None
     # _logger: str = None
 
     def __init__(self):
-        self._apiKey = LX_API_KEY
-        self._baseURL = urljoin(LX_BASE_URL, "/v1/metrics")
+        self._apiKey = LytixCreds.LX_API_KEY
+        self._baseURL = urljoin(LytixCreds.LX_BASE_URL, "/v1/metrics")
         pass
 
 
     """
     Interal wrapper to send a post request
     """
     def _sendPostRequest(self, endpoint: str, body: dict):
```

### Comparing `lytix_py-1.2.2/src/lytix_py.egg-info/PKG-INFO` & `lytix_py-1.3.0/src/lytix_py.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lytix-py
-Version: 1.2.2
+Version: 1.3.0
 Summary: Official Lytix Client Packages
 Author-email: Lytix <support@lytix.com>
 Project-URL: Homepage, https://github.com/Lytix-Labs/lytix-py
 Project-URL: Issues, https://github.com/Lytix-Labs/lytix-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

