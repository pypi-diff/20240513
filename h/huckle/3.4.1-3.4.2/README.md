# Comparing `tmp/huckle-3.4.1.tar.gz` & `tmp/huckle-3.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huckle-3.4.1.tar", last modified: Fri Apr 26 03:27:21 2024, max compression
+gzip compressed data, was "huckle-3.4.2.tar", last modified: Mon May 13 20:32:17 2024, max compression
```

## Comparing `huckle-3.4.1.tar` & `huckle-3.4.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2024-04-26 03:27:21.959309 huckle-3.4.1/
--rwxr-x---   0 jeff       (501) staff       (20)     1056 2022-03-20 22:23:06.000000 huckle-3.4.1/LICENSE.txt
--rwxr-x---   0 jeff       (501) staff       (20)       90 2022-03-20 22:23:06.000000 huckle-3.4.1/MANIFEST.in
--rw-r--r--   0 jeff       (501) staff       (20)    10753 2024-04-26 03:27:21.959406 huckle-3.4.1/PKG-INFO
--rw-r--r--   0 jeff       (501) staff       (20)     9885 2024-04-26 02:48:09.000000 huckle-3.4.1/README.rst
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2024-04-26 03:27:21.958359 huckle-3.4.1/huckle/
--rwxr-x---   0 jeff       (501) staff       (20)      463 2024-04-26 03:22:34.000000 huckle-3.4.1/huckle/__init__.py
--rw-r--r--   0 jeff       (501) staff       (20)      885 2024-04-07 23:22:42.000000 huckle-3.4.1/huckle/__main__.py
--rwxr-xr-x   0 jeff       (501) staff       (20)     6054 2024-04-07 23:05:17.000000 huckle-3.4.1/huckle/config.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2024-04-26 03:27:21.959205 huckle-3.4.1/huckle/data/
--rw-r--r--   0 jeff       (501) staff       (20)     3481 2024-04-07 23:05:17.000000 huckle-3.4.1/huckle/data/huckle.1
--rwxr-xr-x   0 jeff       (501) staff       (20)    11484 2024-04-07 23:26:21.000000 huckle-3.4.1/huckle/hclinav.py
--rwxr-xr-x   0 jeff       (501) staff       (20)     4290 2024-04-26 03:07:06.000000 huckle-3.4.1/huckle/huckle.py
--rwxr-xr-x   0 jeff       (501) staff       (20)      850 2024-04-07 23:05:17.000000 huckle-3.4.1/huckle/hutils.py
--rwxr-xr-x   0 jeff       (501) staff       (20)     2955 2023-08-17 01:36:09.000000 huckle-3.4.1/huckle/logger.py
--rwxr-xr-x   0 jeff       (501) staff       (20)      248 2024-04-26 03:27:13.000000 huckle-3.4.1/huckle/package.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2024-04-26 03:27:21.959090 huckle-3.4.1/huckle.egg-info/
--rw-r--r--   0 jeff       (501) staff       (20)    10753 2024-04-26 03:27:21.000000 huckle-3.4.1/huckle.egg-info/PKG-INFO
--rw-r--r--   0 jeff       (501) staff       (20)      398 2024-04-26 03:27:21.000000 huckle-3.4.1/huckle.egg-info/SOURCES.txt
--rw-r--r--   0 jeff       (501) staff       (20)        1 2024-04-26 03:27:21.000000 huckle-3.4.1/huckle.egg-info/dependency_links.txt
--rw-r--r--   0 jeff       (501) staff       (20)       48 2024-04-26 03:27:21.000000 huckle-3.4.1/huckle.egg-info/entry_points.txt
--rw-r--r--   0 jeff       (501) staff       (20)       84 2024-04-26 03:27:21.000000 huckle-3.4.1/huckle.egg-info/requires.txt
--rw-r--r--   0 jeff       (501) staff       (20)        7 2024-04-26 03:27:21.000000 huckle-3.4.1/huckle.egg-info/top_level.txt
--rwxr-x---   0 jeff       (501) staff       (20)       67 2024-04-26 03:27:21.959674 huckle-3.4.1/setup.cfg
--rw-r--r--   0 jeff       (501) staff       (20)     3335 2024-04-07 23:05:17.000000 huckle-3.4.1/setup.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2024-05-13 20:32:17.743512 huckle-3.4.2/
+-rwxr-x---   0 jeff       (501) staff       (20)     1056 2022-03-20 22:23:06.000000 huckle-3.4.2/LICENSE.txt
+-rwxr-x---   0 jeff       (501) staff       (20)       90 2022-03-20 22:23:06.000000 huckle-3.4.2/MANIFEST.in
+-rw-r--r--   0 jeff       (501) staff       (20)    10753 2024-05-13 20:32:17.743587 huckle-3.4.2/PKG-INFO
+-rwxr-x---   0 jeff       (501) staff       (20)     9885 2024-04-26 02:48:09.000000 huckle-3.4.2/README.rst
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2024-05-13 20:32:17.742563 huckle-3.4.2/huckle/
+-rwxr-x---   0 jeff       (501) staff       (20)      463 2024-04-26 03:22:34.000000 huckle-3.4.2/huckle/__init__.py
+-rw-r--r--   0 jeff       (501) staff       (20)      885 2024-05-13 20:20:54.000000 huckle-3.4.2/huckle/__main__.py
+-rwxr-xr-x   0 jeff       (501) staff       (20)     6054 2024-04-07 23:05:17.000000 huckle-3.4.2/huckle/config.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2024-05-13 20:32:17.743409 huckle-3.4.2/huckle/data/
+-rw-r--r--   0 jeff       (501) staff       (20)     3481 2024-04-07 23:05:17.000000 huckle-3.4.2/huckle/data/huckle.1
+-rwxr-xr-x   0 jeff       (501) staff       (20)    11484 2024-04-07 23:26:21.000000 huckle-3.4.2/huckle/hclinav.py
+-rwxr-xr-x   0 jeff       (501) staff       (20)     4290 2024-04-29 23:51:42.000000 huckle-3.4.2/huckle/huckle.py
+-rwxr-xr-x   0 jeff       (501) staff       (20)      850 2024-04-07 23:05:17.000000 huckle-3.4.2/huckle/hutils.py
+-rwxr-xr-x   0 jeff       (501) staff       (20)     2955 2024-05-13 20:21:40.000000 huckle-3.4.2/huckle/logger.py
+-rwxr-xr-x   0 jeff       (501) staff       (20)      248 2024-05-13 20:31:17.000000 huckle-3.4.2/huckle/package.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2024-05-13 20:32:17.743286 huckle-3.4.2/huckle.egg-info/
+-rw-r--r--   0 jeff       (501) staff       (20)    10753 2024-05-13 20:32:17.000000 huckle-3.4.2/huckle.egg-info/PKG-INFO
+-rw-r--r--   0 jeff       (501) staff       (20)      398 2024-05-13 20:32:17.000000 huckle-3.4.2/huckle.egg-info/SOURCES.txt
+-rw-r--r--   0 jeff       (501) staff       (20)        1 2024-05-13 20:32:17.000000 huckle-3.4.2/huckle.egg-info/dependency_links.txt
+-rw-r--r--   0 jeff       (501) staff       (20)       48 2024-05-13 20:32:17.000000 huckle-3.4.2/huckle.egg-info/entry_points.txt
+-rw-r--r--   0 jeff       (501) staff       (20)       84 2024-05-13 20:32:17.000000 huckle-3.4.2/huckle.egg-info/requires.txt
+-rw-r--r--   0 jeff       (501) staff       (20)        7 2024-05-13 20:32:17.000000 huckle-3.4.2/huckle.egg-info/top_level.txt
+-rwxr-x---   0 jeff       (501) staff       (20)       67 2024-05-13 20:32:17.743802 huckle-3.4.2/setup.cfg
+-rwxr-x---   0 jeff       (501) staff       (20)     3335 2024-04-07 23:05:17.000000 huckle-3.4.2/setup.py
```

### Comparing `huckle-3.4.1/LICENSE.txt` & `huckle-3.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `huckle-3.4.1/PKG-INFO` & `huckle-3.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: huckle
-Version: 3.4.1
+Version: 3.4.2
 Summary: A CLI, and python library, that can act as an impostor for any CLI expressed through hypertext command line interface (HCLI) semantics.
 Home-page: https://github.com/cometaj2/huckle
 Author: Jeff Michaud
 Author-email: cometaj2@comcast.net
 License: MIT
 Keywords: cli client hypermedia rest generic development
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `huckle-3.4.1/README.rst` & `huckle-3.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `huckle-3.4.1/huckle/__main__.py` & `huckle-3.4.2/huckle/__main__.py`

 * *Files identical despite different names*

### Comparing `huckle-3.4.1/huckle/config.py` & `huckle-3.4.2/huckle/config.py`

 * *Files identical despite different names*

### Comparing `huckle-3.4.1/huckle/data/huckle.1` & `huckle-3.4.2/huckle/data/huckle.1`

 * *Files identical despite different names*

### Comparing `huckle-3.4.1/huckle/hclinav.py` & `huckle-3.4.2/huckle/hclinav.py`

 * *Files identical despite different names*

### Comparing `huckle-3.4.1/huckle/huckle.py` & `huckle-3.4.2/huckle/huckle.py`

 * *Files identical despite different names*

### Comparing `huckle-3.4.1/huckle/hutils.py` & `huckle-3.4.2/huckle/hutils.py`

 * *Files identical despite different names*

### Comparing `huckle-3.4.1/huckle/logger.py` & `huckle-3.4.2/huckle/logger.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,15 +41,15 @@
             if self.instance is None:
                 self.instance = super().__new__(self, *args, **kwargs)
             return self.instance
 
     def __init__(self, *args, **kwargs):
         with self.lock:
             if not self.initialized:
-                self.instance = logging.getLogger("crumbs")
+                self.instance = logging.getLogger("huckle")
 
                 date_format = "%Y-%m-%d %H:%M:%S %z"
                 message_format = "[%(asctime)s] [%(levelname)-5s] [%(filename)13s:%(lineno)-3s] %(message)s"
 
                 formatter = logging.Formatter(fmt=message_format, datefmt=date_format)
 
                 self.streamHandler = logging.StreamHandler()
@@ -59,15 +59,15 @@
                 self.clientHandler = DequeHandler()
                 self.clientHandler.setFormatter(formatter)
                 self.instance.addHandler(self.clientHandler)
 
                 self.initialized = True
 
     def setLevel(self, level):
-        logging.getLogger("crumbs").setLevel(level)
+        logging.getLogger("huckle").setLevel(level)
         return
 
     def info(self, msg, *args, **kwargs):
         self.instance.info(msg, *args, stacklevel=2, **kwargs)
 
     def debug(self, msg, *args, **kwargs):
         self.instance.debug(msg, *args, stacklevel=2, **kwargs)
```

### Comparing `huckle-3.4.1/huckle.egg-info/PKG-INFO` & `huckle-3.4.2/huckle.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: huckle
-Version: 3.4.1
+Version: 3.4.2
 Summary: A CLI, and python library, that can act as an impostor for any CLI expressed through hypertext command line interface (HCLI) semantics.
 Home-page: https://github.com/cometaj2/huckle
 Author: Jeff Michaud
 Author-email: cometaj2@comcast.net
 License: MIT
 Keywords: cli client hypermedia rest generic development
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `huckle-3.4.1/setup.py` & `huckle-3.4.2/setup.py`

 * *Files identical despite different names*

