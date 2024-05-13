# Comparing `tmp/nchuchain-1.0.3.tar.gz` & `tmp/nchuchain-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nchuchain-1.0.3.tar", last modified: Mon May 13 11:56:00 2024, max compression
+gzip compressed data, was "nchuchain-1.0.4.tar", last modified: Mon May 13 11:58:28 2024, max compression
```

## Comparing `nchuchain-1.0.3.tar` & `nchuchain-1.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)        0 2024-05-13 11:56:00.652584 nchuchain-1.0.3/
--rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)     1068 2024-05-07 09:39:28.000000 nchuchain-1.0.3/LICENSE
--rw-r--r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)      867 2024-05-13 11:56:00.652584 nchuchain-1.0.3/PKG-INFO
--rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)       12 2024-05-13 11:51:17.000000 nchuchain-1.0.3/README.md
-drwxrwxr-x   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)        0 2024-05-13 11:56:00.648584 nchuchain-1.0.3/nchuchain.egg-info/
--rw-r--r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)      867 2024-05-13 11:56:00.000000 nchuchain-1.0.3/nchuchain.egg-info/PKG-INFO
--rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)      190 2024-05-13 11:56:00.000000 nchuchain-1.0.3/nchuchain.egg-info/SOURCES.txt
--rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)        1 2024-05-13 11:56:00.000000 nchuchain-1.0.3/nchuchain.egg-info/dependency_links.txt
--rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)      179 2024-05-13 11:56:00.000000 nchuchain-1.0.3/nchuchain.egg-info/requires.txt
--rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)        1 2024-05-13 11:56:00.000000 nchuchain-1.0.3/nchuchain.egg-info/top_level.txt
--rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)       38 2024-05-13 11:56:00.652584 nchuchain-1.0.3/setup.cfg
--rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)     1320 2024-05-13 11:55:42.000000 nchuchain-1.0.3/setup.py
+drwxrwxr-x   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)        0 2024-05-13 11:58:28.090975 nchuchain-1.0.4/
+-rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)     1068 2024-05-07 09:39:28.000000 nchuchain-1.0.4/LICENSE
+-rw-r--r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)      908 2024-05-13 11:58:28.090975 nchuchain-1.0.4/PKG-INFO
+-rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)       12 2024-05-13 11:51:17.000000 nchuchain-1.0.4/README.md
+drwxrwxr-x   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)        0 2024-05-13 11:58:28.090975 nchuchain-1.0.4/nchuchain.egg-info/
+-rw-r--r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)      908 2024-05-13 11:58:28.000000 nchuchain-1.0.4/nchuchain.egg-info/PKG-INFO
+-rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)      190 2024-05-13 11:58:28.000000 nchuchain-1.0.4/nchuchain.egg-info/SOURCES.txt
+-rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)        1 2024-05-13 11:58:28.000000 nchuchain-1.0.4/nchuchain.egg-info/dependency_links.txt
+-rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)      179 2024-05-13 11:58:28.000000 nchuchain-1.0.4/nchuchain.egg-info/requires.txt
+-rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)        1 2024-05-13 11:58:28.000000 nchuchain-1.0.4/nchuchain.egg-info/top_level.txt
+-rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)       38 2024-05-13 11:58:28.090975 nchuchain-1.0.4/setup.cfg
+-rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)     1361 2024-05-13 11:58:25.000000 nchuchain-1.0.4/setup.py
```

### Comparing `nchuchain-1.0.3/LICENSE` & `nchuchain-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nchuchain-1.0.3/PKG-INFO` & `nchuchain-1.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: nchuchain
-Version: 1.0.3
+Version: 1.0.4
 Summary: A set of data tools in Python
-Home-page: 
+Home-page: https://github.com/good22014040/nchuchain
 Download-URL: https://pypi.org/project/nchuchain/
 Author: WenChuan Hsu
 Author-email: wenchuan19991111@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `nchuchain-1.0.3/nchuchain.egg-info/PKG-INFO` & `nchuchain-1.0.4/nchuchain.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: nchuchain
-Version: 1.0.3
+Version: 1.0.4
 Summary: A set of data tools in Python
-Home-page: 
+Home-page: https://github.com/good22014040/nchuchain
 Download-URL: https://pypi.org/project/nchuchain/
 Author: WenChuan Hsu
 Author-email: wenchuan19991111@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `nchuchain-1.0.3/setup.py` & `nchuchain-1.0.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 from setuptools import setup, find_packages
  
 HERE = pathlib.Path(__file__).parent.resolve()
  
 PACKAGE_NAME = "nchuchain"
 AUTHOR = "WenChuan Hsu"
 AUTHOR_EMAIL = "wenchuan19991111@gmail.com"
-URL = ""
+URL = "https://github.com/good22014040/nchuchain"
 DOWNLOAD_URL = "https://pypi.org/project/nchuchain/"
  
 LICENSE = "MIT"
-VERSION = "1.0.3"
+VERSION = "1.0.4"
 DESCRIPTION = "A set of data tools in Python"
 LONG_DESCRIPTION = (HERE / "README.md").read_text(encoding="utf8")
 LONG_DESC_TYPE = "text/markdown"
  
 requirements = (HERE / "requirements.txt").read_text(encoding="utf8")
 INSTALL_REQUIRES = [s.strip() for s in requirements.split("\n")]
```

