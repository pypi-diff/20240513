# Comparing `tmp/redistensor-0.0.4.tar.gz` & `tmp/redistensor-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redistensor-0.0.4.tar", last modified: Mon May 13 04:28:41 2024, max compression
+gzip compressed data, was "redistensor-0.0.5.tar", last modified: Mon May 13 05:43:55 2024, max compression
```

## Comparing `redistensor-0.0.4.tar` & `redistensor-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 hayang    (1000) hayang    (1000)        0 2024-05-13 04:28:41.997512 redistensor-0.0.4/
--rw-r--r--   0 hayang    (1000) hayang    (1000)      923 2024-05-13 04:28:41.997512 redistensor-0.0.4/PKG-INFO
--rw-rw-r--   0 hayang    (1000) hayang    (1000)      516 2024-05-10 09:14:45.000000 redistensor-0.0.4/README.md
-drwxrwxr-x   0 hayang    (1000) hayang    (1000)        0 2024-05-13 04:28:41.997512 redistensor-0.0.4/redistensor/
--rw-rw-r--   0 hayang    (1000) hayang    (1000)       72 2024-05-13 04:28:26.000000 redistensor-0.0.4/redistensor/__init__.py
--rw-rw-r--   0 hayang    (1000) hayang    (1000)     1933 2024-05-13 04:17:27.000000 redistensor-0.0.4/redistensor/filetensor.py
--rw-rw-r--   0 hayang    (1000) hayang    (1000)     2943 2024-05-13 04:16:54.000000 redistensor-0.0.4/redistensor/redistensor.py
-drwxrwxr-x   0 hayang    (1000) hayang    (1000)        0 2024-05-13 04:28:41.997512 redistensor-0.0.4/redistensor.egg-info/
--rw-r--r--   0 hayang    (1000) hayang    (1000)      923 2024-05-13 04:28:41.000000 redistensor-0.0.4/redistensor.egg-info/PKG-INFO
--rw-rw-r--   0 hayang    (1000) hayang    (1000)      269 2024-05-13 04:28:41.000000 redistensor-0.0.4/redistensor.egg-info/SOURCES.txt
--rw-rw-r--   0 hayang    (1000) hayang    (1000)        1 2024-05-13 04:28:41.000000 redistensor-0.0.4/redistensor.egg-info/dependency_links.txt
--rw-rw-r--   0 hayang    (1000) hayang    (1000)       12 2024-05-13 04:28:41.000000 redistensor-0.0.4/redistensor.egg-info/requires.txt
--rw-rw-r--   0 hayang    (1000) hayang    (1000)       12 2024-05-13 04:28:41.000000 redistensor-0.0.4/redistensor.egg-info/top_level.txt
--rw-rw-r--   0 hayang    (1000) hayang    (1000)       38 2024-05-13 04:28:41.997512 redistensor-0.0.4/setup.cfg
--rw-rw-r--   0 hayang    (1000) hayang    (1000)      665 2024-05-13 04:28:37.000000 redistensor-0.0.4/setup.py
+drwxrwxr-x   0 hayang    (1000) hayang    (1000)        0 2024-05-13 05:43:55.473379 redistensor-0.0.5/
+-rw-rw-r--   0 hayang    (1000) hayang    (1000)      881 2024-05-13 05:43:55.473379 redistensor-0.0.5/PKG-INFO
+-rw-rw-r--   0 hayang    (1000) hayang    (1000)      516 2024-05-10 09:14:45.000000 redistensor-0.0.5/README.md
+drwxrwxr-x   0 hayang    (1000) hayang    (1000)        0 2024-05-13 05:43:55.473379 redistensor-0.0.5/redistensor/
+-rw-rw-r--   0 hayang    (1000) hayang    (1000)       72 2024-05-13 04:28:26.000000 redistensor-0.0.5/redistensor/__init__.py
+-rw-rw-r--   0 hayang    (1000) hayang    (1000)     1940 2024-05-13 05:43:03.000000 redistensor-0.0.5/redistensor/filetensor.py
+-rw-rw-r--   0 hayang    (1000) hayang    (1000)     2943 2024-05-13 04:16:54.000000 redistensor-0.0.5/redistensor/redistensor.py
+drwxrwxr-x   0 hayang    (1000) hayang    (1000)        0 2024-05-13 05:43:55.473379 redistensor-0.0.5/redistensor.egg-info/
+-rw-rw-r--   0 hayang    (1000) hayang    (1000)      881 2024-05-13 05:43:55.000000 redistensor-0.0.5/redistensor.egg-info/PKG-INFO
+-rw-rw-r--   0 hayang    (1000) hayang    (1000)      269 2024-05-13 05:43:55.000000 redistensor-0.0.5/redistensor.egg-info/SOURCES.txt
+-rw-rw-r--   0 hayang    (1000) hayang    (1000)        1 2024-05-13 05:43:55.000000 redistensor-0.0.5/redistensor.egg-info/dependency_links.txt
+-rw-rw-r--   0 hayang    (1000) hayang    (1000)       12 2024-05-13 05:43:55.000000 redistensor-0.0.5/redistensor.egg-info/requires.txt
+-rw-rw-r--   0 hayang    (1000) hayang    (1000)       12 2024-05-13 05:43:55.000000 redistensor-0.0.5/redistensor.egg-info/top_level.txt
+-rw-rw-r--   0 hayang    (1000) hayang    (1000)       38 2024-05-13 05:43:55.473379 redistensor-0.0.5/setup.cfg
+-rw-rw-r--   0 hayang    (1000) hayang    (1000)      665 2024-05-13 05:43:52.000000 redistensor-0.0.5/setup.py
```

### Comparing `redistensor-0.0.4/PKG-INFO` & `redistensor-0.0.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: redistensor
-Version: 0.0.4
+Version: 0.0.5
 Summary: using redis to store tensor data
 Home-page: 
 Author: hayang
 Author-email: 469358331@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Requires-Dist: numpy
-Requires-Dist: redis
 
 # save numpy tensor using redis
 
 ## prepare
 install redis-server
 
 ## using
```

### Comparing `redistensor-0.0.4/README.md` & `redistensor-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `redistensor-0.0.4/redistensor/filetensor.py` & `redistensor-0.0.5/redistensor/filetensor.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         else:
             self.path = path + '/'
 
     def shape_to_str(self, shape:tuple):
         return str(shape).replace(' ', '')
     
     def str_to_shape(self, shape:str):
-        tuple(map(int, filter(None, shape[1:-1].split(','))))
+        return tuple(map(int, filter(None, shape[1:-1].split(','))))
 
     def set(self, key:str, tensor:np.ndarray):
         key_shape = key + "_shape"
         key_dtype = key + "_dtype"
         key_tensor = key + "_tensor"
 
         try:
```

### Comparing `redistensor-0.0.4/redistensor/redistensor.py` & `redistensor-0.0.5/redistensor/redistensor.py`

 * *Files identical despite different names*

### Comparing `redistensor-0.0.4/redistensor.egg-info/PKG-INFO` & `redistensor-0.0.5/redistensor.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: redistensor
-Version: 0.0.4
+Version: 0.0.5
 Summary: using redis to store tensor data
 Home-page: 
 Author: hayang
 Author-email: 469358331@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Requires-Dist: numpy
-Requires-Dist: redis
 
 # save numpy tensor using redis
 
 ## prepare
 install redis-server
 
 ## using
```

### Comparing `redistensor-0.0.4/setup.py` & `redistensor-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="redistensor",
-    version="0.0.4",
+    version="0.0.5",
     author="hayang",
     author_email="469358331@qq.com",
     description="using redis to store tensor data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

