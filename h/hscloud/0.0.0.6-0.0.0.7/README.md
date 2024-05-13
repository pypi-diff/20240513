# Comparing `tmp/hscloud-0.0.0.6.tar.gz` & `tmp/hscloud-0.0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hscloud-0.0.0.6.tar", last modified: Mon May 13 03:34:09 2024, max compression
+gzip compressed data, was "hscloud-0.0.0.7.tar", last modified: Mon May 13 06:21:52 2024, max compression
```

## Comparing `hscloud-0.0.0.6.tar` & `hscloud-0.0.0.7.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 03:34:09.372006 hscloud-0.0.0.6/
--rw-rw-rw-   0        0        0        0 2023-12-18 08:14:13.000000 hscloud-0.0.0.6/LICENSE
--rw-rw-rw-   0        0        0      432 2024-05-13 03:34:09.370006 hscloud-0.0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     2505 2024-05-09 10:10:45.000000 hscloud-0.0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-13 03:34:09.353004 hscloud-0.0.0.6/hscloud/
--rw-rw-rw-   0        0        0      258 2024-05-09 07:57:46.000000 hscloud-0.0.0.6/hscloud/__init__.py
--rw-rw-rw-   0        0        0     4182 2024-05-13 03:29:08.000000 hscloud-0.0.0.6/hscloud/helpers.py
--rw-rw-rw-   0        0        0      829 2024-05-13 03:25:20.000000 hscloud-0.0.0.6/hscloud/hscloud.py
--rw-rw-rw-   0        0        0      289 2024-05-13 03:32:42.000000 hscloud-0.0.0.6/hscloud/hscloudexception.py
-drwxrwxrwx   0        0        0        0 2024-05-13 03:34:09.368004 hscloud-0.0.0.6/hscloud.egg-info/
--rw-rw-rw-   0        0        0      432 2024-05-13 03:34:09.000000 hscloud-0.0.0.6/hscloud.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      300 2024-05-13 03:34:09.000000 hscloud-0.0.0.6/hscloud.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 03:34:09.000000 hscloud-0.0.0.6/hscloud.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2024-05-13 03:34:09.000000 hscloud-0.0.0.6/hscloud.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       36 2024-05-13 03:34:09.000000 hscloud-0.0.0.6/hscloud.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-13 03:34:09.000000 hscloud-0.0.0.6/hscloud.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-13 03:34:09.372006 hscloud-0.0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      887 2024-05-13 03:33:40.000000 hscloud-0.0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 06:21:52.777007 hscloud-0.0.0.7/
+-rw-rw-rw-   0        0        0        0 2023-12-18 08:14:13.000000 hscloud-0.0.0.7/LICENSE
+-rw-rw-rw-   0        0        0      432 2024-05-13 06:21:52.775005 hscloud-0.0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2505 2024-05-09 10:10:45.000000 hscloud-0.0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 06:21:52.753005 hscloud-0.0.0.7/hscloud/
+-rw-rw-rw-   0        0        0      258 2024-05-09 07:57:46.000000 hscloud-0.0.0.7/hscloud/__init__.py
+-rw-rw-rw-   0        0        0     3980 2024-05-13 06:16:45.000000 hscloud-0.0.0.7/hscloud/helpers.py
+-rw-rw-rw-   0        0        0      916 2024-05-13 06:16:07.000000 hscloud-0.0.0.7/hscloud/hscloud.py
+drwxrwxrwx   0        0        0        0 2024-05-13 06:21:52.773005 hscloud-0.0.0.7/hscloud.egg-info/
+-rw-rw-rw-   0        0        0      432 2024-05-13 06:21:52.000000 hscloud-0.0.0.7/hscloud.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2024-05-13 06:21:52.000000 hscloud-0.0.0.7/hscloud.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 06:21:52.000000 hscloud-0.0.0.7/hscloud.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2024-05-13 06:21:52.000000 hscloud-0.0.0.7/hscloud.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       36 2024-05-13 06:21:52.000000 hscloud-0.0.0.7/hscloud.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-13 06:21:52.000000 hscloud-0.0.0.7/hscloud.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 06:21:52.777007 hscloud-0.0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      887 2024-05-13 06:21:35.000000 hscloud-0.0.0.7/setup.py
```

### Comparing `hscloud-0.0.0.6/README.md` & `hscloud-0.0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `hscloud-0.0.0.6/hscloud/helpers.py` & `hscloud-0.0.0.7/hscloud/helpers.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import requests
 from datetime import datetime
 from typing import Optional
-from .hscloudexception import HsCloudAccessDenied, HsCloudException
 import logging
 
 logger = logging.getLogger(__name__)
 
 class Helpers:
 
     @staticmethod
@@ -40,16 +39,14 @@
             'UA': 'openapi/1.0.0'
         }
 
         params = {
             'timestamp': Helpers.timestamp()
         }
 
-        result = Helpers.call_api(endpoint + "/api/device/list", "get", headers, params)
-
         return Helpers.call_api(endpoint + "/api/device/list", "get", headers, params)
 
     @staticmethod
     def status(endpoint=None, access_token=None, devicesn=None):
         headers = {
             'Content-Type': 'application/json',
             'Authorization': f'Bearer {access_token}',
@@ -94,22 +91,23 @@
         else:
             if response.status_code == 200:
                 response_body = response.json()
                 code = response_body.get("code")
                 if code == 0:
                     response = response_body.get("data")
                 elif code == 401:
-                    raise HsCloudAccessDenied("Cannot execute request. token invalid. Make sure to login.")
+                    logger.error("Cannot execute request. token invalid. Make sure to login.")
                 else:
-                    raise HsCloudException(response_body.get("msg"))
+                    logger.error(response_body.get("msg"))
 
             elif response.status_code == 429:
-                raise HsCloudException("Your request is too frequent, please try again later.")
+                logger.error("Your request is too frequent, please try again later.")
             else:
-                raise HsCloudException("There is a service problem, please try again later.")
+                logger.error("There is a service problem, please try again later.")
+
         return response
 
     @staticmethod
     def update_body(devicesn, **kwargs):
         data = {
             'devicesn': devicesn
         }
```

### Comparing `hscloud-0.0.0.6/hscloud/hscloud.py` & `hscloud-0.0.0.7/hscloud/hscloud.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,17 +7,20 @@
         self.username = username
         self.password = password
         self.endpoint = None
         self.access_token = None
 
     def login(self):
         response = Helpers.login(self.username, self.password)
-        self.endpoint = response.get("endpoint")
-        self.access_token = response.get("access_token")
-        return True
+        if response is not None:
+            self.endpoint = response.get("endpoint")
+            self.access_token = response.get("access_token")
+            return True
+        else:
+            return False
 
     def get_devices(self):
         return Helpers.devices(self.endpoint, self.access_token)
 
     def get_status(self, devicesn):
         return Helpers.status(self.endpoint, self.access_token, devicesn)
```

### Comparing `hscloud-0.0.0.6/setup.py` & `hscloud-0.0.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name = 'hscloud',
     packages = ['hscloud'],
     include_package_data=True,
-    version = '0.0.0.6',
+    version = '0.0.0.7',
     license='MIT',
     description = 'Library to login to Dreo cloud and get device info.',
     author = 'Kane Wang',
     author_email = 'app@hesung.com',
     url = 'https://github.com/dreo-team/hscloud',
     download_url = 'https://github.com/dreo-team/hscloud/dist/hscloud-0.0.11.tar.gz',
     install_requires=[
```

