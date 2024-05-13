# Comparing `tmp/py2saber-0.15.2.tar.gz` & `tmp/py2saber-0.15.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py2saber-0.15.2.tar", last modified: Mon May 13 16:22:44 2024, max compression
+gzip compressed data, was "py2saber-0.15.3.tar", last modified: Mon May 13 17:00:57 2024, max compression
```

## Comparing `py2saber-0.15.2.tar` & `py2saber-0.15.3.tar`

### file list

```diff
@@ -1,14 +1,49 @@
-drwxr-xr-x   0 jramboz    (501) staff       (20)        0 2024-05-13 16:22:44.120959 py2saber-0.15.2/
--rw-r--r--   0 jramboz    (501) staff       (20)    35149 2023-05-23 13:52:35.000000 py2saber-0.15.2/COPYING
--rw-r--r--   0 jramboz    (501) staff       (20)    43211 2024-05-13 16:22:44.120777 py2saber-0.15.2/PKG-INFO
--rw-r--r--   0 jramboz    (501) staff       (20)     2047 2024-03-20 16:03:37.000000 py2saber-0.15.2/README.md
-drwxr-xr-x   0 jramboz    (501) staff       (20)        0 2024-05-13 16:22:44.120533 py2saber-0.15.2/py2saber.egg-info/
--rw-r--r--   0 jramboz    (501) staff       (20)    43211 2024-05-13 16:22:44.000000 py2saber-0.15.2/py2saber.egg-info/PKG-INFO
--rw-r--r--   0 jramboz    (501) staff       (20)      238 2024-05-13 16:22:44.000000 py2saber-0.15.2/py2saber.egg-info/SOURCES.txt
--rw-r--r--   0 jramboz    (501) staff       (20)        1 2024-05-13 16:22:44.000000 py2saber-0.15.2/py2saber.egg-info/dependency_links.txt
--rw-r--r--   0 jramboz    (501) staff       (20)       48 2024-05-13 16:22:44.000000 py2saber-0.15.2/py2saber.egg-info/entry_points.txt
--rw-r--r--   0 jramboz    (501) staff       (20)       23 2024-05-13 16:22:44.000000 py2saber-0.15.2/py2saber.egg-info/requires.txt
--rw-r--r--   0 jramboz    (501) staff       (20)       13 2024-05-13 16:22:44.000000 py2saber-0.15.2/py2saber.egg-info/top_level.txt
--rw-r--r--   0 jramboz    (501) staff       (20)    30549 2024-05-13 16:16:24.000000 py2saber-0.15.2/py2saber.py
--rw-r--r--   0 jramboz    (501) staff       (20)      793 2024-05-13 16:16:24.000000 py2saber-0.15.2/pyproject.toml
--rw-r--r--   0 jramboz    (501) staff       (20)       38 2024-05-13 16:22:44.120993 py2saber-0.15.2/setup.cfg
+drwxr-xr-x   0 jramboz    (501) staff       (20)        0 2024-05-13 17:00:57.644857 py2saber-0.15.3/
+-rw-r--r--   0 jramboz    (501) staff       (20)    35149 2023-05-23 13:52:35.000000 py2saber-0.15.3/COPYING
+-rw-r--r--   0 jramboz    (501) staff       (20)       36 2024-05-13 16:57:53.000000 py2saber-0.15.3/MANIFEST.in
+drwxr-xr-x   0 jramboz    (501) staff       (20)        0 2024-05-13 17:00:57.642950 py2saber-0.15.3/OpenCore_OEM/
+-rw-r--r--   0 jramboz    (501) staff       (20)    12004 2024-05-13 14:59:27.000000 py2saber-0.15.3/OpenCore_OEM/BEEP.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    88656 2024-05-13 14:59:27.000000 py2saber-0.15.3/OpenCore_OEM/CLASH_10_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    88200 2024-05-13 14:59:27.000000 py2saber-0.15.3/OpenCore_OEM/CLASH_1_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    88200 2024-05-13 14:59:27.000000 py2saber-0.15.3/OpenCore_OEM/CLASH_2_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    88200 2024-05-13 14:59:27.000000 py2saber-0.15.3/OpenCore_OEM/CLASH_3_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    88200 2024-05-13 14:59:27.000000 py2saber-0.15.3/OpenCore_OEM/CLASH_4_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    88200 2024-05-13 14:59:27.000000 py2saber-0.15.3/OpenCore_OEM/CLASH_5_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    88200 2024-05-13 14:59:27.000000 py2saber-0.15.3/OpenCore_OEM/CLASH_6_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    88200 2024-05-13 14:59:27.000000 py2saber-0.15.3/OpenCore_OEM/CLASH_7_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    88200 2024-05-13 14:59:27.000000 py2saber-0.15.3/OpenCore_OEM/CLASH_8_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    88200 2024-05-13 14:59:27.000000 py2saber-0.15.3/OpenCore_OEM/CLASH_9_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.3/OpenCore_OEM/HUM_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    88200 2024-05-13 14:59:27.000000 py2saber-0.15.3/OpenCore_OEM/POWEROFF_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    88200 2024-05-13 14:59:27.000000 py2saber-0.15.3/OpenCore_OEM/POWERON_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.3/OpenCore_OEM/SMOOTHSWING.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.3/OpenCore_OEM/SMOOTHSWINGH_1_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.3/OpenCore_OEM/SMOOTHSWINGH_2_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.3/OpenCore_OEM/SMOOTHSWINGH_3_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.3/OpenCore_OEM/SMOOTHSWINGH_4_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.3/OpenCore_OEM/SMOOTHSWINGH_5_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.3/OpenCore_OEM/SMOOTHSWINGH_6_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.3/OpenCore_OEM/SMOOTHSWINGH_7_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.3/OpenCore_OEM/SMOOTHSWINGH_8_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.3/OpenCore_OEM/SMOOTHSWINGL_1_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.3/OpenCore_OEM/SMOOTHSWINGL_2_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.3/OpenCore_OEM/SMOOTHSWINGL_3_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.3/OpenCore_OEM/SMOOTHSWINGL_4_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.3/OpenCore_OEM/SMOOTHSWINGL_5_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.3/OpenCore_OEM/SMOOTHSWINGL_6_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.3/OpenCore_OEM/SMOOTHSWINGL_7_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.3/OpenCore_OEM/SMOOTHSWINGL_8_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    43211 2024-05-13 17:00:57.644632 py2saber-0.15.3/PKG-INFO
+-rw-r--r--   0 jramboz    (501) staff       (20)     2047 2024-03-20 16:03:37.000000 py2saber-0.15.3/README.md
+drwxr-xr-x   0 jramboz    (501) staff       (20)        0 2024-05-13 17:00:57.643081 py2saber-0.15.3/dist/
+-rwxr-xr-x   0 jramboz    (501) staff       (20)    20380 2023-07-23 18:03:06.000000 py2saber-0.15.3/dist/pycodesign.py
+drwxr-xr-x   0 jramboz    (501) staff       (20)        0 2024-05-13 17:00:57.644358 py2saber-0.15.3/py2saber.egg-info/
+-rw-r--r--   0 jramboz    (501) staff       (20)    43211 2024-05-13 17:00:57.000000 py2saber-0.15.3/py2saber.egg-info/PKG-INFO
+-rw-r--r--   0 jramboz    (501) staff       (20)     1213 2024-05-13 17:00:57.000000 py2saber-0.15.3/py2saber.egg-info/SOURCES.txt
+-rw-r--r--   0 jramboz    (501) staff       (20)        1 2024-05-13 17:00:57.000000 py2saber-0.15.3/py2saber.egg-info/dependency_links.txt
+-rw-r--r--   0 jramboz    (501) staff       (20)       48 2024-05-13 17:00:57.000000 py2saber-0.15.3/py2saber.egg-info/entry_points.txt
+-rw-r--r--   0 jramboz    (501) staff       (20)       23 2024-05-13 17:00:57.000000 py2saber-0.15.3/py2saber.egg-info/requires.txt
+-rw-r--r--   0 jramboz    (501) staff       (20)       13 2024-05-13 17:00:57.000000 py2saber-0.15.3/py2saber.egg-info/top_level.txt
+-rw-r--r--   0 jramboz    (501) staff       (20)    30549 2024-05-13 16:59:40.000000 py2saber-0.15.3/py2saber.py
+-rw-r--r--   0 jramboz    (501) staff       (20)      793 2024-05-13 16:59:40.000000 py2saber-0.15.3/pyproject.toml
+-rw-r--r--   0 jramboz    (501) staff       (20)       38 2024-05-13 17:00:57.644890 py2saber-0.15.3/setup.cfg
```

### Comparing `py2saber-0.15.2/COPYING` & `py2saber-0.15.3/COPYING`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.2/PKG-INFO` & `py2saber-0.15.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py2saber
-Version: 0.15.2
+Version: 0.15.3
 Summary: Python-based utility for OpenCore lightsabers
 Author-email: Jason Ramboz <jramboz@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `py2saber-0.15.2/README.md` & `py2saber-0.15.3/README.md`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.2/py2saber.egg-info/PKG-INFO` & `py2saber-0.15.3/py2saber.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py2saber
-Version: 0.15.2
+Version: 0.15.3
 Summary: Python-based utility for OpenCore lightsabers
 Author-email: Jason Ramboz <jramboz@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `py2saber-0.15.2/py2saber.py` & `py2saber-0.15.3/py2saber.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 import errno
 from getch import pause_exit
 import glob
 import time
 
 basedir = os.path.dirname(os.path.realpath(__file__))
 
-script_version = '0.15.2'
+script_version = '0.15.3'
 script_authors = 'Jason Ramboz'
 script_repo = 'https://github.com/jramboz/py2saber'
 
 # adapted from https://stackoverflow.com/a/66491013
 class DocDefaultException(Exception):
     """Subclass exceptions use docstring as default message"""
     def __init__(self, msg=None, *args, **kwargs):
```

### Comparing `py2saber-0.15.2/pyproject.toml` & `py2saber-0.15.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "py2saber"
-version = "0.15.2"
+version = "0.15.3"
 description = "Python-based utility for OpenCore lightsabers"
 readme = "README.md"
 authors = [{name = "Jason Ramboz", email = "jramboz@gmail.com"}]
 license = {file = "COPYING"}
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python",
```

