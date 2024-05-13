# Comparing `tmp/hscloud-0.0.0.7.tar.gz` & `tmp/hscloud-0.0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hscloud-0.0.0.7.tar", last modified: Mon May 13 06:21:52 2024, max compression
+gzip compressed data, was "hscloud-0.0.0.8.tar", last modified: Mon May 13 06:40:11 2024, max compression
```

## Comparing `hscloud-0.0.0.7.tar` & `hscloud-0.0.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 06:21:52.777007 hscloud-0.0.0.7/
--rw-rw-rw-   0        0        0        0 2023-12-18 08:14:13.000000 hscloud-0.0.0.7/LICENSE
--rw-rw-rw-   0        0        0      432 2024-05-13 06:21:52.775005 hscloud-0.0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     2505 2024-05-09 10:10:45.000000 hscloud-0.0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-13 06:21:52.753005 hscloud-0.0.0.7/hscloud/
--rw-rw-rw-   0        0        0      258 2024-05-09 07:57:46.000000 hscloud-0.0.0.7/hscloud/__init__.py
--rw-rw-rw-   0        0        0     3980 2024-05-13 06:16:45.000000 hscloud-0.0.0.7/hscloud/helpers.py
--rw-rw-rw-   0        0        0      916 2024-05-13 06:16:07.000000 hscloud-0.0.0.7/hscloud/hscloud.py
-drwxrwxrwx   0        0        0        0 2024-05-13 06:21:52.773005 hscloud-0.0.0.7/hscloud.egg-info/
--rw-rw-rw-   0        0        0      432 2024-05-13 06:21:52.000000 hscloud-0.0.0.7/hscloud.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2024-05-13 06:21:52.000000 hscloud-0.0.0.7/hscloud.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 06:21:52.000000 hscloud-0.0.0.7/hscloud.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2024-05-13 06:21:52.000000 hscloud-0.0.0.7/hscloud.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       36 2024-05-13 06:21:52.000000 hscloud-0.0.0.7/hscloud.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-13 06:21:52.000000 hscloud-0.0.0.7/hscloud.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-13 06:21:52.777007 hscloud-0.0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      887 2024-05-13 06:21:35.000000 hscloud-0.0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 06:40:11.511534 hscloud-0.0.0.8/
+-rw-rw-rw-   0        0        0        0 2023-12-18 08:14:13.000000 hscloud-0.0.0.8/LICENSE
+-rw-rw-rw-   0        0        0      432 2024-05-13 06:40:11.509534 hscloud-0.0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2505 2024-05-09 10:10:45.000000 hscloud-0.0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 06:40:11.491532 hscloud-0.0.0.8/hscloud/
+-rw-rw-rw-   0        0        0      258 2024-05-09 07:57:46.000000 hscloud-0.0.0.8/hscloud/__init__.py
+-rw-rw-rw-   0        0        0     3999 2024-05-13 06:32:11.000000 hscloud-0.0.0.8/hscloud/helpers.py
+-rw-rw-rw-   0        0        0     1267 2024-05-13 06:38:22.000000 hscloud-0.0.0.8/hscloud/hscloud.py
+drwxrwxrwx   0        0        0        0 2024-05-13 06:40:11.507533 hscloud-0.0.0.8/hscloud.egg-info/
+-rw-rw-rw-   0        0        0      432 2024-05-13 06:40:11.000000 hscloud-0.0.0.8/hscloud.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2024-05-13 06:40:11.000000 hscloud-0.0.0.8/hscloud.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 06:40:11.000000 hscloud-0.0.0.8/hscloud.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2024-05-13 06:40:11.000000 hscloud-0.0.0.8/hscloud.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       36 2024-05-13 06:40:11.000000 hscloud-0.0.0.8/hscloud.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-13 06:40:11.000000 hscloud-0.0.0.8/hscloud.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 06:40:11.512534 hscloud-0.0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      887 2024-05-13 06:39:39.000000 hscloud-0.0.0.8/setup.py
```

### Comparing `hscloud-0.0.0.7/README.md` & `hscloud-0.0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `hscloud-0.0.0.7/hscloud/helpers.py` & `hscloud-0.0.0.8/hscloud/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,14 +72,15 @@
             'timestamp': Helpers.timestamp()
         }
 
         return Helpers.call_api(endpoint + "/api/device/control", "post", headers, params, Helpers.update_body(devicesn, **kwargs))
 
     @staticmethod
     def call_api(api: str, method: str, headers: Optional[dict] = None, params: Optional[dict] = None, json_body: Optional[dict] = None) -> tuple:
+        result = None
         response = None
         try:
             if method.lower() == "get":
                 response = requests.get(api, headers=headers, params=params, timeout=8)
 
             elif method.lower() == "post":
                 response = requests.post(api, headers=headers, params=params, json=json_body, timeout=8)
@@ -89,26 +90,26 @@
         except Exception as e:
             logger.error(e)
         else:
             if response.status_code == 200:
                 response_body = response.json()
                 code = response_body.get("code")
                 if code == 0:
-                    response = response_body.get("data")
+                    result = response_body.get("data")
                 elif code == 401:
                     logger.error("Cannot execute request. token invalid. Make sure to login.")
                 else:
                     logger.error(response_body.get("msg"))
 
             elif response.status_code == 429:
                 logger.error("Your request is too frequent, please try again later.")
             else:
                 logger.error("There is a service problem, please try again later.")
 
-        return response
+        return result
 
     @staticmethod
     def update_body(devicesn, **kwargs):
         data = {
             'devicesn': devicesn
         }
```

### Comparing `hscloud-0.0.0.7/setup.py` & `hscloud-0.0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name = 'hscloud',
     packages = ['hscloud'],
     include_package_data=True,
-    version = '0.0.0.7',
+    version = '0.0.0.8',
     license='MIT',
     description = 'Library to login to Dreo cloud and get device info.',
     author = 'Kane Wang',
     author_email = 'app@hesung.com',
     url = 'https://github.com/dreo-team/hscloud',
     download_url = 'https://github.com/dreo-team/hscloud/dist/hscloud-0.0.11.tar.gz',
     install_requires=[
```

