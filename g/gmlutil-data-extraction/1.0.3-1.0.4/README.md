# Comparing `tmp/gmlutil-data-extraction-1.0.3.tar.gz` & `tmp/gmlutil-data-extraction-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmlutil-data-extraction-1.0.3.tar", last modified: Tue Feb 27 03:29:02 2024, max compression
+gzip compressed data, was "gmlutil-data-extraction-1.0.4.tar", last modified: Mon May 13 20:59:23 2024, max compression
```

## Comparing `gmlutil-data-extraction-1.0.3.tar` & `gmlutil-data-extraction-1.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 Phillip.Kim@ejgallo.com   (502) staff       (20)        0 2024-02-27 03:29:02.075289 gmlutil-data-extraction-1.0.3/
--rw-r--r--   0 Phillip.Kim@ejgallo.com   (502) staff       (20)      767 2024-02-27 03:29:02.075185 gmlutil-data-extraction-1.0.3/PKG-INFO
--rw-r--r--   0 Phillip.Kim@ejgallo.com   (502) staff       (20)     6303 2024-02-22 22:08:31.000000 gmlutil-data-extraction-1.0.3/README.md
-drwxr-xr-x   0 Phillip.Kim@ejgallo.com   (502) staff       (20)        0 2024-02-27 03:29:02.074182 gmlutil-data-extraction-1.0.3/gmlutil_data_extraction/
--rw-r--r--   0 Phillip.Kim@ejgallo.com   (502) staff       (20)      162 2024-02-13 01:11:59.000000 gmlutil-data-extraction-1.0.3/gmlutil_data_extraction/config.py
--rw-r--r--   0 Phillip.Kim@ejgallo.com   (502) staff       (20)    10357 2024-02-27 01:48:07.000000 gmlutil-data-extraction-1.0.3/gmlutil_data_extraction/data_extraction.py
-drwxr-xr-x   0 Phillip.Kim@ejgallo.com   (502) staff       (20)        0 2024-02-27 03:29:02.074996 gmlutil-data-extraction-1.0.3/gmlutil_data_extraction.egg-info/
--rw-r--r--   0 Phillip.Kim@ejgallo.com   (502) staff       (20)      767 2024-02-27 03:29:02.000000 gmlutil-data-extraction-1.0.3/gmlutil_data_extraction.egg-info/PKG-INFO
--rw-r--r--   0 Phillip.Kim@ejgallo.com   (502) staff       (20)      329 2024-02-27 03:29:02.000000 gmlutil-data-extraction-1.0.3/gmlutil_data_extraction.egg-info/SOURCES.txt
--rw-r--r--   0 Phillip.Kim@ejgallo.com   (502) staff       (20)        1 2024-02-27 03:29:02.000000 gmlutil-data-extraction-1.0.3/gmlutil_data_extraction.egg-info/dependency_links.txt
--rw-r--r--   0 Phillip.Kim@ejgallo.com   (502) staff       (20)      315 2024-02-27 03:29:02.000000 gmlutil-data-extraction-1.0.3/gmlutil_data_extraction.egg-info/requires.txt
--rw-r--r--   0 Phillip.Kim@ejgallo.com   (502) staff       (20)       24 2024-02-27 03:29:02.000000 gmlutil-data-extraction-1.0.3/gmlutil_data_extraction.egg-info/top_level.txt
--rw-r--r--   0 Phillip.Kim@ejgallo.com   (502) staff       (20)       38 2024-02-27 03:29:02.075337 gmlutil-data-extraction-1.0.3/setup.cfg
--rw-r--r--   0 Phillip.Kim@ejgallo.com   (502) staff       (20)     1387 2024-02-27 03:26:11.000000 gmlutil-data-extraction-1.0.3/setup.py
+drwxr-xr-x   0 Phillip.Kim@ejgallo.com   (502) staff       (20)        0 2024-05-13 20:59:23.125176 gmlutil-data-extraction-1.0.4/
+-rw-r--r--   0 Phillip.Kim@ejgallo.com   (502) staff       (20)      767 2024-05-13 20:59:23.124941 gmlutil-data-extraction-1.0.4/PKG-INFO
+-rw-r--r--   0 Phillip.Kim@ejgallo.com   (502) staff       (20)     6303 2024-02-22 22:08:31.000000 gmlutil-data-extraction-1.0.4/README.md
+drwxr-xr-x   0 Phillip.Kim@ejgallo.com   (502) staff       (20)        0 2024-05-13 20:59:23.108708 gmlutil-data-extraction-1.0.4/gmlutil_data_extraction/
+-rw-r--r--   0 Phillip.Kim@ejgallo.com   (502) staff       (20)      162 2024-02-13 01:11:59.000000 gmlutil-data-extraction-1.0.4/gmlutil_data_extraction/config.py
+-rw-r--r--   0 Phillip.Kim@ejgallo.com   (502) staff       (20)    19450 2024-05-13 20:50:24.000000 gmlutil-data-extraction-1.0.4/gmlutil_data_extraction/data_extraction.py
+drwxr-xr-x   0 Phillip.Kim@ejgallo.com   (502) staff       (20)        0 2024-05-13 20:59:23.124626 gmlutil-data-extraction-1.0.4/gmlutil_data_extraction.egg-info/
+-rw-r--r--   0 Phillip.Kim@ejgallo.com   (502) staff       (20)      767 2024-05-13 20:59:23.000000 gmlutil-data-extraction-1.0.4/gmlutil_data_extraction.egg-info/PKG-INFO
+-rw-r--r--   0 Phillip.Kim@ejgallo.com   (502) staff       (20)      329 2024-05-13 20:59:23.000000 gmlutil-data-extraction-1.0.4/gmlutil_data_extraction.egg-info/SOURCES.txt
+-rw-r--r--   0 Phillip.Kim@ejgallo.com   (502) staff       (20)        1 2024-05-13 20:59:23.000000 gmlutil-data-extraction-1.0.4/gmlutil_data_extraction.egg-info/dependency_links.txt
+-rw-r--r--   0 Phillip.Kim@ejgallo.com   (502) staff       (20)      315 2024-05-13 20:59:23.000000 gmlutil-data-extraction-1.0.4/gmlutil_data_extraction.egg-info/requires.txt
+-rw-r--r--   0 Phillip.Kim@ejgallo.com   (502) staff       (20)       24 2024-05-13 20:59:23.000000 gmlutil-data-extraction-1.0.4/gmlutil_data_extraction.egg-info/top_level.txt
+-rw-r--r--   0 Phillip.Kim@ejgallo.com   (502) staff       (20)       38 2024-05-13 20:59:23.125224 gmlutil-data-extraction-1.0.4/setup.cfg
+-rw-r--r--   0 Phillip.Kim@ejgallo.com   (502) staff       (20)     1387 2024-05-13 20:59:12.000000 gmlutil-data-extraction-1.0.4/setup.py
```

### Comparing `gmlutil-data-extraction-1.0.3/PKG-INFO` & `gmlutil-data-extraction-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmlutil-data-extraction
-Version: 1.0.3
+Version: 1.0.4
 Summary: General Machine Learning Utility Package for Data Extraction
 Home-page: https://github.com/Phillip1982/gmlutil_data_extraction
 Author: Phillip Kim
 Author-email: phillip.kim@ejgallo.com
 License: BSD 2-clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: IPython
```

### Comparing `gmlutil-data-extraction-1.0.3/README.md` & `gmlutil-data-extraction-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `gmlutil-data-extraction-1.0.3/gmlutil_data_extraction.egg-info/PKG-INFO` & `gmlutil-data-extraction-1.0.4/gmlutil_data_extraction.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmlutil-data-extraction
-Version: 1.0.3
+Version: 1.0.4
 Summary: General Machine Learning Utility Package for Data Extraction
 Home-page: https://github.com/Phillip1982/gmlutil_data_extraction
 Author: Phillip Kim
 Author-email: phillip.kim@ejgallo.com
 License: BSD 2-clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: IPython
```

### Comparing `gmlutil-data-extraction-1.0.3/setup.py` & `gmlutil-data-extraction-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='gmlutil-data-extraction',
-    version='1.0.3',    
+    version='1.0.4',    
     description='General Machine Learning Utility Package for Data Extraction',
     url='https://github.com/Phillip1982/gmlutil_data_extraction',
     author='Phillip Kim',
     author_email='phillip.kim@ejgallo.com',
     license='BSD 2-clause', ## Change this
     packages=['gmlutil_data_extraction'],
     install_requires=[ # package>=0.2,<0.3
```

