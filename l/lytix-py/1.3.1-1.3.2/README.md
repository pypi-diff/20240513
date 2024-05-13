# Comparing `tmp/lytix_py-1.3.1.tar.gz` & `tmp/lytix_py-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lytix_py-1.3.1.tar", last modified: Mon May 13 18:41:16 2024, max compression
+gzip compressed data, was "lytix_py-1.3.2.tar", last modified: Mon May 13 18:46:20 2024, max compression
```

## Comparing `lytix_py-1.3.1.tar` & `lytix_py-1.3.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-13 18:41:16.505933 lytix_py-1.3.1/
--rw-r--r--   0 sidpremkumar   (501) staff       (20)     1081 2024-05-05 21:16:18.000000 lytix_py-1.3.1/LICENSE.md
--rw-r--r--   0 sidpremkumar   (501) staff       (20)     1008 2024-05-13 18:41:16.505732 lytix_py-1.3.1/PKG-INFO
--rw-r--r--   0 sidpremkumar   (501) staff       (20)      450 2024-05-05 21:16:53.000000 lytix_py-1.3.1/README.md
--rw-r--r--   0 sidpremkumar   (501) staff       (20)      625 2024-05-13 18:41:12.000000 lytix_py-1.3.1/pyproject.toml
--rw-r--r--   0 sidpremkumar   (501) staff       (20)       38 2024-05-13 18:41:16.505974 lytix_py-1.3.1/setup.cfg
-drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-13 18:41:16.502986 lytix_py-1.3.1/src/
-drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-13 18:41:16.503924 lytix_py-1.3.1/src/lytix_py/
-drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-13 18:41:16.505061 lytix_py-1.3.1/src/lytix_py/LLLogger/
--rw-r--r--   0 sidpremkumar   (501) staff       (20)      886 2024-05-06 00:20:17.000000 lytix_py-1.3.1/src/lytix_py/LLLogger/LLLogger.py
-drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-13 18:41:16.505188 lytix_py-1.3.1/src/lytix_py/MetricCollector/
--rw-r--r--   0 sidpremkumar   (501) staff       (20)     2652 2024-05-13 18:39:50.000000 lytix_py-1.3.1/src/lytix_py/MetricCollector/MetricCollector.py
--rw-r--r--   0 sidpremkumar   (501) staff       (20)      133 2024-05-13 18:41:07.000000 lytix_py-1.3.1/src/lytix_py/__init__.py
--rw-r--r--   0 sidpremkumar   (501) staff       (20)      575 2024-05-13 18:39:42.000000 lytix_py-1.3.1/src/lytix_py/envVars.py
-drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-13 18:41:16.505503 lytix_py-1.3.1/src/lytix_py.egg-info/
--rw-r--r--   0 sidpremkumar   (501) staff       (20)     1008 2024-05-13 18:41:16.000000 lytix_py-1.3.1/src/lytix_py.egg-info/PKG-INFO
--rw-r--r--   0 sidpremkumar   (501) staff       (20)      345 2024-05-13 18:41:16.000000 lytix_py-1.3.1/src/lytix_py.egg-info/SOURCES.txt
--rw-r--r--   0 sidpremkumar   (501) staff       (20)        1 2024-05-13 18:41:16.000000 lytix_py-1.3.1/src/lytix_py.egg-info/dependency_links.txt
--rw-r--r--   0 sidpremkumar   (501) staff       (20)       32 2024-05-13 18:41:16.000000 lytix_py-1.3.1/src/lytix_py.egg-info/requires.txt
--rw-r--r--   0 sidpremkumar   (501) staff       (20)        9 2024-05-13 18:41:16.000000 lytix_py-1.3.1/src/lytix_py.egg-info/top_level.txt
+drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-13 18:46:20.158022 lytix_py-1.3.2/
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)     1081 2024-05-05 21:16:18.000000 lytix_py-1.3.2/LICENSE.md
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)     1008 2024-05-13 18:46:20.157791 lytix_py-1.3.2/PKG-INFO
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)      450 2024-05-05 21:16:53.000000 lytix_py-1.3.2/README.md
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)      625 2024-05-13 18:43:01.000000 lytix_py-1.3.2/pyproject.toml
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)       38 2024-05-13 18:46:20.158071 lytix_py-1.3.2/setup.cfg
+drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-13 18:46:20.155857 lytix_py-1.3.2/src/
+drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-13 18:46:20.156573 lytix_py-1.3.2/src/lytix_py/
+drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-13 18:46:20.157252 lytix_py-1.3.2/src/lytix_py/LLLogger/
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)      886 2024-05-06 00:20:17.000000 lytix_py-1.3.2/src/lytix_py/LLLogger/LLLogger.py
+drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-13 18:46:20.157371 lytix_py-1.3.2/src/lytix_py/MetricCollector/
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)     2794 2024-05-13 18:46:14.000000 lytix_py-1.3.2/src/lytix_py/MetricCollector/MetricCollector.py
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)      133 2024-05-13 18:41:07.000000 lytix_py-1.3.2/src/lytix_py/__init__.py
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)      575 2024-05-13 18:39:42.000000 lytix_py-1.3.2/src/lytix_py/envVars.py
+drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-13 18:46:20.157552 lytix_py-1.3.2/src/lytix_py.egg-info/
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)     1008 2024-05-13 18:46:20.000000 lytix_py-1.3.2/src/lytix_py.egg-info/PKG-INFO
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)      345 2024-05-13 18:46:20.000000 lytix_py-1.3.2/src/lytix_py.egg-info/SOURCES.txt
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)        1 2024-05-13 18:46:20.000000 lytix_py-1.3.2/src/lytix_py.egg-info/dependency_links.txt
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)       32 2024-05-13 18:46:20.000000 lytix_py-1.3.2/src/lytix_py.egg-info/requires.txt
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)        9 2024-05-13 18:46:20.000000 lytix_py-1.3.2/src/lytix_py.egg-info/top_level.txt
```

### Comparing `lytix_py-1.3.1/LICENSE.md` & `lytix_py-1.3.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lytix_py-1.3.1/PKG-INFO` & `lytix_py-1.3.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lytix-py
-Version: 1.3.1
+Version: 1.3.2
 Summary: Official Lytix Client Packages
 Author-email: Lytix <support@lytix.com>
 Project-URL: Homepage, https://github.com/Lytix-Labs/lytix-py
 Project-URL: Issues, https://github.com/Lytix-Labs/lytix-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lytix_py-1.3.1/pyproject.toml` & `lytix_py-1.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lytix-py"
-version = "1.3.1"
+version = "1.3.2"
 authors = [
   { name="Lytix", email="support@lytix.com" },
 ]
 description = "Official Lytix Client Packages"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `lytix_py-1.3.1/src/lytix_py/LLLogger/LLLogger.py` & `lytix_py-1.3.2/src/lytix_py/LLLogger/LLLogger.py`

 * *Files identical despite different names*

### Comparing `lytix_py-1.3.1/src/lytix_py/MetricCollector/MetricCollector.py` & `lytix_py-1.3.2/src/lytix_py/MetricCollector/MetricCollector.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,68 +5,75 @@
 from lytix_py.envVars import LytixCreds
 
 """
  Main class to collect and report metrics
  back to HQ
 """
 class _MetricCollector:
-    _apiKey: str = None
     _baseURL: str = None
     # _logger: str = None
 
     def __init__(self):
-        self._apiKey = LytixCreds.LX_API_KEY
         self._baseURL = urljoin(LytixCreds.LX_BASE_URL, "/v1/metrics")
         pass
 
 
     """
     Interal wrapper to send a post request
     """
     def _sendPostRequest(self, endpoint: str, body: dict):
         url = os.path.join(self._baseURL, endpoint)
         headers = {
             "Content-Type": "application/json",
-            "lx-api-key": self._apiKey,
+            "lx-api-key": LytixCreds.LX_API_KEY,
         }
         response = requests.post(url, headers=headers, json=body)
         if (response.status_code != 200):
             print(f"Failed to send post request to {url} with status code {response.status_code} and response {response.text}")
 
     """
     Increment a given metric
     """
     def increment(self, metricName: str, metricValue: int = 1, metricMetadata: dict = None):
+        if LytixCreds.LX_API_KEY is None: 
+            return 
+
         if metricMetadata is None:
             metricMetadata = {}
         body = {
             "metricName": metricName,
             "metricValue": metricValue,
             "metadata": metricMetadata
         }
         self._sendPostRequest("increment", body)
 
     """
     Capture a model input/output
     """
     def captureModelIO(self, modelName: str, userInput: str, modelOutput: str, metricMetadata: dict = None):
+        if LytixCreds.LX_API_KEY is None: 
+            return 
+
         if metricMetadata is None:
             metricMetadata = {}
         body = {
             "modelName": modelName,
             "userInput": userInput,
             "modelOutput": modelOutput,
             "metricMetadata": metricMetadata
         }
         self._sendPostRequest("modelIO", body)
 
     """
     Capture a model io event while also capturing the time to respond
     """
     def captureModelTrace(self, modelName: str, userInput: str, callback, metricMetadata: dict = None):
+        if LytixCreds.LX_API_KEY is None: 
+            return callback()
+
         startTime = time.time()
         modelOutput = callback()
         try:
             responseTime = int((time.time() - startTime) * 1000)  # Convert to milliseconds
             # Capture modelIO event along with the response time
             self.captureModelIO(modelName, userInput, modelOutput, metricMetadata)
             self.increment("model.responseTime", responseTime, {"modelName": modelName})
```

### Comparing `lytix_py-1.3.1/src/lytix_py/envVars.py` & `lytix_py-1.3.2/src/lytix_py/envVars.py`

 * *Files identical despite different names*

### Comparing `lytix_py-1.3.1/src/lytix_py.egg-info/PKG-INFO` & `lytix_py-1.3.2/src/lytix_py.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lytix-py
-Version: 1.3.1
+Version: 1.3.2
 Summary: Official Lytix Client Packages
 Author-email: Lytix <support@lytix.com>
 Project-URL: Homepage, https://github.com/Lytix-Labs/lytix-py
 Project-URL: Issues, https://github.com/Lytix-Labs/lytix-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

