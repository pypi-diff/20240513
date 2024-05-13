# Comparing `tmp/wkutils-0.0.9.tar.gz` & `tmp/wkutils-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wkutils-0.0.9.tar", last modified: Sun May 12 09:32:56 2024, max compression
+gzip compressed data, was "wkutils-0.1.0.tar", last modified: Mon May 13 07:48:54 2024, max compression
```

## Comparing `wkutils-0.0.9.tar` & `wkutils-0.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 werner    (1000) werner    (1000)        0 2024-05-12 09:32:56.909546 wkutils-0.0.9/
--rw-rw-r--   0 werner    (1000) werner    (1000)      596 2024-05-12 09:32:56.909546 wkutils-0.0.9/PKG-INFO
--rw-rw-r--   0 werner    (1000) werner    (1000)       31 2024-05-10 18:43:09.000000 wkutils-0.0.9/README.md
--rw-rw-r--   0 werner    (1000) werner    (1000)       38 2024-05-12 09:32:56.909546 wkutils-0.0.9/setup.cfg
--rw-rw-r--   0 werner    (1000) werner    (1000)      922 2024-05-12 09:28:36.000000 wkutils-0.0.9/setup.py
-drwxrwxr-x   0 werner    (1000) werner    (1000)        0 2024-05-12 09:32:56.909546 wkutils-0.0.9/wkutils/
--rw-rw-r--   0 werner    (1000) werner    (1000)     1492 2024-05-12 09:30:57.000000 wkutils-0.0.9/wkutils/__init__.py
-drwxrwxr-x   0 werner    (1000) werner    (1000)        0 2024-05-12 09:32:56.909546 wkutils-0.0.9/wkutils.egg-info/
--rw-rw-r--   0 werner    (1000) werner    (1000)      596 2024-05-12 09:32:56.000000 wkutils-0.0.9/wkutils.egg-info/PKG-INFO
--rw-rw-r--   0 werner    (1000) werner    (1000)      192 2024-05-12 09:32:56.000000 wkutils-0.0.9/wkutils.egg-info/SOURCES.txt
--rw-rw-r--   0 werner    (1000) werner    (1000)        1 2024-05-12 09:32:56.000000 wkutils-0.0.9/wkutils.egg-info/dependency_links.txt
--rw-rw-r--   0 werner    (1000) werner    (1000)       16 2024-05-12 09:32:56.000000 wkutils-0.0.9/wkutils.egg-info/requires.txt
--rw-rw-r--   0 werner    (1000) werner    (1000)        8 2024-05-12 09:32:56.000000 wkutils-0.0.9/wkutils.egg-info/top_level.txt
+drwxrwxr-x   0 werner    (1000) werner    (1000)        0 2024-05-13 07:48:54.618105 wkutils-0.1.0/
+-rw-rw-r--   0 werner    (1000) werner    (1000)      596 2024-05-13 07:48:54.618105 wkutils-0.1.0/PKG-INFO
+-rw-rw-r--   0 werner    (1000) werner    (1000)       31 2024-05-10 18:43:09.000000 wkutils-0.1.0/README.md
+-rw-rw-r--   0 werner    (1000) werner    (1000)       38 2024-05-13 07:48:54.618105 wkutils-0.1.0/setup.cfg
+-rw-rw-r--   0 werner    (1000) werner    (1000)      922 2024-05-13 07:48:43.000000 wkutils-0.1.0/setup.py
+drwxrwxr-x   0 werner    (1000) werner    (1000)        0 2024-05-13 07:48:54.618105 wkutils-0.1.0/wkutils/
+-rw-rw-r--   0 werner    (1000) werner    (1000)     2391 2024-05-13 07:48:27.000000 wkutils-0.1.0/wkutils/__init__.py
+drwxrwxr-x   0 werner    (1000) werner    (1000)        0 2024-05-13 07:48:54.618105 wkutils-0.1.0/wkutils.egg-info/
+-rw-rw-r--   0 werner    (1000) werner    (1000)      596 2024-05-13 07:48:54.000000 wkutils-0.1.0/wkutils.egg-info/PKG-INFO
+-rw-rw-r--   0 werner    (1000) werner    (1000)      192 2024-05-13 07:48:54.000000 wkutils-0.1.0/wkutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 werner    (1000) werner    (1000)        1 2024-05-13 07:48:54.000000 wkutils-0.1.0/wkutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 werner    (1000) werner    (1000)       16 2024-05-13 07:48:54.000000 wkutils-0.1.0/wkutils.egg-info/requires.txt
+-rw-rw-r--   0 werner    (1000) werner    (1000)        8 2024-05-13 07:48:54.000000 wkutils-0.1.0/wkutils.egg-info/top_level.txt
```

### Comparing `wkutils-0.0.9/PKG-INFO` & `wkutils-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wkutils
-Version: 0.0.9
+Version: 0.1.0
 Summary: Useful utilities for python
 Author: Werner Kruger
 Author-email: <python@wkruger.com>
 Keywords: python,utilities,financial,calculator
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `wkutils-0.0.9/setup.py` & `wkutils-0.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.9'
+VERSION = '0.1.0'
 DESCRIPTION = 'Useful utilities for python'
 LONG_DESCRIPTION = 'A package that contains a bunch of useful utilities I have collected over the years'
 
 # Setting up
 setup(
     name="wkutils",
     version=VERSION,
```

### Comparing `wkutils-0.0.9/wkutils.egg-info/PKG-INFO` & `wkutils-0.1.0/wkutils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wkutils
-Version: 0.0.9
+Version: 0.1.0
 Summary: Useful utilities for python
 Author: Werner Kruger
 Author-email: <python@wkruger.com>
 Keywords: python,utilities,financial,calculator
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

