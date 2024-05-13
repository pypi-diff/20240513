# Comparing `tmp/redistensor-0.0.2.tar.gz` & `tmp/redistensor-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redistensor-0.0.2.tar", last modified: Fri May 10 09:30:08 2024, max compression
+gzip compressed data, was "redistensor-0.0.3.tar", last modified: Mon May 13 04:25:51 2024, max compression
```

## Comparing `redistensor-0.0.2.tar` & `redistensor-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxr-x   0 hayang    (1000) hayang    (1000)        0 2024-05-10 09:30:08.150327 redistensor-0.0.2/
--rw-rw-r--   0 hayang    (1000) hayang    (1000)      881 2024-05-10 09:30:08.150327 redistensor-0.0.2/PKG-INFO
--rw-rw-r--   0 hayang    (1000) hayang    (1000)      516 2024-05-10 09:14:45.000000 redistensor-0.0.2/README.md
-drwxrwxr-x   0 hayang    (1000) hayang    (1000)        0 2024-05-10 09:30:08.150327 redistensor-0.0.2/redistensor/
--rw-rw-r--   0 hayang    (1000) hayang    (1000)       37 2024-05-10 09:14:04.000000 redistensor-0.0.2/redistensor/__init__.py
--rw-rw-r--   0 hayang    (1000) hayang    (1000)     2936 2024-05-10 09:29:18.000000 redistensor-0.0.2/redistensor/redistensor.py
-drwxrwxr-x   0 hayang    (1000) hayang    (1000)        0 2024-05-10 09:30:08.150327 redistensor-0.0.2/redistensor.egg-info/
--rw-rw-r--   0 hayang    (1000) hayang    (1000)      881 2024-05-10 09:30:08.000000 redistensor-0.0.2/redistensor.egg-info/PKG-INFO
--rw-rw-r--   0 hayang    (1000) hayang    (1000)      243 2024-05-10 09:30:08.000000 redistensor-0.0.2/redistensor.egg-info/SOURCES.txt
--rw-rw-r--   0 hayang    (1000) hayang    (1000)        1 2024-05-10 09:30:08.000000 redistensor-0.0.2/redistensor.egg-info/dependency_links.txt
--rw-rw-r--   0 hayang    (1000) hayang    (1000)       12 2024-05-10 09:30:08.000000 redistensor-0.0.2/redistensor.egg-info/requires.txt
--rw-rw-r--   0 hayang    (1000) hayang    (1000)       12 2024-05-10 09:30:08.000000 redistensor-0.0.2/redistensor.egg-info/top_level.txt
--rw-rw-r--   0 hayang    (1000) hayang    (1000)       38 2024-05-10 09:30:08.150327 redistensor-0.0.2/setup.cfg
--rw-rw-r--   0 hayang    (1000) hayang    (1000)      665 2024-05-10 09:30:01.000000 redistensor-0.0.2/setup.py
+drwxrwxr-x   0 hayang    (1000) hayang    (1000)        0 2024-05-13 04:25:51.947543 redistensor-0.0.3/
+-rw-r--r--   0 hayang    (1000) hayang    (1000)      923 2024-05-13 04:25:51.947543 redistensor-0.0.3/PKG-INFO
+-rw-rw-r--   0 hayang    (1000) hayang    (1000)      516 2024-05-10 09:14:45.000000 redistensor-0.0.3/README.md
+drwxrwxr-x   0 hayang    (1000) hayang    (1000)        0 2024-05-13 04:25:51.947543 redistensor-0.0.3/redistensor/
+-rw-rw-r--   0 hayang    (1000) hayang    (1000)       73 2024-05-13 04:20:38.000000 redistensor-0.0.3/redistensor/__init__.py
+-rw-rw-r--   0 hayang    (1000) hayang    (1000)     1933 2024-05-13 04:17:27.000000 redistensor-0.0.3/redistensor/filetensor.py
+-rw-rw-r--   0 hayang    (1000) hayang    (1000)     2943 2024-05-13 04:16:54.000000 redistensor-0.0.3/redistensor/redistensor.py
+drwxrwxr-x   0 hayang    (1000) hayang    (1000)        0 2024-05-13 04:25:51.947543 redistensor-0.0.3/redistensor.egg-info/
+-rw-r--r--   0 hayang    (1000) hayang    (1000)      923 2024-05-13 04:25:51.000000 redistensor-0.0.3/redistensor.egg-info/PKG-INFO
+-rw-rw-r--   0 hayang    (1000) hayang    (1000)      269 2024-05-13 04:25:51.000000 redistensor-0.0.3/redistensor.egg-info/SOURCES.txt
+-rw-rw-r--   0 hayang    (1000) hayang    (1000)        1 2024-05-13 04:25:51.000000 redistensor-0.0.3/redistensor.egg-info/dependency_links.txt
+-rw-rw-r--   0 hayang    (1000) hayang    (1000)       12 2024-05-13 04:25:51.000000 redistensor-0.0.3/redistensor.egg-info/requires.txt
+-rw-rw-r--   0 hayang    (1000) hayang    (1000)       12 2024-05-13 04:25:51.000000 redistensor-0.0.3/redistensor.egg-info/top_level.txt
+-rw-rw-r--   0 hayang    (1000) hayang    (1000)       38 2024-05-13 04:25:51.947543 redistensor-0.0.3/setup.cfg
+-rw-rw-r--   0 hayang    (1000) hayang    (1000)      665 2024-05-13 04:21:39.000000 redistensor-0.0.3/setup.py
```

### Comparing `redistensor-0.0.2/PKG-INFO` & `redistensor-0.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: redistensor
-Version: 0.0.2
+Version: 0.0.3
 Summary: using redis to store tensor data
 Home-page: 
 Author: hayang
 Author-email: 469358331@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Requires-Dist: numpy
+Requires-Dist: redis
 
 # save numpy tensor using redis
 
 ## prepare
 install redis-server
 
 ## using
```

### Comparing `redistensor-0.0.2/README.md` & `redistensor-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `redistensor-0.0.2/redistensor/redistensor.py` & `redistensor-0.0.3/redistensor/redistensor.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
             print(e)
             raise Exception("Failed to connect to Redis")
 
     def shape_to_str(self, shape:tuple):
         return str(shape).replace(' ', '')
     
     def str_to_shape(self, shape:str):
-        return tuple(map(int, shape[1:-1].split(',')))
+        tuple(map(int, filter(None, shape[1:-1].split(','))))
     
     def set(self, key:str, tensor:np.ndarray):
         key_shape = key + "_shape"
         key_dtype = key + "_dtype"
         key_tensor = key + "_tensor"
 
         try:
```

### Comparing `redistensor-0.0.2/redistensor.egg-info/PKG-INFO` & `redistensor-0.0.3/redistensor.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: redistensor
-Version: 0.0.2
+Version: 0.0.3
 Summary: using redis to store tensor data
 Home-page: 
 Author: hayang
 Author-email: 469358331@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Requires-Dist: numpy
+Requires-Dist: redis
 
 # save numpy tensor using redis
 
 ## prepare
 install redis-server
 
 ## using
```

### Comparing `redistensor-0.0.2/setup.py` & `redistensor-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="redistensor",
-    version="0.0.2",
+    version="0.0.3",
     author="hayang",
     author_email="469358331@qq.com",
     description="using redis to store tensor data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

