# Comparing `tmp/vonage-3.99.0a8.tar.gz` & `tmp/vonage-3.99.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vonage-3.99.0a8.tar", last modified: Mon Apr 29 01:52:08 2024, max compression
+gzip compressed data, was "vonage-3.99.0a9.tar", last modified: Thu May  9 15:01:57 2024, max compression
```

## Comparing `vonage-3.99.0a8.tar` & `vonage-3.99.0a9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-29 01:52:08.203313 vonage-3.99.0a8/
--rw-r--r--   0 mkahan     (503) staff       (20)     2496 2024-04-29 01:52:08.202703 vonage-3.99.0a8/PKG-INFO
--rw-r--r--   0 mkahan     (503) staff       (20)     1429 2024-04-29 01:52:07.000000 vonage-3.99.0a8/README.md
--rw-r--r--   0 mkahan     (503) staff       (20)      751 2024-04-29 01:52:07.000000 vonage-3.99.0a8/backend_shim.py
--rw-r--r--   0 mkahan     (503) staff       (20)     1133 2024-04-29 01:52:07.000000 vonage-3.99.0a8/pyproject.toml
--rw-r--r--   0 mkahan     (503) staff       (20)       38 2024-04-29 01:52:08.203377 vonage-3.99.0a8/setup.cfg
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-29 01:52:08.196635 vonage-3.99.0a8/src/
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-29 01:52:08.198550 vonage-3.99.0a8/src/vonage/
--rw-r--r--   0 mkahan     (503) staff       (20)      430 2024-04-29 01:52:07.000000 vonage-3.99.0a8/src/vonage/__init__.py
--rw-r--r--   0 mkahan     (503) staff       (20)       25 2024-04-29 01:52:07.000000 vonage-3.99.0a8/src/vonage/_version.py
--rw-r--r--   0 mkahan     (503) staff       (20)     1645 2024-04-29 01:52:07.000000 vonage-3.99.0a8/src/vonage/vonage.py
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-29 01:52:08.202040 vonage-3.99.0a8/src/vonage.egg-info/
--rw-r--r--   0 mkahan     (503) staff       (20)     2496 2024-04-29 01:52:08.000000 vonage-3.99.0a8/src/vonage.egg-info/PKG-INFO
--rw-r--r--   0 mkahan     (503) staff       (20)      276 2024-04-29 01:52:08.000000 vonage-3.99.0a8/src/vonage.egg-info/SOURCES.txt
--rw-r--r--   0 mkahan     (503) staff       (20)        1 2024-04-29 01:52:08.000000 vonage-3.99.0a8/src/vonage.egg-info/dependency_links.txt
--rw-r--r--   0 mkahan     (503) staff       (20)      235 2024-04-29 01:52:08.000000 vonage-3.99.0a8/src/vonage.egg-info/requires.txt
--rw-r--r--   0 mkahan     (503) staff       (20)        7 2024-04-29 01:52:08.000000 vonage-3.99.0a8/src/vonage.egg-info/top_level.txt
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-05-09 15:01:57.987883 vonage-3.99.0a9/
+-rw-r--r--   0 mkahan     (503) staff       (20)     2496 2024-05-09 15:01:57.987175 vonage-3.99.0a9/PKG-INFO
+-rw-r--r--   0 mkahan     (503) staff       (20)     1429 2024-05-09 15:01:57.000000 vonage-3.99.0a9/README.md
+-rw-r--r--   0 mkahan     (503) staff       (20)      751 2024-05-09 15:01:57.000000 vonage-3.99.0a9/backend_shim.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     1133 2024-05-09 15:01:57.000000 vonage-3.99.0a9/pyproject.toml
+-rw-r--r--   0 mkahan     (503) staff       (20)       38 2024-05-09 15:01:57.987969 vonage-3.99.0a9/setup.cfg
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-05-09 15:01:57.980361 vonage-3.99.0a9/src/
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-05-09 15:01:57.983589 vonage-3.99.0a9/src/vonage/
+-rw-r--r--   0 mkahan     (503) staff       (20)      466 2024-05-09 15:01:57.000000 vonage-3.99.0a9/src/vonage/__init__.py
+-rw-r--r--   0 mkahan     (503) staff       (20)       25 2024-05-09 15:01:57.000000 vonage-3.99.0a9/src/vonage/_version.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     1758 2024-05-09 15:01:57.000000 vonage-3.99.0a9/src/vonage/vonage.py
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-05-09 15:01:57.986415 vonage-3.99.0a9/src/vonage.egg-info/
+-rw-r--r--   0 mkahan     (503) staff       (20)     2496 2024-05-09 15:01:57.000000 vonage-3.99.0a9/src/vonage.egg-info/PKG-INFO
+-rw-r--r--   0 mkahan     (503) staff       (20)      276 2024-05-09 15:01:57.000000 vonage-3.99.0a9/src/vonage.egg-info/SOURCES.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)        1 2024-05-09 15:01:57.000000 vonage-3.99.0a9/src/vonage.egg-info/dependency_links.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)      235 2024-05-09 15:01:57.000000 vonage-3.99.0a9/src/vonage.egg-info/requires.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)        7 2024-05-09 15:01:57.000000 vonage-3.99.0a9/src/vonage.egg-info/top_level.txt
```

### Comparing `vonage-3.99.0a8/PKG-INFO` & `vonage-3.99.0a9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vonage
-Version: 3.99.0a8
+Version: 3.99.0a9
 Summary: Python Server SDK for using Vonage APIs
 Author-email: Vonage <devrel@vonage.com>
 Project-URL: homepage, https://github.com/Vonage/vonage-python-sdk
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `vonage-3.99.0a8/README.md` & `vonage-3.99.0a9/README.md`

 * *Files identical despite different names*

### Comparing `vonage-3.99.0a8/backend_shim.py` & `vonage-3.99.0a9/backend_shim.py`

 * *Files identical despite different names*

### Comparing `vonage-3.99.0a8/pyproject.toml` & `vonage-3.99.0a9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vonage-3.99.0a8/src/vonage/vonage.py` & `vonage-3.99.0a9/src/vonage/vonage.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Optional
 
+from vonage_application.application import Application
 from vonage_http_client import Auth, HttpClient, HttpClientOptions
 from vonage_messages import Messages
 from vonage_number_insight import NumberInsight
 from vonage_number_insight_v2 import NumberInsightV2
 from vonage_sms import Sms
 from vonage_users import Users
 from vonage_verify import Verify
@@ -27,14 +28,15 @@
     """
 
     def __init__(
         self, auth: Auth, http_client_options: Optional[HttpClientOptions] = None
     ):
         self._http_client = HttpClient(auth, http_client_options, __version__)
 
+        self.application = Application(self._http_client)
         self.messages = Messages(self._http_client)
         self.number_insight = NumberInsight(self._http_client)
         self.number_insight_v2 = NumberInsightV2(self._http_client)
         self.sms = Sms(self._http_client)
         self.users = Users(self._http_client)
         self.verify = Verify(self._http_client)
         self.verify_v2 = VerifyV2(self._http_client)
```

### Comparing `vonage-3.99.0a8/src/vonage.egg-info/PKG-INFO` & `vonage-3.99.0a9/src/vonage.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vonage
-Version: 3.99.0a8
+Version: 3.99.0a9
 Summary: Python Server SDK for using Vonage APIs
 Author-email: Vonage <devrel@vonage.com>
 Project-URL: homepage, https://github.com/Vonage/vonage-python-sdk
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

