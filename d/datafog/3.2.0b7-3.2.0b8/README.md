# Comparing `tmp/datafog-3.2.0b7.tar.gz` & `tmp/datafog-3.2.0b8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datafog-3.2.0b7.tar", last modified: Mon May 13 19:30:09 2024, max compression
+gzip compressed data, was "datafog-3.2.0b8.tar", last modified: Mon May 13 19:36:58 2024, max compression
```

## Comparing `datafog-3.2.0b7.tar` & `datafog-3.2.0b8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-13 19:30:09.075606 datafog-3.2.0b7/
--rw-r--r--   0 sidmohan   (501) staff       (20)     1091 2024-05-13 14:18:11.000000 datafog-3.2.0b7/LICENSE
--rw-r--r--   0 sidmohan   (501) staff       (20)     6510 2024-05-13 19:30:09.075466 datafog-3.2.0b7/PKG-INFO
--rw-r--r--   0 sidmohan   (501) staff       (20)     5289 2024-05-13 14:50:51.000000 datafog-3.2.0b7/README.md
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-13 19:30:09.074205 datafog-3.2.0b7/datafog/
--rw-r--r--   0 sidmohan   (501) staff       (20)       24 2024-05-13 19:21:21.000000 datafog-3.2.0b7/datafog/__about__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)      494 2024-05-13 19:26:51.000000 datafog-3.2.0b7/datafog/__init__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)      222 2024-05-13 18:39:10.000000 datafog-3.2.0b7/datafog/config.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     2970 2024-05-13 19:29:53.000000 datafog-3.2.0b7/datafog/main.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-13 19:30:09.074959 datafog-3.2.0b7/datafog.egg-info/
--rw-r--r--   0 sidmohan   (501) staff       (20)     6510 2024-05-13 19:30:09.000000 datafog-3.2.0b7/datafog.egg-info/PKG-INFO
--rw-r--r--   0 sidmohan   (501) staff       (20)      274 2024-05-13 19:30:09.000000 datafog-3.2.0b7/datafog.egg-info/SOURCES.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)        1 2024-05-13 19:30:09.000000 datafog-3.2.0b7/datafog.egg-info/dependency_links.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)      159 2024-05-13 19:30:09.000000 datafog-3.2.0b7/datafog.egg-info/requires.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)        8 2024-05-13 19:30:09.000000 datafog-3.2.0b7/datafog.egg-info/top_level.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)       38 2024-05-13 19:30:09.075661 datafog-3.2.0b7/setup.cfg
--rw-r--r--   0 sidmohan   (501) staff       (20)     1920 2024-05-13 19:30:01.000000 datafog-3.2.0b7/setup.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-13 19:30:09.075096 datafog-3.2.0b7/tests/
--rw-r--r--   0 sidmohan   (501) staff       (20)     2889 2024-05-13 18:39:10.000000 datafog-3.2.0b7/tests/test_main.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-13 19:36:58.774448 datafog-3.2.0b8/
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1091 2024-05-13 14:18:11.000000 datafog-3.2.0b8/LICENSE
+-rw-r--r--   0 sidmohan   (501) staff       (20)     6510 2024-05-13 19:36:58.774311 datafog-3.2.0b8/PKG-INFO
+-rw-r--r--   0 sidmohan   (501) staff       (20)     5289 2024-05-13 14:50:51.000000 datafog-3.2.0b8/README.md
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-13 19:36:58.773118 datafog-3.2.0b8/datafog/
+-rw-r--r--   0 sidmohan   (501) staff       (20)       24 2024-05-13 19:21:21.000000 datafog-3.2.0b8/datafog/__about__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)      810 2024-05-13 19:36:05.000000 datafog-3.2.0b8/datafog/__init__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)      222 2024-05-13 18:39:10.000000 datafog-3.2.0b8/datafog/config.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     2970 2024-05-13 19:29:53.000000 datafog-3.2.0b8/datafog/main.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-13 19:36:58.773880 datafog-3.2.0b8/datafog.egg-info/
+-rw-r--r--   0 sidmohan   (501) staff       (20)     6510 2024-05-13 19:36:58.000000 datafog-3.2.0b8/datafog.egg-info/PKG-INFO
+-rw-r--r--   0 sidmohan   (501) staff       (20)      274 2024-05-13 19:36:58.000000 datafog-3.2.0b8/datafog.egg-info/SOURCES.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)        1 2024-05-13 19:36:58.000000 datafog-3.2.0b8/datafog.egg-info/dependency_links.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)      159 2024-05-13 19:36:58.000000 datafog-3.2.0b8/datafog.egg-info/requires.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)        8 2024-05-13 19:36:58.000000 datafog-3.2.0b8/datafog.egg-info/top_level.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)       38 2024-05-13 19:36:58.774498 datafog-3.2.0b8/setup.cfg
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1920 2024-05-13 19:36:53.000000 datafog-3.2.0b8/setup.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-13 19:36:58.774004 datafog-3.2.0b8/tests/
+-rw-r--r--   0 sidmohan   (501) staff       (20)     2889 2024-05-13 18:39:10.000000 datafog-3.2.0b8/tests/test_main.py
```

### Comparing `datafog-3.2.0b7/LICENSE` & `datafog-3.2.0b8/LICENSE`

 * *Files identical despite different names*

### Comparing `datafog-3.2.0b7/PKG-INFO` & `datafog-3.2.0b8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datafog
-Version: 3.2.0b7
+Version: 3.2.0b8
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
-Metadata-Version: 2.1 Name: datafog Version: 3.2.0b7 Summary: Scan, redact, and
+Metadata-Version: 2.1 Name: datafog Version: 3.2.0b8 Summary: Scan, redact, and
 manage PII in your documents before they get uploaded to a Retrieval Augmented
 Generation (RAG) system. Home-page: https://datafog.ai Author: DataFog Author-
 email: hi@datafog.ai Maintainer: DataFog Maintainer-email: hi@datafog.ai
 License: MIT Project-URL: Homepage, https://datafog.ai Project-URL:
 Documentation, https://docs.datafog.ai Project-URL: Discord, https://
 discord.gg/bzDth394R4 Project-URL: Twitter, https://twitter.com/datafoginc
 Project-URL: GitHub, https://github.com/datafog/datafog-python Keywords:
```

### Comparing `datafog-3.2.0b7/README.md` & `datafog-3.2.0b8/README.md`

 * *Files identical despite different names*

### Comparing `datafog-3.2.0b7/datafog/main.py` & `datafog-3.2.0b8/datafog/main.py`

 * *Files identical despite different names*

### Comparing `datafog-3.2.0b7/datafog.egg-info/PKG-INFO` & `datafog-3.2.0b8/datafog.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datafog
-Version: 3.2.0b7
+Version: 3.2.0b8
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
-Metadata-Version: 2.1 Name: datafog Version: 3.2.0b7 Summary: Scan, redact, and
+Metadata-Version: 2.1 Name: datafog Version: 3.2.0b8 Summary: Scan, redact, and
 manage PII in your documents before they get uploaded to a Retrieval Augmented
 Generation (RAG) system. Home-page: https://datafog.ai Author: DataFog Author-
 email: hi@datafog.ai Maintainer: DataFog Maintainer-email: hi@datafog.ai
 License: MIT Project-URL: Homepage, https://datafog.ai Project-URL:
 Documentation, https://docs.datafog.ai Project-URL: Discord, https://
 discord.gg/bzDth394R4 Project-URL: Twitter, https://twitter.com/datafoginc
 Project-URL: GitHub, https://github.com/datafog/datafog-python Keywords:
```

### Comparing `datafog-3.2.0b7/setup.py` & `datafog-3.2.0b8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read README for the long description
 with open("README.md", "r") as f:
     long_description = f.read()
 
 
 def __version__():
-    return "3.2.0b7"
+    return "3.2.0b8"
 
 
 project_urls = {
     "Homepage": "https://datafog.ai",
     "Documentation": "https://docs.datafog.ai",
     "Discord": "https://discord.gg/bzDth394R4",
     "Twitter": "https://twitter.com/datafoginc",
```

### Comparing `datafog-3.2.0b7/tests/test_main.py` & `datafog-3.2.0b8/tests/test_main.py`

 * *Files identical despite different names*

