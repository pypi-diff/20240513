# Comparing `tmp/redistensor-0.0.3.tar.gz` & `tmp/redistensor-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redistensor-0.0.3.tar", last modified: Mon May 13 04:25:51 2024, max compression
+gzip compressed data, was "redistensor-0.0.4.tar", last modified: Mon May 13 04:28:41 2024, max compression
```

## Comparing `redistensor-0.0.3.tar` & `redistensor-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 hayang    (1000) hayang    (1000)        0 2024-05-13 04:25:51.947543 redistensor-0.0.3/
--rw-r--r--   0 hayang    (1000) hayang    (1000)      923 2024-05-13 04:25:51.947543 redistensor-0.0.3/PKG-INFO
--rw-rw-r--   0 hayang    (1000) hayang    (1000)      516 2024-05-10 09:14:45.000000 redistensor-0.0.3/README.md
-drwxrwxr-x   0 hayang    (1000) hayang    (1000)        0 2024-05-13 04:25:51.947543 redistensor-0.0.3/redistensor/
--rw-rw-r--   0 hayang    (1000) hayang    (1000)       73 2024-05-13 04:20:38.000000 redistensor-0.0.3/redistensor/__init__.py
--rw-rw-r--   0 hayang    (1000) hayang    (1000)     1933 2024-05-13 04:17:27.000000 redistensor-0.0.3/redistensor/filetensor.py
--rw-rw-r--   0 hayang    (1000) hayang    (1000)     2943 2024-05-13 04:16:54.000000 redistensor-0.0.3/redistensor/redistensor.py
-drwxrwxr-x   0 hayang    (1000) hayang    (1000)        0 2024-05-13 04:25:51.947543 redistensor-0.0.3/redistensor.egg-info/
--rw-r--r--   0 hayang    (1000) hayang    (1000)      923 2024-05-13 04:25:51.000000 redistensor-0.0.3/redistensor.egg-info/PKG-INFO
--rw-rw-r--   0 hayang    (1000) hayang    (1000)      269 2024-05-13 04:25:51.000000 redistensor-0.0.3/redistensor.egg-info/SOURCES.txt
--rw-rw-r--   0 hayang    (1000) hayang    (1000)        1 2024-05-13 04:25:51.000000 redistensor-0.0.3/redistensor.egg-info/dependency_links.txt
--rw-rw-r--   0 hayang    (1000) hayang    (1000)       12 2024-05-13 04:25:51.000000 redistensor-0.0.3/redistensor.egg-info/requires.txt
--rw-rw-r--   0 hayang    (1000) hayang    (1000)       12 2024-05-13 04:25:51.000000 redistensor-0.0.3/redistensor.egg-info/top_level.txt
--rw-rw-r--   0 hayang    (1000) hayang    (1000)       38 2024-05-13 04:25:51.947543 redistensor-0.0.3/setup.cfg
--rw-rw-r--   0 hayang    (1000) hayang    (1000)      665 2024-05-13 04:21:39.000000 redistensor-0.0.3/setup.py
+drwxrwxr-x   0 hayang    (1000) hayang    (1000)        0 2024-05-13 04:28:41.997512 redistensor-0.0.4/
+-rw-r--r--   0 hayang    (1000) hayang    (1000)      923 2024-05-13 04:28:41.997512 redistensor-0.0.4/PKG-INFO
+-rw-rw-r--   0 hayang    (1000) hayang    (1000)      516 2024-05-10 09:14:45.000000 redistensor-0.0.4/README.md
+drwxrwxr-x   0 hayang    (1000) hayang    (1000)        0 2024-05-13 04:28:41.997512 redistensor-0.0.4/redistensor/
+-rw-rw-r--   0 hayang    (1000) hayang    (1000)       72 2024-05-13 04:28:26.000000 redistensor-0.0.4/redistensor/__init__.py
+-rw-rw-r--   0 hayang    (1000) hayang    (1000)     1933 2024-05-13 04:17:27.000000 redistensor-0.0.4/redistensor/filetensor.py
+-rw-rw-r--   0 hayang    (1000) hayang    (1000)     2943 2024-05-13 04:16:54.000000 redistensor-0.0.4/redistensor/redistensor.py
+drwxrwxr-x   0 hayang    (1000) hayang    (1000)        0 2024-05-13 04:28:41.997512 redistensor-0.0.4/redistensor.egg-info/
+-rw-r--r--   0 hayang    (1000) hayang    (1000)      923 2024-05-13 04:28:41.000000 redistensor-0.0.4/redistensor.egg-info/PKG-INFO
+-rw-rw-r--   0 hayang    (1000) hayang    (1000)      269 2024-05-13 04:28:41.000000 redistensor-0.0.4/redistensor.egg-info/SOURCES.txt
+-rw-rw-r--   0 hayang    (1000) hayang    (1000)        1 2024-05-13 04:28:41.000000 redistensor-0.0.4/redistensor.egg-info/dependency_links.txt
+-rw-rw-r--   0 hayang    (1000) hayang    (1000)       12 2024-05-13 04:28:41.000000 redistensor-0.0.4/redistensor.egg-info/requires.txt
+-rw-rw-r--   0 hayang    (1000) hayang    (1000)       12 2024-05-13 04:28:41.000000 redistensor-0.0.4/redistensor.egg-info/top_level.txt
+-rw-rw-r--   0 hayang    (1000) hayang    (1000)       38 2024-05-13 04:28:41.997512 redistensor-0.0.4/setup.cfg
+-rw-rw-r--   0 hayang    (1000) hayang    (1000)      665 2024-05-13 04:28:37.000000 redistensor-0.0.4/setup.py
```

### Comparing `redistensor-0.0.3/PKG-INFO` & `redistensor-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redistensor
-Version: 0.0.3
+Version: 0.0.4
 Summary: using redis to store tensor data
 Home-page: 
 Author: hayang
 Author-email: 469358331@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `redistensor-0.0.3/README.md` & `redistensor-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `redistensor-0.0.3/redistensor/filetensor.py` & `redistensor-0.0.4/redistensor/filetensor.py`

 * *Files identical despite different names*

### Comparing `redistensor-0.0.3/redistensor/redistensor.py` & `redistensor-0.0.4/redistensor/redistensor.py`

 * *Files identical despite different names*

### Comparing `redistensor-0.0.3/redistensor.egg-info/PKG-INFO` & `redistensor-0.0.4/redistensor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redistensor
-Version: 0.0.3
+Version: 0.0.4
 Summary: using redis to store tensor data
 Home-page: 
 Author: hayang
 Author-email: 469358331@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `redistensor-0.0.3/setup.py` & `redistensor-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="redistensor",
-    version="0.0.3",
+    version="0.0.4",
     author="hayang",
     author_email="469358331@qq.com",
     description="using redis to store tensor data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

