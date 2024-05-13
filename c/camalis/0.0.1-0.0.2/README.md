# Comparing `tmp/camalis-0.0.1.tar.gz` & `tmp/camalis-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "camalis-0.0.1.tar", max compression
+gzip compressed data, was "camalis-0.0.2.tar", max compression
```

## Comparing `camalis-0.0.1.tar` & `camalis-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      113 2024-05-09 14:48:58.269856 camalis-0.0.1/camalis/__init__.py
--rw-r--r--   0        0        0     1332 2024-05-09 13:53:09.835202 camalis-0.0.1/camalis/core.py
--rw-r--r--   0        0        0      188 2024-04-24 11:51:17.662890 camalis-0.0.1/camalis/event.py
--rw-r--r--   0        0        0      167 2024-04-23 16:23:39.038037 camalis-0.0.1/camalis/exceptions.py
--rw-r--r--   0        0        0     1690 2024-05-09 14:53:47.266607 camalis-0.0.1/camalis/main.py
--rw-r--r--   0        0        0      810 2024-04-25 14:33:17.981011 camalis-0.0.1/camalis/state.py
--rw-r--r--   0        0        0      795 2024-05-09 12:44:56.932449 camalis-0.0.1/camalis/utils.py
--rw-r--r--   0        0        0     2491 2024-05-09 13:11:52.072437 camalis-0.0.1/camalis/variable.py
--rw-r--r--   0        0        0      527 2024-05-09 13:54:36.785075 camalis-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      141 2024-04-22 14:15:12.162481 camalis-0.0.1/README.md
--rw-r--r--   0        0        0      564 1970-01-01 00:00:00.000000 camalis-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      113 2024-05-09 14:48:58.269856 camalis-0.0.2/camalis/__init__.py
+-rw-r--r--   0        0        0     1335 2024-05-09 19:47:55.427179 camalis-0.0.2/camalis/core.py
+-rw-r--r--   0        0        0      188 2024-04-24 11:51:17.662890 camalis-0.0.2/camalis/event.py
+-rw-r--r--   0        0        0      167 2024-04-23 16:23:39.038037 camalis-0.0.2/camalis/exceptions.py
+-rw-r--r--   0        0        0     1881 2024-05-09 19:47:55.433250 camalis-0.0.2/camalis/main.py
+-rw-r--r--   0        0        0      810 2024-04-25 14:33:17.981011 camalis-0.0.2/camalis/state.py
+-rw-r--r--   0        0        0      795 2024-05-09 12:44:56.932449 camalis-0.0.2/camalis/utils.py
+-rw-r--r--   0        0        0     2491 2024-05-09 13:11:52.072437 camalis-0.0.2/camalis/variable.py
+-rw-r--r--   0        0        0      527 2024-05-13 13:20:18.561245 camalis-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      141 2024-04-22 14:15:12.162481 camalis-0.0.2/README.md
+-rw-r--r--   0        0        0      564 1970-01-01 00:00:00.000000 camalis-0.0.2/PKG-INFO
```

### Comparing `camalis-0.0.1/camalis/core.py` & `camalis-0.0.2/camalis/core.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,17 +4,18 @@
 from camalis.exceptions import CamalisApiException
 
 load_dotenv()
 
 
 class BaseCamalisClient:
     token = None
-    base_url = 'http://localhost:8080/api/v1/integracao'
+    base_url = ''
 
-    def __init__(self, token):
+    def __init__(self, api_url, token):
+        self.base_url = api_url
         self.token = token
 
     def _check_status(self, response):
         if response.status_code in [200, 201]:
             return response.json()
 
         if response.status_code == 400:
```

### Comparing `camalis-0.0.1/camalis/main.py` & `camalis-0.0.2/camalis/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -33,20 +33,24 @@
             result.append(Variable(self._camalis, id=variable_id))
         return result
 
 
 class Camalis(BaseCamalisClient):
     variable: CamalisVariableClient = None
 
-    def __init__(self, token=None):
+    def __init__(self, api_url=None, token=None):
         request_token = os.environ.get('CAMALIS_TOKEN', token)
+        camalis_url = os.environ.get('CAMALIS_API_URL', api_url)
         if request_token is None:
             raise CamalisAuthException('Token is required')
 
-        super().__init__(request_token)
+        if camalis_url is None:
+            raise CamalisAuthException('API URL is required')
+
+        super().__init__(camalis_url, request_token)
         self.variable = CamalisVariableClient(self)
 
     def state(self) -> State:
         return State(self)
 
     def event(self) -> Event:
         return Event(self)
```

### Comparing `camalis-0.0.1/camalis/state.py` & `camalis-0.0.2/camalis/state.py`

 * *Files identical despite different names*

### Comparing `camalis-0.0.1/camalis/utils.py` & `camalis-0.0.2/camalis/utils.py`

 * *Files identical despite different names*

### Comparing `camalis-0.0.1/camalis/variable.py` & `camalis-0.0.2/camalis/variable.py`

 * *Files identical despite different names*

### Comparing `camalis-0.0.1/pyproject.toml` & `camalis-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "camalis"
-version = "0.0.1"
+version = "0.0.2"
 description = ""
 authors = ["RN Tecnologia <contato@rntecnologia.com.br>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.12"
 requests = "^2.31.0"
```

### Comparing `camalis-0.0.1/PKG-INFO` & `camalis-0.0.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: camalis
-Version: 0.0.1
+Version: 0.0.2
 Summary: 
 Author: RN Tecnologia
 Author-email: contato@rntecnologia.com.br
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pytest-mock (>=3.14.0,<4.0.0)
```

