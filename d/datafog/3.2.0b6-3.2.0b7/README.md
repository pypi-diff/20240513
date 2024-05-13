# Comparing `tmp/datafog-3.2.0b6.tar.gz` & `tmp/datafog-3.2.0b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datafog-3.2.0b6.tar", last modified: Mon May 13 19:27:41 2024, max compression
+gzip compressed data, was "datafog-3.2.0b7.tar", last modified: Mon May 13 19:30:09 2024, max compression
```

## Comparing `datafog-3.2.0b6.tar` & `datafog-3.2.0b7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-13 19:27:41.658434 datafog-3.2.0b6/
--rw-r--r--   0 sidmohan   (501) staff       (20)     1091 2024-05-13 14:18:11.000000 datafog-3.2.0b6/LICENSE
--rw-r--r--   0 sidmohan   (501) staff       (20)     6510 2024-05-13 19:27:41.658274 datafog-3.2.0b6/PKG-INFO
--rw-r--r--   0 sidmohan   (501) staff       (20)     5289 2024-05-13 14:50:51.000000 datafog-3.2.0b6/README.md
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-13 19:27:41.657077 datafog-3.2.0b6/datafog/
--rw-r--r--   0 sidmohan   (501) staff       (20)       24 2024-05-13 19:21:21.000000 datafog-3.2.0b6/datafog/__about__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)      494 2024-05-13 19:26:51.000000 datafog-3.2.0b6/datafog/__init__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)      222 2024-05-13 18:39:10.000000 datafog-3.2.0b6/datafog/config.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     3005 2024-05-13 19:21:45.000000 datafog-3.2.0b6/datafog/main.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-13 19:27:41.657771 datafog-3.2.0b6/datafog.egg-info/
--rw-r--r--   0 sidmohan   (501) staff       (20)     6510 2024-05-13 19:27:41.000000 datafog-3.2.0b6/datafog.egg-info/PKG-INFO
--rw-r--r--   0 sidmohan   (501) staff       (20)      274 2024-05-13 19:27:41.000000 datafog-3.2.0b6/datafog.egg-info/SOURCES.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)        1 2024-05-13 19:27:41.000000 datafog-3.2.0b6/datafog.egg-info/dependency_links.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)      159 2024-05-13 19:27:41.000000 datafog-3.2.0b6/datafog.egg-info/requires.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)        8 2024-05-13 19:27:41.000000 datafog-3.2.0b6/datafog.egg-info/top_level.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)       38 2024-05-13 19:27:41.658487 datafog-3.2.0b6/setup.cfg
--rw-r--r--   0 sidmohan   (501) staff       (20)     1920 2024-05-13 19:27:23.000000 datafog-3.2.0b6/setup.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-13 19:27:41.657892 datafog-3.2.0b6/tests/
--rw-r--r--   0 sidmohan   (501) staff       (20)     2889 2024-05-13 18:39:10.000000 datafog-3.2.0b6/tests/test_main.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-13 19:30:09.075606 datafog-3.2.0b7/
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1091 2024-05-13 14:18:11.000000 datafog-3.2.0b7/LICENSE
+-rw-r--r--   0 sidmohan   (501) staff       (20)     6510 2024-05-13 19:30:09.075466 datafog-3.2.0b7/PKG-INFO
+-rw-r--r--   0 sidmohan   (501) staff       (20)     5289 2024-05-13 14:50:51.000000 datafog-3.2.0b7/README.md
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-13 19:30:09.074205 datafog-3.2.0b7/datafog/
+-rw-r--r--   0 sidmohan   (501) staff       (20)       24 2024-05-13 19:21:21.000000 datafog-3.2.0b7/datafog/__about__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)      494 2024-05-13 19:26:51.000000 datafog-3.2.0b7/datafog/__init__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)      222 2024-05-13 18:39:10.000000 datafog-3.2.0b7/datafog/config.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     2970 2024-05-13 19:29:53.000000 datafog-3.2.0b7/datafog/main.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-13 19:30:09.074959 datafog-3.2.0b7/datafog.egg-info/
+-rw-r--r--   0 sidmohan   (501) staff       (20)     6510 2024-05-13 19:30:09.000000 datafog-3.2.0b7/datafog.egg-info/PKG-INFO
+-rw-r--r--   0 sidmohan   (501) staff       (20)      274 2024-05-13 19:30:09.000000 datafog-3.2.0b7/datafog.egg-info/SOURCES.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)        1 2024-05-13 19:30:09.000000 datafog-3.2.0b7/datafog.egg-info/dependency_links.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)      159 2024-05-13 19:30:09.000000 datafog-3.2.0b7/datafog.egg-info/requires.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)        8 2024-05-13 19:30:09.000000 datafog-3.2.0b7/datafog.egg-info/top_level.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)       38 2024-05-13 19:30:09.075661 datafog-3.2.0b7/setup.cfg
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1920 2024-05-13 19:30:01.000000 datafog-3.2.0b7/setup.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-13 19:30:09.075096 datafog-3.2.0b7/tests/
+-rw-r--r--   0 sidmohan   (501) staff       (20)     2889 2024-05-13 18:39:10.000000 datafog-3.2.0b7/tests/test_main.py
```

### Comparing `datafog-3.2.0b6/LICENSE` & `datafog-3.2.0b7/LICENSE`

 * *Files identical despite different names*

### Comparing `datafog-3.2.0b6/PKG-INFO` & `datafog-3.2.0b7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datafog
-Version: 3.2.0b6
+Version: 3.2.0b7
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
-Metadata-Version: 2.1 Name: datafog Version: 3.2.0b6 Summary: Scan, redact, and
+Metadata-Version: 2.1 Name: datafog Version: 3.2.0b7 Summary: Scan, redact, and
 manage PII in your documents before they get uploaded to a Retrieval Augmented
 Generation (RAG) system. Home-page: https://datafog.ai Author: DataFog Author-
 email: hi@datafog.ai Maintainer: DataFog Maintainer-email: hi@datafog.ai
 License: MIT Project-URL: Homepage, https://datafog.ai Project-URL:
 Documentation, https://docs.datafog.ai Project-URL: Discord, https://
 discord.gg/bzDth394R4 Project-URL: Twitter, https://twitter.com/datafoginc
 Project-URL: GitHub, https://github.com/datafog/datafog-python Keywords:
```

### Comparing `datafog-3.2.0b6/README.md` & `datafog-3.2.0b7/README.md`

 * *Files identical despite different names*

### Comparing `datafog-3.2.0b6/datafog/main.py` & `datafog-3.2.0b7/datafog/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import asyncio
 import json
 from typing import List
 
 import aiohttp
 
 from .config import OperationType
-from datafog.processing.image_processing.donut_processor import DonutProcessor
-from datafog.processing.text_processing.spacy_pii_annotator import SpacyPIIAnnotator
-from datafog.services.image_service import ImageService
-from datafog.services.spark_service import SparkService
-from datafog.services.text_service import TextService
+from .processing.image_processing.donut_processor import DonutProcessor
+from .processing.text_processing.spacy_pii_annotator import SpacyPIIAnnotator
+from .services.image_service import ImageService
+from .services.spark_service import SparkService
+from .services.text_service import TextService
 
 
 
 class DataFog:
     def __init__(self, operations: List[OperationType] = [OperationType.ANNOTATE_PII]):
         self.image_service = ImageService()
         self.text_service = TextService()
```

### Comparing `datafog-3.2.0b6/datafog.egg-info/PKG-INFO` & `datafog-3.2.0b7/datafog.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datafog
-Version: 3.2.0b6
+Version: 3.2.0b7
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
-Metadata-Version: 2.1 Name: datafog Version: 3.2.0b6 Summary: Scan, redact, and
+Metadata-Version: 2.1 Name: datafog Version: 3.2.0b7 Summary: Scan, redact, and
 manage PII in your documents before they get uploaded to a Retrieval Augmented
 Generation (RAG) system. Home-page: https://datafog.ai Author: DataFog Author-
 email: hi@datafog.ai Maintainer: DataFog Maintainer-email: hi@datafog.ai
 License: MIT Project-URL: Homepage, https://datafog.ai Project-URL:
 Documentation, https://docs.datafog.ai Project-URL: Discord, https://
 discord.gg/bzDth394R4 Project-URL: Twitter, https://twitter.com/datafoginc
 Project-URL: GitHub, https://github.com/datafog/datafog-python Keywords:
```

### Comparing `datafog-3.2.0b6/setup.py` & `datafog-3.2.0b7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read README for the long description
 with open("README.md", "r") as f:
     long_description = f.read()
 
 
 def __version__():
-    return "3.2.0b6"
+    return "3.2.0b7"
 
 
 project_urls = {
     "Homepage": "https://datafog.ai",
     "Documentation": "https://docs.datafog.ai",
     "Discord": "https://discord.gg/bzDth394R4",
     "Twitter": "https://twitter.com/datafoginc",
```

### Comparing `datafog-3.2.0b6/tests/test_main.py` & `datafog-3.2.0b7/tests/test_main.py`

 * *Files identical despite different names*

