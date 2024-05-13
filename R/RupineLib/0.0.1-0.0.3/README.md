# Comparing `tmp/RupineLib-0.0.1.tar.gz` & `tmp/RupineLib-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RupineLib-0.0.1.tar", last modified: Mon May 13 07:46:39 2024, max compression
+gzip compressed data, was "RupineLib-0.0.3.tar", last modified: Mon May 13 08:26:21 2024, max compression
```

## Comparing `RupineLib-0.0.1.tar` & `RupineLib-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,20 @@
-drwxr-xr-x   0 bentstark  (1000) bentstark  (1000)        0 2024-05-13 07:46:39.052659 RupineLib-0.0.1/
--rw-r--r--   0 bentstark  (1000) bentstark  (1000)     1067 2024-05-13 06:21:24.000000 RupineLib-0.0.1/LICENSE
--rw-r--r--   0 bentstark  (1000) bentstark  (1000)      542 2024-05-13 07:46:39.052659 RupineLib-0.0.1/PKG-INFO
--rw-r--r--   0 bentstark  (1000) bentstark  (1000)       10 2024-05-13 06:21:24.000000 RupineLib-0.0.1/README.md
-drwxr-xr-x   0 bentstark  (1000) bentstark  (1000)        0 2024-05-13 07:46:39.052659 RupineLib-0.0.1/RupineLib.egg-info/
--rw-r--r--   0 bentstark  (1000) bentstark  (1000)      542 2024-05-13 07:46:38.000000 RupineLib-0.0.1/RupineLib.egg-info/PKG-INFO
--rw-r--r--   0 bentstark  (1000) bentstark  (1000)      266 2024-05-13 07:46:38.000000 RupineLib-0.0.1/RupineLib.egg-info/SOURCES.txt
--rw-r--r--   0 bentstark  (1000) bentstark  (1000)        1 2024-05-13 07:46:38.000000 RupineLib-0.0.1/RupineLib.egg-info/dependency_links.txt
--rw-r--r--   0 bentstark  (1000) bentstark  (1000)        7 2024-05-13 07:46:38.000000 RupineLib-0.0.1/RupineLib.egg-info/top_level.txt
-drwxr-xr-x   0 bentstark  (1000) bentstark  (1000)        0 2024-05-13 07:46:39.052659 RupineLib-0.0.1/dbCode/
--rw-r--r--   0 bentstark  (1000) bentstark  (1000)        0 2024-05-13 07:02:54.000000 RupineLib-0.0.1/dbCode/__init__.py
--rw-r--r--   0 bentstark  (1000) bentstark  (1000)    14816 2024-05-13 07:11:04.000000 RupineLib-0.0.1/dbCode/advancedDBOperation.py
--rw-r--r--   0 bentstark  (1000) bentstark  (1000)      355 2024-05-13 07:04:46.000000 RupineLib-0.0.1/dbCode/connection.py
--rw-r--r--   0 bentstark  (1000) bentstark  (1000)     2939 2024-05-13 07:44:21.000000 RupineLib-0.0.1/dbCode/directDBOperation.py
--rw-r--r--   0 bentstark  (1000) bentstark  (1000)       79 2024-05-13 07:46:39.052659 RupineLib-0.0.1/setup.cfg
--rw-r--r--   0 bentstark  (1000) bentstark  (1000)      981 2024-05-13 07:07:10.000000 RupineLib-0.0.1/setup.py
+drwxr-xr-x   0 bentstark  (1000) bentstark  (1000)        0 2024-05-13 08:26:21.202627 RupineLib-0.0.3/
+-rw-r--r--   0 bentstark  (1000) bentstark  (1000)     1067 2024-05-13 06:21:24.000000 RupineLib-0.0.3/LICENSE
+-rw-r--r--   0 bentstark  (1000) bentstark  (1000)      542 2024-05-13 08:26:21.202627 RupineLib-0.0.3/PKG-INFO
+-rw-r--r--   0 bentstark  (1000) bentstark  (1000)       10 2024-05-13 06:21:24.000000 RupineLib-0.0.3/README.md
+drwxr-xr-x   0 bentstark  (1000) bentstark  (1000)        0 2024-05-13 08:26:21.202627 RupineLib-0.0.3/RupineLib/
+-rw-r--r--   0 bentstark  (1000) bentstark  (1000)        0 2024-05-13 08:25:06.000000 RupineLib-0.0.3/RupineLib/__init__.py
+-rw-r--r--   0 bentstark  (1000) bentstark  (1000)     2642 2024-05-13 08:23:38.000000 RupineLib-0.0.3/RupineLib/db.py
+drwxr-xr-x   0 bentstark  (1000) bentstark  (1000)        0 2024-05-13 08:26:21.202627 RupineLib-0.0.3/RupineLib/dbCode/
+-rw-r--r--   0 bentstark  (1000) bentstark  (1000)        0 2024-05-13 07:02:54.000000 RupineLib-0.0.3/RupineLib/dbCode/__init__.py
+-rw-r--r--   0 bentstark  (1000) bentstark  (1000)    14816 2024-05-13 07:11:04.000000 RupineLib-0.0.3/RupineLib/dbCode/advancedDBOperation.py
+-rw-r--r--   0 bentstark  (1000) bentstark  (1000)      355 2024-05-13 07:04:46.000000 RupineLib-0.0.3/RupineLib/dbCode/connection.py
+-rw-r--r--   0 bentstark  (1000) bentstark  (1000)     2939 2024-05-13 07:44:21.000000 RupineLib-0.0.3/RupineLib/dbCode/directDBOperation.py
+-rw-r--r--   0 bentstark  (1000) bentstark  (1000)       77 2024-05-13 08:23:42.000000 RupineLib-0.0.3/RupineLib/timer.py
+drwxr-xr-x   0 bentstark  (1000) bentstark  (1000)        0 2024-05-13 08:26:21.202627 RupineLib-0.0.3/RupineLib.egg-info/
+-rw-r--r--   0 bentstark  (1000) bentstark  (1000)      542 2024-05-13 08:26:21.000000 RupineLib-0.0.3/RupineLib.egg-info/PKG-INFO
+-rw-r--r--   0 bentstark  (1000) bentstark  (1000)      363 2024-05-13 08:26:21.000000 RupineLib-0.0.3/RupineLib.egg-info/SOURCES.txt
+-rw-r--r--   0 bentstark  (1000) bentstark  (1000)        1 2024-05-13 08:26:21.000000 RupineLib-0.0.3/RupineLib.egg-info/dependency_links.txt
+-rw-r--r--   0 bentstark  (1000) bentstark  (1000)       10 2024-05-13 08:26:21.000000 RupineLib-0.0.3/RupineLib.egg-info/top_level.txt
+-rw-r--r--   0 bentstark  (1000) bentstark  (1000)       79 2024-05-13 08:26:21.202627 RupineLib-0.0.3/setup.cfg
+-rw-r--r--   0 bentstark  (1000) bentstark  (1000)      981 2024-05-13 08:25:39.000000 RupineLib-0.0.3/setup.py
```

### Comparing `RupineLib-0.0.1/LICENSE` & `RupineLib-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `RupineLib-0.0.1/PKG-INFO` & `RupineLib-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RupineLib
-Version: 0.0.1
+Version: 0.0.3
 Summary: RupineLib
 Home-page: UNKNOWN
 Author: RupineLabs
 Author-email: <abc@def.com>
 License: UNKNOWN
 Keywords: web3
 Platform: UNKNOWN
```

### Comparing `RupineLib-0.0.1/RupineLib.egg-info/PKG-INFO` & `RupineLib-0.0.3/RupineLib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RupineLib
-Version: 0.0.1
+Version: 0.0.3
 Summary: RupineLib
 Home-page: UNKNOWN
 Author: RupineLabs
 Author-email: <abc@def.com>
 License: UNKNOWN
 Keywords: web3
 Platform: UNKNOWN
```

### Comparing `RupineLib-0.0.1/dbCode/advancedDBOperation.py` & `RupineLib-0.0.3/RupineLib/dbCode/advancedDBOperation.py`

 * *Files identical despite different names*

### Comparing `RupineLib-0.0.1/dbCode/directDBOperation.py` & `RupineLib-0.0.3/RupineLib/dbCode/directDBOperation.py`

 * *Files identical despite different names*

### Comparing `RupineLib-0.0.1/setup.py` & `RupineLib-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.1'
+VERSION = '0.0.3'
 DESCRIPTION = 'RupineLib'
 LONG_DESCRIPTION = 'Rupine Python Library'
 
 # Setting up
 setup(
     name="RupineLib",
     version=VERSION,
```

