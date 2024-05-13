# Comparing `tmp/datafog-3.2.0b2.tar.gz` & `tmp/datafog-3.2.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datafog-3.2.0b2.tar", last modified: Mon May 13 18:57:19 2024, max compression
+gzip compressed data, was "datafog-3.2.0b3.tar", last modified: Mon May 13 19:01:08 2024, max compression
```

## Comparing `datafog-3.2.0b2.tar` & `datafog-3.2.0b3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-13 18:57:19.153817 datafog-3.2.0b2/
--rw-r--r--   0 sidmohan   (501) staff       (20)     1091 2024-05-13 14:18:11.000000 datafog-3.2.0b2/LICENSE
--rw-r--r--   0 sidmohan   (501) staff       (20)     6510 2024-05-13 18:57:19.153695 datafog-3.2.0b2/PKG-INFO
--rw-r--r--   0 sidmohan   (501) staff       (20)     5289 2024-05-13 14:50:51.000000 datafog-3.2.0b2/README.md
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-13 18:57:19.152418 datafog-3.2.0b2/datafog/
--rw-r--r--   0 sidmohan   (501) staff       (20)       24 2024-05-13 18:56:44.000000 datafog-3.2.0b2/datafog/__about__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)      150 2024-05-13 18:39:10.000000 datafog-3.2.0b2/datafog/__init__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)      222 2024-05-13 18:39:10.000000 datafog-3.2.0b2/datafog/config.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     2969 2024-05-13 18:39:10.000000 datafog-3.2.0b2/datafog/main.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-13 18:57:19.153202 datafog-3.2.0b2/datafog.egg-info/
--rw-r--r--   0 sidmohan   (501) staff       (20)     6510 2024-05-13 18:57:19.000000 datafog-3.2.0b2/datafog.egg-info/PKG-INFO
--rw-r--r--   0 sidmohan   (501) staff       (20)      274 2024-05-13 18:57:19.000000 datafog-3.2.0b2/datafog.egg-info/SOURCES.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)        1 2024-05-13 18:57:19.000000 datafog-3.2.0b2/datafog.egg-info/dependency_links.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)      167 2024-05-13 18:57:19.000000 datafog-3.2.0b2/datafog.egg-info/requires.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)        8 2024-05-13 18:57:19.000000 datafog-3.2.0b2/datafog.egg-info/top_level.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)       38 2024-05-13 18:57:19.153864 datafog-3.2.0b2/setup.cfg
--rw-r--r--   0 sidmohan   (501) staff       (20)     1939 2024-05-13 18:57:03.000000 datafog-3.2.0b2/setup.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-13 18:57:19.153319 datafog-3.2.0b2/tests/
--rw-r--r--   0 sidmohan   (501) staff       (20)     2889 2024-05-13 18:39:10.000000 datafog-3.2.0b2/tests/test_main.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-13 19:01:08.425448 datafog-3.2.0b3/
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1091 2024-05-13 14:18:11.000000 datafog-3.2.0b3/LICENSE
+-rw-r--r--   0 sidmohan   (501) staff       (20)     6510 2024-05-13 19:01:08.425270 datafog-3.2.0b3/PKG-INFO
+-rw-r--r--   0 sidmohan   (501) staff       (20)     5289 2024-05-13 14:50:51.000000 datafog-3.2.0b3/README.md
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-13 19:01:08.423627 datafog-3.2.0b3/datafog/
+-rw-r--r--   0 sidmohan   (501) staff       (20)       24 2024-05-13 19:01:02.000000 datafog-3.2.0b3/datafog/__about__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)      604 2024-05-13 19:00:22.000000 datafog-3.2.0b3/datafog/__init__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)      222 2024-05-13 18:39:10.000000 datafog-3.2.0b3/datafog/config.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     2969 2024-05-13 18:39:10.000000 datafog-3.2.0b3/datafog/main.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-13 19:01:08.424671 datafog-3.2.0b3/datafog.egg-info/
+-rw-r--r--   0 sidmohan   (501) staff       (20)     6510 2024-05-13 19:01:08.000000 datafog-3.2.0b3/datafog.egg-info/PKG-INFO
+-rw-r--r--   0 sidmohan   (501) staff       (20)      274 2024-05-13 19:01:08.000000 datafog-3.2.0b3/datafog.egg-info/SOURCES.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)        1 2024-05-13 19:01:08.000000 datafog-3.2.0b3/datafog.egg-info/dependency_links.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)      167 2024-05-13 19:01:08.000000 datafog-3.2.0b3/datafog.egg-info/requires.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)        8 2024-05-13 19:01:08.000000 datafog-3.2.0b3/datafog.egg-info/top_level.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)       38 2024-05-13 19:01:08.425506 datafog-3.2.0b3/setup.cfg
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1939 2024-05-13 19:00:46.000000 datafog-3.2.0b3/setup.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-13 19:01:08.424806 datafog-3.2.0b3/tests/
+-rw-r--r--   0 sidmohan   (501) staff       (20)     2889 2024-05-13 18:39:10.000000 datafog-3.2.0b3/tests/test_main.py
```

### Comparing `datafog-3.2.0b2/LICENSE` & `datafog-3.2.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `datafog-3.2.0b2/PKG-INFO` & `datafog-3.2.0b3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datafog
-Version: 3.2.0b2
+Version: 3.2.0b3
 Summary: Scan, redact, and manage PII in your documents before they get uploaded to a Retrieval Augmented Generation (RAG) system.
 Home-page: https://datafog.ai
 Author: DataFog
 Author-email: hi@datafog.ai
 Maintainer: DataFog
 Maintainer-email: hi@datafog.ai
 License: MIT
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: datafog Version: 3.2.0b2 Summary: Scan, redact, and
+Metadata-Version: 2.1 Name: datafog Version: 3.2.0b3 Summary: Scan, redact, and
 manage PII in your documents before they get uploaded to a Retrieval Augmented
 Generation (RAG) system. Home-page: https://datafog.ai Author: DataFog Author-
 email: hi@datafog.ai Maintainer: DataFog Maintainer-email: hi@datafog.ai
 License: MIT Project-URL: Homepage, https://datafog.ai Project-URL:
 Documentation, https://docs.datafog.ai Project-URL: Discord, https://
 discord.gg/bzDth394R4 Project-URL: Twitter, https://twitter.com/datafoginc
 Project-URL: GitHub, https://github.com/datafog/datafog-python Keywords:
```

### Comparing `datafog-3.2.0b2/README.md` & `datafog-3.2.0b3/README.md`

 * *Files identical despite different names*

### Comparing `datafog-3.2.0b2/datafog/main.py` & `datafog-3.2.0b3/datafog/main.py`

 * *Files identical despite different names*

### Comparing `datafog-3.2.0b2/datafog.egg-info/PKG-INFO` & `datafog-3.2.0b3/datafog.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datafog
-Version: 3.2.0b2
+Version: 3.2.0b3
 Summary: Scan, redact, and manage PII in your documents before they get uploaded to a Retrieval Augmented Generation (RAG) system.
 Home-page: https://datafog.ai
 Author: DataFog
 Author-email: hi@datafog.ai
 Maintainer: DataFog
 Maintainer-email: hi@datafog.ai
 License: MIT
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: datafog Version: 3.2.0b2 Summary: Scan, redact, and
+Metadata-Version: 2.1 Name: datafog Version: 3.2.0b3 Summary: Scan, redact, and
 manage PII in your documents before they get uploaded to a Retrieval Augmented
 Generation (RAG) system. Home-page: https://datafog.ai Author: DataFog Author-
 email: hi@datafog.ai Maintainer: DataFog Maintainer-email: hi@datafog.ai
 License: MIT Project-URL: Homepage, https://datafog.ai Project-URL:
 Documentation, https://docs.datafog.ai Project-URL: Discord, https://
 discord.gg/bzDth394R4 Project-URL: Twitter, https://twitter.com/datafoginc
 Project-URL: GitHub, https://github.com/datafog/datafog-python Keywords:
```

### Comparing `datafog-3.2.0b2/setup.py` & `datafog-3.2.0b3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read README for the long description
 with open("README.md", "r") as f:
     long_description = f.read()
 
 
 def __version__():
-    return "3.2.0b2"
+    return "3.2.0b3"
 
 
 project_urls = {
     "Homepage": "https://datafog.ai",
     "Documentation": "https://docs.datafog.ai",
     "Discord": "https://discord.gg/bzDth394R4",
     "Twitter": "https://twitter.com/datafoginc",
```

### Comparing `datafog-3.2.0b2/tests/test_main.py` & `datafog-3.2.0b3/tests/test_main.py`

 * *Files identical despite different names*

