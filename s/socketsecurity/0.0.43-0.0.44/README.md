# Comparing `tmp/socketsecurity-0.0.43.tar.gz` & `tmp/socketsecurity-0.0.44.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socketsecurity-0.0.43.tar", last modified: Mon May 13 20:25:45 2024, max compression
+gzip compressed data, was "socketsecurity-0.0.44.tar", last modified: Mon May 13 20:32:39 2024, max compression
```

## Comparing `socketsecurity-0.0.43.tar` & `socketsecurity-0.0.44.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-13 20:25:45.626503 socketsecurity-0.0.43/
--rw-r--r--   0 douglascoburn   (501) staff       (20)      141 2024-05-13 20:25:45.626288 socketsecurity-0.0.43/PKG-INFO
-drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-13 20:25:45.625260 socketsecurity-0.0.43/core/
--rw-r--r--   0 douglascoburn   (501) staff       (20)    25969 2024-05-08 17:09:44.000000 socketsecurity-0.0.43/core/__init__.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)     8665 2024-05-07 20:28:21.000000 socketsecurity-0.0.43/core/classes.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)      626 2024-04-29 13:52:20.000000 socketsecurity-0.0.43/core/exceptions.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)    11251 2024-05-08 17:15:58.000000 socketsecurity-0.0.43/core/github.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)    11208 2024-05-05 18:30:58.000000 socketsecurity-0.0.43/core/glitlab.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)    67547 2024-05-05 17:36:53.000000 socketsecurity-0.0.43/core/issues.py
--rw-r--r--   0 douglascoburn   (501) staff       (20) 17442610 2024-05-06 19:45:31.000000 socketsecurity-0.0.43/core/licenses.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)    11834 2024-05-08 17:02:42.000000 socketsecurity-0.0.43/core/messages.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)       38 2024-05-13 20:25:45.626541 socketsecurity-0.0.43/setup.cfg
--rw-r--r--   0 douglascoburn   (501) staff       (20)      330 2024-05-13 20:24:12.000000 socketsecurity-0.0.43/setup.py
-drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-13 20:25:45.626082 socketsecurity-0.0.43/socketsecurity.egg-info/
--rw-r--r--   0 douglascoburn   (501) staff       (20)      141 2024-05-13 20:25:45.000000 socketsecurity-0.0.43/socketsecurity.egg-info/PKG-INFO
--rw-r--r--   0 douglascoburn   (501) staff       (20)      370 2024-05-13 20:25:45.000000 socketsecurity-0.0.43/socketsecurity.egg-info/SOURCES.txt
--rw-r--r--   0 douglascoburn   (501) staff       (20)        1 2024-05-13 20:25:45.000000 socketsecurity-0.0.43/socketsecurity.egg-info/dependency_links.txt
--rw-r--r--   0 douglascoburn   (501) staff       (20)       60 2024-05-13 20:25:45.000000 socketsecurity-0.0.43/socketsecurity.egg-info/entry_points.txt
--rw-r--r--   0 douglascoburn   (501) staff       (20)       37 2024-05-13 20:25:45.000000 socketsecurity-0.0.43/socketsecurity.egg-info/requires.txt
--rw-r--r--   0 douglascoburn   (501) staff       (20)        5 2024-05-13 20:25:45.000000 socketsecurity-0.0.43/socketsecurity.egg-info/top_level.txt
+drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-13 20:32:39.507270 socketsecurity-0.0.44/
+-rw-r--r--   0 douglascoburn   (501) staff       (20)      141 2024-05-13 20:32:39.507070 socketsecurity-0.0.44/PKG-INFO
+-rw-r--r--   0 douglascoburn   (501) staff       (20)       38 2024-05-13 20:32:39.507311 socketsecurity-0.0.44/setup.cfg
+-rw-r--r--   0 douglascoburn   (501) staff       (20)      330 2024-05-13 20:28:07.000000 socketsecurity-0.0.44/setup.py
+drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-13 20:32:39.491146 socketsecurity-0.0.44/socketsecurity/
+-rw-r--r--   0 douglascoburn   (501) staff       (20)       48 2024-05-13 20:30:22.000000 socketsecurity-0.0.44/socketsecurity/__init__.py
+drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-13 20:32:39.506560 socketsecurity-0.0.44/socketsecurity/core/
+-rw-r--r--   0 douglascoburn   (501) staff       (20)    25969 2024-05-13 20:28:07.000000 socketsecurity-0.0.44/socketsecurity/core/__init__.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)     8665 2024-05-07 20:28:21.000000 socketsecurity-0.0.44/socketsecurity/core/classes.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)      626 2024-04-29 13:52:20.000000 socketsecurity-0.0.44/socketsecurity/core/exceptions.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)    11251 2024-05-08 17:15:58.000000 socketsecurity-0.0.44/socketsecurity/core/github.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)    11208 2024-05-05 18:30:58.000000 socketsecurity-0.0.44/socketsecurity/core/glitlab.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)    67547 2024-05-05 17:36:53.000000 socketsecurity-0.0.44/socketsecurity/core/issues.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20) 17442610 2024-05-06 19:45:31.000000 socketsecurity-0.0.44/socketsecurity/core/licenses.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)    11834 2024-05-08 17:02:42.000000 socketsecurity-0.0.44/socketsecurity/core/messages.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)     5434 2024-05-07 20:55:48.000000 socketsecurity-0.0.44/socketsecurity/socketcli.py
+drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-13 20:32:39.506832 socketsecurity-0.0.44/socketsecurity.egg-info/
+-rw-r--r--   0 douglascoburn   (501) staff       (20)      141 2024-05-13 20:32:39.000000 socketsecurity-0.0.44/socketsecurity.egg-info/PKG-INFO
+-rw-r--r--   0 douglascoburn   (501) staff       (20)      545 2024-05-13 20:32:39.000000 socketsecurity-0.0.44/socketsecurity.egg-info/SOURCES.txt
+-rw-r--r--   0 douglascoburn   (501) staff       (20)        1 2024-05-13 20:32:39.000000 socketsecurity-0.0.44/socketsecurity.egg-info/dependency_links.txt
+-rw-r--r--   0 douglascoburn   (501) staff       (20)       60 2024-05-13 20:32:39.000000 socketsecurity-0.0.44/socketsecurity.egg-info/entry_points.txt
+-rw-r--r--   0 douglascoburn   (501) staff       (20)       37 2024-05-13 20:32:39.000000 socketsecurity-0.0.44/socketsecurity.egg-info/requires.txt
+-rw-r--r--   0 douglascoburn   (501) staff       (20)       15 2024-05-13 20:32:39.000000 socketsecurity-0.0.44/socketsecurity.egg-info/top_level.txt
```

### Comparing `socketsecurity-0.0.43/core/__init__.py` & `socketsecurity-0.0.44/socketsecurity/core/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 )
 import platform
 from glob import glob
 import time
 
 
 __author__ = 'socket.dev'
-__version__ = '0.0.38'
+__version__ = '0.0.44'
 __all__ = [
     "Core",
     "log"
 ]
 
 
 global encoded_key
```

### Comparing `socketsecurity-0.0.43/core/classes.py` & `socketsecurity-0.0.44/socketsecurity/core/classes.py`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.43/core/exceptions.py` & `socketsecurity-0.0.44/socketsecurity/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.43/core/github.py` & `socketsecurity-0.0.44/socketsecurity/core/github.py`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.43/core/glitlab.py` & `socketsecurity-0.0.44/socketsecurity/core/glitlab.py`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.43/core/issues.py` & `socketsecurity-0.0.44/socketsecurity/core/issues.py`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.43/core/licenses.py` & `socketsecurity-0.0.44/socketsecurity/core/licenses.py`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.43/core/messages.py` & `socketsecurity-0.0.44/socketsecurity/core/messages.py`

 * *Files identical despite different names*

