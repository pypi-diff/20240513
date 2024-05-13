# Comparing `tmp/py2saber-0.15.1.tar.gz` & `tmp/py2saber-0.15.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py2saber-0.15.1.tar", last modified: Mon May 13 15:51:30 2024, max compression
+gzip compressed data, was "py2saber-0.15.2.tar", last modified: Mon May 13 16:22:44 2024, max compression
```

## Comparing `py2saber-0.15.1.tar` & `py2saber-0.15.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 jramboz    (501) staff       (20)        0 2024-05-13 15:51:30.304156 py2saber-0.15.1/
--rw-r--r--   0 jramboz    (501) staff       (20)    35149 2023-05-23 13:52:35.000000 py2saber-0.15.1/COPYING
--rw-r--r--   0 jramboz    (501) staff       (20)    43211 2024-05-13 15:51:30.303940 py2saber-0.15.1/PKG-INFO
--rw-r--r--   0 jramboz    (501) staff       (20)     2047 2024-03-20 16:03:37.000000 py2saber-0.15.1/README.md
-drwxr-xr-x   0 jramboz    (501) staff       (20)        0 2024-05-13 15:51:30.303634 py2saber-0.15.1/py2saber.egg-info/
--rw-r--r--   0 jramboz    (501) staff       (20)    43211 2024-05-13 15:51:30.000000 py2saber-0.15.1/py2saber.egg-info/PKG-INFO
--rw-r--r--   0 jramboz    (501) staff       (20)      238 2024-05-13 15:51:30.000000 py2saber-0.15.1/py2saber.egg-info/SOURCES.txt
--rw-r--r--   0 jramboz    (501) staff       (20)        1 2024-05-13 15:51:30.000000 py2saber-0.15.1/py2saber.egg-info/dependency_links.txt
--rw-r--r--   0 jramboz    (501) staff       (20)       48 2024-05-13 15:51:30.000000 py2saber-0.15.1/py2saber.egg-info/entry_points.txt
--rw-r--r--   0 jramboz    (501) staff       (20)       23 2024-05-13 15:51:30.000000 py2saber-0.15.1/py2saber.egg-info/requires.txt
--rw-r--r--   0 jramboz    (501) staff       (20)       13 2024-05-13 15:51:30.000000 py2saber-0.15.1/py2saber.egg-info/top_level.txt
--rw-r--r--   0 jramboz    (501) staff       (20)    30496 2024-05-13 15:40:45.000000 py2saber-0.15.1/py2saber.py
--rw-r--r--   0 jramboz    (501) staff       (20)      793 2024-05-13 15:40:12.000000 py2saber-0.15.1/pyproject.toml
--rw-r--r--   0 jramboz    (501) staff       (20)       38 2024-05-13 15:51:30.304208 py2saber-0.15.1/setup.cfg
+drwxr-xr-x   0 jramboz    (501) staff       (20)        0 2024-05-13 16:22:44.120959 py2saber-0.15.2/
+-rw-r--r--   0 jramboz    (501) staff       (20)    35149 2023-05-23 13:52:35.000000 py2saber-0.15.2/COPYING
+-rw-r--r--   0 jramboz    (501) staff       (20)    43211 2024-05-13 16:22:44.120777 py2saber-0.15.2/PKG-INFO
+-rw-r--r--   0 jramboz    (501) staff       (20)     2047 2024-03-20 16:03:37.000000 py2saber-0.15.2/README.md
+drwxr-xr-x   0 jramboz    (501) staff       (20)        0 2024-05-13 16:22:44.120533 py2saber-0.15.2/py2saber.egg-info/
+-rw-r--r--   0 jramboz    (501) staff       (20)    43211 2024-05-13 16:22:44.000000 py2saber-0.15.2/py2saber.egg-info/PKG-INFO
+-rw-r--r--   0 jramboz    (501) staff       (20)      238 2024-05-13 16:22:44.000000 py2saber-0.15.2/py2saber.egg-info/SOURCES.txt
+-rw-r--r--   0 jramboz    (501) staff       (20)        1 2024-05-13 16:22:44.000000 py2saber-0.15.2/py2saber.egg-info/dependency_links.txt
+-rw-r--r--   0 jramboz    (501) staff       (20)       48 2024-05-13 16:22:44.000000 py2saber-0.15.2/py2saber.egg-info/entry_points.txt
+-rw-r--r--   0 jramboz    (501) staff       (20)       23 2024-05-13 16:22:44.000000 py2saber-0.15.2/py2saber.egg-info/requires.txt
+-rw-r--r--   0 jramboz    (501) staff       (20)       13 2024-05-13 16:22:44.000000 py2saber-0.15.2/py2saber.egg-info/top_level.txt
+-rw-r--r--   0 jramboz    (501) staff       (20)    30549 2024-05-13 16:16:24.000000 py2saber-0.15.2/py2saber.py
+-rw-r--r--   0 jramboz    (501) staff       (20)      793 2024-05-13 16:16:24.000000 py2saber-0.15.2/pyproject.toml
+-rw-r--r--   0 jramboz    (501) staff       (20)       38 2024-05-13 16:22:44.120993 py2saber-0.15.2/setup.cfg
```

### Comparing `py2saber-0.15.1/COPYING` & `py2saber-0.15.2/COPYING`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.1/PKG-INFO` & `py2saber-0.15.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py2saber
-Version: 0.15.1
+Version: 0.15.2
 Summary: Python-based utility for OpenCore lightsabers
 Author-email: Jason Ramboz <jramboz@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `py2saber-0.15.1/README.md` & `py2saber-0.15.2/README.md`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.1/py2saber.egg-info/PKG-INFO` & `py2saber-0.15.2/py2saber.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py2saber
-Version: 0.15.1
+Version: 0.15.2
 Summary: Python-based utility for OpenCore lightsabers
 Author-email: Jason Ramboz <jramboz@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `py2saber-0.15.1/py2saber.py` & `py2saber-0.15.2/py2saber.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 import errno
 from getch import pause_exit
 import glob
 import time
 
 basedir = os.path.dirname(os.path.realpath(__file__))
 
-script_version = '0.15.1'
+script_version = '0.15.2'
 script_authors = 'Jason Ramboz'
 script_repo = 'https://github.com/jramboz/py2saber'
 
 # adapted from https://stackoverflow.com/a/66491013
 class DocDefaultException(Exception):
     """Subclass exceptions use docstring as default message"""
     def __init__(self, msg=None, *args, **kwargs):
@@ -326,14 +326,15 @@
                 print(c.decode(), end='', flush=True)
                 c = self._ser.read(1)
             # manually read the next line using the serial connection and combine it with the last char read.
             response = c + self._ser.readline()
             self.log.debug(f'Received response: {response}') # b'OK, Now re-load your sound files.\n'
             response = self.read_line() # b'OK, Serial Flash Erased.\n'
             response = self.read_line() # b'\n'
+            if self.gui: progress_callback.emit(100)
             self._ser.timeout = self._SERIAL_SETTINGS['timeout']
         else:
             raise AnimaNotReadyException
 
     def get_free_space(self) -> int:
         '''Returns the amount of free space in Anima storage in bytes.'''
         self.log.info('Getting free space on Anima.')
```

### Comparing `py2saber-0.15.1/pyproject.toml` & `py2saber-0.15.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "py2saber"
-version = "0.15.1"
+version = "0.15.2"
 description = "Python-based utility for OpenCore lightsabers"
 readme = "README.md"
 authors = [{name = "Jason Ramboz", email = "jramboz@gmail.com"}]
 license = {file = "COPYING"}
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python",
```

