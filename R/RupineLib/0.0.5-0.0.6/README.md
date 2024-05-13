# Comparing `tmp/RupineLib-0.0.5.tar.gz` & `tmp/RupineLib-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RupineLib-0.0.5.tar", last modified: Mon May 13 08:54:43 2024, max compression
+gzip compressed data, was "RupineLib-0.0.6.tar", last modified: Mon May 13 08:57:20 2024, max compression
```

## Comparing `RupineLib-0.0.5.tar` & `RupineLib-0.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 bentstark  (1000) bentstark  (1000)        0 2024-05-13 08:54:43.142603 RupineLib-0.0.5/
--rw-r--r--   0 bentstark  (1000) bentstark  (1000)     1067 2024-05-13 06:21:24.000000 RupineLib-0.0.5/LICENSE
--rw-r--r--   0 bentstark  (1000) bentstark  (1000)      542 2024-05-13 08:54:43.142603 RupineLib-0.0.5/PKG-INFO
--rw-r--r--   0 bentstark  (1000) bentstark  (1000)       10 2024-05-13 06:21:24.000000 RupineLib-0.0.5/README.md
-drwxr-xr-x   0 bentstark  (1000) bentstark  (1000)        0 2024-05-13 08:54:43.122604 RupineLib-0.0.5/RupineLib/
--rw-r--r--   0 bentstark  (1000) bentstark  (1000)        0 2024-05-13 08:25:06.000000 RupineLib-0.0.5/RupineLib/__init__.py
--rw-r--r--   0 bentstark  (1000) bentstark  (1000)     2642 2024-05-13 08:23:38.000000 RupineLib-0.0.5/RupineLib/db.py
-drwxr-xr-x   0 bentstark  (1000) bentstark  (1000)        0 2024-05-13 08:54:43.142603 RupineLib-0.0.5/RupineLib/dbCode/
--rw-r--r--   0 bentstark  (1000) bentstark  (1000)        0 2024-05-13 07:02:54.000000 RupineLib-0.0.5/RupineLib/dbCode/__init__.py
--rw-r--r--   0 bentstark  (1000) bentstark  (1000)    14816 2024-05-13 07:11:04.000000 RupineLib-0.0.5/RupineLib/dbCode/advancedDBOperation.py
--rw-r--r--   0 bentstark  (1000) bentstark  (1000)      355 2024-05-13 07:04:46.000000 RupineLib-0.0.5/RupineLib/dbCode/connection.py
--rw-r--r--   0 bentstark  (1000) bentstark  (1000)     2939 2024-05-13 07:44:21.000000 RupineLib-0.0.5/RupineLib/dbCode/directDBOperation.py
--rw-r--r--   0 bentstark  (1000) bentstark  (1000)      775 2024-05-13 08:54:32.000000 RupineLib-0.0.5/RupineLib/timer.py
-drwxr-xr-x   0 bentstark  (1000) bentstark  (1000)        0 2024-05-13 08:54:43.132604 RupineLib-0.0.5/RupineLib.egg-info/
--rw-r--r--   0 bentstark  (1000) bentstark  (1000)      542 2024-05-13 08:54:42.000000 RupineLib-0.0.5/RupineLib.egg-info/PKG-INFO
--rw-r--r--   0 bentstark  (1000) bentstark  (1000)      395 2024-05-13 08:54:42.000000 RupineLib-0.0.5/RupineLib.egg-info/SOURCES.txt
--rw-r--r--   0 bentstark  (1000) bentstark  (1000)        1 2024-05-13 08:54:42.000000 RupineLib-0.0.5/RupineLib.egg-info/dependency_links.txt
--rw-r--r--   0 bentstark  (1000) bentstark  (1000)       16 2024-05-13 08:54:42.000000 RupineLib-0.0.5/RupineLib.egg-info/requires.txt
--rw-r--r--   0 bentstark  (1000) bentstark  (1000)       10 2024-05-13 08:54:42.000000 RupineLib-0.0.5/RupineLib.egg-info/top_level.txt
--rw-r--r--   0 bentstark  (1000) bentstark  (1000)       79 2024-05-13 08:54:43.142603 RupineLib-0.0.5/setup.cfg
--rw-r--r--   0 bentstark  (1000) bentstark  (1000)     1000 2024-05-13 08:54:39.000000 RupineLib-0.0.5/setup.py
+drwxr-xr-x   0 bentstark  (1000) bentstark  (1000)        0 2024-05-13 08:57:20.692601 RupineLib-0.0.6/
+-rw-r--r--   0 bentstark  (1000) bentstark  (1000)     1067 2024-05-13 06:21:24.000000 RupineLib-0.0.6/LICENSE
+-rw-r--r--   0 bentstark  (1000) bentstark  (1000)      542 2024-05-13 08:57:20.692601 RupineLib-0.0.6/PKG-INFO
+-rw-r--r--   0 bentstark  (1000) bentstark  (1000)       10 2024-05-13 06:21:24.000000 RupineLib-0.0.6/README.md
+drwxr-xr-x   0 bentstark  (1000) bentstark  (1000)        0 2024-05-13 08:57:20.682601 RupineLib-0.0.6/RupineLib/
+-rw-r--r--   0 bentstark  (1000) bentstark  (1000)        0 2024-05-13 08:25:06.000000 RupineLib-0.0.6/RupineLib/__init__.py
+-rw-r--r--   0 bentstark  (1000) bentstark  (1000)     2612 2024-05-13 08:57:11.000000 RupineLib-0.0.6/RupineLib/db.py
+drwxr-xr-x   0 bentstark  (1000) bentstark  (1000)        0 2024-05-13 08:57:20.692601 RupineLib-0.0.6/RupineLib/dbCode/
+-rw-r--r--   0 bentstark  (1000) bentstark  (1000)        0 2024-05-13 07:02:54.000000 RupineLib-0.0.6/RupineLib/dbCode/__init__.py
+-rw-r--r--   0 bentstark  (1000) bentstark  (1000)    14816 2024-05-13 07:11:04.000000 RupineLib-0.0.6/RupineLib/dbCode/advancedDBOperation.py
+-rw-r--r--   0 bentstark  (1000) bentstark  (1000)      355 2024-05-13 07:04:46.000000 RupineLib-0.0.6/RupineLib/dbCode/connection.py
+-rw-r--r--   0 bentstark  (1000) bentstark  (1000)     2939 2024-05-13 07:44:21.000000 RupineLib-0.0.6/RupineLib/dbCode/directDBOperation.py
+-rw-r--r--   0 bentstark  (1000) bentstark  (1000)      775 2024-05-13 08:54:32.000000 RupineLib-0.0.6/RupineLib/timer.py
+drwxr-xr-x   0 bentstark  (1000) bentstark  (1000)        0 2024-05-13 08:57:20.692601 RupineLib-0.0.6/RupineLib.egg-info/
+-rw-r--r--   0 bentstark  (1000) bentstark  (1000)      542 2024-05-13 08:57:20.000000 RupineLib-0.0.6/RupineLib.egg-info/PKG-INFO
+-rw-r--r--   0 bentstark  (1000) bentstark  (1000)      395 2024-05-13 08:57:20.000000 RupineLib-0.0.6/RupineLib.egg-info/SOURCES.txt
+-rw-r--r--   0 bentstark  (1000) bentstark  (1000)        1 2024-05-13 08:57:20.000000 RupineLib-0.0.6/RupineLib.egg-info/dependency_links.txt
+-rw-r--r--   0 bentstark  (1000) bentstark  (1000)       16 2024-05-13 08:57:20.000000 RupineLib-0.0.6/RupineLib.egg-info/requires.txt
+-rw-r--r--   0 bentstark  (1000) bentstark  (1000)       10 2024-05-13 08:57:20.000000 RupineLib-0.0.6/RupineLib.egg-info/top_level.txt
+-rw-r--r--   0 bentstark  (1000) bentstark  (1000)       79 2024-05-13 08:57:20.692601 RupineLib-0.0.6/setup.cfg
+-rw-r--r--   0 bentstark  (1000) bentstark  (1000)     1000 2024-05-13 08:57:18.000000 RupineLib-0.0.6/setup.py
```

### Comparing `RupineLib-0.0.5/LICENSE` & `RupineLib-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `RupineLib-0.0.5/PKG-INFO` & `RupineLib-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RupineLib
-Version: 0.0.5
+Version: 0.0.6
 Summary: RupineLib
 Home-page: UNKNOWN
 Author: RupineLabs
 Author-email: <abc@def.com>
 License: UNKNOWN
 Keywords: web3
 Platform: UNKNOWN
```

### Comparing `RupineLib-0.0.5/RupineLib/db.py` & `RupineLib-0.0.6/RupineLib/db.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-import RupineLib.dbCode.connection as conn
-import RupineLib.dbCode.directDBOperation as directOP
-import RupineLib.dbCode.advancedDBOperation as advOP
+import dbCode.connection as conn
+import dbCode.directDBOperation as directOP
+import dbCode.advancedDBOperation as advOP
 
 def connect(user,pw,host,Port,database):
     return conn.connect(user,pw,host,Port,database)
 
 def connectURI(connectionStr):
     return conn.connectURI(connectionStr)
```

### Comparing `RupineLib-0.0.5/RupineLib/dbCode/advancedDBOperation.py` & `RupineLib-0.0.6/RupineLib/dbCode/advancedDBOperation.py`

 * *Files identical despite different names*

### Comparing `RupineLib-0.0.5/RupineLib/dbCode/directDBOperation.py` & `RupineLib-0.0.6/RupineLib/dbCode/directDBOperation.py`

 * *Files identical despite different names*

### Comparing `RupineLib-0.0.5/RupineLib/timer.py` & `RupineLib-0.0.6/RupineLib/timer.py`

 * *Files identical despite different names*

### Comparing `RupineLib-0.0.5/RupineLib.egg-info/PKG-INFO` & `RupineLib-0.0.6/RupineLib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RupineLib
-Version: 0.0.5
+Version: 0.0.6
 Summary: RupineLib
 Home-page: UNKNOWN
 Author: RupineLabs
 Author-email: <abc@def.com>
 License: UNKNOWN
 Keywords: web3
 Platform: UNKNOWN
```

### Comparing `RupineLib-0.0.5/setup.py` & `RupineLib-0.0.6/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.5'
+VERSION = '0.0.6'
 DESCRIPTION = 'RupineLib'
 LONG_DESCRIPTION = 'Rupine Python Library'
 
 # Setting up
 setup(
     name="RupineLib",
     version=VERSION,
```

