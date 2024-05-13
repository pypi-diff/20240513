# Comparing `tmp/RupineLib-0.0.8.tar.gz` & `tmp/RupineLib-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RupineLib-0.0.8.tar", last modified: Mon May 13 09:03:22 2024, max compression
+gzip compressed data, was "RupineLib-0.0.9.tar", last modified: Mon May 13 09:07:43 2024, max compression
```

## Comparing `RupineLib-0.0.8.tar` & `RupineLib-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 bentstark  (1000) bentstark  (1000)        0 2024-05-13 09:03:22.402597 RupineLib-0.0.8/
--rw-r--r--   0 bentstark  (1000) bentstark  (1000)     1067 2024-05-13 06:21:24.000000 RupineLib-0.0.8/LICENSE
--rw-r--r--   0 bentstark  (1000) bentstark  (1000)      542 2024-05-13 09:03:22.402597 RupineLib-0.0.8/PKG-INFO
--rw-r--r--   0 bentstark  (1000) bentstark  (1000)       10 2024-05-13 06:21:24.000000 RupineLib-0.0.8/README.md
-drwxr-xr-x   0 bentstark  (1000) bentstark  (1000)        0 2024-05-13 09:03:22.392596 RupineLib-0.0.8/RupineLib/
--rw-r--r--   0 bentstark  (1000) bentstark  (1000)        0 2024-05-13 08:25:06.000000 RupineLib-0.0.8/RupineLib/__init__.py
--rw-r--r--   0 bentstark  (1000) bentstark  (1000)     2612 2024-05-13 09:02:46.000000 RupineLib-0.0.8/RupineLib/db.py
-drwxr-xr-x   0 bentstark  (1000) bentstark  (1000)        0 2024-05-13 09:03:22.392596 RupineLib-0.0.8/RupineLib/dbCode/
--rw-r--r--   0 bentstark  (1000) bentstark  (1000)        0 2024-05-13 07:02:54.000000 RupineLib-0.0.8/RupineLib/dbCode/__init__.py
--rw-r--r--   0 bentstark  (1000) bentstark  (1000)    14816 2024-05-13 07:11:04.000000 RupineLib-0.0.8/RupineLib/dbCode/advancedDBOperation.py
--rw-r--r--   0 bentstark  (1000) bentstark  (1000)      355 2024-05-13 07:04:46.000000 RupineLib-0.0.8/RupineLib/dbCode/connection.py
--rw-r--r--   0 bentstark  (1000) bentstark  (1000)     2939 2024-05-13 07:44:21.000000 RupineLib-0.0.8/RupineLib/dbCode/directDBOperation.py
--rw-r--r--   0 bentstark  (1000) bentstark  (1000)      775 2024-05-13 08:54:32.000000 RupineLib-0.0.8/RupineLib/timer.py
-drwxr-xr-x   0 bentstark  (1000) bentstark  (1000)        0 2024-05-13 09:03:22.392596 RupineLib-0.0.8/RupineLib.egg-info/
--rw-r--r--   0 bentstark  (1000) bentstark  (1000)      542 2024-05-13 09:03:22.000000 RupineLib-0.0.8/RupineLib.egg-info/PKG-INFO
--rw-r--r--   0 bentstark  (1000) bentstark  (1000)      395 2024-05-13 09:03:22.000000 RupineLib-0.0.8/RupineLib.egg-info/SOURCES.txt
--rw-r--r--   0 bentstark  (1000) bentstark  (1000)        1 2024-05-13 09:03:22.000000 RupineLib-0.0.8/RupineLib.egg-info/dependency_links.txt
--rw-r--r--   0 bentstark  (1000) bentstark  (1000)       16 2024-05-13 09:03:22.000000 RupineLib-0.0.8/RupineLib.egg-info/requires.txt
--rw-r--r--   0 bentstark  (1000) bentstark  (1000)       10 2024-05-13 09:03:22.000000 RupineLib-0.0.8/RupineLib.egg-info/top_level.txt
--rw-r--r--   0 bentstark  (1000) bentstark  (1000)       79 2024-05-13 09:03:22.402597 RupineLib-0.0.8/setup.cfg
--rw-r--r--   0 bentstark  (1000) bentstark  (1000)     1000 2024-05-13 09:03:14.000000 RupineLib-0.0.8/setup.py
+drwxr-xr-x   0 bentstark  (1000) bentstark  (1000)        0 2024-05-13 09:07:43.252593 RupineLib-0.0.9/
+-rw-r--r--   0 bentstark  (1000) bentstark  (1000)     1067 2024-05-13 06:21:24.000000 RupineLib-0.0.9/LICENSE
+-rw-r--r--   0 bentstark  (1000) bentstark  (1000)      542 2024-05-13 09:07:43.252593 RupineLib-0.0.9/PKG-INFO
+-rw-r--r--   0 bentstark  (1000) bentstark  (1000)       10 2024-05-13 06:21:24.000000 RupineLib-0.0.9/README.md
+drwxr-xr-x   0 bentstark  (1000) bentstark  (1000)        0 2024-05-13 09:07:43.242593 RupineLib-0.0.9/RupineLib/
+-rw-r--r--   0 bentstark  (1000) bentstark  (1000)        0 2024-05-13 08:25:06.000000 RupineLib-0.0.9/RupineLib/__init__.py
+-rw-r--r--   0 bentstark  (1000) bentstark  (1000)     2657 2024-05-13 09:07:34.000000 RupineLib-0.0.9/RupineLib/db.py
+drwxr-xr-x   0 bentstark  (1000) bentstark  (1000)        0 2024-05-13 09:07:43.252593 RupineLib-0.0.9/RupineLib/dbCode/
+-rw-r--r--   0 bentstark  (1000) bentstark  (1000)        0 2024-05-13 07:02:54.000000 RupineLib-0.0.9/RupineLib/dbCode/__init__.py
+-rw-r--r--   0 bentstark  (1000) bentstark  (1000)    14816 2024-05-13 07:11:04.000000 RupineLib-0.0.9/RupineLib/dbCode/advancedDBOperation.py
+-rw-r--r--   0 bentstark  (1000) bentstark  (1000)      355 2024-05-13 07:04:46.000000 RupineLib-0.0.9/RupineLib/dbCode/connection.py
+-rw-r--r--   0 bentstark  (1000) bentstark  (1000)     2939 2024-05-13 07:44:21.000000 RupineLib-0.0.9/RupineLib/dbCode/directDBOperation.py
+-rw-r--r--   0 bentstark  (1000) bentstark  (1000)      775 2024-05-13 08:54:32.000000 RupineLib-0.0.9/RupineLib/timer.py
+drwxr-xr-x   0 bentstark  (1000) bentstark  (1000)        0 2024-05-13 09:07:43.252593 RupineLib-0.0.9/RupineLib.egg-info/
+-rw-r--r--   0 bentstark  (1000) bentstark  (1000)      542 2024-05-13 09:07:43.000000 RupineLib-0.0.9/RupineLib.egg-info/PKG-INFO
+-rw-r--r--   0 bentstark  (1000) bentstark  (1000)      395 2024-05-13 09:07:43.000000 RupineLib-0.0.9/RupineLib.egg-info/SOURCES.txt
+-rw-r--r--   0 bentstark  (1000) bentstark  (1000)        1 2024-05-13 09:07:43.000000 RupineLib-0.0.9/RupineLib.egg-info/dependency_links.txt
+-rw-r--r--   0 bentstark  (1000) bentstark  (1000)       16 2024-05-13 09:07:43.000000 RupineLib-0.0.9/RupineLib.egg-info/requires.txt
+-rw-r--r--   0 bentstark  (1000) bentstark  (1000)       10 2024-05-13 09:07:43.000000 RupineLib-0.0.9/RupineLib.egg-info/top_level.txt
+-rw-r--r--   0 bentstark  (1000) bentstark  (1000)       79 2024-05-13 09:07:43.262593 RupineLib-0.0.9/setup.cfg
+-rw-r--r--   0 bentstark  (1000) bentstark  (1000)     1000 2024-05-13 09:07:41.000000 RupineLib-0.0.9/setup.py
```

### Comparing `RupineLib-0.0.8/LICENSE` & `RupineLib-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `RupineLib-0.0.8/PKG-INFO` & `RupineLib-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RupineLib
-Version: 0.0.8
+Version: 0.0.9
 Summary: RupineLib
 Home-page: UNKNOWN
 Author: RupineLabs
 Author-email: <abc@def.com>
 License: UNKNOWN
 Keywords: web3
 Platform: UNKNOWN
```

### Comparing `RupineLib-0.0.8/RupineLib/db.py` & `RupineLib-0.0.9/RupineLib/db.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-import dbCode.connection as conn
-import dbCode.directDBOperation as directOP
-import dbCode.advancedDBOperation as advOP
+from RupineLib.dbCode import connection as conn
+from RupineLib.dbCode import directDBOperation as directOP
+from RupineLib.dbCode import advancedDBOperation as advOP
 
 def connect(user,pw,host,Port,database):
     return conn.connect(user,pw,host,Port,database)
 
 def connectURI(connectionStr):
     return conn.connectURI(connectionStr)
```

### Comparing `RupineLib-0.0.8/RupineLib/dbCode/advancedDBOperation.py` & `RupineLib-0.0.9/RupineLib/dbCode/advancedDBOperation.py`

 * *Files identical despite different names*

### Comparing `RupineLib-0.0.8/RupineLib/dbCode/directDBOperation.py` & `RupineLib-0.0.9/RupineLib/dbCode/directDBOperation.py`

 * *Files identical despite different names*

### Comparing `RupineLib-0.0.8/RupineLib/timer.py` & `RupineLib-0.0.9/RupineLib/timer.py`

 * *Files identical despite different names*

### Comparing `RupineLib-0.0.8/RupineLib.egg-info/PKG-INFO` & `RupineLib-0.0.9/RupineLib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RupineLib
-Version: 0.0.8
+Version: 0.0.9
 Summary: RupineLib
 Home-page: UNKNOWN
 Author: RupineLabs
 Author-email: <abc@def.com>
 License: UNKNOWN
 Keywords: web3
 Platform: UNKNOWN
```

### Comparing `RupineLib-0.0.8/setup.py` & `RupineLib-0.0.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 DESCRIPTION = 'RupineLib'
 LONG_DESCRIPTION = 'Rupine Python Library'
 
 # Setting up
 setup(
     name="RupineLib",
     version=VERSION,
```
