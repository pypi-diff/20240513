# Comparing `tmp/lytix_py-1.3.0.tar.gz` & `tmp/lytix_py-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lytix_py-1.3.0.tar", last modified: Mon May 13 18:40:10 2024, max compression
+gzip compressed data, was "lytix_py-1.3.1.tar", last modified: Mon May 13 18:41:16 2024, max compression
```

## Comparing `lytix_py-1.3.0.tar` & `lytix_py-1.3.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-13 18:40:10.096819 lytix_py-1.3.0/
--rw-r--r--   0 sidpremkumar   (501) staff       (20)     1081 2024-05-05 21:16:18.000000 lytix_py-1.3.0/LICENSE.md
--rw-r--r--   0 sidpremkumar   (501) staff       (20)     1008 2024-05-13 18:40:10.096591 lytix_py-1.3.0/PKG-INFO
--rw-r--r--   0 sidpremkumar   (501) staff       (20)      450 2024-05-05 21:16:53.000000 lytix_py-1.3.0/README.md
--rw-r--r--   0 sidpremkumar   (501) staff       (20)      625 2024-05-13 18:39:59.000000 lytix_py-1.3.0/pyproject.toml
--rw-r--r--   0 sidpremkumar   (501) staff       (20)       38 2024-05-13 18:40:10.096861 lytix_py-1.3.0/setup.cfg
-drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-13 18:40:10.094345 lytix_py-1.3.0/src/
-drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-13 18:40:10.095116 lytix_py-1.3.0/src/lytix_py/
-drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-13 18:40:10.095993 lytix_py-1.3.0/src/lytix_py/LLLogger/
--rw-r--r--   0 sidpremkumar   (501) staff       (20)      886 2024-05-06 00:20:17.000000 lytix_py-1.3.0/src/lytix_py/LLLogger/LLLogger.py
-drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-13 18:40:10.096131 lytix_py-1.3.0/src/lytix_py/MetricCollector/
--rw-r--r--   0 sidpremkumar   (501) staff       (20)     2652 2024-05-13 18:39:50.000000 lytix_py-1.3.0/src/lytix_py/MetricCollector/MetricCollector.py
--rw-r--r--   0 sidpremkumar   (501) staff       (20)      133 2024-05-13 18:39:31.000000 lytix_py-1.3.0/src/lytix_py/__init__.py
--rw-r--r--   0 sidpremkumar   (501) staff       (20)      575 2024-05-13 18:39:42.000000 lytix_py-1.3.0/src/lytix_py/envVars.py
-drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-13 18:40:10.096323 lytix_py-1.3.0/src/lytix_py.egg-info/
--rw-r--r--   0 sidpremkumar   (501) staff       (20)     1008 2024-05-13 18:40:10.000000 lytix_py-1.3.0/src/lytix_py.egg-info/PKG-INFO
--rw-r--r--   0 sidpremkumar   (501) staff       (20)      345 2024-05-13 18:40:10.000000 lytix_py-1.3.0/src/lytix_py.egg-info/SOURCES.txt
--rw-r--r--   0 sidpremkumar   (501) staff       (20)        1 2024-05-13 18:40:10.000000 lytix_py-1.3.0/src/lytix_py.egg-info/dependency_links.txt
--rw-r--r--   0 sidpremkumar   (501) staff       (20)       32 2024-05-13 18:40:10.000000 lytix_py-1.3.0/src/lytix_py.egg-info/requires.txt
--rw-r--r--   0 sidpremkumar   (501) staff       (20)        9 2024-05-13 18:40:10.000000 lytix_py-1.3.0/src/lytix_py.egg-info/top_level.txt
+drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-13 18:41:16.505933 lytix_py-1.3.1/
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)     1081 2024-05-05 21:16:18.000000 lytix_py-1.3.1/LICENSE.md
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)     1008 2024-05-13 18:41:16.505732 lytix_py-1.3.1/PKG-INFO
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)      450 2024-05-05 21:16:53.000000 lytix_py-1.3.1/README.md
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)      625 2024-05-13 18:41:12.000000 lytix_py-1.3.1/pyproject.toml
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)       38 2024-05-13 18:41:16.505974 lytix_py-1.3.1/setup.cfg
+drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-13 18:41:16.502986 lytix_py-1.3.1/src/
+drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-13 18:41:16.503924 lytix_py-1.3.1/src/lytix_py/
+drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-13 18:41:16.505061 lytix_py-1.3.1/src/lytix_py/LLLogger/
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)      886 2024-05-06 00:20:17.000000 lytix_py-1.3.1/src/lytix_py/LLLogger/LLLogger.py
+drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-13 18:41:16.505188 lytix_py-1.3.1/src/lytix_py/MetricCollector/
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)     2652 2024-05-13 18:39:50.000000 lytix_py-1.3.1/src/lytix_py/MetricCollector/MetricCollector.py
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)      133 2024-05-13 18:41:07.000000 lytix_py-1.3.1/src/lytix_py/__init__.py
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)      575 2024-05-13 18:39:42.000000 lytix_py-1.3.1/src/lytix_py/envVars.py
+drwxr-xr-x   0 sidpremkumar   (501) staff       (20)        0 2024-05-13 18:41:16.505503 lytix_py-1.3.1/src/lytix_py.egg-info/
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)     1008 2024-05-13 18:41:16.000000 lytix_py-1.3.1/src/lytix_py.egg-info/PKG-INFO
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)      345 2024-05-13 18:41:16.000000 lytix_py-1.3.1/src/lytix_py.egg-info/SOURCES.txt
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)        1 2024-05-13 18:41:16.000000 lytix_py-1.3.1/src/lytix_py.egg-info/dependency_links.txt
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)       32 2024-05-13 18:41:16.000000 lytix_py-1.3.1/src/lytix_py.egg-info/requires.txt
+-rw-r--r--   0 sidpremkumar   (501) staff       (20)        9 2024-05-13 18:41:16.000000 lytix_py-1.3.1/src/lytix_py.egg-info/top_level.txt
```

### Comparing `lytix_py-1.3.0/LICENSE.md` & `lytix_py-1.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lytix_py-1.3.0/PKG-INFO` & `lytix_py-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lytix-py
-Version: 1.3.0
+Version: 1.3.1
 Summary: Official Lytix Client Packages
 Author-email: Lytix <support@lytix.com>
 Project-URL: Homepage, https://github.com/Lytix-Labs/lytix-py
 Project-URL: Issues, https://github.com/Lytix-Labs/lytix-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lytix_py-1.3.0/pyproject.toml` & `lytix_py-1.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lytix-py"
-version = "1.3.0"
+version = "1.3.1"
 authors = [
   { name="Lytix", email="support@lytix.com" },
 ]
 description = "Official Lytix Client Packages"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `lytix_py-1.3.0/src/lytix_py/LLLogger/LLLogger.py` & `lytix_py-1.3.1/src/lytix_py/LLLogger/LLLogger.py`

 * *Files identical despite different names*

### Comparing `lytix_py-1.3.0/src/lytix_py/MetricCollector/MetricCollector.py` & `lytix_py-1.3.1/src/lytix_py/MetricCollector/MetricCollector.py`

 * *Files identical despite different names*

### Comparing `lytix_py-1.3.0/src/lytix_py/envVars.py` & `lytix_py-1.3.1/src/lytix_py/envVars.py`

 * *Files identical despite different names*

### Comparing `lytix_py-1.3.0/src/lytix_py.egg-info/PKG-INFO` & `lytix_py-1.3.1/src/lytix_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lytix-py
-Version: 1.3.0
+Version: 1.3.1
 Summary: Official Lytix Client Packages
 Author-email: Lytix <support@lytix.com>
 Project-URL: Homepage, https://github.com/Lytix-Labs/lytix-py
 Project-URL: Issues, https://github.com/Lytix-Labs/lytix-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

