# Comparing `tmp/vipas-0.0.7.tar.gz` & `tmp/vipas-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vipas-0.0.7.tar", last modified: Mon May 13 12:04:34 2024, max compression
+gzip compressed data, was "vipas-0.0.8.tar", last modified: Mon May 13 13:48:50 2024, max compression
```

## Comparing `vipas-0.0.7.tar` & `vipas-0.0.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2024-05-13 12:04:34.135311 vipas-0.0.7/
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     2487 2024-04-30 05:46:43.000000 vipas-0.0.7/LICENSE.md
--rw-r--r--   0 aditya    (1001) aditya    (1001)      360 2024-05-13 12:04:34.135311 vipas-0.0.7/PKG-INFO
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     1598 2024-05-01 12:56:58.000000 vipas-0.0.7/README.md
--rw-rw-r--   0 aditya    (1001) aditya    (1001)       91 2024-05-11 09:29:37.000000 vipas-0.0.7/pyproject.toml
--rw-rw-r--   0 aditya    (1001) aditya    (1001)      443 2024-05-13 12:04:34.135311 vipas-0.0.7/setup.cfg
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     1273 2024-05-13 12:04:13.000000 vipas-0.0.7/setup.py
-drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2024-05-13 12:04:34.135311 vipas-0.0.7/test/
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     2818 2024-05-12 09:48:23.000000 vipas-0.0.7/test/test_model_client.py
-drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2024-05-13 12:04:34.135311 vipas-0.0.7/vipas/
--rw-rw-r--   0 aditya    (1001) aditya    (1001)      725 2024-04-30 15:42:34.000000 vipas-0.0.7/vipas/__init__.py
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     2084 2024-05-02 09:27:49.000000 vipas-0.0.7/vipas/_rest.py
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     4120 2024-05-13 12:04:00.000000 vipas-0.0.7/vipas/config.py
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     3555 2024-05-01 08:36:27.000000 vipas-0.0.7/vipas/exceptions.py
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     6279 2024-05-12 09:47:51.000000 vipas-0.0.7/vipas/model.py
-drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2024-05-13 12:04:34.135311 vipas-0.0.7/vipas.egg-info/
--rw-r--r--   0 aditya    (1001) aditya    (1001)      360 2024-05-13 12:04:34.000000 vipas-0.0.7/vipas.egg-info/PKG-INFO
--rw-rw-r--   0 aditya    (1001) aditya    (1001)      308 2024-05-13 12:04:34.000000 vipas-0.0.7/vipas.egg-info/SOURCES.txt
--rw-rw-r--   0 aditya    (1001) aditya    (1001)        1 2024-05-13 12:04:34.000000 vipas-0.0.7/vipas.egg-info/dependency_links.txt
--rw-rw-r--   0 aditya    (1001) aditya    (1001)       65 2024-05-13 12:04:34.000000 vipas-0.0.7/vipas.egg-info/requires.txt
--rw-rw-r--   0 aditya    (1001) aditya    (1001)        6 2024-05-13 12:04:34.000000 vipas-0.0.7/vipas.egg-info/top_level.txt
+drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2024-05-13 13:48:50.738830 vipas-0.0.8/
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     2487 2024-04-30 05:46:43.000000 vipas-0.0.8/LICENSE.md
+-rw-r--r--   0 aditya    (1001) aditya    (1001)      360 2024-05-13 13:48:50.738830 vipas-0.0.8/PKG-INFO
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     1598 2024-05-01 12:56:58.000000 vipas-0.0.8/README.md
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)       91 2024-05-11 09:29:37.000000 vipas-0.0.8/pyproject.toml
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)      443 2024-05-13 13:48:50.738830 vipas-0.0.8/setup.cfg
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     1273 2024-05-13 13:48:13.000000 vipas-0.0.8/setup.py
+drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2024-05-13 13:48:50.734831 vipas-0.0.8/test/
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     2818 2024-05-12 09:48:23.000000 vipas-0.0.8/test/test_model_client.py
+drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2024-05-13 13:48:50.738830 vipas-0.0.8/vipas/
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)      725 2024-04-30 15:42:34.000000 vipas-0.0.8/vipas/__init__.py
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     2084 2024-05-02 09:27:49.000000 vipas-0.0.8/vipas/_rest.py
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     4121 2024-05-13 13:47:59.000000 vipas-0.0.8/vipas/config.py
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     3555 2024-05-01 08:36:27.000000 vipas-0.0.8/vipas/exceptions.py
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     6279 2024-05-12 09:47:51.000000 vipas-0.0.8/vipas/model.py
+drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2024-05-13 13:48:50.738830 vipas-0.0.8/vipas.egg-info/
+-rw-r--r--   0 aditya    (1001) aditya    (1001)      360 2024-05-13 13:48:50.000000 vipas-0.0.8/vipas.egg-info/PKG-INFO
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)      308 2024-05-13 13:48:50.000000 vipas-0.0.8/vipas.egg-info/SOURCES.txt
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)        1 2024-05-13 13:48:50.000000 vipas-0.0.8/vipas.egg-info/dependency_links.txt
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)       65 2024-05-13 13:48:50.000000 vipas-0.0.8/vipas.egg-info/requires.txt
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)        6 2024-05-13 13:48:50.000000 vipas-0.0.8/vipas.egg-info/top_level.txt
```

### Comparing `vipas-0.0.7/LICENSE.md` & `vipas-0.0.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `vipas-0.0.7/README.md` & `vipas-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `vipas-0.0.7/setup.py` & `vipas-0.0.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 NAME = "vipas"
-VERSION = "0.0.7"
+VERSION = "0.0.8"
 PYTHON_REQUIRES = ">=3.7"
 REQUIRES = [
     "urllib3",
     "pydantic",
     "typing-extensions",
     "ratelimit",
     "pybreaker",
```

### Comparing `vipas-0.0.7/test/test_model_client.py` & `vipas-0.0.8/test/test_model_client.py`

 * *Files identical despite different names*

### Comparing `vipas-0.0.7/vipas/__init__.py` & `vipas-0.0.8/vipas/__init__.py`

 * *Files identical despite different names*

### Comparing `vipas-0.0.7/vipas/_rest.py` & `vipas-0.0.8/vipas/_rest.py`

 * *Files identical despite different names*

### Comparing `vipas-0.0.7/vipas/config.py` & `vipas-0.0.8/vipas/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
     _default = None
 
     def __init__(self, vps_auth_token=None) -> None:
         """
             Constructor for the configuration class
         """
-        self.host = "http://proxy.vipas.dev" 
+        self.host = "https://proxy.vipas.dev" 
         """
             Default Host for the proxy service.
         """
 
         # Authentication Settings
         self.vps_auth_token = None
         if vps_auth_token:
```

### Comparing `vipas-0.0.7/vipas/exceptions.py` & `vipas-0.0.8/vipas/exceptions.py`

 * *Files identical despite different names*

### Comparing `vipas-0.0.7/vipas/model.py` & `vipas-0.0.8/vipas/model.py`

 * *Files identical despite different names*

