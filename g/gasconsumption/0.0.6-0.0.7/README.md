# Comparing `tmp/gasconsumption-0.0.6.tar.gz` & `tmp/gasconsumption-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gasconsumption-0.0.6.tar", last modified: Thu Apr 25 12:14:12 2024, max compression
+gzip compressed data, was "gasconsumption-0.0.7.tar", last modified: Mon May 13 09:42:18 2024, max compression
```

## Comparing `gasconsumption-0.0.6.tar` & `gasconsumption-0.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 12:14:12.324068 gasconsumption-0.0.6/
--rw-rw-rw-   0        0        0      611 2024-04-25 12:14:12.323068 gasconsumption-0.0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-25 12:14:12.322068 gasconsumption-0.0.6/gasconsumption.egg-info/
--rw-rw-rw-   0        0        0      611 2024-04-25 12:14:12.000000 gasconsumption-0.0.6/gasconsumption.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2024-04-25 12:14:12.000000 gasconsumption-0.0.6/gasconsumption.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 12:14:12.000000 gasconsumption-0.0.6/gasconsumption.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-25 12:14:12.000000 gasconsumption-0.0.6/gasconsumption.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-25 12:14:12.000000 gasconsumption-0.0.6/gasconsumption.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-25 12:14:12.323068 gasconsumption-0.0.6/libname/
--rw-rw-rw-   0        0        0       37 2024-04-24 18:49:33.000000 gasconsumption-0.0.6/libname/__init__.py
--rw-rw-rw-   0        0        0     8217 2024-04-25 12:05:44.000000 gasconsumption-0.0.6/libname/fastapiwrapper.py
--rw-rw-rw-   0        0        0       42 2024-04-25 12:14:12.324068 gasconsumption-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      937 2024-04-25 12:11:59.000000 gasconsumption-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 09:42:18.742280 gasconsumption-0.0.7/
+-rw-rw-rw-   0        0        0      611 2024-05-13 09:42:18.741268 gasconsumption-0.0.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-13 09:42:18.739231 gasconsumption-0.0.7/gasconsumption.egg-info/
+-rw-rw-rw-   0        0        0      611 2024-05-13 09:42:18.000000 gasconsumption-0.0.7/gasconsumption.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2024-05-13 09:42:18.000000 gasconsumption-0.0.7/gasconsumption.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 09:42:18.000000 gasconsumption-0.0.7/gasconsumption.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-13 09:42:18.000000 gasconsumption-0.0.7/gasconsumption.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-13 09:42:18.000000 gasconsumption-0.0.7/gasconsumption.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-13 09:42:18.740235 gasconsumption-0.0.7/libname/
+-rw-rw-rw-   0        0        0       37 2024-04-24 18:49:33.000000 gasconsumption-0.0.7/libname/__init__.py
+-rw-rw-rw-   0        0        0     8217 2024-04-25 12:25:14.000000 gasconsumption-0.0.7/libname/fastapiwrapper.py
+-rw-rw-rw-   0        0        0       42 2024-05-13 09:42:18.742280 gasconsumption-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      937 2024-05-13 09:38:21.000000 gasconsumption-0.0.7/setup.py
```

### Comparing `gasconsumption-0.0.6/PKG-INFO` & `gasconsumption-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gasconsumption
-Version: 0.0.6
+Version: 0.0.7
 Summary: fitching Deftable and timeseries table
 Author: Ahmad Riad
 Author-email: meuralengine@outlook.com
 Keywords: python,Deftable,timeseries table
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `gasconsumption-0.0.6/gasconsumption.egg-info/PKG-INFO` & `gasconsumption-0.0.7/gasconsumption.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gasconsumption
-Version: 0.0.6
+Version: 0.0.7
 Summary: fitching Deftable and timeseries table
 Author: Ahmad Riad
 Author-email: meuralengine@outlook.com
 Keywords: python,Deftable,timeseries table
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `gasconsumption-0.0.6/libname/fastapiwrapper.py` & `gasconsumption-0.0.7/libname/fastapiwrapper.py`

 * *Files identical despite different names*

### Comparing `gasconsumption-0.0.6/setup.py` & `gasconsumption-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.6'
+VERSION = '0.0.7'
 DESCRIPTION = 'fitching Deftable and timeseries table'
 LONG_DESCRIPTION = 'contain an api wrapper that helps to fetch gas cconsumption data.'
 
 # Setting up
 setup(
     name="gasconsumption",
     version=VERSION,
```

