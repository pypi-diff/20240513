# Comparing `tmp/scrippy-api-1.1.84.tar.gz` & `tmp/scrippy_api-1.1.85.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrippy-api-1.1.84.tar", last modified: Tue Oct 10 11:41:01 2023, max compression
+gzip compressed data, was "scrippy_api-1.1.85.tar", last modified: Mon May 13 07:57:40 2024, max compression
```

## Comparing `scrippy-api-1.1.84.tar` & `scrippy_api-1.1.85.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-10 11:41:01.464515 scrippy-api-1.1.84/
--rwxr-xr-x   0 root         (0) root         (0)     1179 2023-10-10 11:39:50.000000 scrippy-api-1.1.84/LICENSE
--rw-r--r--   0 root         (0) root         (0)     7568 2023-10-10 11:41:01.464515 scrippy-api-1.1.84/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5965 2023-10-10 11:39:50.000000 scrippy-api-1.1.84/README.md
--rw-r--r--   0 root         (0) root         (0)      210 2023-10-10 11:39:50.000000 scrippy-api-1.1.84/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1330 2023-10-10 11:41:01.465515 scrippy-api-1.1.84/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)       38 2023-10-10 11:39:50.000000 scrippy-api-1.1.84/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-10 11:41:01.452515 scrippy-api-1.1.84/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-10 11:41:01.454516 scrippy-api-1.1.84/src/scrippy_api/
--rw-r--r--   0 root         (0) root         (0)      219 2023-10-10 11:39:50.000000 scrippy-api-1.1.84/src/scrippy_api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-10 11:41:01.457515 scrippy-api-1.1.84/src/scrippy_api/api/
--rw-r--r--   0 root         (0) root         (0)       90 2023-10-10 11:39:50.000000 scrippy-api-1.1.84/src/scrippy_api/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1708 2023-10-10 11:39:50.000000 scrippy-api-1.1.84/src/scrippy_api/api/apiloader.py
--rw-r--r--   0 root         (0) root         (0)     4997 2023-10-10 11:39:50.000000 scrippy-api-1.1.84/src/scrippy_api/api/client.py
--rw-r--r--   0 root         (0) root         (0)      327 2023-10-10 11:39:50.000000 scrippy-api-1.1.84/src/scrippy_api/api/validator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-10 11:41:01.456515 scrippy-api-1.1.84/src/scrippy_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7568 2023-10-10 11:41:01.000000 scrippy-api-1.1.84/src/scrippy_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      444 2023-10-10 11:41:01.000000 scrippy-api-1.1.84/src/scrippy_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-10 11:41:01.000000 scrippy-api-1.1.84/src/scrippy_api.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      313 2023-10-10 11:41:01.000000 scrippy-api-1.1.84/src/scrippy_api.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-10-10 11:41:01.000000 scrippy-api-1.1.84/src/scrippy_api.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-10 11:41:01.458515 scrippy-api-1.1.84/tests/
--rw-r--r--   0 root         (0) root         (0)     1584 2023-10-10 11:39:50.000000 scrippy-api-1.1.84/tests/test_basic_url.py
--rw-r--r--   0 root         (0) root         (0)     3320 2023-10-10 11:39:50.000000 scrippy-api-1.1.84/tests/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 07:57:40.791099 scrippy_api-1.1.85/
+-rwxr-xr-x   0 root         (0) root         (0)     1179 2024-05-13 07:56:41.000000 scrippy_api-1.1.85/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     7666 2024-05-13 07:57:40.791099 scrippy_api-1.1.85/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6063 2024-05-13 07:56:41.000000 scrippy_api-1.1.85/README.md
+-rw-r--r--   0 root         (0) root         (0)      210 2024-05-13 07:56:41.000000 scrippy_api-1.1.85/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1330 2024-05-13 07:57:40.816098 scrippy_api-1.1.85/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)       38 2024-05-13 07:56:41.000000 scrippy_api-1.1.85/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 07:57:40.778099 scrippy_api-1.1.85/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 07:57:40.781099 scrippy_api-1.1.85/src/scrippy_api/
+-rw-r--r--   0 root         (0) root         (0)      219 2024-05-13 07:56:41.000000 scrippy_api-1.1.85/src/scrippy_api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 07:57:40.784099 scrippy_api-1.1.85/src/scrippy_api/api/
+-rw-r--r--   0 root         (0) root         (0)       90 2024-05-13 07:56:41.000000 scrippy_api-1.1.85/src/scrippy_api/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1708 2024-05-13 07:56:41.000000 scrippy_api-1.1.85/src/scrippy_api/api/apiloader.py
+-rw-r--r--   0 root         (0) root         (0)     5787 2024-05-13 07:56:41.000000 scrippy_api-1.1.85/src/scrippy_api/api/client.py
+-rw-r--r--   0 root         (0) root         (0)      327 2024-05-13 07:56:41.000000 scrippy_api-1.1.85/src/scrippy_api/api/validator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 07:57:40.785099 scrippy_api-1.1.85/src/scrippy_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7666 2024-05-13 07:57:40.000000 scrippy_api-1.1.85/src/scrippy_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      444 2024-05-13 07:57:40.000000 scrippy_api-1.1.85/src/scrippy_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-13 07:57:40.000000 scrippy_api-1.1.85/src/scrippy_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      313 2024-05-13 07:57:40.000000 scrippy_api-1.1.85/src/scrippy_api.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-05-13 07:57:40.000000 scrippy_api-1.1.85/src/scrippy_api.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 07:57:40.785099 scrippy_api-1.1.85/tests/
+-rw-r--r--   0 root         (0) root         (0)     1584 2024-05-13 07:56:41.000000 scrippy_api-1.1.85/tests/test_basic_url.py
+-rw-r--r--   0 root         (0) root         (0)     3320 2024-05-13 07:56:41.000000 scrippy_api-1.1.85/tests/test_post.py
```

### Comparing `scrippy-api-1.1.84/LICENSE` & `scrippy_api-1.1.85/LICENSE`

 * *Files identical despite different names*

### Comparing `scrippy-api-1.1.84/PKG-INFO` & `scrippy_api-1.1.85/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrippy-api
-Version: 1.1.84
+Version: 1.1.85
 Summary: "Fonctions d'utilisation d'API ReST."
 Home-page: https://codeberg.org/scrippy/scrippy-api
 Author: Michael Costa, Florent Chevalier
 Author-email: michael.costa@mcos.nc, florent.chevalier.nc@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -115,15 +115,14 @@
 | `headers` | Dictionary | Headers to be sent with the request | `None` |
 | `proxies` | List | List of proxy servers to use for the connection | `None` |
 | `auth`    | Tuple | Username and password for _BASIC AUTH_ authentication |
 | `data`    | Dictionary | Data to be sent with the request. Not applicable with `GET` method | `None` |
 | `json`    | Dictionary | Data in _JSON_ format to be sent with the request. Not applicable with `GET` method. Use when `data` and `file` are not specified | `None` |
 | `files`   | Dictionary | Files to be uploaded in _multipart_. The dictionary takes the form `{<file name>: <file>}`  | `None` |
 
-
 Implemented HTTP methods:
 
 | HTTP method | Description |
 | -----------| ------------ |
 | `GET`        | Retrieve a resource or list of resource URIs |
 | `POST`       | Create a resource |
 | `PUT`        | Replace or create a resource |
@@ -179,14 +178,16 @@
 ```python
 from scrippy_api.api import Client
 files = {"dead_parrot.png": open("./images/dead_parrot.png", "rb"), "flying_circus.mp4": open("./images/flying_circus.mp4", "rb")}
 client = Client()
 response = client.request(method="POST", url="https://montypython.org/upload", data=data)
 ```
 
+All `POST` parameters are available for upload.
+
 ##### Resource Modification
 
 Replaces the password of the `Luiggi Vercotti` user
 
 ```python
 from scrippy_api.api import Client
 auth = ("Luiggi Vercotti", "dead/parrot")
@@ -206,7 +207,9 @@
 url = "https://monthy.python/inquisition.zip"
 local_dir = "/home/luiggi.vercotti"
 local_filename = "spanish_inquisition.zip"
 client = Client()
 if client.download(url, local_dir, local_filename):
   print("No one expects the Spanish inquisition")
 ```
+
+All `GET` parameters are available for download.
```

### Comparing `scrippy-api-1.1.84/README.md` & `scrippy_api-1.1.85/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,14 @@
 | `headers` | Dictionary | Headers to be sent with the request | `None` |
 | `proxies` | List | List of proxy servers to use for the connection | `None` |
 | `auth`    | Tuple | Username and password for _BASIC AUTH_ authentication |
 | `data`    | Dictionary | Data to be sent with the request. Not applicable with `GET` method | `None` |
 | `json`    | Dictionary | Data in _JSON_ format to be sent with the request. Not applicable with `GET` method. Use when `data` and `file` are not specified | `None` |
 | `files`   | Dictionary | Files to be uploaded in _multipart_. The dictionary takes the form `{<file name>: <file>}`  | `None` |
 
-
 Implemented HTTP methods:
 
 | HTTP method | Description |
 | -----------| ------------ |
 | `GET`        | Retrieve a resource or list of resource URIs |
 | `POST`       | Create a resource |
 | `PUT`        | Replace or create a resource |
@@ -141,14 +140,16 @@
 ```python
 from scrippy_api.api import Client
 files = {"dead_parrot.png": open("./images/dead_parrot.png", "rb"), "flying_circus.mp4": open("./images/flying_circus.mp4", "rb")}
 client = Client()
 response = client.request(method="POST", url="https://montypython.org/upload", data=data)
 ```
 
+All `POST` parameters are available for upload.
+
 ##### Resource Modification
 
 Replaces the password of the `Luiggi Vercotti` user
 
 ```python
 from scrippy_api.api import Client
 auth = ("Luiggi Vercotti", "dead/parrot")
@@ -168,7 +169,9 @@
 url = "https://monthy.python/inquisition.zip"
 local_dir = "/home/luiggi.vercotti"
 local_filename = "spanish_inquisition.zip"
 client = Client()
 if client.download(url, local_dir, local_filename):
   print("No one expects the Spanish inquisition")
 ```
+
+All `GET` parameters are available for download.
```

### Comparing `scrippy-api-1.1.84/setup.cfg` & `scrippy_api-1.1.85/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-version = 1.1.84
+version = 1.1.85
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Topic :: Software Development :: Libraries :: Application Frameworks
 	Intended Audience :: Developers
 	Intended Audience :: System Administrators
```

### Comparing `scrippy-api-1.1.84/src/scrippy_api/api/apiloader.py` & `scrippy_api-1.1.85/src/scrippy_api/api/apiloader.py`

 * *Files identical despite different names*

### Comparing `scrippy-api-1.1.84/src/scrippy_api/api/client.py` & `scrippy_api-1.1.85/src/scrippy_api/api/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,45 +19,58 @@
     """
     self.exit_on_error = exit_on_error
     self.verify = verify
     self.session = requests.Session()
     if not self.verify:
       requests.packages.urllib3.disable_warnings(requests.packages.urllib3.exceptions.InsecureRequestWarning)
 
-  def download(self, url, local_path, filename='', timeout=30):
+  def download(self, url, local_path, filename='',
+               timeout=30, params=None, headers=None,
+               cookies=None, proxies=None, auth=None):
     """
     Enables file download.
 
     :param url: The URL from which to download the file.
     :param local_path: The directory in which to save the file.
     :param filename: The local file name.
-    :param timeout: The maximum wait time, defaults to 30s.
+    :param timeout: The maximum wait time, defaults to None.
+    :param params: The query parameters (GET) for the request, defaults to None.
+    :param headers: The headers for the request, defaults to None.
+    :param cookies: The cookies for the request, defaults to None.
+    :param proxies: The list of proxy servers to use, defaults to None.
+    :param auth: The authentication information (BASIC AUTH) as a tuple (user, password), defaults to None.
+    :return: Boolean. True if succeed. If exit_on_error is set to True and download is unsuccessful raise a ScrippyApiError.
+    :rtype: Boolean
     """
     if len(filename) == 0:
       filename = url.split('/')[-1]
     filename = os.path.join(local_path, filename)
     logger.debug("[+] Downloading file")
     logger.debug(f" '-> From: {url}")
     logger.debug(f" '-> To: {filename}")
     try:
-      with requests.get(url, stream=True, timeout=timeout) as response:
+      with requests.get(url, stream=True, params=params, headers=headers,
+                        cookies=cookies, proxies=proxies, auth=auth,
+                        verify=self.verify) as response:
         response.raise_for_status()
         with open(filename, 'wb') as dl_file:
           for chunk in response.iter_content(chunk_size=8192):
             dl_file.write(chunk)
       return True
     except Exception as err:
       if self.exit_on_error:
         err_msg = f"Request error: [{err.__class__.__name__}] {err}"
         raise ScrippyApiError(err_msg) from err
       else:
         logger.warning(f"Request error: [{err.__class__.__name__}] {err}")
-        return response
+        return False
 
-  def request(self, method, url, params=None, data=None, headers=None, cookies=None, files=None, auth=None, timeout=None, proxies=None, json=None):
+  def request(self, method, url, params=None, data=None, headers=None,
+              cookies=None, files=None, auth=None, timeout=None,
+              proxies=None, json=None):
     """
     Allows the execution of an HTTP request.
 
     :param method: The HTTP method to use.
     :param url: The URL to reach.
     :param params: The query parameters (GET) for the request, defaults to None.
     :param data: The data parameters (POST) for the request, defaults to None.
```

### Comparing `scrippy-api-1.1.84/src/scrippy_api.egg-info/PKG-INFO` & `scrippy_api-1.1.85/src/scrippy_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrippy-api
-Version: 1.1.84
+Version: 1.1.85
 Summary: "Fonctions d'utilisation d'API ReST."
 Home-page: https://codeberg.org/scrippy/scrippy-api
 Author: Michael Costa, Florent Chevalier
 Author-email: michael.costa@mcos.nc, florent.chevalier.nc@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -115,15 +115,14 @@
 | `headers` | Dictionary | Headers to be sent with the request | `None` |
 | `proxies` | List | List of proxy servers to use for the connection | `None` |
 | `auth`    | Tuple | Username and password for _BASIC AUTH_ authentication |
 | `data`    | Dictionary | Data to be sent with the request. Not applicable with `GET` method | `None` |
 | `json`    | Dictionary | Data in _JSON_ format to be sent with the request. Not applicable with `GET` method. Use when `data` and `file` are not specified | `None` |
 | `files`   | Dictionary | Files to be uploaded in _multipart_. The dictionary takes the form `{<file name>: <file>}`  | `None` |
 
-
 Implemented HTTP methods:
 
 | HTTP method | Description |
 | -----------| ------------ |
 | `GET`        | Retrieve a resource or list of resource URIs |
 | `POST`       | Create a resource |
 | `PUT`        | Replace or create a resource |
@@ -179,14 +178,16 @@
 ```python
 from scrippy_api.api import Client
 files = {"dead_parrot.png": open("./images/dead_parrot.png", "rb"), "flying_circus.mp4": open("./images/flying_circus.mp4", "rb")}
 client = Client()
 response = client.request(method="POST", url="https://montypython.org/upload", data=data)
 ```
 
+All `POST` parameters are available for upload.
+
 ##### Resource Modification
 
 Replaces the password of the `Luiggi Vercotti` user
 
 ```python
 from scrippy_api.api import Client
 auth = ("Luiggi Vercotti", "dead/parrot")
@@ -206,7 +207,9 @@
 url = "https://monthy.python/inquisition.zip"
 local_dir = "/home/luiggi.vercotti"
 local_filename = "spanish_inquisition.zip"
 client = Client()
 if client.download(url, local_dir, local_filename):
   print("No one expects the Spanish inquisition")
 ```
+
+All `GET` parameters are available for download.
```

### Comparing `scrippy-api-1.1.84/tests/test_basic_url.py` & `scrippy_api-1.1.85/tests/test_basic_url.py`

 * *Files identical despite different names*

### Comparing `scrippy-api-1.1.84/tests/test_post.py` & `scrippy_api-1.1.85/tests/test_post.py`

 * *Files identical despite different names*

