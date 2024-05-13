# Comparing `tmp/py2saber-0.14.1.tar.gz` & `tmp/py2saber-0.15.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py2saber-0.14.1.tar", last modified: Tue May  7 00:15:50 2024, max compression
+gzip compressed data, was "py2saber-0.15.1.tar", last modified: Mon May 13 15:51:30 2024, max compression
```

## Comparing `py2saber-0.14.1.tar` & `py2saber-0.15.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 jramboz    (501) staff       (20)        0 2024-05-07 00:15:50.374795 py2saber-0.14.1/
--rw-r--r--   0 jramboz    (501) staff       (20)    35149 2023-05-23 13:52:35.000000 py2saber-0.14.1/COPYING
--rw-r--r--   0 jramboz    (501) staff       (20)    43211 2024-05-07 00:15:50.374598 py2saber-0.14.1/PKG-INFO
--rw-r--r--   0 jramboz    (501) staff       (20)     2047 2024-03-20 16:03:37.000000 py2saber-0.14.1/README.md
-drwxr-xr-x   0 jramboz    (501) staff       (20)        0 2024-05-07 00:15:50.374327 py2saber-0.14.1/py2saber.egg-info/
--rw-r--r--   0 jramboz    (501) staff       (20)    43211 2024-05-07 00:15:50.000000 py2saber-0.14.1/py2saber.egg-info/PKG-INFO
--rw-r--r--   0 jramboz    (501) staff       (20)      238 2024-05-07 00:15:50.000000 py2saber-0.14.1/py2saber.egg-info/SOURCES.txt
--rw-r--r--   0 jramboz    (501) staff       (20)        1 2024-05-07 00:15:50.000000 py2saber-0.14.1/py2saber.egg-info/dependency_links.txt
--rw-r--r--   0 jramboz    (501) staff       (20)       48 2024-05-07 00:15:50.000000 py2saber-0.14.1/py2saber.egg-info/entry_points.txt
--rw-r--r--   0 jramboz    (501) staff       (20)       23 2024-05-07 00:15:50.000000 py2saber-0.14.1/py2saber.egg-info/requires.txt
--rw-r--r--   0 jramboz    (501) staff       (20)        9 2024-05-07 00:15:50.000000 py2saber-0.14.1/py2saber.egg-info/top_level.txt
--rw-r--r--   0 jramboz    (501) staff       (20)    29657 2024-05-07 00:13:53.000000 py2saber-0.14.1/py2saber.py
--rw-r--r--   0 jramboz    (501) staff       (20)      793 2024-05-06 22:14:03.000000 py2saber-0.14.1/pyproject.toml
--rw-r--r--   0 jramboz    (501) staff       (20)       38 2024-05-07 00:15:50.374830 py2saber-0.14.1/setup.cfg
+drwxr-xr-x   0 jramboz    (501) staff       (20)        0 2024-05-13 15:51:30.304156 py2saber-0.15.1/
+-rw-r--r--   0 jramboz    (501) staff       (20)    35149 2023-05-23 13:52:35.000000 py2saber-0.15.1/COPYING
+-rw-r--r--   0 jramboz    (501) staff       (20)    43211 2024-05-13 15:51:30.303940 py2saber-0.15.1/PKG-INFO
+-rw-r--r--   0 jramboz    (501) staff       (20)     2047 2024-03-20 16:03:37.000000 py2saber-0.15.1/README.md
+drwxr-xr-x   0 jramboz    (501) staff       (20)        0 2024-05-13 15:51:30.303634 py2saber-0.15.1/py2saber.egg-info/
+-rw-r--r--   0 jramboz    (501) staff       (20)    43211 2024-05-13 15:51:30.000000 py2saber-0.15.1/py2saber.egg-info/PKG-INFO
+-rw-r--r--   0 jramboz    (501) staff       (20)      238 2024-05-13 15:51:30.000000 py2saber-0.15.1/py2saber.egg-info/SOURCES.txt
+-rw-r--r--   0 jramboz    (501) staff       (20)        1 2024-05-13 15:51:30.000000 py2saber-0.15.1/py2saber.egg-info/dependency_links.txt
+-rw-r--r--   0 jramboz    (501) staff       (20)       48 2024-05-13 15:51:30.000000 py2saber-0.15.1/py2saber.egg-info/entry_points.txt
+-rw-r--r--   0 jramboz    (501) staff       (20)       23 2024-05-13 15:51:30.000000 py2saber-0.15.1/py2saber.egg-info/requires.txt
+-rw-r--r--   0 jramboz    (501) staff       (20)       13 2024-05-13 15:51:30.000000 py2saber-0.15.1/py2saber.egg-info/top_level.txt
+-rw-r--r--   0 jramboz    (501) staff       (20)    30496 2024-05-13 15:40:45.000000 py2saber-0.15.1/py2saber.py
+-rw-r--r--   0 jramboz    (501) staff       (20)      793 2024-05-13 15:40:12.000000 py2saber-0.15.1/pyproject.toml
+-rw-r--r--   0 jramboz    (501) staff       (20)       38 2024-05-13 15:51:30.304208 py2saber-0.15.1/setup.cfg
```

### Comparing `py2saber-0.14.1/COPYING` & `py2saber-0.15.1/COPYING`

 * *Files identical despite different names*

### Comparing `py2saber-0.14.1/PKG-INFO` & `py2saber-0.15.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py2saber
-Version: 0.14.1
+Version: 0.15.1
 Summary: Python-based utility for OpenCore lightsabers
 Author-email: Jason Ramboz <jramboz@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `py2saber-0.14.1/README.md` & `py2saber-0.15.1/README.md`

 * *Files identical despite different names*

### Comparing `py2saber-0.14.1/py2saber.egg-info/PKG-INFO` & `py2saber-0.15.1/py2saber.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py2saber
-Version: 0.14.1
+Version: 0.15.1
 Summary: Python-based utility for OpenCore lightsabers
 Author-email: Jason Ramboz <jramboz@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `py2saber-0.14.1/py2saber.py` & `py2saber-0.15.1/py2saber.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,17 @@
 import sys
 import argparse
 import errno
 from getch import pause_exit
 import glob
 import time
 
-script_version = '0.14.1'
+basedir = os.path.dirname(os.path.realpath(__file__))
+
+script_version = '0.15.1'
 script_authors = 'Jason Ramboz'
 script_repo = 'https://github.com/jramboz/py2saber'
 
 # adapted from https://stackoverflow.com/a/66491013
 class DocDefaultException(Exception):
     """Subclass exceptions use docstring as default message"""
     def __init__(self, msg=None, *args, **kwargs):
@@ -376,19 +378,34 @@
             # read one byte at a time, since last line isn't terminated with \n
             config += self._ser.read()
 
         self.log.debug(f'Raw config string: {config}')
         # slice off first and last char ('2' and '3')
         return config.decode().strip()[1:-1]
 
-    def write_files_to_saber(self, files: list[str], progress_callback: callable = None) -> None:
+    def anima_is_NXT(self) -> bool:
+        '''Returns True if the attached saber is an NXT, False if not.'''
+        info = self.get_saber_info()
+        if info['version'][:4] == 'NXT_':
+            return True
+        return False
+
+    def write_files_to_saber(self, files: list[str], progress_callback: callable = None, add_beep: bool = True) -> None:
         '''Write file(s) to saber. Expects a list of file names.
+        
+        If add_beep is True (default), this method will automatically add the defauly BEEP.RAW for NXT sabers if no other BEEP.RAW is supplied or already on saber.
 
         NB: This method does no checking that files exist either on disk or saber. Please verify files before calling this method.'''
         files.sort()
+
+        current_files = self.list_files_on_saber()
+        if self.anima_is_NXT() and not any("BEEP.RAW" in file for file in files) and 'BEEP.RAW' not in current_files.keys():
+            self.log.info('NXT saber detected and no BEEP.RAW provided. Adding default BEEP.RAW.')
+            files.append(os.path.join(basedir, 'OpenCore_OEM', 'BEEP.RAW'))
+
         self.log.info(f'Preparing to write file(s) to saber: {files}')
         for file in files:
             self.log.info(f'Writing file to saber: {file}')
             
             # Check for enough free space
             file_size = os.path.getsize(file)
             self.log.debug(f'File size: {file_size}')
```

### Comparing `py2saber-0.14.1/pyproject.toml` & `py2saber-0.15.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "py2saber"
-version = "0.14.1"
+version = "0.15.1"
 description = "Python-based utility for OpenCore lightsabers"
 readme = "README.md"
 authors = [{name = "Jason Ramboz", email = "jramboz@gmail.com"}]
 license = {file = "COPYING"}
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python",
```

