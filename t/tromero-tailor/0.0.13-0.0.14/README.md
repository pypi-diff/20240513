# Comparing `tmp/tromero_tailor-0.0.13.tar.gz` & `tmp/tromero_tailor-0.0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tromero_tailor-0.0.13.tar", last modified: Thu May  9 14:34:54 2024, max compression
+gzip compressed data, was "tromero_tailor-0.0.14.tar", last modified: Mon May 13 13:43:58 2024, max compression
```

## Comparing `tromero_tailor-0.0.13.tar` & `tromero_tailor-0.0.14.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 tadhgamin   (501) staff       (20)        0 2024-05-09 14:34:54.322718 tromero_tailor-0.0.13/
--rw-r--r--   0 tadhgamin   (501) staff       (20)     1937 2024-05-09 14:34:54.322509 tromero_tailor-0.0.13/PKG-INFO
--rw-r--r--   0 tadhgamin   (501) staff       (20)      942 2024-04-08 16:49:32.000000 tromero_tailor-0.0.13/README.md
--rw-r--r--   0 tadhgamin   (501) staff       (20)       38 2024-05-09 14:34:54.322758 tromero_tailor-0.0.13/setup.cfg
--rw-r--r--   0 tadhgamin   (501) staff       (20)     1633 2024-05-09 14:34:42.000000 tromero_tailor-0.0.13/setup.py
-drwxr-xr-x   0 tadhgamin   (501) staff       (20)        0 2024-05-09 14:34:54.320394 tromero_tailor-0.0.13/tests/
--rw-r--r--   0 tadhgamin   (501) staff       (20)     3672 2024-04-17 14:55:07.000000 tromero_tailor-0.0.13/tests/test.py
-drwxr-xr-x   0 tadhgamin   (501) staff       (20)        0 2024-05-09 14:34:54.321341 tromero_tailor-0.0.13/tromero_tailor/
--rw-r--r--   0 tadhgamin   (501) staff       (20)       30 2024-04-08 15:07:54.000000 tromero_tailor-0.0.13/tromero_tailor/__init__.py
--rw-r--r--   0 tadhgamin   (501) staff       (20)     1336 2024-05-09 14:32:30.000000 tromero_tailor-0.0.13/tromero_tailor/tromero_requests.py
--rw-r--r--   0 tadhgamin   (501) staff       (20)      446 2024-04-12 11:06:15.000000 tromero_tailor-0.0.13/tromero_tailor/tromero_utils.py
--rw-r--r--   0 tadhgamin   (501) staff       (20)     2828 2024-04-23 11:05:42.000000 tromero_tailor-0.0.13/tromero_tailor/wrapper.py
-drwxr-xr-x   0 tadhgamin   (501) staff       (20)        0 2024-05-09 14:34:54.322215 tromero_tailor-0.0.13/tromero_tailor.egg-info/
--rw-r--r--   0 tadhgamin   (501) staff       (20)     1937 2024-05-09 14:34:54.000000 tromero_tailor-0.0.13/tromero_tailor.egg-info/PKG-INFO
--rw-r--r--   0 tadhgamin   (501) staff       (20)      341 2024-05-09 14:34:54.000000 tromero_tailor-0.0.13/tromero_tailor.egg-info/SOURCES.txt
--rw-r--r--   0 tadhgamin   (501) staff       (20)        1 2024-05-09 14:34:54.000000 tromero_tailor-0.0.13/tromero_tailor.egg-info/dependency_links.txt
--rw-r--r--   0 tadhgamin   (501) staff       (20)      304 2024-05-09 14:34:54.000000 tromero_tailor-0.0.13/tromero_tailor.egg-info/requires.txt
--rw-r--r--   0 tadhgamin   (501) staff       (20)       15 2024-05-09 14:34:54.000000 tromero_tailor-0.0.13/tromero_tailor.egg-info/top_level.txt
+drwxr-xr-x   0 tadhgamin   (501) staff       (20)        0 2024-05-13 13:43:58.274478 tromero_tailor-0.0.14/
+-rw-r--r--   0 tadhgamin   (501) staff       (20)     1937 2024-05-13 13:43:58.274235 tromero_tailor-0.0.14/PKG-INFO
+-rw-r--r--   0 tadhgamin   (501) staff       (20)      942 2024-04-08 16:49:32.000000 tromero_tailor-0.0.14/README.md
+-rw-r--r--   0 tadhgamin   (501) staff       (20)       38 2024-05-13 13:43:58.274524 tromero_tailor-0.0.14/setup.cfg
+-rw-r--r--   0 tadhgamin   (501) staff       (20)     1633 2024-05-13 13:43:49.000000 tromero_tailor-0.0.14/setup.py
+drwxr-xr-x   0 tadhgamin   (501) staff       (20)        0 2024-05-13 13:43:58.272447 tromero_tailor-0.0.14/tests/
+-rw-r--r--   0 tadhgamin   (501) staff       (20)     3672 2024-04-17 14:55:07.000000 tromero_tailor-0.0.14/tests/test.py
+drwxr-xr-x   0 tadhgamin   (501) staff       (20)        0 2024-05-13 13:43:58.273172 tromero_tailor-0.0.14/tromero_tailor/
+-rw-r--r--   0 tadhgamin   (501) staff       (20)       30 2024-04-08 15:07:54.000000 tromero_tailor-0.0.14/tromero_tailor/__init__.py
+-rw-r--r--   0 tadhgamin   (501) staff       (20)     1678 2024-05-13 13:41:50.000000 tromero_tailor-0.0.14/tromero_tailor/tromero_requests.py
+-rw-r--r--   0 tadhgamin   (501) staff       (20)      446 2024-04-12 11:06:15.000000 tromero_tailor-0.0.14/tromero_tailor/tromero_utils.py
+-rw-r--r--   0 tadhgamin   (501) staff       (20)     2942 2024-05-13 13:42:50.000000 tromero_tailor-0.0.14/tromero_tailor/wrapper.py
+drwxr-xr-x   0 tadhgamin   (501) staff       (20)        0 2024-05-13 13:43:58.273967 tromero_tailor-0.0.14/tromero_tailor.egg-info/
+-rw-r--r--   0 tadhgamin   (501) staff       (20)     1937 2024-05-13 13:43:58.000000 tromero_tailor-0.0.14/tromero_tailor.egg-info/PKG-INFO
+-rw-r--r--   0 tadhgamin   (501) staff       (20)      341 2024-05-13 13:43:58.000000 tromero_tailor-0.0.14/tromero_tailor.egg-info/SOURCES.txt
+-rw-r--r--   0 tadhgamin   (501) staff       (20)        1 2024-05-13 13:43:58.000000 tromero_tailor-0.0.14/tromero_tailor.egg-info/dependency_links.txt
+-rw-r--r--   0 tadhgamin   (501) staff       (20)      304 2024-05-13 13:43:58.000000 tromero_tailor-0.0.14/tromero_tailor.egg-info/requires.txt
+-rw-r--r--   0 tadhgamin   (501) staff       (20)       15 2024-05-13 13:43:58.000000 tromero_tailor-0.0.14/tromero_tailor.egg-info/top_level.txt
```

### Comparing `tromero_tailor-0.0.13/PKG-INFO` & `tromero_tailor-0.0.14/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tromero_tailor
-Version: 0.0.13
+Version: 0.0.14
 Summary: A short description of your package
 Home-page: http://yourpackagehomepage.com
 Author: Tromero
 Author-email: tadhg.amin@tromero.ai
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tromero_tailor-0.0.13/README.md` & `tromero_tailor-0.0.14/README.md`

 * *Files identical despite different names*

### Comparing `tromero_tailor-0.0.13/setup.py` & `tromero_tailor-0.0.14/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="tromero_tailor",  # Replace with your package name
-    version="0.0.13",  # Replace with your package's version
+    version="0.0.14",  # Replace with your package's version
     author="Tromero",  # Replace with your name
     author_email="tadhg.amin@tromero.ai",  # Replace with your email address
     description="A short description of your package",  # Provide a short description
     long_description=open('README.md').read(),  # This will read your long description from README.md
     long_description_content_type='text/markdown',  # Indicates that the long description is in Markdown
     url="http://yourpackagehomepage.com",  # Replace with the URL to your package's homepage
     license="MIT",  # Replace with your chosen license
```

### Comparing `tromero_tailor-0.0.13/tests/test.py` & `tromero_tailor-0.0.14/tests/test.py`

 * *Files identical despite different names*

### Comparing `tromero_tailor-0.0.13/tromero_tailor/tromero_requests.py` & `tromero_tailor-0.0.14/tromero_tailor/tromero_requests.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,42 @@
 import requests
 
 data_url = "https://midyear-grid-402910.lm.r.appspot.com/tailor/v1/data"
 models_url = "http://35.246.163.71:5000/generate"
+self_hosted_models_url = "https://midyear-grid-402910.lm.r.appspot.com/tailor/v1/hosted_server/generate"
 
 def post_data(data, auth_token):
     headers = {
         'X-API-KEY': auth_token,
         'Content-Type': 'application/json'
     }
     try:
         response = requests.post(data_url, json=data, headers=headers)
         response.raise_for_status()  # Raises HTTPError for bad responses (4XX, 5XX)
         return response.json()  # Return the JSON response if request was successful
     except Exception as e:
         return {'error': f'An error occurred: {e}', 'status_code': response.status_code if 'response' in locals() else 'N/A'}
     
 
-def tromero_model_create(model, messages, tromero_key):
-    headers = {
-        'Authorization': tromero_key,
-        'Content-Type': 'application/json'
-    }
-
+def tromero_model_create(model, messages, tromero_key, self_hosted=False):
+    url = self_hosted_models_url if self_hosted else models_url
+    headers = {'Content-Type': 'application/json'}
     data = {
         "adapter_name": model,
         "messages": messages,
     }
+    if self_hosted:
+        url = self_hosted_models_url
+        headers['X-API-KEY'] = tromero_key
+        data["model"] = model  
+    else:
+        url = models_url
+        headers['Authorization'] = tromero_key
     try:
-        response = requests.post(models_url, json=data, headers=headers)
+        response = requests.post(url, json=data, headers=headers)
         response.raise_for_status()  # Raises HTTPError for bad responses (4XX, 5XX)
         return response.json()  # Return the JSON response if request was successful
     except Exception as e:
         return {'error': f'An error occurred: {e}', 'status_code': response.status_code if 'response' in locals() else 'N/A'}
```

### Comparing `tromero_tailor-0.0.13/tromero_tailor/wrapper.py` & `tromero_tailor-0.0.14/tromero_tailor/wrapper.py`

 * *Files 10% similar despite different names*

```diff
@@ -52,17 +52,18 @@
                                     "kwargs": formatted_kwargs,
                                     "creation_time": str(datetime.datetime.now().isoformat()),
                                     "usage": usage,
                                     "tags": tags
                                     })
         else:
             messages = kwargs['messages']
-            res = tromero_model_create(kwargs['model'], messages, self._client.tromero_key)
+            res = tromero_model_create(kwargs['model'], messages, self._client.tromero_key, self._client.self_hosted)
             # check if res has field 'generated_text'
             if 'generated_text' in res:
+                print("here")
                 res = mock_openai_format(res['generated_text'])
         return res
 
 
 class MockChat(Chat):
     def __init__(self, client):
         super().__init__(client)
@@ -70,12 +71,13 @@
     @cached_property
     def completions(self) -> Completions:
         return MockCompletions(self._client)
 
 
 class TailorAI(OpenAI):
     chat: MockChat
-    def __init__(self, api_key, tromero_key):
+    def __init__(self, api_key, tromero_key, self_hosted=False):
         super().__init__(api_key=api_key)
         self.current_prompt = []
         self.chat = MockChat(self)
         self.tromero_key = tromero_key
+        self.self_hosted = self_hosted
```

### Comparing `tromero_tailor-0.0.13/tromero_tailor.egg-info/PKG-INFO` & `tromero_tailor-0.0.14/tromero_tailor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tromero_tailor
-Version: 0.0.13
+Version: 0.0.14
 Summary: A short description of your package
 Home-page: http://yourpackagehomepage.com
 Author: Tromero
 Author-email: tadhg.amin@tromero.ai
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

