# Comparing `tmp/directus-sdk-py-1.0.0.tar.gz` & `tmp/directus-sdk-py-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "directus-sdk-py-1.0.0.tar", last modified: Mon Apr  8 13:47:12 2024, max compression
+gzip compressed data, was "directus-sdk-py-1.0.1.tar", last modified: Mon May 13 10:57:33 2024, max compression
```

## Comparing `directus-sdk-py-1.0.0.tar` & `directus-sdk-py-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 alban     (1000) alban     (1000)        0 2024-04-08 13:47:12.432857 directus-sdk-py-1.0.0/
--rw-r--r--   0 alban     (1000) alban     (1000)     5742 2024-04-08 13:47:12.432857 directus-sdk-py-1.0.0/PKG-INFO
--rw-rw-r--   0 alban     (1000) alban     (1000)     5107 2024-04-08 13:40:49.000000 directus-sdk-py-1.0.0/README.md
-drwxrwxr-x   0 alban     (1000) alban     (1000)        0 2024-04-08 13:47:12.432857 directus-sdk-py-1.0.0/directus_sdk_py/
--rw-rw-r--   0 alban     (1000) alban     (1000)       76 2024-04-08 13:17:01.000000 directus-sdk-py-1.0.0/directus_sdk_py/__init__.py
--rw-rw-r--   0 alban     (1000) alban     (1000)    22895 2024-04-08 13:18:45.000000 directus-sdk-py-1.0.0/directus_sdk_py/main.py
-drwxrwxr-x   0 alban     (1000) alban     (1000)        0 2024-04-08 13:47:12.432857 directus-sdk-py-1.0.0/directus_sdk_py.egg-info/
--rw-r--r--   0 alban     (1000) alban     (1000)     5742 2024-04-08 13:47:12.000000 directus-sdk-py-1.0.0/directus_sdk_py.egg-info/PKG-INFO
--rw-rw-r--   0 alban     (1000) alban     (1000)      306 2024-04-08 13:47:12.000000 directus-sdk-py-1.0.0/directus_sdk_py.egg-info/SOURCES.txt
--rw-rw-r--   0 alban     (1000) alban     (1000)        1 2024-04-08 13:47:12.000000 directus-sdk-py-1.0.0/directus_sdk_py.egg-info/dependency_links.txt
--rw-rw-r--   0 alban     (1000) alban     (1000)       66 2024-04-08 13:47:12.000000 directus-sdk-py-1.0.0/directus_sdk_py.egg-info/entry_points.txt
--rw-rw-r--   0 alban     (1000) alban     (1000)        9 2024-04-08 13:47:12.000000 directus-sdk-py-1.0.0/directus_sdk_py.egg-info/requires.txt
--rw-rw-r--   0 alban     (1000) alban     (1000)       16 2024-04-08 13:47:12.000000 directus-sdk-py-1.0.0/directus_sdk_py.egg-info/top_level.txt
--rw-rw-r--   0 alban     (1000) alban     (1000)       38 2024-04-08 13:47:12.432857 directus-sdk-py-1.0.0/setup.cfg
--rw-rw-r--   0 alban     (1000) alban     (1000)     1183 2024-04-08 13:45:59.000000 directus-sdk-py-1.0.0/setup.py
+drwxrwxr-x   0 alban     (1000) alban     (1000)        0 2024-05-13 10:57:33.100055 directus-sdk-py-1.0.1/
+-rw-r--r--   0 alban     (1000) alban     (1000)     5742 2024-05-13 10:57:33.100055 directus-sdk-py-1.0.1/PKG-INFO
+-rw-rw-r--   0 alban     (1000) alban     (1000)     5107 2024-04-10 12:28:57.000000 directus-sdk-py-1.0.1/README.md
+drwxrwxr-x   0 alban     (1000) alban     (1000)        0 2024-05-13 10:57:33.100055 directus-sdk-py-1.0.1/directus_sdk_py/
+-rw-rw-r--   0 alban     (1000) alban     (1000)       76 2024-04-08 13:17:01.000000 directus-sdk-py-1.0.1/directus_sdk_py/__init__.py
+-rw-rw-r--   0 alban     (1000) alban     (1000)    23140 2024-05-13 10:34:32.000000 directus-sdk-py-1.0.1/directus_sdk_py/main.py
+drwxrwxr-x   0 alban     (1000) alban     (1000)        0 2024-05-13 10:57:33.100055 directus-sdk-py-1.0.1/directus_sdk_py.egg-info/
+-rw-r--r--   0 alban     (1000) alban     (1000)     5742 2024-05-13 10:57:32.000000 directus-sdk-py-1.0.1/directus_sdk_py.egg-info/PKG-INFO
+-rw-rw-r--   0 alban     (1000) alban     (1000)      306 2024-05-13 10:57:32.000000 directus-sdk-py-1.0.1/directus_sdk_py.egg-info/SOURCES.txt
+-rw-rw-r--   0 alban     (1000) alban     (1000)        1 2024-05-13 10:57:32.000000 directus-sdk-py-1.0.1/directus_sdk_py.egg-info/dependency_links.txt
+-rw-rw-r--   0 alban     (1000) alban     (1000)       66 2024-05-13 10:57:32.000000 directus-sdk-py-1.0.1/directus_sdk_py.egg-info/entry_points.txt
+-rw-rw-r--   0 alban     (1000) alban     (1000)        9 2024-05-13 10:57:32.000000 directus-sdk-py-1.0.1/directus_sdk_py.egg-info/requires.txt
+-rw-rw-r--   0 alban     (1000) alban     (1000)       16 2024-05-13 10:57:32.000000 directus-sdk-py-1.0.1/directus_sdk_py.egg-info/top_level.txt
+-rw-rw-r--   0 alban     (1000) alban     (1000)       38 2024-05-13 10:57:33.100055 directus-sdk-py-1.0.1/setup.cfg
+-rw-rw-r--   0 alban     (1000) alban     (1000)     1183 2024-05-13 10:53:44.000000 directus-sdk-py-1.0.1/setup.py
```

### Comparing `directus-sdk-py-1.0.0/PKG-INFO` & `directus-sdk-py-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: directus-sdk-py
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python SDK for interacting with Directus API (colletion, items, users, files)
 Home-page: https://github.com/reise69/directus-py-sdk
 Author: Alban Lamberet
 Author-email: contact@refbax.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -13,17 +13,17 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 
 # Directus Python SDK
 
-[![PyPI version](https://badge.fury.io/py/directus-py-sdk.svg)](https://badge.fury.io/py/directus-py-sdk)
+[![PyPI version](https://badge.fury.io/py/directus-sdk-py.svg)](https://badge.fury.io/py/directus-sdk-py)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-[![Python Version](https://img.shields.io/pypi/pyversions/directus-py-sdk.svg)](https://pypi.org/project/directus-py-sdk/)
+[![Python Version](https://img.shields.io/pypi/pyversions/directus-sdk-py.svg)](https://pypi.org/project/directus-sdk-py/)
 
 A Python SDK for interacting with Directus, an open-source headless CMS and API platform.
 
 
 ## About Directus
 
 [Directus](https://directus.io/) is a powerful and flexible open-source headless CMS and API platform. It provides a
```

### Comparing `directus-sdk-py-1.0.0/README.md` & `directus-sdk-py-1.0.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Directus Python SDK
 
-[![PyPI version](https://badge.fury.io/py/directus-py-sdk.svg)](https://badge.fury.io/py/directus-py-sdk)
+[![PyPI version](https://badge.fury.io/py/directus-sdk-py.svg)](https://badge.fury.io/py/directus-sdk-py)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-[![Python Version](https://img.shields.io/pypi/pyversions/directus-py-sdk.svg)](https://pypi.org/project/directus-py-sdk/)
+[![Python Version](https://img.shields.io/pypi/pyversions/directus-sdk-py.svg)](https://pypi.org/project/directus-sdk-py/)
 
 A Python SDK for interacting with Directus, an open-source headless CMS and API platform.
 
 
 ## About Directus
 
 [Directus](https://directus.io/) is a powerful and flexible open-source headless CMS and API platform. It provides a
```

### Comparing `directus-sdk-py-1.0.0/directus_sdk_py/main.py` & `directus-sdk-py-1.0.1/directus_sdk_py/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,15 +133,19 @@
             **kwargs
         )
         if 'errors' in data.text:
             raise AssertionError(data.json()['errors'])
         if output_type == 'csv':
             return data.text
 
-        return data.json()['data']
+        try:
+            return data.json()['data']
+        except Exception as e:
+            return {'error': f'No data found for this request : {e}'}
+
 
     def post(self, path, **kwargs):
         """
         Perform a POST request to the specified path.
 
         Args:
             path (str): The API endpoint path.
@@ -172,16 +176,18 @@
 
         Returns:
             dict: The response data.
         """
         headers = {"Authorization": f"Bearer {self.get_token()}"}
         response = requests.request("SEARCH", f"{self.url}{path}", headers=headers, json=query, verify=self.verify,
                                     **kwargs)
-
-        return response.json()['data']
+        try:
+            return response.json()['data']
+        except Exception as e:
+            return {'error': f'No data found for this request : {e}'}
 
     def delete(self, path, **kwargs):
         """
         Perform a DELETE request to the specified path.
 
         Args:
             path (str): The API endpoint path.
@@ -338,15 +344,15 @@
         headers = {"Authorization": f"Bearer {self.get_token()}"}
         response = requests.get(url, headers=headers, params=display, verify=self.verify)
         if response.status_code != 200:
             raise AssertionError(response.text)
         with open(file_path, "wb") as file:
             file.write(response.content)
 
-    def get_url_file(self, file_id: str, display: dict, transform: list) -> Union[str, bytes]:
+    def get_url_file(self, file_id: str, display: dict = {}, transform: list = []) -> Union[str, bytes]:
         """
         Retrieve a file.
 
         Args:
             file_id (str): The file ID.
             **kwargs: Additional keyword arguments to pass to the request.
 
@@ -642,8 +648,7 @@
         try:
             self.post(f"/relations", json=relation)
         except AssertionError as e:
             if '"id" has to be unique' in str(e):
                 self.post_relation(relation)
             else:
                 raise
-
```

### Comparing `directus-sdk-py-1.0.0/directus_sdk_py.egg-info/PKG-INFO` & `directus-sdk-py-1.0.1/directus_sdk_py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: directus-sdk-py
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python SDK for interacting with Directus API (colletion, items, users, files)
 Home-page: https://github.com/reise69/directus-py-sdk
 Author: Alban Lamberet
 Author-email: contact@refbax.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -13,17 +13,17 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 
 # Directus Python SDK
 
-[![PyPI version](https://badge.fury.io/py/directus-py-sdk.svg)](https://badge.fury.io/py/directus-py-sdk)
+[![PyPI version](https://badge.fury.io/py/directus-sdk-py.svg)](https://badge.fury.io/py/directus-sdk-py)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-[![Python Version](https://img.shields.io/pypi/pyversions/directus-py-sdk.svg)](https://pypi.org/project/directus-py-sdk/)
+[![Python Version](https://img.shields.io/pypi/pyversions/directus-sdk-py.svg)](https://pypi.org/project/directus-sdk-py/)
 
 A Python SDK for interacting with Directus, an open-source headless CMS and API platform.
 
 
 ## About Directus
 
 [Directus](https://directus.io/) is a powerful and flexible open-source headless CMS and API platform. It provides a
```

### Comparing `directus-sdk-py-1.0.0/setup.py` & `directus-sdk-py-1.0.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="directus-sdk-py",
-    version="1.0.0",
+    version="1.0.1",
     description="Python SDK for interacting with Directus API (colletion, items, users, files)",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/reise69/directus-py-sdk",
     author="Alban Lamberet",
     author_email="contact@refbax.com",
     license="MIT",
```

