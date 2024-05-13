# Comparing `tmp/easytl-0.3.1.tar.gz` & `tmp/easytl-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easytl-0.3.1.tar", last modified: Sat May 11 03:06:02 2024, max compression
+gzip compressed data, was "easytl-0.3.2.tar", last modified: Mon May 13 19:49:27 2024, max compression
```

## Comparing `easytl-0.3.1.tar` & `easytl-0.3.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:06:02.672974 easytl-0.3.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:06:02.664974 easytl-0.3.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:06:02.668974 easytl-0.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-05-11 03:04:38.000000 easytl-0.3.1/.github/workflows/workflow.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-05-11 03:04:38.000000 easytl-0.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-05-11 03:04:38.000000 easytl-0.3.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     8229 2024-05-11 03:06:02.672974 easytl-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7304 2024-05-11 03:04:38.000000 easytl-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4619 2024-05-11 03:04:38.000000 easytl-0.3.1/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-11 03:04:38.000000 easytl-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 03:06:02.672974 easytl-0.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:06:02.664974 easytl-0.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:06:02.668974 easytl-0.3.1/src/easytl/
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-11 03:04:38.000000 easytl-0.3.1/src/easytl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-05-11 03:04:38.000000 easytl-0.3.1/src/easytl/classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-05-11 03:04:38.000000 easytl-0.3.1/src/easytl/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)    10444 2024-05-11 03:04:38.000000 easytl-0.3.1/src/easytl/deepl_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    71506 2024-05-11 03:04:38.000000 easytl-0.3.1/src/easytl/easytl.py
--rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-05-11 03:04:38.000000 easytl-0.3.1/src/easytl/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    14874 2024-05-11 03:04:38.000000 easytl-0.3.1/src/easytl/gemini_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     9103 2024-05-11 03:04:38.000000 easytl-0.3.1/src/easytl/googletl_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    17993 2024-05-11 03:04:38.000000 easytl-0.3.1/src/easytl/openai_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    25791 2024-05-11 03:04:38.000000 easytl-0.3.1/src/easytl/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-11 03:04:38.000000 easytl-0.3.1/src/easytl/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:06:02.672974 easytl-0.3.1/src/easytl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8229 2024-05-11 03:06:02.000000 easytl-0.3.1/src/easytl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-11 03:06:02.000000 easytl-0.3.1/src/easytl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 03:06:02.000000 easytl-0.3.1/src/easytl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-11 03:06:02.000000 easytl-0.3.1/src/easytl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-11 03:06:02.000000 easytl-0.3.1/src/easytl.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:06:02.672974 easytl-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-05-11 03:04:38.000000 easytl-0.3.1/tests/issue_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    13247 2024-05-11 03:04:38.000000 easytl-0.3.1/tests/passing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:49:27.465074 easytl-0.3.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:49:27.461073 easytl-0.3.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:49:27.461073 easytl-0.3.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-05-13 19:47:59.000000 easytl-0.3.2/.github/workflows/workflow.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-05-13 19:47:59.000000 easytl-0.3.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-05-13 19:47:59.000000 easytl-0.3.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8229 2024-05-13 19:49:27.465074 easytl-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7304 2024-05-13 19:47:59.000000 easytl-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4619 2024-05-13 19:47:59.000000 easytl-0.3.2/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-13 19:47:59.000000 easytl-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 19:49:27.465074 easytl-0.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:49:27.461073 easytl-0.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:49:27.465074 easytl-0.3.2/src/easytl/
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-13 19:47:59.000000 easytl-0.3.2/src/easytl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-05-13 19:47:59.000000 easytl-0.3.2/src/easytl/classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-05-13 19:47:59.000000 easytl-0.3.2/src/easytl/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10505 2024-05-13 19:47:59.000000 easytl-0.3.2/src/easytl/deepl_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71506 2024-05-13 19:47:59.000000 easytl-0.3.2/src/easytl/easytl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-05-13 19:47:59.000000 easytl-0.3.2/src/easytl/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14874 2024-05-13 19:47:59.000000 easytl-0.3.2/src/easytl/gemini_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9132 2024-05-13 19:47:59.000000 easytl-0.3.2/src/easytl/googletl_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17993 2024-05-13 19:47:59.000000 easytl-0.3.2/src/easytl/openai_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26492 2024-05-13 19:47:59.000000 easytl-0.3.2/src/easytl/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-13 19:47:59.000000 easytl-0.3.2/src/easytl/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:49:27.465074 easytl-0.3.2/src/easytl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8229 2024-05-13 19:49:27.000000 easytl-0.3.2/src/easytl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-13 19:49:27.000000 easytl-0.3.2/src/easytl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 19:49:27.000000 easytl-0.3.2/src/easytl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-13 19:49:27.000000 easytl-0.3.2/src/easytl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-13 19:49:27.000000 easytl-0.3.2/src/easytl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:49:27.465074 easytl-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-05-13 19:47:59.000000 easytl-0.3.2/tests/issue_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13247 2024-05-13 19:47:59.000000 easytl-0.3.2/tests/passing.py
```

### Comparing `easytl-0.3.1/.github/workflows/workflow.yml` & `easytl-0.3.2/.github/workflows/workflow.yml`

 * *Files identical despite different names*

### Comparing `easytl-0.3.1/.gitignore` & `easytl-0.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `easytl-0.3.1/LICENSE.md` & `easytl-0.3.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `easytl-0.3.1/PKG-INFO` & `easytl-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easytl
-Version: 0.3.1
+Version: 0.3.2
 Summary: Seamless Multi-API Translation: Simplifying Language Barriers with DeepL, OpenAI, Gemini and Google Translate.
 Author-email: Bikatr7 <Bikatr7@proton.me>
 Project-URL: Homepage, https://github.com/Bikatr7/EasyTL
 Project-URL: Issues, https://github.com/Bikatr7/EasyTL/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `easytl-0.3.1/README.md` & `easytl-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `easytl-0.3.1/SECURITY.md` & `easytl-0.3.2/SECURITY.md`

 * *Files identical despite different names*

### Comparing `easytl-0.3.1/pyproject.toml` & `easytl-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     "openai==1.13.3",
     "backoff==2.2.1",
     "tiktoken==0.6.0",
     "google-cloud-translate==3.15.3"
 ]
 
 name = "easytl"
-version = "v0.3.1"
+version = "v0.3.2"
 authors = [
   { name="Bikatr7", email="Bikatr7@proton.me" },
 ]
 description = "Seamless Multi-API Translation: Simplifying Language Barriers with DeepL, OpenAI, Gemini and Google Translate."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `easytl-0.3.1/src/easytl/__init__.py` & `easytl-0.3.2/src/easytl/__init__.py`

 * *Files identical despite different names*

### Comparing `easytl-0.3.1/src/easytl/classes.py` & `easytl-0.3.2/src/easytl/classes.py`

 * *Files identical despite different names*

### Comparing `easytl-0.3.1/src/easytl/decorators.py` & `easytl-0.3.2/src/easytl/decorators.py`

 * *Files identical despite different names*

### Comparing `easytl-0.3.1/src/easytl/deepl_service.py` & `easytl-0.3.2/src/easytl/deepl_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 ## third-party libraries
 from deepl.translator import Translator
 
 import deepl
 
 ## custom modules
+from .version import VERSION
 from .util import _convert_iterable_to_str
 from .decorators import _async_logging_decorator, _sync_logging_decorator
 from .classes import Language, SplitSentences, Formality, GlossaryInfo, TextResult
 
 class DeepLService:
 
     _api_key:str = ""
@@ -241,15 +242,15 @@
 
         """
 
         _validity = False
 
         try:
 
-            DeepLService._translator = Translator(DeepLService._api_key)
+            DeepLService._translator = Translator(DeepLService._api_key).set_app_info("EasyTL", VERSION)
 
             DeepLService._translator.translate_text("私", target_lang="JA")
 
             _validity = True
 
             return _validity, None
```

### Comparing `easytl-0.3.1/src/easytl/easytl.py` & `easytl-0.3.2/src/easytl/easytl.py`

 * *Files identical despite different names*

### Comparing `easytl-0.3.1/src/easytl/exceptions.py` & `easytl-0.3.2/src/easytl/exceptions.py`

 * *Files identical despite different names*

### Comparing `easytl-0.3.1/src/easytl/gemini_service.py` & `easytl-0.3.2/src/easytl/gemini_service.py`

 * *Files identical despite different names*

### Comparing `easytl-0.3.1/src/easytl/googletl_service.py` & `easytl-0.3.2/src/easytl/googletl_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from google.cloud import translate_v2 as translate
 from google.cloud.translate_v2 import Client
 
 from google.oauth2 import service_account
 from google.oauth2.service_account import Credentials
 
 ## custom modules
+from .version import VERSION
 from .util import _convert_iterable_to_str
 from .decorators import _sync_logging_decorator, _async_logging_decorator
 
 class GoogleTLService:
```

### Comparing `easytl-0.3.1/src/easytl/openai_service.py` & `easytl-0.3.2/src/easytl/openai_service.py`

 * *Files identical despite different names*

### Comparing `easytl-0.3.1/src/easytl/util.py` & `easytl-0.3.2/src/easytl/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -339,14 +339,18 @@
             print("Warning: gpt-4-turbo-preview may change over time. Estimating cost assuming gpt-4-0125-preview as it is the most recent version of gpt-4-turbo-preview.")
             return _estimate_cost(text, model="gpt-4-0125-preview")
         
         elif(model == "gpt-4-vision-preview"):
             print("Warning: gpt-4-vision-preview may change over time. Estimating cost assuming gpt-4-1106-vision-preview as it is the most recent version of gpt-4-1106-vision-preview.")
             return _estimate_cost(text, model="gpt-4-1106-vision-preview")
         
+        elif(model == "gpt-4o"):
+            print("Warning: gpt-4o may change over time. Estimating cost assuming gpt-4o-2024-05-13 as it is the most recent version of gpt-4o.")
+            return _estimate_cost(text, model="gpt-4o-2024-05-13")
+        
         elif(model == "gpt-3.5-turbo-0613"):
             print("Warning: gpt-3.5-turbo-0613 is considered depreciated by OpenAI as of November 6, 2023 and could be shutdown as early as June 13, 2024. Consider switching to gpt-3.5-turbo-0125.")
             return _estimate_cost(text, model=model, price_case=1)
 
         elif(model == "gpt-3.5-turbo-0301"):
             print("Warning: gpt-3.5-turbo-0301 is considered depreciated by OpenAI as of June 13, 2023 and could be shutdown as early as June 13, 2024. Consider switching to gpt-3.5-turbo-0125 unless you are specifically trying to break the filter.")
             return _estimate_cost(text, model=model, price_case=1)
@@ -384,14 +388,17 @@
         elif(model == "gpt-4-32k-0314"):
             print("Warning: gpt-4-32k-0314 is considered depreciated by OpenAI as of June 13, 2023 and could be shutdown as early as June 13, 2024. Consider switching to gpt-4-32k-0613.")
             return _estimate_cost(text, model=model, price_case=6)
         
         elif(model == "gpt-4-32k-0613"):
             return _estimate_cost(text, model=model, price_case=6)
         
+        elif(model == "gpt-4o-2024-05-13"):
+            return _estimate_cost(text, model=model, price_case=10)
+        
         elif(model == "gemini-pro"):
             print(f"Warning: gemini-pro may change over time. Estimating cost assuming gemini-1.0-pro-001 as it is the most recent version of gemini-1.0-pro.")
             return _estimate_cost(text, model="gemini-1.0-pro-001", price_case=8)
         
         elif(model == "gemini-pro-vision"):
             print("Warning: gemini-pro-vision may change over time. Estimating cost assuming gemini-1.0-pro-vision-001 as it is the most recent version of gemini-1.0-pro-vision.")
             return _estimate_cost(text, model="gemini-1.0-pro-vision-001", price_case=8)
@@ -479,21 +486,29 @@
     "gpt-4-turbo",
     "gpt-4-turbo-preview",
     "gpt-4-turbo-2024-04-09",
     "gpt-4-0125-preview",
     "gpt-4-1106-preview",
     "gpt-4-vision-preview",
     "gpt-4-1106-vision-preview",
+    "gpt-4o",
+    "gpt-4o-2024-05-13"
 ]
 
 VALID_JSON_OPENAI_MODELS = [
     "gpt-3.5-turbo-0125",
     "gpt-4-turbo",
     "gpt-4-turbo-preview",
     "gpt-4-turbo-2024-04-09",
+    "gpt-4-0125-preview",
+    "gpt-4-1106-preview",
+    "gpt-4-vision-preview",
+    "gpt-4-1106-vision-preview",
+    "gpt-4o-2024-05-13",
+    "gpt-4o"    
 ]
 
 ## Costs & Models are determined and updated manually, listed in USD. Updated by Bikatr7 as of 2024-04-18
 ## https://ai.google.dev/models/gemini
 ALLOWED_GEMINI_MODELS = [
     "gemini-1.0-pro-001",
     "gemini-1.0-pro",
@@ -504,34 +519,37 @@
     "gemini-1.5-pro-latest",
   ##  "gemini-1.0-ultra-latest",
     "gemini-pro",
     "gemini-pro-vision",
   ##  "gemini-ultra"
 ]
 
-## Costs & Models are determined and updated manually, listed in USD. Updated by Bikatr7 as of 2024-04-18
+## Costs & Models are determined and updated manually, listed in USD. Updated by Bikatr7 as of 2024-05-13
 MODEL_COSTS = {
     # Grouping GPT-3.5 models together
     "gpt-3.5-turbo-0125": {"price_case": 7, "_input_cost": 0.0005, "_output_cost": 0.0015},
     "gpt-3.5-turbo-0301": {"price_case": 1, "_input_cost": 0.0015, "_output_cost": 0.0020},
     "gpt-3.5-turbo-0613": {"price_case": 1, "_input_cost": 0.0015, "_output_cost": 0.0020},
     "gpt-3.5-turbo-1106": {"price_case": 2, "_input_cost": 0.0010, "_output_cost": 0.0020},
     "gpt-3.5-turbo-16k-0613": {"price_case": 3, "_input_cost": 0.0030, "_output_cost": 0.0040},
     
-    # Grouping GPT-4 models by their capabilities and versions
+    ## Grouping GPT-4 models by their capabilities and versions
     "gpt-4-0314": {"price_case": 5, "_input_cost": 0.03, "_output_cost": 0.06},
     "gpt-4-0613": {"price_case": 5, "_input_cost": 0.03, "_output_cost": 0.06},
     "gpt-4-32k-0314": {"price_case": 6, "_input_cost": 0.06, "_output_cost": 0.012},
     "gpt-4-32k-0613": {"price_case": 6, "_input_cost": 0.06, "_output_cost": 0.012},
     "gpt-4-1106-preview": {"price_case": 8, "_input_cost": 0.01, "_output_cost": 0.03},
     "gpt-4-0125-preview": {"price_case": 8, "_input_cost": 0.01, "_output_cost": 0.03},
     "gpt-4-1106-vision-preview": {"price_case": 8, "_input_cost": 0.01, "_output_cost": 0.03},
     "gpt-4-turbo-2024-04-09": {"price_case": 8, "_input_cost": 0.01, "_output_cost": 0.03},
+
+    ## Grouping GPT-4o models together
+    "gpt-4o-2024-05-13": {"price_case": 10, "_input_cost": 0.005, "_output_cost": 0.015},
     
-    # Grouping Gemini models together
+    ## Grouping Gemini models together
     "gemini-1.0-pro-001": {"price_case": 9, "_input_cost": 0.0, "_output_cost": 0.0},
     "gemini-1.0-pro-vision-001": {"price_case": 9, "_input_cost": 0.0, "_output_cost": 0.0},
     "gemini-1.0-pro": {"price_case": 9, "_input_cost": 0.0, "_output_cost": 0.0},
     "gemini-1.0-pro-vision": {"price_case": 9, "_input_cost": 0.0, "_output_cost": 0.0},
     "gemini-1.0-pro-latest": {"price_case": 9, "_input_cost": 0.0, "_output_cost": 0.0},
     "gemini-1.0-pro-vision-latest": {"price_case": 9, "_input_cost": 0.0, "_output_cost": 0.0},
     "gemini-1.5-pro-latest": {"price_case": 9, "_input_cost": 0.0, "_output_cost": 0.0},
```

### Comparing `easytl-0.3.1/src/easytl.egg-info/PKG-INFO` & `easytl-0.3.2/src/easytl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easytl
-Version: 0.3.1
+Version: 0.3.2
 Summary: Seamless Multi-API Translation: Simplifying Language Barriers with DeepL, OpenAI, Gemini and Google Translate.
 Author-email: Bikatr7 <Bikatr7@proton.me>
 Project-URL: Homepage, https://github.com/Bikatr7/EasyTL
 Project-URL: Issues, https://github.com/Bikatr7/EasyTL/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `easytl-0.3.1/src/easytl.egg-info/SOURCES.txt` & `easytl-0.3.2/src/easytl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `easytl-0.3.1/tests/issue_template.py` & `easytl-0.3.2/tests/issue_template.py`

 * *Files identical despite different names*

### Comparing `easytl-0.3.1/tests/passing.py` & `easytl-0.3.2/tests/passing.py`

 * *Files identical despite different names*

