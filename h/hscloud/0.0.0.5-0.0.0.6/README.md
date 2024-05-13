# Comparing `tmp/hscloud-0.0.0.5.tar.gz` & `tmp/hscloud-0.0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hscloud-0.0.0.5.tar", last modified: Mon May 13 02:00:01 2024, max compression
+gzip compressed data, was "hscloud-0.0.0.6.tar", last modified: Mon May 13 03:34:09 2024, max compression
```

## Comparing `hscloud-0.0.0.5.tar` & `hscloud-0.0.0.6.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 02:00:01.459643 hscloud-0.0.0.5/
--rw-rw-rw-   0        0        0        0 2023-12-18 08:14:13.000000 hscloud-0.0.0.5/LICENSE
--rw-rw-rw-   0        0        0      432 2024-05-13 02:00:01.457642 hscloud-0.0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2505 2024-05-09 10:10:45.000000 hscloud-0.0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-13 02:00:01.440642 hscloud-0.0.0.5/hscloud/
--rw-rw-rw-   0        0        0      258 2024-05-09 07:57:46.000000 hscloud-0.0.0.5/hscloud/__init__.py
--rw-rw-rw-   0        0        0     3653 2024-05-09 07:55:39.000000 hscloud-0.0.0.5/hscloud/helpers.py
--rw-rw-rw-   0        0        0      953 2024-05-13 01:58:22.000000 hscloud-0.0.0.5/hscloud/hscloud.py
-drwxrwxrwx   0        0        0        0 2024-05-13 02:00:01.455642 hscloud-0.0.0.5/hscloud.egg-info/
--rw-rw-rw-   0        0        0      432 2024-05-13 02:00:01.000000 hscloud-0.0.0.5/hscloud.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2024-05-13 02:00:01.000000 hscloud-0.0.0.5/hscloud.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 02:00:01.000000 hscloud-0.0.0.5/hscloud.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2024-05-13 02:00:01.000000 hscloud-0.0.0.5/hscloud.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       36 2024-05-13 02:00:01.000000 hscloud-0.0.0.5/hscloud.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-13 02:00:01.000000 hscloud-0.0.0.5/hscloud.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-13 02:00:01.459643 hscloud-0.0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      887 2024-05-13 01:58:47.000000 hscloud-0.0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 03:34:09.372006 hscloud-0.0.0.6/
+-rw-rw-rw-   0        0        0        0 2023-12-18 08:14:13.000000 hscloud-0.0.0.6/LICENSE
+-rw-rw-rw-   0        0        0      432 2024-05-13 03:34:09.370006 hscloud-0.0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2505 2024-05-09 10:10:45.000000 hscloud-0.0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 03:34:09.353004 hscloud-0.0.0.6/hscloud/
+-rw-rw-rw-   0        0        0      258 2024-05-09 07:57:46.000000 hscloud-0.0.0.6/hscloud/__init__.py
+-rw-rw-rw-   0        0        0     4182 2024-05-13 03:29:08.000000 hscloud-0.0.0.6/hscloud/helpers.py
+-rw-rw-rw-   0        0        0      829 2024-05-13 03:25:20.000000 hscloud-0.0.0.6/hscloud/hscloud.py
+-rw-rw-rw-   0        0        0      289 2024-05-13 03:32:42.000000 hscloud-0.0.0.6/hscloud/hscloudexception.py
+drwxrwxrwx   0        0        0        0 2024-05-13 03:34:09.368004 hscloud-0.0.0.6/hscloud.egg-info/
+-rw-rw-rw-   0        0        0      432 2024-05-13 03:34:09.000000 hscloud-0.0.0.6/hscloud.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      300 2024-05-13 03:34:09.000000 hscloud-0.0.0.6/hscloud.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 03:34:09.000000 hscloud-0.0.0.6/hscloud.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2024-05-13 03:34:09.000000 hscloud-0.0.0.6/hscloud.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       36 2024-05-13 03:34:09.000000 hscloud-0.0.0.6/hscloud.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-13 03:34:09.000000 hscloud-0.0.0.6/hscloud.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 03:34:09.372006 hscloud-0.0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      887 2024-05-13 03:33:40.000000 hscloud-0.0.0.6/setup.py
```

### Comparing `hscloud-0.0.0.5/README.md` & `hscloud-0.0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `hscloud-0.0.0.5/hscloud/helpers.py` & `hscloud-0.0.0.6/hscloud/helpers.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import requests
-import json
 from datetime import datetime
-from typing import NamedTuple, Optional, Union
+from typing import Optional
+from .hscloudexception import HsCloudAccessDenied, HsCloudException
 import logging
 
 logger = logging.getLogger(__name__)
 
 class Helpers:
 
     @staticmethod
-    def login(username=None, password=None) -> tuple:
+    def login(username=None, password=None):
         base_url = 'http://10.10.20.109:2070'
 
         headers = {
             'Content-Type': 'application/json',
             'UA': 'openapi/1.0.0'
         }
 
@@ -29,44 +29,46 @@
             "email": username,
             "password": password
         }
 
         return Helpers.call_api(base_url + "/api/oauth/login", "post", headers, params, body)
 
     @staticmethod
-    def devices(endpoint=None, access_token=None) -> tuple:
+    def devices(endpoint=None, access_token=None):
         headers = {
             'Content-Type': 'application/json',
             'Authorization': f'Bearer {access_token}',
             'UA': 'openapi/1.0.0'
         }
 
         params = {
             'timestamp': Helpers.timestamp()
         }
 
+        result = Helpers.call_api(endpoint + "/api/device/list", "get", headers, params)
+
         return Helpers.call_api(endpoint + "/api/device/list", "get", headers, params)
 
     @staticmethod
-    def status(endpoint=None, access_token=None, devicesn=None) -> tuple:
+    def status(endpoint=None, access_token=None, devicesn=None):
         headers = {
             'Content-Type': 'application/json',
             'Authorization': f'Bearer {access_token}',
             'UA': 'openapi/1.0.0'
         }
 
         params = {
             'deviceSn': devicesn,
             'timestamp': Helpers.timestamp()
         }
 
         return Helpers.call_api(endpoint + "/api/device/state", "get", headers, params)
 
     @staticmethod
-    def update(endpoint=None, access_token=None, devicesn=None,  **kwargs) -> tuple:
+    def update(endpoint=None, access_token=None, devicesn=None,  **kwargs):
         headers = {
             'Content-Type': 'application/json',
             'Authorization': f'Bearer {access_token}',
             'UA': 'openapi/1.0.0'
         }
 
         params = {
@@ -74,34 +76,41 @@
         }
 
         return Helpers.call_api(endpoint + "/api/device/control", "post", headers, params, Helpers.update_body(devicesn, **kwargs))
 
     @staticmethod
     def call_api(api: str, method: str, headers: Optional[dict] = None, params: Optional[dict] = None, json_body: Optional[dict] = None) -> tuple:
         response = None
-        response_code = None
-        response_data = None
-
         try:
             if method.lower() == "get":
                 response = requests.get(api, headers=headers, params=params, timeout=8)
 
             elif method.lower() == "post":
                 response = requests.post(api, headers=headers, params=params, json=json_body, timeout=8)
 
         except requests.exceptions.RequestException as e:
             logger.error(e)
         except Exception as e:
             logger.error(e)
         else:
             if response.status_code == 200:
                 response_body = response.json()
-                response_code = response_body.get("code")
-                response_data = response_body.get("data")
-        return response_code, response_data
+                code = response_body.get("code")
+                if code == 0:
+                    response = response_body.get("data")
+                elif code == 401:
+                    raise HsCloudAccessDenied("Cannot execute request. token invalid. Make sure to login.")
+                else:
+                    raise HsCloudException(response_body.get("msg"))
+
+            elif response.status_code == 429:
+                raise HsCloudException("Your request is too frequent, please try again later.")
+            else:
+                raise HsCloudException("There is a service problem, please try again later.")
+        return response
 
     @staticmethod
     def update_body(devicesn, **kwargs):
         data = {
             'devicesn': devicesn
         }
```

### Comparing `hscloud-0.0.0.5/setup.py` & `hscloud-0.0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name = 'hscloud',
     packages = ['hscloud'],
     include_package_data=True,
-    version = '0.0.0.5',
+    version = '0.0.0.6',
     license='MIT',
     description = 'Library to login to Dreo cloud and get device info.',
     author = 'Kane Wang',
     author_email = 'app@hesung.com',
     url = 'https://github.com/dreo-team/hscloud',
     download_url = 'https://github.com/dreo-team/hscloud/dist/hscloud-0.0.11.tar.gz',
     install_requires=[
```

