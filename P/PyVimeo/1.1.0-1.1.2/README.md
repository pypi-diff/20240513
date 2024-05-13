# Comparing `tmp/PyVimeo-1.1.0.tar.gz` & `tmp/pyvimeo-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PyVimeo-1.1.0.tar", last modified: Mon Jul 13 19:20:54 2020, max compression
+gzip compressed data, was "pyvimeo-1.1.2.tar", last modified: Mon May 13 19:52:53 2024, max compression
```

## Comparing `PyVimeo-1.1.0.tar` & `pyvimeo-1.1.2.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 mattfisher   (502) staff       (20)        0 2020-07-13 19:20:54.000000 PyVimeo-1.1.0/
--rw-r--r--   0 mattfisher   (502) staff       (20)     1044 2020-07-13 19:20:54.000000 PyVimeo-1.1.0/PKG-INFO
-drwxr-xr-x   0 mattfisher   (502) staff       (20)        0 2020-07-13 19:20:54.000000 PyVimeo-1.1.0/PyVimeo.egg-info/
--rw-r--r--   0 mattfisher   (502) staff       (20)     1044 2020-07-13 19:20:54.000000 PyVimeo-1.1.0/PyVimeo.egg-info/PKG-INFO
--rw-r--r--   0 mattfisher   (502) staff       (20)      350 2020-07-13 19:20:54.000000 PyVimeo-1.1.0/PyVimeo.egg-info/SOURCES.txt
--rw-r--r--   0 mattfisher   (502) staff       (20)       29 2020-07-13 19:20:54.000000 PyVimeo-1.1.0/PyVimeo.egg-info/requires.txt
--rw-r--r--   0 mattfisher   (502) staff       (20)       17 2020-07-13 19:20:54.000000 PyVimeo-1.1.0/PyVimeo.egg-info/top_level.txt
--rw-r--r--   0 mattfisher   (502) staff       (20)        1 2020-07-13 19:20:54.000000 PyVimeo-1.1.0/PyVimeo.egg-info/dependency_links.txt
-drwxr-xr-x   0 mattfisher   (502) staff       (20)        0 2020-07-13 19:20:54.000000 PyVimeo-1.1.0/vimeo/
--rw-r--r--   0 mattfisher   (502) staff       (20)    10655 2020-07-13 16:38:22.000000 PyVimeo-1.1.0/vimeo/upload.py
-drwxr-xr-x   0 mattfisher   (502) staff       (20)        0 2020-07-13 19:20:54.000000 PyVimeo-1.1.0/vimeo/auth/
--rw-r--r--   0 mattfisher   (502) staff       (20)      118 2020-07-13 16:38:22.000000 PyVimeo-1.1.0/vimeo/auth/__init__.py
--rw-r--r--   0 mattfisher   (502) staff       (20)     1348 2020-07-13 16:38:22.000000 PyVimeo-1.1.0/vimeo/auth/authorization_code.py
--rw-r--r--   0 mattfisher   (502) staff       (20)      820 2020-07-13 16:38:22.000000 PyVimeo-1.1.0/vimeo/auth/client_credentials.py
--rw-r--r--   0 mattfisher   (502) staff       (20)      533 2020-07-13 16:38:22.000000 PyVimeo-1.1.0/vimeo/auth/base.py
--rw-r--r--   0 mattfisher   (502) staff       (20)     3306 2020-07-13 16:38:22.000000 PyVimeo-1.1.0/vimeo/client.py
--rw-r--r--   0 mattfisher   (502) staff       (20)      121 2020-07-13 16:38:22.000000 PyVimeo-1.1.0/vimeo/__init__.py
--rw-r--r--   0 mattfisher   (502) staff       (20)     4904 2020-07-13 16:38:22.000000 PyVimeo-1.1.0/vimeo/exceptions.py
--rw-r--r--   0 mattfisher   (502) staff       (20)     8537 2020-07-13 16:38:22.000000 PyVimeo-1.1.0/README.md
--rw-r--r--   0 mattfisher   (502) staff       (20)     1191 2020-07-13 19:16:12.000000 PyVimeo-1.1.0/setup.py
--rw-r--r--   0 mattfisher   (502) staff       (20)       38 2020-07-13 19:20:54.000000 PyVimeo-1.1.0/setup.cfg
+drwxr-xr-x   0 dominick.modica   (502) staff       (20)        0 2024-05-13 19:52:53.151219 pyvimeo-1.1.2/
+-rw-r--r--   0 dominick.modica   (502) staff       (20)    11341 2024-05-13 14:53:20.000000 pyvimeo-1.1.2/LICENSE
+-rw-r--r--   0 dominick.modica   (502) staff       (20)     1069 2024-05-13 19:52:53.150893 pyvimeo-1.1.2/PKG-INFO
+drwxr-xr-x   0 dominick.modica   (502) staff       (20)        0 2024-05-13 19:52:53.150399 pyvimeo-1.1.2/PyVimeo.egg-info/
+-rw-r--r--   0 dominick.modica   (502) staff       (20)     1069 2024-05-13 19:52:53.000000 pyvimeo-1.1.2/PyVimeo.egg-info/PKG-INFO
+-rw-r--r--   0 dominick.modica   (502) staff       (20)      358 2024-05-13 19:52:53.000000 pyvimeo-1.1.2/PyVimeo.egg-info/SOURCES.txt
+-rw-r--r--   0 dominick.modica   (502) staff       (20)        1 2024-05-13 19:52:53.000000 pyvimeo-1.1.2/PyVimeo.egg-info/dependency_links.txt
+-rw-r--r--   0 dominick.modica   (502) staff       (20)       29 2024-05-13 19:52:53.000000 pyvimeo-1.1.2/PyVimeo.egg-info/requires.txt
+-rw-r--r--   0 dominick.modica   (502) staff       (20)       17 2024-05-13 19:52:53.000000 pyvimeo-1.1.2/PyVimeo.egg-info/top_level.txt
+-rw-r--r--   0 dominick.modica   (502) staff       (20)     1432 2024-05-13 14:53:20.000000 pyvimeo-1.1.2/README.md
+-rw-r--r--   0 dominick.modica   (502) staff       (20)       38 2024-05-13 19:52:53.151267 pyvimeo-1.1.2/setup.cfg
+-rw-r--r--   0 dominick.modica   (502) staff       (20)     1191 2024-05-13 19:52:10.000000 pyvimeo-1.1.2/setup.py
+drwxr-xr-x   0 dominick.modica   (502) staff       (20)        0 2024-05-13 19:52:53.148744 pyvimeo-1.1.2/vimeo/
+-rw-r--r--   0 dominick.modica   (502) staff       (20)      121 2024-05-13 14:53:20.000000 pyvimeo-1.1.2/vimeo/__init__.py
+drwxr-xr-x   0 dominick.modica   (502) staff       (20)        0 2024-05-13 19:52:53.149878 pyvimeo-1.1.2/vimeo/auth/
+-rw-r--r--   0 dominick.modica   (502) staff       (20)      118 2024-05-13 14:53:20.000000 pyvimeo-1.1.2/vimeo/auth/__init__.py
+-rw-r--r--   0 dominick.modica   (502) staff       (20)     1348 2024-05-13 14:53:20.000000 pyvimeo-1.1.2/vimeo/auth/authorization_code.py
+-rw-r--r--   0 dominick.modica   (502) staff       (20)      533 2024-05-13 14:53:20.000000 pyvimeo-1.1.2/vimeo/auth/base.py
+-rw-r--r--   0 dominick.modica   (502) staff       (20)      820 2024-05-13 14:53:20.000000 pyvimeo-1.1.2/vimeo/auth/client_credentials.py
+-rw-r--r--   0 dominick.modica   (502) staff       (20)     3306 2024-05-13 14:53:20.000000 pyvimeo-1.1.2/vimeo/client.py
+-rw-r--r--   0 dominick.modica   (502) staff       (20)     5071 2024-05-13 19:45:48.000000 pyvimeo-1.1.2/vimeo/exceptions.py
+-rw-r--r--   0 dominick.modica   (502) staff       (20)    10655 2024-05-13 14:53:20.000000 pyvimeo-1.1.2/vimeo/upload.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `PyVimeo-1.1.0/PKG-INFO` & `pyvimeo-1.1.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,14 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: PyVimeo
-Version: 1.1.0
+Version: 1.1.2
 Summary: Simple interaction with the Vimeo API.
 Home-page: https://developer.vimeo.com/
 Author: Vimeo
 Author-email: support@vimeo.com
-License: UNKNOWN
-Description: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -21,7 +18,10 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Internet
 Classifier: Topic :: Multimedia :: Video
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.5
+License-File: LICENSE
+Requires-Dist: requests>=2.4.0
+Requires-Dist: tuspy>=0.2.4
```

### Comparing `PyVimeo-1.1.0/PyVimeo.egg-info/PKG-INFO` & `pyvimeo-1.1.2/PyVimeo.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,14 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: PyVimeo
-Version: 1.1.0
+Version: 1.1.2
 Summary: Simple interaction with the Vimeo API.
 Home-page: https://developer.vimeo.com/
 Author: Vimeo
 Author-email: support@vimeo.com
-License: UNKNOWN
-Description: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -21,7 +18,10 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Internet
 Classifier: Topic :: Multimedia :: Video
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.5
+License-File: LICENSE
+Requires-Dist: requests>=2.4.0
+Requires-Dist: tuspy>=0.2.4
```

### Comparing `PyVimeo-1.1.0/vimeo/upload.py` & `pyvimeo-1.1.2/vimeo/upload.py`

 * *Files identical despite different names*

### Comparing `PyVimeo-1.1.0/vimeo/auth/authorization_code.py` & `pyvimeo-1.1.2/vimeo/auth/authorization_code.py`

 * *Files identical despite different names*

### Comparing `PyVimeo-1.1.0/vimeo/auth/client_credentials.py` & `pyvimeo-1.1.2/vimeo/auth/client_credentials.py`

 * *Files identical despite different names*

### Comparing `PyVimeo-1.1.0/vimeo/auth/base.py` & `pyvimeo-1.1.2/vimeo/auth/base.py`

 * *Files identical despite different names*

### Comparing `PyVimeo-1.1.0/vimeo/client.py` & `pyvimeo-1.1.2/vimeo/client.py`

 * *Files identical despite different names*

### Comparing `PyVimeo-1.1.0/vimeo/exceptions.py` & `pyvimeo-1.1.2/vimeo/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,28 +2,30 @@
 
 
 class BaseVimeoException(Exception):
     """Base class for Vimeo Exceptions."""
 
     def __get_message(self, response):
         if type(response) is Exception:
-            return response.message
+            default_message = 'There was an unexpected error'
+            return response.message if response.message is not None else default_message
 
         json = None
         try:
             json = response.json()
         except Exception:
             pass
 
+        message = None
         if json:
             message = json.get('error') or json.get('Description')
         elif hasattr(response, 'text'):
             response_message = getattr(response, 'message', 'There was an unexpected error.')
             message = getattr(response, 'text', response_message)
-        else:
+        elif hasattr(response, 'message'):
             message = getattr(response, 'message')
 
         return message
 
     def __init__(self, response, message):
         """Base Exception class init."""
         # API error message
```

### Comparing `PyVimeo-1.1.0/setup.py` & `pyvimeo-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #! /usr/bin/env python
 # encoding: utf-8
 
 from setuptools import setup
 
 setup(name='PyVimeo',
-    version='1.1.0',
+    version='1.1.2',
     description='Simple interaction with the Vimeo API.',
     url='https://developer.vimeo.com/',
     author='Vimeo',
     author_email='support@vimeo.com',
     packages=['vimeo', 'vimeo/auth'],
     install_requires=['requests>=2.4.0', 'tuspy>=0.2.4'],
       python_requires='>=3.5',
```

