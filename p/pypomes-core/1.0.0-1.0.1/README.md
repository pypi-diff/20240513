# Comparing `tmp/pypomes_core-1.0.0.tar.gz` & `tmp/pypomes_core-1.0.1.tar.gz`

## Comparing `pypomes_core-1.0.0.tar` & `pypomes_core-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     6919 2020-02-02 00:00:00.000000 pypomes_core-1.0.0/src/pypomes_core/.ruff.toml
--rw-r--r--   0        0        0     3807 2020-02-02 00:00:00.000000 pypomes_core-1.0.0/src/pypomes_core/__init__.py
--rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 pypomes_core-1.0.0/src/pypomes_core/datetime_pomes.py
--rw-r--r--   0        0        0    28318 2020-02-02 00:00:00.000000 pypomes_core-1.0.0/src/pypomes_core/dict_pomes.py
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 pypomes_core-1.0.0/src/pypomes_core/email_pomes.py
--rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 pypomes_core-1.0.0/src/pypomes_core/encoding_pomes.py
--rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 pypomes_core-1.0.0/src/pypomes_core/env_pomes.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pypomes_core-1.0.0/src/pypomes_core/exception_pomes.py
--rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 pypomes_core-1.0.0/src/pypomes_core/file_pomes.py
--rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 pypomes_core-1.0.0/src/pypomes_core/json_pomes.py
--rw-r--r--   0        0        0     6328 2020-02-02 00:00:00.000000 pypomes_core-1.0.0/src/pypomes_core/list_pomes.py
--rw-r--r--   0        0        0     4199 2020-02-02 00:00:00.000000 pypomes_core-1.0.0/src/pypomes_core/str_pomes.py
--rw-r--r--   0        0        0     5417 2020-02-02 00:00:00.000000 pypomes_core-1.0.0/src/pypomes_core/validation_msgs.py
--rw-r--r--   0        0        0    24392 2020-02-02 00:00:00.000000 pypomes_core-1.0.0/src/pypomes_core/validation_pomes.py
--rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 pypomes_core-1.0.0/src/pypomes_core/xml_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_core-1.0.0/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_core-1.0.0/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_core-1.0.0/README.md
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pypomes_core-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pypomes_core-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     6919 2020-02-02 00:00:00.000000 pypomes_core-1.0.1/src/pypomes_core/.ruff.toml
+-rw-r--r--   0        0        0     3807 2020-02-02 00:00:00.000000 pypomes_core-1.0.1/src/pypomes_core/__init__.py
+-rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 pypomes_core-1.0.1/src/pypomes_core/datetime_pomes.py
+-rw-r--r--   0        0        0    28318 2020-02-02 00:00:00.000000 pypomes_core-1.0.1/src/pypomes_core/dict_pomes.py
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 pypomes_core-1.0.1/src/pypomes_core/email_pomes.py
+-rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 pypomes_core-1.0.1/src/pypomes_core/encoding_pomes.py
+-rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 pypomes_core-1.0.1/src/pypomes_core/env_pomes.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pypomes_core-1.0.1/src/pypomes_core/exception_pomes.py
+-rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 pypomes_core-1.0.1/src/pypomes_core/file_pomes.py
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 pypomes_core-1.0.1/src/pypomes_core/json_pomes.py
+-rw-r--r--   0        0        0     6328 2020-02-02 00:00:00.000000 pypomes_core-1.0.1/src/pypomes_core/list_pomes.py
+-rw-r--r--   0        0        0     4199 2020-02-02 00:00:00.000000 pypomes_core-1.0.1/src/pypomes_core/str_pomes.py
+-rw-r--r--   0        0        0     5417 2020-02-02 00:00:00.000000 pypomes_core-1.0.1/src/pypomes_core/validation_msgs.py
+-rw-r--r--   0        0        0    24625 2020-02-02 00:00:00.000000 pypomes_core-1.0.1/src/pypomes_core/validation_pomes.py
+-rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 pypomes_core-1.0.1/src/pypomes_core/xml_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_core-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_core-1.0.1/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_core-1.0.1/README.md
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pypomes_core-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pypomes_core-1.0.1/PKG-INFO
```

### Comparing `pypomes_core-1.0.0/src/pypomes_core/.ruff.toml` & `pypomes_core-1.0.1/src/pypomes_core/.ruff.toml`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.0/src/pypomes_core/__init__.py` & `pypomes_core-1.0.1/src/pypomes_core/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.0/src/pypomes_core/datetime_pomes.py` & `pypomes_core-1.0.1/src/pypomes_core/datetime_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.0/src/pypomes_core/dict_pomes.py` & `pypomes_core-1.0.1/src/pypomes_core/dict_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.0/src/pypomes_core/email_pomes.py` & `pypomes_core-1.0.1/src/pypomes_core/email_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.0/src/pypomes_core/encoding_pomes.py` & `pypomes_core-1.0.1/src/pypomes_core/encoding_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.0/src/pypomes_core/env_pomes.py` & `pypomes_core-1.0.1/src/pypomes_core/env_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.0/src/pypomes_core/exception_pomes.py` & `pypomes_core-1.0.1/src/pypomes_core/exception_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.0/src/pypomes_core/file_pomes.py` & `pypomes_core-1.0.1/src/pypomes_core/file_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.0/src/pypomes_core/json_pomes.py` & `pypomes_core-1.0.1/src/pypomes_core/json_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.0/src/pypomes_core/list_pomes.py` & `pypomes_core-1.0.1/src/pypomes_core/list_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.0/src/pypomes_core/str_pomes.py` & `pypomes_core-1.0.1/src/pypomes_core/str_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.0/src/pypomes_core/validation_msgs.py` & `pypomes_core-1.0.1/src/pypomes_core/validation_msgs.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.0/src/pypomes_core/validation_pomes.py` & `pypomes_core-1.0.1/src/pypomes_core/validation_pomes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from datetime import date, datetime
 from logging import Logger
-from typing import Final
+from typing import Any, Final
 from .datetime_pomes import TIMEZONE_LOCAL
 from .env_pomes import APP_PREFIX, env_get_str
 from .str_pomes import str_sanitize, str_find_whitespace
 
 VALIDATION_MSG_LANGUAGE: Final[str] = env_get_str(f"{APP_PREFIX}_VALIDATION_MSG_LANGUAGE", "en")
 VALIDATION_MSG_PREFIX: Final[str] = env_get_str(f"{APP_PREFIX}_VALIDATION_MSG_PREFIX", APP_PREFIX)
 
 
 def validate_value(attr: str,
                    val: str | int | float,
                    min_val: int = None,
                    max_val: int = None,
-                   default: bool | list[any] = None) -> str:
+                   default: bool | list[Any] = None) -> str:
     """
     Validate *val* according to value, range, or membership in values list, as specified.
 
     :param attr: the name of the attribute
     :param val: the value to be validated
     :param min_val: if val is a string, specifies its minimum length; otherwise, specifies its minimum value
     :param max_val: if val is a string, specifies its maximum length; otherwise, specifies its maximum value
@@ -26,30 +26,34 @@
     """
     # initialize the return variable
     result: str | None = None
 
     # 'val' can be None, and None can be in 'default'
     if isinstance(default, list):
         if val not in default:
-            if val is None:
+            if not val:
                 # 112: Required attribute
                 result = validate_format_error(112, f"@{attr}")
             else:
                 length: int = len(default)
                 if length == 1:
                     # 125: Invalid value {}: must be {}
                     result = validate_format_error(125, val, default[0], f"@{attr}")
                 else:
-                    # is 'None' the last element in list ?
-                    if default[-1] is None:
+                    # is 'None' or '' the last element in list ?
+                    if default[-1] in ("", None):
+                        # yes, omit it from the message
+                        length -= 1
+                    # again, is 'None' or '' the last element in list ?
+                    if default[-1] in ("", None):
                         # yes, omit it from the message
                         length -= 1
                     # 126: Invalid value {}: must be one of {}
                     result = validate_format_error(126, val, default[:length], f"@{attr}")
-    elif val is None:
+    elif not val:
         if isinstance(default, bool) and default:
             # 112: Required attribute
             result = validate_format_error(112, f"@{attr}")
     elif isinstance(val, str):
         length: int = len(val)
         if min_val is not None and max_val == min_val and length != min_val:
             # 124: Invalid value {}: length must be {}
@@ -260,15 +264,15 @@
     """
     stat: str | None = None
     pos: int = attr.rfind(".") + 1
     suffix: str = attr[pos:]
 
     # obtain and validate the value
     result: str | None = scheme.get(suffix)
-    if result is not None and not isinstance(result, str):
+    if result and not isinstance(result, str):
         # 128: Invalid value {}: must be type {}
         stat = validate_format_error(128, result, "str", f"@{attr}")
     elif isinstance(default, str):
         if result is None:
             result = default
         else:
             stat = validate_value(attr, result, min_length, max_length)
@@ -312,15 +316,15 @@
     pos: int = attr.rfind(".") + 1
     suffix: str = attr[pos:]
 
     # obtain and validate the value
     try:
         date_str: str = scheme[suffix]
         result = date_parse(date_str, dayfirst=day_first)
-        if result is None:
+        if not result:
             # 121: Invalid value {}
             stat = validate_format_error(121, date_str, f"@{attr}")
         elif result > datetime.now(TIMEZONE_LOCAL).date():
             # 129: Invalid value {}: date is later than the current date
             stat = validate_format_error(129, date_str, f"@{attr}")
     except KeyError:
         if isinstance(default, bool) and default:
@@ -365,15 +369,15 @@
     pos: int = attr.rfind(".") + 1
     suffix: str = attr[pos:]
 
     # obtain and validate the value
     try:
         date_str: str = scheme[suffix]
         result = datetime_parse(date_str, dayfirst=day_first)
-        if result is None:
+        if not result:
             # 121: Invalid value {}
             stat = validate_format_error(121, date_str, f"@{attr}")
         elif result > datetime.now(TIMEZONE_LOCAL):
             # 129: Invalid value {}: date is later than the current date
             stat = validate_format_error(129, date_str, f"@{attr}")
     except KeyError:
         if isinstance(default, bool) and default:
@@ -406,21 +410,21 @@
     :param min_val: the minimum value accepted
     :param max_val:  the maximum value accepted
     :param mandatory: whether the list of values must be provided
     :param logger: optional logger
     :return: the list of validated values, or None if validation failed
     """
     # initialize the return variable
-    result: list[any] | None = None
+    result: list[Any] | None = None
 
     stat: str | None = None
     pos: int = attr.rfind(".") + 1
     suffix: str = attr[pos:]
     try:
-        values: list[any] = scheme[suffix]
+        values: list[Any] = scheme[suffix]
         if isinstance(values, list):
             result = []
             if len(values) > 0:
                 for inx, value in enumerate(values):
                     result.append(value)
                     if isinstance(value, int):
                         stat = validate_value(f"@{attr}[{inx+1}]", value, min_val, max_val)
@@ -462,21 +466,21 @@
     :param min_length: the minimum length accepted
     :param max_length:  the maximum length accepted
     :param mandatory: whether the list of values must be provided
     :param logger: optional logger
     :return: the list of validated values, or None if validation failed
     """
     # initialize the return variable
-    result: list[any] | None = None
+    result: list[Any] | None = None
 
     stat: str | None = None
     pos: int = attr.rfind(".") + 1
     suffix: str = attr[pos:]
     try:
-        values: list[any] = scheme[suffix]
+        values: list[Any] = scheme[suffix]
         if isinstance(values, list):
             result = []
             if len(values) > 0:
                 for inx, value in enumerate(values):
                     result.append(value)
                     if isinstance(value, str):
                         stat = validate_value(f"@{attr}[{inx+1}]", value, min_length, max_length)
@@ -497,15 +501,15 @@
     if stat:
         __validate_log(errors, stat, logger)
 
     return result
 
 
 def validate_format_error(error_id: int,
-                          *args: any) -> str:
+                          *args: Any) -> str:
     """
     Format and return the error message identified by *err_id* in the standard messages list.
 
     The message is built from the message element in the standard messages list, identified by *err_id*.
     The occurrences of '{}' in the element are sequentially replaced by the given *args*.
 
     :param error_id: the identification of the message element
@@ -575,15 +579,15 @@
         else:
             # yes
             term: str = "attribute" if VALIDATION_MSG_LANGUAGE == "en" else "atributo"
             out_error: dict = {term: error[pos + 1:]}
             desc: str = error[:pos - 1]
 
         # does the text contain an error code ?
-        if desc.startswith(VALIDATION_MSG_PREFIX):
+        if VALIDATION_MSG_PREFIX and desc.startswith(VALIDATION_MSG_PREFIX):
             # yes
             term: str = "code" if VALIDATION_MSG_LANGUAGE == "en" else "codigo"
             pos: int = desc.find(":")
             out_error[term] = desc[0:pos]
             desc = desc[pos+2:]
 
         term: str = "description" if VALIDATION_MSG_LANGUAGE == "en" else "descricao"
```

### Comparing `pypomes_core-1.0.0/src/pypomes_core/xml_pomes.py` & `pypomes_core-1.0.1/src/pypomes_core/xml_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.0/LICENSE` & `pypomes_core-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.0/pyproject.toml` & `pypomes_core-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_core"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (core modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_core-1.0.0/PKG-INFO` & `pypomes_core-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypomes_core
-Version: 1.0.0
+Version: 1.0.1
 Summary: A collection of Python pomes, pennyeach (core modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-Core
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-Core/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

