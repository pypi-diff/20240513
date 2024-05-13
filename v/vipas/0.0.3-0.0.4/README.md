# Comparing `tmp/vipas-0.0.3.tar.gz` & `tmp/vipas-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vipas-0.0.3.tar", last modified: Sun May 12 07:43:47 2024, max compression
+gzip compressed data, was "vipas-0.0.4.tar", last modified: Mon May 13 10:18:34 2024, max compression
```

## Comparing `vipas-0.0.3.tar` & `vipas-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2024-05-12 07:43:47.391628 vipas-0.0.3/
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     2487 2024-04-30 05:46:43.000000 vipas-0.0.3/LICENSE.md
--rw-r--r--   0 aditya    (1001) aditya    (1001)      360 2024-05-12 07:43:47.391628 vipas-0.0.3/PKG-INFO
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     1598 2024-05-01 12:56:58.000000 vipas-0.0.3/README.md
--rw-rw-r--   0 aditya    (1001) aditya    (1001)       91 2024-05-11 09:29:37.000000 vipas-0.0.3/pyproject.toml
--rw-rw-r--   0 aditya    (1001) aditya    (1001)      443 2024-05-12 07:43:47.391628 vipas-0.0.3/setup.cfg
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     1273 2024-05-12 07:43:12.000000 vipas-0.0.3/setup.py
-drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2024-05-12 07:43:47.391628 vipas-0.0.3/test/
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     2847 2024-05-11 11:43:02.000000 vipas-0.0.3/test/test_model_client.py
-drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2024-05-12 07:43:47.391628 vipas-0.0.3/vipas/
--rw-rw-r--   0 aditya    (1001) aditya    (1001)      725 2024-04-30 15:42:34.000000 vipas-0.0.3/vipas/__init__.py
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     2084 2024-05-02 09:27:49.000000 vipas-0.0.3/vipas/_rest.py
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     4091 2024-05-12 05:58:19.000000 vipas-0.0.3/vipas/config.py
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     3555 2024-05-01 08:36:27.000000 vipas-0.0.3/vipas/exceptions.py
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     6279 2024-05-12 06:07:10.000000 vipas-0.0.3/vipas/model.py
-drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2024-05-12 07:43:47.391628 vipas-0.0.3/vipas.egg-info/
--rw-r--r--   0 aditya    (1001) aditya    (1001)      360 2024-05-12 07:43:47.000000 vipas-0.0.3/vipas.egg-info/PKG-INFO
--rw-rw-r--   0 aditya    (1001) aditya    (1001)      308 2024-05-12 07:43:47.000000 vipas-0.0.3/vipas.egg-info/SOURCES.txt
--rw-rw-r--   0 aditya    (1001) aditya    (1001)        1 2024-05-12 07:43:47.000000 vipas-0.0.3/vipas.egg-info/dependency_links.txt
--rw-rw-r--   0 aditya    (1001) aditya    (1001)       65 2024-05-12 07:43:47.000000 vipas-0.0.3/vipas.egg-info/requires.txt
--rw-rw-r--   0 aditya    (1001) aditya    (1001)        6 2024-05-12 07:43:47.000000 vipas-0.0.3/vipas.egg-info/top_level.txt
+drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2024-05-13 10:18:34.059213 vipas-0.0.4/
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     2487 2024-04-30 05:46:43.000000 vipas-0.0.4/LICENSE.md
+-rw-r--r--   0 aditya    (1001) aditya    (1001)      360 2024-05-13 10:18:34.059213 vipas-0.0.4/PKG-INFO
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     1598 2024-05-01 12:56:58.000000 vipas-0.0.4/README.md
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)       91 2024-05-11 09:29:37.000000 vipas-0.0.4/pyproject.toml
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)      443 2024-05-13 10:18:34.059213 vipas-0.0.4/setup.cfg
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     1273 2024-05-13 10:17:07.000000 vipas-0.0.4/setup.py
+drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2024-05-13 10:18:34.059213 vipas-0.0.4/test/
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     2818 2024-05-12 09:48:23.000000 vipas-0.0.4/test/test_model_client.py
+drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2024-05-13 10:18:34.059213 vipas-0.0.4/vipas/
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)      725 2024-04-30 15:42:34.000000 vipas-0.0.4/vipas/__init__.py
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     2084 2024-05-02 09:27:49.000000 vipas-0.0.4/vipas/_rest.py
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     4089 2024-05-13 09:13:56.000000 vipas-0.0.4/vipas/config.py
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     3555 2024-05-01 08:36:27.000000 vipas-0.0.4/vipas/exceptions.py
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     6279 2024-05-12 09:47:51.000000 vipas-0.0.4/vipas/model.py
+drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2024-05-13 10:18:34.059213 vipas-0.0.4/vipas.egg-info/
+-rw-r--r--   0 aditya    (1001) aditya    (1001)      360 2024-05-13 10:18:34.000000 vipas-0.0.4/vipas.egg-info/PKG-INFO
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)      308 2024-05-13 10:18:34.000000 vipas-0.0.4/vipas.egg-info/SOURCES.txt
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)        1 2024-05-13 10:18:34.000000 vipas-0.0.4/vipas.egg-info/dependency_links.txt
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)       65 2024-05-13 10:18:34.000000 vipas-0.0.4/vipas.egg-info/requires.txt
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)        6 2024-05-13 10:18:34.000000 vipas-0.0.4/vipas.egg-info/top_level.txt
```

### Comparing `vipas-0.0.3/LICENSE.md` & `vipas-0.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `vipas-0.0.3/README.md` & `vipas-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `vipas-0.0.3/setup.py` & `vipas-0.0.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 NAME = "vipas"
-VERSION = "0.0.3"
+VERSION = "0.0.4"
 PYTHON_REQUIRES = ">=3.7"
 REQUIRES = [
     "urllib3",
     "pydantic",
     "typing-extensions",
     "ratelimit",
     "pybreaker",
```

### Comparing `vipas-0.0.3/test/test_model_client.py` & `vipas-0.0.4/test/test_model_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,16 +30,16 @@
         # Check if the result is as expected
         self.assertEqual(result, {"status": "success"})
 
         # Ensure that the request was called with correct parameters
         self.client.rest_client.request.assert_called_with(
             'POST',
             self.config.host + '/predict?model_id=test-model',
-            headers={'Accept': 'application/json', 'vps-auth-token': 'fake_token'},
-            body={"input_data": "Sample data"}
+            headers={'Accept': '*/*', 'vps-auth-token': 'fake_token'},
+            body="Sample data"
         )
         
     def test_predict_api_failure_input_validation_failed(self):
         # Setup mock response
         self.client.rest_client.request.return_value = self.mock_response
 
         over_1mb_string = 'a' * 1048600
```

### Comparing `vipas-0.0.3/vipas/__init__.py` & `vipas-0.0.4/vipas/__init__.py`

 * *Files identical despite different names*

### Comparing `vipas-0.0.3/vipas/_rest.py` & `vipas-0.0.4/vipas/_rest.py`

 * *Files identical despite different names*

### Comparing `vipas-0.0.3/vipas/config.py` & `vipas-0.0.4/vipas/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
     _default = None
 
     def __init__(self, vps_auth_token=None) -> None:
         """
             Constructor for the configuration class
         """
-        self.host = "http://a56fc111a2a174cf8b4ccaa9f2129611-725931850.ap-south-1.elb.amazonaws.com" 
+        self.host = "http://proxy.vipas.dev" 
         """
             Default Host for the proxy service.
         """
 
         # Authentication Settings
         self.vps_auth_token = None
         if vps_auth_token:
@@ -52,14 +52,15 @@
         if not self.vps_auth_token:
             self.setup_api_key()
 
     def setup_api_key(self):
         """Set up API key based on environment."""
         env_type = os.getenv("VPS_ENV_TYPE")
         if env_type == "vipas-streamlit":
+            self.host = "http://vps-proxy-service:80"
             self.vps_auth_token = self.extract_websocket_api_key()
         else:
             self.vps_auth_token = os.getenv("VPS_AUTH_TOKEN")
             if self.vps_auth_token is None or len(self.vps_auth_token) == 0:
                 raise ClientException(400, "VPS_AUTH_TOKEN is not set in the environment variables or it is empty")
 
     def extract_websocket_api_key(self):
```

### Comparing `vipas-0.0.3/vipas/exceptions.py` & `vipas-0.0.4/vipas/exceptions.py`

 * *Files identical despite different names*

### Comparing `vipas-0.0.3/vipas/model.py` & `vipas-0.0.4/vipas/model.py`

 * *Files identical despite different names*

