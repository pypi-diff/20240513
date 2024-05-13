# Comparing `tmp/okta_expression_parser-0.2.0.tar.gz` & `tmp/okta_expression_parser-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "okta_expression_parser-0.2.0.tar", max compression
+gzip compressed data, was "okta_expression_parser-0.2.1.tar", max compression
```

## Comparing `okta_expression_parser-0.2.0.tar` & `okta_expression_parser-0.2.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       25 2024-02-07 18:36:50.904598 okta_expression_parser-0.2.0/README.md
--rw-r--r--   0        0        0        0 2024-01-24 17:39:56.968382 okta_expression_parser-0.2.0/okta_expression_parser/__init__.py
--rw-r--r--   0        0        0      153 2024-02-14 17:13:57.668654 okta_expression_parser-0.2.0/okta_expression_parser/expression_classes/__init__.py
--rw-r--r--   0        0        0     1737 2024-02-14 17:13:57.680267 okta_expression_parser-0.2.0/okta_expression_parser/expression_classes/arrays.py
--rw-r--r--   0        0        0      344 2024-02-14 14:53:37.731479 okta_expression_parser-0.2.0/okta_expression_parser/expression_classes/convert.py
--rw-r--r--   0        0        0      818 2024-02-14 17:13:57.677989 okta_expression_parser-0.2.0/okta_expression_parser/expression_classes/groups.py
--rw-r--r--   0        0        0    22766 2024-02-14 17:13:57.838616 okta_expression_parser-0.2.0/okta_expression_parser/expression_classes/iso3166convert.py
--rw-r--r--   0        0        0     3132 2024-02-14 17:13:57.703726 okta_expression_parser-0.2.0/okta_expression_parser/expression_classes/string.py
--rw-r--r--   0        0        0     1447 2024-02-14 15:49:07.639688 okta_expression_parser-0.2.0/okta_expression_parser/lexer.py
--rw-r--r--   0        0        0     9618 2024-02-14 17:16:40.270738 okta_expression_parser-0.2.0/okta_expression_parser/parser.py
--rw-r--r--   0        0        0      561 2024-02-13 20:45:38.266760 okta_expression_parser-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      505 1970-01-01 00:00:00.000000 okta_expression_parser-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       25 2024-02-07 18:36:50.904598 okta_expression_parser-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2024-01-24 17:39:56.968382 okta_expression_parser-0.2.1/okta_expression_parser/__init__.py
+-rw-r--r--   0        0        0      153 2024-02-14 17:13:57.668654 okta_expression_parser-0.2.1/okta_expression_parser/expression_classes/__init__.py
+-rw-r--r--   0        0        0     1737 2024-02-14 17:13:57.680267 okta_expression_parser-0.2.1/okta_expression_parser/expression_classes/arrays.py
+-rw-r--r--   0        0        0      344 2024-02-14 14:53:37.731479 okta_expression_parser-0.2.1/okta_expression_parser/expression_classes/convert.py
+-rw-r--r--   0        0        0      818 2024-02-14 17:13:57.677989 okta_expression_parser-0.2.1/okta_expression_parser/expression_classes/groups.py
+-rw-r--r--   0        0        0    22766 2024-02-14 17:13:57.838616 okta_expression_parser-0.2.1/okta_expression_parser/expression_classes/iso3166convert.py
+-rw-r--r--   0        0        0     3259 2024-05-13 17:46:42.187846 okta_expression_parser-0.2.1/okta_expression_parser/expression_classes/string.py
+-rw-r--r--   0        0        0     1447 2024-02-14 15:49:07.639688 okta_expression_parser-0.2.1/okta_expression_parser/lexer.py
+-rw-r--r--   0        0        0     9618 2024-02-14 17:16:40.270738 okta_expression_parser-0.2.1/okta_expression_parser/parser.py
+-rw-r--r--   0        0        0      561 2024-05-13 17:39:34.805943 okta_expression_parser-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      505 1970-01-01 00:00:00.000000 okta_expression_parser-0.2.1/PKG-INFO
```

### Comparing `okta_expression_parser-0.2.0/okta_expression_parser/expression_classes/arrays.py` & `okta_expression_parser-0.2.1/okta_expression_parser/expression_classes/arrays.py`

 * *Files identical despite different names*

### Comparing `okta_expression_parser-0.2.0/okta_expression_parser/expression_classes/groups.py` & `okta_expression_parser-0.2.1/okta_expression_parser/expression_classes/groups.py`

 * *Files identical despite different names*

### Comparing `okta_expression_parser-0.2.0/okta_expression_parser/expression_classes/iso3166convert.py` & `okta_expression_parser-0.2.1/okta_expression_parser/expression_classes/iso3166convert.py`

 * *Files identical despite different names*

### Comparing `okta_expression_parser-0.2.0/okta_expression_parser/expression_classes/string.py` & `okta_expression_parser-0.2.1/okta_expression_parser/expression_classes/string.py`

 * *Files 5% similar despite different names*

```diff
@@ -83,29 +83,35 @@
 
             if k in val:
                 return v
 
         return default
 
     @classmethod
-    def substring(val: str, start: int, end: int):
+    def substring(self, val: str, start: int, end: int):
         """Return a substring of val starting at index start"""
+        if not isinstance(val, str):
+            return ""
+
+        if end > len(val):
+            end = -1
+
         return val[int(start) : int(end)]
 
     @classmethod
-    def substringAfter(val: str, search: str):
+    def substringAfter(self, val: str, search: str):
         try:
             start = str(val).index(str(search))
         except ValueError:
             return val
 
         return val[start:]
 
     @classmethod
-    def substringBefore(val: str, search: str):
+    def substringBefore(self, val: str, search: str):
         """Return substring of val starting after the index of search string"""
         try:
             end = str(val).index(str(search))
         except ValueError:
             return val
 
         return val[0:end]
```

### Comparing `okta_expression_parser-0.2.0/okta_expression_parser/lexer.py` & `okta_expression_parser-0.2.1/okta_expression_parser/lexer.py`

 * *Files identical despite different names*

### Comparing `okta_expression_parser-0.2.0/okta_expression_parser/parser.py` & `okta_expression_parser-0.2.1/okta_expression_parser/parser.py`

 * *Files identical despite different names*

### Comparing `okta_expression_parser-0.2.0/pyproject.toml` & `okta_expression_parser-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "okta-expression-parser"
-version = "0.2.0"
+version = "0.2.1"
 description = "Returns a boolean by passing Okta profile data to an Okta Expression using Okta Expression Language"
 authors = ["Mathew Moon <me@mathewmoon.net>"]
 readme = "README.md"
 packages = [{include = "okta_expression_parser", from = "."}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

