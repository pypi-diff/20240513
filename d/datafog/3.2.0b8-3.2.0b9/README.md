# Comparing `tmp/datafog-3.2.0b8.tar.gz` & `tmp/datafog-3.2.0b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datafog-3.2.0b8.tar", last modified: Mon May 13 19:36:58 2024, max compression
+gzip compressed data, was "datafog-3.2.0b9.tar", last modified: Mon May 13 19:45:36 2024, max compression
```

## Comparing `datafog-3.2.0b8.tar` & `datafog-3.2.0b9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-13 19:36:58.774448 datafog-3.2.0b8/
--rw-r--r--   0 sidmohan   (501) staff       (20)     1091 2024-05-13 14:18:11.000000 datafog-3.2.0b8/LICENSE
--rw-r--r--   0 sidmohan   (501) staff       (20)     6510 2024-05-13 19:36:58.774311 datafog-3.2.0b8/PKG-INFO
--rw-r--r--   0 sidmohan   (501) staff       (20)     5289 2024-05-13 14:50:51.000000 datafog-3.2.0b8/README.md
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-13 19:36:58.773118 datafog-3.2.0b8/datafog/
--rw-r--r--   0 sidmohan   (501) staff       (20)       24 2024-05-13 19:21:21.000000 datafog-3.2.0b8/datafog/__about__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)      810 2024-05-13 19:36:05.000000 datafog-3.2.0b8/datafog/__init__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)      222 2024-05-13 18:39:10.000000 datafog-3.2.0b8/datafog/config.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     2970 2024-05-13 19:29:53.000000 datafog-3.2.0b8/datafog/main.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-13 19:36:58.773880 datafog-3.2.0b8/datafog.egg-info/
--rw-r--r--   0 sidmohan   (501) staff       (20)     6510 2024-05-13 19:36:58.000000 datafog-3.2.0b8/datafog.egg-info/PKG-INFO
--rw-r--r--   0 sidmohan   (501) staff       (20)      274 2024-05-13 19:36:58.000000 datafog-3.2.0b8/datafog.egg-info/SOURCES.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)        1 2024-05-13 19:36:58.000000 datafog-3.2.0b8/datafog.egg-info/dependency_links.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)      159 2024-05-13 19:36:58.000000 datafog-3.2.0b8/datafog.egg-info/requires.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)        8 2024-05-13 19:36:58.000000 datafog-3.2.0b8/datafog.egg-info/top_level.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)       38 2024-05-13 19:36:58.774498 datafog-3.2.0b8/setup.cfg
--rw-r--r--   0 sidmohan   (501) staff       (20)     1920 2024-05-13 19:36:53.000000 datafog-3.2.0b8/setup.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-13 19:36:58.774004 datafog-3.2.0b8/tests/
--rw-r--r--   0 sidmohan   (501) staff       (20)     2889 2024-05-13 18:39:10.000000 datafog-3.2.0b8/tests/test_main.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-13 19:45:36.964847 datafog-3.2.0b9/
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1091 2024-05-13 14:18:11.000000 datafog-3.2.0b9/LICENSE
+-rw-r--r--   0 sidmohan   (501) staff       (20)     6510 2024-05-13 19:45:36.964714 datafog-3.2.0b9/PKG-INFO
+-rw-r--r--   0 sidmohan   (501) staff       (20)     5289 2024-05-13 14:50:51.000000 datafog-3.2.0b9/README.md
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-13 19:45:36.963432 datafog-3.2.0b9/datafog/
+-rw-r--r--   0 sidmohan   (501) staff       (20)       24 2024-05-13 19:21:21.000000 datafog-3.2.0b9/datafog/__about__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)      821 2024-05-13 19:44:16.000000 datafog-3.2.0b9/datafog/__init__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)      222 2024-05-13 18:39:10.000000 datafog-3.2.0b9/datafog/config.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     2892 2024-05-13 19:44:17.000000 datafog-3.2.0b9/datafog/main.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-13 19:45:36.964228 datafog-3.2.0b9/datafog.egg-info/
+-rw-r--r--   0 sidmohan   (501) staff       (20)     6510 2024-05-13 19:45:36.000000 datafog-3.2.0b9/datafog.egg-info/PKG-INFO
+-rw-r--r--   0 sidmohan   (501) staff       (20)      274 2024-05-13 19:45:36.000000 datafog-3.2.0b9/datafog.egg-info/SOURCES.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)        1 2024-05-13 19:45:36.000000 datafog-3.2.0b9/datafog.egg-info/dependency_links.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)      159 2024-05-13 19:45:36.000000 datafog-3.2.0b9/datafog.egg-info/requires.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)        8 2024-05-13 19:45:36.000000 datafog-3.2.0b9/datafog.egg-info/top_level.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)       38 2024-05-13 19:45:36.964893 datafog-3.2.0b9/setup.cfg
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1920 2024-05-13 19:45:31.000000 datafog-3.2.0b9/setup.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-13 19:45:36.964355 datafog-3.2.0b9/tests/
+-rw-r--r--   0 sidmohan   (501) staff       (20)     2905 2024-05-13 19:44:48.000000 datafog-3.2.0b9/tests/test_main.py
```

### Comparing `datafog-3.2.0b8/LICENSE` & `datafog-3.2.0b9/LICENSE`

 * *Files identical despite different names*

### Comparing `datafog-3.2.0b8/PKG-INFO` & `datafog-3.2.0b9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datafog
-Version: 3.2.0b8
+Version: 3.2.0b9
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
-Metadata-Version: 2.1 Name: datafog Version: 3.2.0b8 Summary: Scan, redact, and
+Metadata-Version: 2.1 Name: datafog Version: 3.2.0b9 Summary: Scan, redact, and
 manage PII in your documents before they get uploaded to a Retrieval Augmented
 Generation (RAG) system. Home-page: https://datafog.ai Author: DataFog Author-
 email: hi@datafog.ai Maintainer: DataFog Maintainer-email: hi@datafog.ai
 License: MIT Project-URL: Homepage, https://datafog.ai Project-URL:
 Documentation, https://docs.datafog.ai Project-URL: Discord, https://
 discord.gg/bzDth394R4 Project-URL: Twitter, https://twitter.com/datafoginc
 Project-URL: GitHub, https://github.com/datafog/datafog-python Keywords:
```

### Comparing `datafog-3.2.0b8/README.md` & `datafog-3.2.0b9/README.md`

 * *Files identical despite different names*

### Comparing `datafog-3.2.0b8/datafog/__init__.py` & `datafog-3.2.0b9/datafog/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,27 @@
-from .main import (
-    DataFog, OCRPIIAnnotator, TextPIIAnnotator
+from .main import (DataFog
+    # DataFog, OCRPIIAnnotator, TextPIIAnnotator
 )
 from .processing.image_processing.donut_processor import DonutProcessor
 from .processing.image_processing.image_downloader import ImageDownloader
 from .processing.image_processing.pytesseract_processor import PytesseractProcessor
 from .processing.text_processing.spacy_pii_annotator import SpacyPIIAnnotator
+
+
 from .services.image_service import ImageService
 from .services.spark_service import SparkService
 from .services.text_service import TextService
 from .config import OperationType
 
 __all__ = [
+    "DonutProcessor",
     "DataFog",
     "ImageService",
     "OCRPIIAnnotator",
     "OperationType",
     "SparkService",
     "TextPIIAnnotator",
     "TextService",
-    "DonutProcessor",
     "SpacyPIIAnnotator",
     "ImageDownloader",
     "PytesseractProcessor",
 ]
```

### Comparing `datafog-3.2.0b8/datafog/main.py` & `datafog-3.2.0b9/datafog/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import asyncio
 import json
 from typing import List
 
 import aiohttp
 
 from .config import OperationType
-from .processing.image_processing.donut_processor import DonutProcessor
-from .processing.text_processing.spacy_pii_annotator import SpacyPIIAnnotator
 from .services.image_service import ImageService
 from .services.spark_service import SparkService
 from .services.text_service import TextService
 
 
 
 class DataFog:
@@ -34,54 +32,54 @@
         """Run the text pipeline asynchronously."""
         if OperationType.ANNOTATE_PII in self.operations:
             annotated_text = await self.text_service.batch_annotate_texts(texts)
             return annotated_text
         return texts
 
 
-class OCRPIIAnnotator:
-    def __init__(self):
-        self.spark_processor: SparkService = None
-        self.image_service = DonutProcessor()
-        self.text_annotator = SpacyPIIAnnotator.create()
-
-    def run(self, image_url, output_path=None):
-        try:
-            # Download and process the image to extract text
-            downloaded_image = self.image_service.download_image(image_url)
-            extracted_text = self.image_service.parse_image(downloaded_image)
-
-            # Annotate the extracted text for PII
-            annotated_text = self.text_annotator.annotate(extracted_text)
-
-            # Optionally, output the results to a JSON file
-            if output_path:
-                with open(output_path, "w") as f:
-                    json.dump(annotated_text, f)
-
-            return annotated_text
-
-        finally:
-            # Ensure Spark resources are released
-            # self.spark_processor.spark.stop()
-            pass
-
-
-class TextPIIAnnotator:
-    def __init__(self):
-        self.text_annotator = SpacyPIIAnnotator.create()
-        self.spark_processor: SparkService = None
-
-    def run(self, text, output_path=None):
-        try:
-            annotated_text = self.text_annotator.annotate(text)
-
-            # Optionally, output the results to a JSON file
-            if output_path:
-                with open(output_path, "w") as f:
-                    json.dump(annotated_text, f)
-
-            return annotated_text
-
-        finally:
-            # Ensure Spark resources are released
-            pass
+# class OCRPIIAnnotator:
+#     def __init__(self):
+#         self.spark_processor: SparkService = None
+#         self.image_service = DonutProcessor()
+#         self.text_annotator = SpacyPIIAnnotator.create()
+
+#     def run(self, image_url, output_path=None):
+#         try:
+#             # Download and process the image to extract text
+#             downloaded_image = self.image_service.download_image(image_url)
+#             extracted_text = self.image_service.parse_image(downloaded_image)
+
+#             # Annotate the extracted text for PII
+#             annotated_text = self.text_annotator.annotate(extracted_text)
+
+#             # Optionally, output the results to a JSON file
+#             if output_path:
+#                 with open(output_path, "w") as f:
+#                     json.dump(annotated_text, f)
+
+#             return annotated_text
+
+#         finally:
+#             # Ensure Spark resources are released
+#             # self.spark_processor.spark.stop()
+#             pass
+
+
+# class TextPIIAnnotator:
+#     def __init__(self):
+#         self.text_annotator = SpacyPIIAnnotator.create()
+#         self.spark_processor: SparkService = None
+
+#     def run(self, text, output_path=None):
+#         try:
+#             annotated_text = self.text_annotator.annotate(text)
+
+#             # Optionally, output the results to a JSON file
+#             if output_path:
+#                 with open(output_path, "w") as f:
+#                     json.dump(annotated_text, f)
+
+#             return annotated_text
+
+#         finally:
+#             # Ensure Spark resources are released
+#             pass
```

### Comparing `datafog-3.2.0b8/datafog.egg-info/PKG-INFO` & `datafog-3.2.0b9/datafog.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datafog
-Version: 3.2.0b8
+Version: 3.2.0b9
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
-Metadata-Version: 2.1 Name: datafog Version: 3.2.0b8 Summary: Scan, redact, and
+Metadata-Version: 2.1 Name: datafog Version: 3.2.0b9 Summary: Scan, redact, and
 manage PII in your documents before they get uploaded to a Retrieval Augmented
 Generation (RAG) system. Home-page: https://datafog.ai Author: DataFog Author-
 email: hi@datafog.ai Maintainer: DataFog Maintainer-email: hi@datafog.ai
 License: MIT Project-URL: Homepage, https://datafog.ai Project-URL:
 Documentation, https://docs.datafog.ai Project-URL: Discord, https://
 discord.gg/bzDth394R4 Project-URL: Twitter, https://twitter.com/datafoginc
 Project-URL: GitHub, https://github.com/datafog/datafog-python Keywords:
```

### Comparing `datafog-3.2.0b8/setup.py` & `datafog-3.2.0b9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read README for the long description
 with open("README.md", "r") as f:
     long_description = f.read()
 
 
 def __version__():
-    return "3.2.0b8"
+    return "3.2.0b9"
 
 
 project_urls = {
     "Homepage": "https://datafog.ai",
     "Documentation": "https://docs.datafog.ai",
     "Discord": "https://discord.gg/bzDth394R4",
     "Twitter": "https://twitter.com/datafoginc",
```

### Comparing `datafog-3.2.0b8/tests/test_main.py` & `datafog-3.2.0b9/tests/test_main.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 
 import aiohttp
 import pytest
 
 from datafog import (
     DataFog,
     ImageService,
-    OCRPIIAnnotator,
+    # OCRPIIAnnotator,
     OperationType,
     SparkService,
-    TextPIIAnnotator,
+    # TextPIIAnnotator,
     TextService,
 )
 
 
 def search_nested_dict(d, target):
     """Recursively search for a target value in nested dictionaries."""
     if isinstance(d, dict):
@@ -24,20 +24,20 @@
                 return True
             elif isinstance(value, dict):
                 if search_nested_dict(value, target):
                     return True
     return False
 
 
-def test_textpii_annotator():
-    """Test the PII annotation functionality."""
-    text = "John Doe lives at 1234 Elm St, Springfield."
-    text_annotator = TextPIIAnnotator()
-    annotated_text = text_annotator.run(text)
-    assert "Springfield" in annotated_text["LOC"], "PII not annotated correctly."
+# def test_textpii_annotator():
+#     """Test the PII annotation functionality."""
+#     text = "John Doe lives at 1234 Elm St, Springfield."
+#     text_annotator = TextPIIAnnotator()
+#     annotated_text = text_annotator.run(text)
+#     assert "Springfield" in annotated_text["LOC"], "PII not annotated correctly."
 
 
 # def test_donut_processor():
 #     """Test the PII annotation functionality for the donutprocessor."""
 #     with open("tests/image_set.json", "r") as f:
 #         image_set = json.load(f)
 #         image_url = image_set["executive_email"]
```

