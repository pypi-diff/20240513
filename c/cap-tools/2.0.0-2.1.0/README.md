# Comparing `tmp/cap_tools-2.0.0.tar.gz` & `tmp/cap_tools-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cap_tools-2.0.0.tar", max compression
+gzip compressed data, was "cap_tools-2.1.0.tar", max compression
```

## Comparing `cap_tools-2.0.0.tar` & `cap_tools-2.1.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1069 2024-05-11 10:01:41.827620 cap_tools-2.0.0/LICENSE
--rw-r--r--   0        0        0      681 2024-05-11 10:01:41.827620 cap_tools-2.0.0/README.md
--rw-r--r--   0        0        0     1894 2024-05-11 10:01:41.827620 cap_tools-2.0.0/pyproject.toml
--rw-r--r--   0        0        0      530 2024-05-11 10:01:41.827620 cap_tools-2.0.0/src/cap_tools/__init__.py
--rw-r--r--   0        0        0    14249 2024-05-11 10:01:41.827620 cap_tools-2.0.0/src/cap_tools/models.py
--rw-r--r--   0        0        0     1170 1970-01-01 00:00:00.000000 cap_tools-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-13 21:56:59.062970 cap_tools-2.1.0/LICENSE
+-rw-r--r--   0        0        0      681 2024-05-13 21:56:59.062970 cap_tools-2.1.0/README.md
+-rw-r--r--   0        0        0     1894 2024-05-13 21:56:59.062970 cap_tools-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0      530 2024-05-13 21:56:59.062970 cap_tools-2.1.0/src/cap_tools/__init__.py
+-rw-r--r--   0        0        0    14800 2024-05-13 21:56:59.062970 cap_tools-2.1.0/src/cap_tools/models.py
+-rw-r--r--   0        0        0     1170 1970-01-01 00:00:00.000000 cap_tools-2.1.0/PKG-INFO
```

### Comparing `cap_tools-2.0.0/LICENSE` & `cap_tools-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cap_tools-2.0.0/README.md` & `cap_tools-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `cap_tools-2.0.0/pyproject.toml` & `cap_tools-2.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 update_changelog_on_bump = true
 
 [tool.coverage.run]
 source = ["src", "tests"]
 
 [tool.poetry]
 name = "cap-tools"
-version = "2.0.0"
+version = "2.1.0"
 description = "Python data bindings for the Common Alerting Protocol Version."
 authors = ["Björn Reetz <git@bjoern-reetz.de>"]
 readme = "README.md"
 packages = [{include = "cap_tools", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `cap_tools-2.0.0/src/cap_tools/__init__.py` & `cap_tools-2.1.0/src/cap_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `cap_tools-2.0.0/src/cap_tools/models.py` & `cap_tools-2.1.0/src/cap_tools/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -446,17 +446,30 @@
             "name": "area",
             "type": "Element",
             "namespace": "urn:oasis:names:tc:emergency:cap:1.2",
         },
     )
 
     def get_language(self) -> str:
+        """Get the language of this Info.
+
+        If the language is not explicitly set,
+        "en-US" is returned as per CAP spec v1.2.
+        """
         return DEFAULT_LANGUAGE if self.language is None else self.language
 
     def set_language(self, language: str | None) -> None:
+        """Set the language of this Info.
+
+        Using this method to set the language to the default language (i.e. passing "en-US" as argument)
+        will set `Info.language` to `None`. Retrieving the language then via `Info.get_language`
+        will correctly return "en-US".
+
+        If you want to set the language to 'en-US' explicitly, use `Info.language = "en-US"` instead.
+        """
         self.language = None if language == DEFAULT_LANGUAGE else language
 
     def event_codes_to_dict(self) -> dict[str, str]:
         return {
             event_code.value_name.value: event_code.value.value
             for event_code in self.event_codes
         }
```

### Comparing `cap_tools-2.0.0/PKG-INFO` & `cap_tools-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cap-tools
-Version: 2.0.0
+Version: 2.1.0
 Summary: Python data bindings for the Common Alerting Protocol Version.
 Author: Björn Reetz
 Author-email: git@bjoern-reetz.de
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

