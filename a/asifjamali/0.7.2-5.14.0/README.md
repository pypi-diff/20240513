# Comparing `tmp/asifjamali-0.7.2.tar.gz` & `tmp/asifjamali-5.14.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asifjamali-0.7.2.tar", last modified: Sun Apr  7 00:04:39 2024, max compression
+gzip compressed data, was "asifjamali-5.14.0.tar", last modified: Mon May 13 19:27:49 2024, max compression
```

## Comparing `asifjamali-0.7.2.tar` & `asifjamali-5.14.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 00:04:39.033252 asifjamali-0.7.2/
--rw-r--r--   0 root         (0) root         (0)     1056 2024-03-14 18:59:11.000000 asifjamali-0.7.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1475 2024-04-07 00:04:39.033252 asifjamali-0.7.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1105 2024-03-14 18:59:11.000000 asifjamali-0.7.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 00:04:39.033252 asifjamali-0.7.2/asifjamali/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-14 19:00:15.000000 asifjamali-0.7.2/asifjamali/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21296 2024-04-07 00:03:25.000000 asifjamali-0.7.2/asifjamali/musibat.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 00:04:39.033252 asifjamali-0.7.2/asifjamali.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1475 2024-04-07 00:04:39.000000 asifjamali-0.7.2/asifjamali.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      240 2024-04-07 00:04:39.000000 asifjamali-0.7.2/asifjamali.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-07 00:04:39.000000 asifjamali-0.7.2/asifjamali.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-04-07 00:04:39.000000 asifjamali-0.7.2/asifjamali.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-04-07 00:04:39.000000 asifjamali-0.7.2/asifjamali.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-07 00:04:39.033252 asifjamali-0.7.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      640 2024-04-07 00:02:56.000000 asifjamali-0.7.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 19:27:49.843946 asifjamali-5.14.0/
+-rw-r--r--   0 root         (0) root         (0)     1056 2024-03-14 23:59:10.000000 asifjamali-5.14.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1476 2024-05-13 19:27:49.843946 asifjamali-5.14.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1105 2024-03-14 23:59:10.000000 asifjamali-5.14.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 19:27:49.843946 asifjamali-5.14.0/asifjamali/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-03-15 00:00:14.000000 asifjamali-5.14.0/asifjamali/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21304 2024-05-14 00:17:38.000000 asifjamali-5.14.0/asifjamali/musibat.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 19:27:49.843946 asifjamali-5.14.0/asifjamali.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1476 2024-05-13 19:27:49.000000 asifjamali-5.14.0/asifjamali.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      240 2024-05-13 19:27:49.000000 asifjamali-5.14.0/asifjamali.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-13 19:27:49.000000 asifjamali-5.14.0/asifjamali.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-13 19:27:49.000000 asifjamali-5.14.0/asifjamali.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-05-13 19:27:49.000000 asifjamali-5.14.0/asifjamali.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-13 19:27:49.843946 asifjamali-5.14.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      641 2024-05-14 00:13:16.000000 asifjamali-5.14.0/setup.py
```

### Comparing `asifjamali-0.7.2/LICENSE` & `asifjamali-5.14.0/LICENSE`

 * *Files identical despite different names*

### Comparing `asifjamali-0.7.2/PKG-INFO` & `asifjamali-5.14.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asifjamali
-Version: 0.7.2
+Version: 5.14.0
 Summary: Team Musibat Bots
 Home-page: https://bitbucket.org/shahzain83/musibat
 Author: Shahzain Khan
 Author-email: technomusibat@hotmail.com
 License: MIT
 Project-URL: Bug Tracker, https://bitbucket.org/shahzain83/musibat/issues
 Description-Content-Type: text/markdown
```

### Comparing `asifjamali-0.7.2/README.md` & `asifjamali-5.14.0/README.md`

 * *Files identical despite different names*

### Comparing `asifjamali-0.7.2/asifjamali/musibat.py` & `asifjamali-5.14.0/asifjamali/musibat.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1 +1 @@
-import os, re, sys, time, json, socket, random, codecs, requests, subprocess
+import os, re, sys, time, json, socket, random, codecs, requests, subprocess
```

### Comparing `asifjamali-0.7.2/asifjamali.egg-info/PKG-INFO` & `asifjamali-5.14.0/asifjamali.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asifjamali
-Version: 0.7.2
+Version: 5.14.0
 Summary: Team Musibat Bots
 Home-page: https://bitbucket.org/shahzain83/musibat
 Author: Shahzain Khan
 Author-email: technomusibat@hotmail.com
 License: MIT
 Project-URL: Bug Tracker, https://bitbucket.org/shahzain83/musibat/issues
 Description-Content-Type: text/markdown
```
