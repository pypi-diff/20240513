# Comparing `tmp/abstract_flask-0.0.0.8.tar.gz` & `tmp/abstract_flask-0.0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_flask-0.0.0.8.tar", last modified: Fri May 10 21:58:27 2024, max compression
+gzip compressed data, was "abstract_flask-0.0.0.9.tar", last modified: Mon May 13 08:02:20 2024, max compression
```

## Comparing `abstract_flask-0.0.0.8.tar` & `abstract_flask-0.0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-10 21:58:27.931733 abstract_flask-0.0.0.8/
--rw-r--r--   0 gamook    (1000) gamook    (1000)      572 2024-05-10 21:58:27.931733 abstract_flask-0.0.0.8/PKG-INFO
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       49 2024-04-08 17:04:50.000000 abstract_flask-0.0.0.8/README.md
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       38 2024-05-10 21:58:27.931733 abstract_flask-0.0.0.8/setup.cfg
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      952 2024-05-10 21:58:21.000000 abstract_flask-0.0.0.8/setup.py
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-10 21:58:27.931733 abstract_flask-0.0.0.8/src/
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-10 21:58:27.931733 abstract_flask-0.0.0.8/src/abstract_flask/
--rw-rw-r--   0 gamook    (1000) gamook    (1000)    12376 2024-05-10 21:56:12.000000 abstract_flask-0.0.0.8/src/abstract_flask/Abs_Manager.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)    13555 2024-05-10 21:56:00.000000 abstract_flask-0.0.0.8/src/abstract_flask/Abs_Manager_dynamic.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       56 2024-05-10 21:58:04.000000 abstract_flask-0.0.0.8/src/abstract_flask/__init__.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     9554 2024-05-10 21:45:03.000000 abstract_flask-0.0.0.8/src/abstract_flask/directories.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      522 2024-05-10 21:41:50.000000 abstract_flask-0.0.0.8/src/abstract_flask/fileManager.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      571 2024-05-10 01:11:01.000000 abstract_flask-0.0.0.8/src/abstract_flask/network_tools.py
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-10 21:58:27.931733 abstract_flask-0.0.0.8/src/abstract_flask.egg-info/
--rw-r--r--   0 gamook    (1000) gamook    (1000)      572 2024-05-10 21:58:27.000000 abstract_flask-0.0.0.8/src/abstract_flask.egg-info/PKG-INFO
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      438 2024-05-10 21:58:27.000000 abstract_flask-0.0.0.8/src/abstract_flask.egg-info/SOURCES.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)        1 2024-05-10 21:58:27.000000 abstract_flask-0.0.0.8/src/abstract_flask.egg-info/dependency_links.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       40 2024-05-10 21:58:27.000000 abstract_flask-0.0.0.8/src/abstract_flask.egg-info/requires.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       15 2024-05-10 21:58:27.000000 abstract_flask-0.0.0.8/src/abstract_flask.egg-info/top_level.txt
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-13 08:02:20.827408 abstract_flask-0.0.0.9/
+-rw-r--r--   0 gamook    (1000) gamook    (1000)      572 2024-05-13 08:02:20.827408 abstract_flask-0.0.0.9/PKG-INFO
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       49 2024-04-08 17:04:50.000000 abstract_flask-0.0.0.9/README.md
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       38 2024-05-13 08:02:20.827408 abstract_flask-0.0.0.9/setup.cfg
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      952 2024-05-13 08:02:11.000000 abstract_flask-0.0.0.9/setup.py
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-13 08:02:20.827408 abstract_flask-0.0.0.9/src/
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-13 08:02:20.827408 abstract_flask-0.0.0.9/src/abstract_flask/
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       56 2024-05-10 21:58:04.000000 abstract_flask-0.0.0.9/src/abstract_flask/__init__.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)    12376 2024-05-10 21:56:12.000000 abstract_flask-0.0.0.9/src/abstract_flask/abs_Manager.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)    13555 2024-05-10 21:56:00.000000 abstract_flask-0.0.0.9/src/abstract_flask/abs_Manager_dynamic.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     9554 2024-05-10 21:45:03.000000 abstract_flask-0.0.0.9/src/abstract_flask/directories.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      522 2024-05-10 21:41:50.000000 abstract_flask-0.0.0.9/src/abstract_flask/fileManager.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      571 2024-05-10 01:11:01.000000 abstract_flask-0.0.0.9/src/abstract_flask/network_tools.py
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-13 08:02:20.827408 abstract_flask-0.0.0.9/src/abstract_flask.egg-info/
+-rw-r--r--   0 gamook    (1000) gamook    (1000)      572 2024-05-13 08:02:20.000000 abstract_flask-0.0.0.9/src/abstract_flask.egg-info/PKG-INFO
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      438 2024-05-13 08:02:20.000000 abstract_flask-0.0.0.9/src/abstract_flask.egg-info/SOURCES.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)        1 2024-05-13 08:02:20.000000 abstract_flask-0.0.0.9/src/abstract_flask.egg-info/dependency_links.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       40 2024-05-13 08:02:20.000000 abstract_flask-0.0.0.9/src/abstract_flask.egg-info/requires.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       15 2024-05-13 08:02:20.000000 abstract_flask-0.0.0.9/src/abstract_flask.egg-info/top_level.txt
```

### Comparing `abstract_flask-0.0.0.8/PKG-INFO` & `abstract_flask-0.0.0.9/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract_flask
-Version: 0.0.0.8
+Version: 0.0.0.9
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `abstract_flask-0.0.0.8/setup.py` & `abstract_flask-0.0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name='abstract_flask',
-    version='0.0.0.8',
+    version='0.0.0.9',
     author='putkoff',
     author_email='partners@abstractendeavors.com',
     description="",
     long_description=long_description,
     long_description_content_type='text/markdown',
     classifiers=[
           'Development Status :: 3 - Alpha',
```

### Comparing `abstract_flask-0.0.0.8/src/abstract_flask/Abs_Manager.py` & `abstract_flask-0.0.0.9/src/abstract_flask/abs_Manager.py`

 * *Files identical despite different names*

### Comparing `abstract_flask-0.0.0.8/src/abstract_flask/Abs_Manager_dynamic.py` & `abstract_flask-0.0.0.9/src/abstract_flask/abs_Manager_dynamic.py`

 * *Files identical despite different names*

### Comparing `abstract_flask-0.0.0.8/src/abstract_flask/directories.py` & `abstract_flask-0.0.0.9/src/abstract_flask/directories.py`

 * *Files identical despite different names*

### Comparing `abstract_flask-0.0.0.8/src/abstract_flask/fileManager.py` & `abstract_flask-0.0.0.9/src/abstract_flask/fileManager.py`

 * *Files identical despite different names*

### Comparing `abstract_flask-0.0.0.8/src/abstract_flask/network_tools.py` & `abstract_flask-0.0.0.9/src/abstract_flask/network_tools.py`

 * *Files identical despite different names*

### Comparing `abstract_flask-0.0.0.8/src/abstract_flask.egg-info/PKG-INFO` & `abstract_flask-0.0.0.9/src/abstract_flask.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract_flask
-Version: 0.0.0.8
+Version: 0.0.0.9
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

