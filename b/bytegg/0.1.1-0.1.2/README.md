# Comparing `tmp/bytegg-0.1.1.tar.gz` & `tmp/bytegg-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bytegg-0.1.1.tar", last modified: Mon May 13 02:36:22 2024, max compression
+gzip compressed data, was "bytegg-0.1.2.tar", last modified: Mon May 13 02:38:08 2024, max compression
```

## Comparing `bytegg-0.1.1.tar` & `bytegg-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 lulu      (1000) lulu      (1000)        0 2024-05-13 02:36:22.639034 bytegg-0.1.1/
--rw-r--r--   0 lulu      (1000) lulu      (1000)     1064 2024-05-13 02:01:16.000000 bytegg-0.1.1/LICENSE
--rw-r--r--   0 lulu      (1000) lulu      (1000)      626 2024-05-13 02:36:22.635034 bytegg-0.1.1/PKG-INFO
--rw-r--r--   0 lulu      (1000) lulu      (1000)     1264 2024-05-13 02:31:44.000000 bytegg-0.1.1/README.md
-drwxr-xr-x   0 lulu      (1000) lulu      (1000)        0 2024-05-13 02:36:22.619034 bytegg-0.1.1/bytegg/
--rw-r--r--   0 lulu      (1000) lulu      (1000)      304 2024-05-13 02:35:33.000000 bytegg-0.1.1/bytegg/__init__.py
--rw-r--r--   0 lulu      (1000) lulu      (1000)      463 2024-05-13 02:35:38.000000 bytegg-0.1.1/bytegg/core.py
-drwxr-xr-x   0 lulu      (1000) lulu      (1000)        0 2024-05-13 02:36:22.631034 bytegg-0.1.1/bytegg.egg-info/
--rw-r--r--   0 lulu      (1000) lulu      (1000)      626 2024-05-13 02:36:22.000000 bytegg-0.1.1/bytegg.egg-info/PKG-INFO
--rw-r--r--   0 lulu      (1000) lulu      (1000)      209 2024-05-13 02:36:22.000000 bytegg-0.1.1/bytegg.egg-info/SOURCES.txt
--rw-r--r--   0 lulu      (1000) lulu      (1000)        1 2024-05-13 02:36:22.000000 bytegg-0.1.1/bytegg.egg-info/dependency_links.txt
--rw-r--r--   0 lulu      (1000) lulu      (1000)       16 2024-05-13 02:36:22.000000 bytegg-0.1.1/bytegg.egg-info/requires.txt
--rw-r--r--   0 lulu      (1000) lulu      (1000)        7 2024-05-13 02:36:22.000000 bytegg-0.1.1/bytegg.egg-info/top_level.txt
--rw-r--r--   0 lulu      (1000) lulu      (1000)       38 2024-05-13 02:36:22.639034 bytegg-0.1.1/setup.cfg
--rw-r--r--   0 lulu      (1000) lulu      (1000)      822 2024-05-13 02:35:47.000000 bytegg-0.1.1/setup.py
+drwxr-xr-x   0 lulu      (1000) lulu      (1000)        0 2024-05-13 02:38:08.525773 bytegg-0.1.2/
+-rw-r--r--   0 lulu      (1000) lulu      (1000)     1064 2024-05-13 02:01:16.000000 bytegg-0.1.2/LICENSE
+-rw-r--r--   0 lulu      (1000) lulu      (1000)      626 2024-05-13 02:38:08.525773 bytegg-0.1.2/PKG-INFO
+-rw-r--r--   0 lulu      (1000) lulu      (1000)     1264 2024-05-13 02:31:44.000000 bytegg-0.1.2/README.md
+drwxr-xr-x   0 lulu      (1000) lulu      (1000)        0 2024-05-13 02:38:08.517773 bytegg-0.1.2/bytegg/
+-rw-r--r--   0 lulu      (1000) lulu      (1000)      304 2024-05-13 02:37:59.000000 bytegg-0.1.2/bytegg/__init__.py
+-rw-r--r--   0 lulu      (1000) lulu      (1000)      481 2024-05-13 02:37:47.000000 bytegg-0.1.2/bytegg/core.py
+drwxr-xr-x   0 lulu      (1000) lulu      (1000)        0 2024-05-13 02:38:08.521773 bytegg-0.1.2/bytegg.egg-info/
+-rw-r--r--   0 lulu      (1000) lulu      (1000)      626 2024-05-13 02:38:08.000000 bytegg-0.1.2/bytegg.egg-info/PKG-INFO
+-rw-r--r--   0 lulu      (1000) lulu      (1000)      209 2024-05-13 02:38:08.000000 bytegg-0.1.2/bytegg.egg-info/SOURCES.txt
+-rw-r--r--   0 lulu      (1000) lulu      (1000)        1 2024-05-13 02:38:08.000000 bytegg-0.1.2/bytegg.egg-info/dependency_links.txt
+-rw-r--r--   0 lulu      (1000) lulu      (1000)       16 2024-05-13 02:38:08.000000 bytegg-0.1.2/bytegg.egg-info/requires.txt
+-rw-r--r--   0 lulu      (1000) lulu      (1000)        7 2024-05-13 02:38:08.000000 bytegg-0.1.2/bytegg.egg-info/top_level.txt
+-rw-r--r--   0 lulu      (1000) lulu      (1000)       38 2024-05-13 02:38:08.525773 bytegg-0.1.2/setup.cfg
+-rw-r--r--   0 lulu      (1000) lulu      (1000)      822 2024-05-13 02:37:55.000000 bytegg-0.1.2/setup.py
```

### Comparing `bytegg-0.1.1/LICENSE` & `bytegg-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bytegg-0.1.1/PKG-INFO` & `bytegg-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bytegg
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python package that bypasses advertisements to streamline user experiences with content.
 Home-page: https://github.com/KirbyHacks/ByteGG
 Author: ! rL⌀w
 Author-email: bytebvrd@gmail.com
 License: MIT
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
```

### Comparing `bytegg-0.1.1/README.md` & `bytegg-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `bytegg-0.1.1/bytegg.egg-info/PKG-INFO` & `bytegg-0.1.2/bytegg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bytegg
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python package that bypasses advertisements to streamline user experiences with content.
 Home-page: https://github.com/KirbyHacks/ByteGG
 Author: ! rL⌀w
 Author-email: bytebvrd@gmail.com
 License: MIT
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
```

### Comparing `bytegg-0.1.1/setup.py` & `bytegg-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='bytegg',
-    version='0.1.1',    
+    version='0.1.2',    
     description='A Python package that bypasses advertisements to streamline user experiences with content.',
     url='https://github.com/KirbyHacks/ByteGG',
     author='! rL⌀w',
     author_email='bytebvrd@gmail.com',
     license='MIT',
     packages=['bytegg'],
     install_requires=['urllib3',
```

