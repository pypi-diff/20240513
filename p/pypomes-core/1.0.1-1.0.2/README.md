# Comparing `tmp/pypomes_core-1.0.1.tar.gz` & `tmp/pypomes_core-1.0.2.tar.gz`

## Comparing `pypomes_core-1.0.1.tar` & `pypomes_core-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     6919 2020-02-02 00:00:00.000000 pypomes_core-1.0.1/src/pypomes_core/.ruff.toml
--rw-r--r--   0        0        0     3807 2020-02-02 00:00:00.000000 pypomes_core-1.0.1/src/pypomes_core/__init__.py
--rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 pypomes_core-1.0.1/src/pypomes_core/datetime_pomes.py
--rw-r--r--   0        0        0    28318 2020-02-02 00:00:00.000000 pypomes_core-1.0.1/src/pypomes_core/dict_pomes.py
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 pypomes_core-1.0.1/src/pypomes_core/email_pomes.py
--rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 pypomes_core-1.0.1/src/pypomes_core/encoding_pomes.py
--rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 pypomes_core-1.0.1/src/pypomes_core/env_pomes.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pypomes_core-1.0.1/src/pypomes_core/exception_pomes.py
--rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 pypomes_core-1.0.1/src/pypomes_core/file_pomes.py
--rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 pypomes_core-1.0.1/src/pypomes_core/json_pomes.py
--rw-r--r--   0        0        0     6328 2020-02-02 00:00:00.000000 pypomes_core-1.0.1/src/pypomes_core/list_pomes.py
--rw-r--r--   0        0        0     4199 2020-02-02 00:00:00.000000 pypomes_core-1.0.1/src/pypomes_core/str_pomes.py
--rw-r--r--   0        0        0     5417 2020-02-02 00:00:00.000000 pypomes_core-1.0.1/src/pypomes_core/validation_msgs.py
--rw-r--r--   0        0        0    24625 2020-02-02 00:00:00.000000 pypomes_core-1.0.1/src/pypomes_core/validation_pomes.py
--rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 pypomes_core-1.0.1/src/pypomes_core/xml_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_core-1.0.1/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_core-1.0.1/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_core-1.0.1/README.md
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pypomes_core-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pypomes_core-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     6919 2020-02-02 00:00:00.000000 pypomes_core-1.0.2/src/pypomes_core/.ruff.toml
+-rw-r--r--   0        0        0     3807 2020-02-02 00:00:00.000000 pypomes_core-1.0.2/src/pypomes_core/__init__.py
+-rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 pypomes_core-1.0.2/src/pypomes_core/datetime_pomes.py
+-rw-r--r--   0        0        0    28318 2020-02-02 00:00:00.000000 pypomes_core-1.0.2/src/pypomes_core/dict_pomes.py
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 pypomes_core-1.0.2/src/pypomes_core/email_pomes.py
+-rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 pypomes_core-1.0.2/src/pypomes_core/encoding_pomes.py
+-rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 pypomes_core-1.0.2/src/pypomes_core/env_pomes.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pypomes_core-1.0.2/src/pypomes_core/exception_pomes.py
+-rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 pypomes_core-1.0.2/src/pypomes_core/file_pomes.py
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 pypomes_core-1.0.2/src/pypomes_core/json_pomes.py
+-rw-r--r--   0        0        0     6328 2020-02-02 00:00:00.000000 pypomes_core-1.0.2/src/pypomes_core/list_pomes.py
+-rw-r--r--   0        0        0     4199 2020-02-02 00:00:00.000000 pypomes_core-1.0.2/src/pypomes_core/str_pomes.py
+-rw-r--r--   0        0        0     5417 2020-02-02 00:00:00.000000 pypomes_core-1.0.2/src/pypomes_core/validation_msgs.py
+-rw-r--r--   0        0        0    24781 2020-02-02 00:00:00.000000 pypomes_core-1.0.2/src/pypomes_core/validation_pomes.py
+-rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 pypomes_core-1.0.2/src/pypomes_core/xml_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_core-1.0.2/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_core-1.0.2/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_core-1.0.2/README.md
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pypomes_core-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pypomes_core-1.0.2/PKG-INFO
```

### Comparing `pypomes_core-1.0.1/src/pypomes_core/.ruff.toml` & `pypomes_core-1.0.2/src/pypomes_core/.ruff.toml`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.1/src/pypomes_core/__init__.py` & `pypomes_core-1.0.2/src/pypomes_core/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.1/src/pypomes_core/datetime_pomes.py` & `pypomes_core-1.0.2/src/pypomes_core/datetime_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.1/src/pypomes_core/dict_pomes.py` & `pypomes_core-1.0.2/src/pypomes_core/dict_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.1/src/pypomes_core/email_pomes.py` & `pypomes_core-1.0.2/src/pypomes_core/email_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.1/src/pypomes_core/encoding_pomes.py` & `pypomes_core-1.0.2/src/pypomes_core/encoding_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.1/src/pypomes_core/env_pomes.py` & `pypomes_core-1.0.2/src/pypomes_core/env_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.1/src/pypomes_core/exception_pomes.py` & `pypomes_core-1.0.2/src/pypomes_core/exception_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.1/src/pypomes_core/file_pomes.py` & `pypomes_core-1.0.2/src/pypomes_core/file_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.1/src/pypomes_core/json_pomes.py` & `pypomes_core-1.0.2/src/pypomes_core/json_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.1/src/pypomes_core/list_pomes.py` & `pypomes_core-1.0.2/src/pypomes_core/list_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.1/src/pypomes_core/str_pomes.py` & `pypomes_core-1.0.2/src/pypomes_core/str_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.1/src/pypomes_core/validation_msgs.py` & `pypomes_core-1.0.2/src/pypomes_core/validation_msgs.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.1/src/pypomes_core/validation_pomes.py` & `pypomes_core-1.0.2/src/pypomes_core/validation_pomes.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,14 +153,18 @@
     stat: str | None = None
     pos: int = attr.rfind(".") + 1
     suffix: str = attr[pos:]
 
     # retrieve the value
     result: int | None = scheme.get(suffix)
 
+    # handle the empty string
+    if result == "":
+        result = None
+
     # validate it
     if isinstance(result, str) and result.isnumeric():
         result = int(result)
     # bool is subtype of int
     elif result is not None and \
             (isinstance(result, bool) or not isinstance(result, int)):
         # 128: Invalid value {}: must be type {}
@@ -208,14 +212,18 @@
     stat: str | None = None
     pos: int = attr.rfind(".") + 1
     suffix: str = attr[pos:]
 
     # retrieve the value
     result: float | None = scheme.get(suffix)
 
+    # handle the empty string
+    if result == "":
+        result = None
+
     # validate it
     if isinstance(result, str) and result.replace(".", "", 1).isnumeric():
         result = float(result)
     elif result is not None and not isinstance(result, int) and not isinstance(result, float):
         # 128: Invalid value {}: must be type {}
         stat = validate_format_error(128, result, "float", f"@{attr}")
     else:
```

### Comparing `pypomes_core-1.0.1/src/pypomes_core/xml_pomes.py` & `pypomes_core-1.0.2/src/pypomes_core/xml_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.1/LICENSE` & `pypomes_core-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.1/pyproject.toml` & `pypomes_core-1.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_core"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (core modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_core-1.0.1/PKG-INFO` & `pypomes_core-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypomes_core
-Version: 1.0.1
+Version: 1.0.2
 Summary: A collection of Python pomes, pennyeach (core modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-Core
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-Core/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

