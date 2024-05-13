# Comparing `tmp/dyno_viewer-0.21.3.tar.gz` & `tmp/dyno_viewer-0.21.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dyno_viewer-0.21.3.tar", max compression
+gzip compressed data, was "dyno_viewer-0.21.4.tar", max compression
```

## Comparing `dyno_viewer-0.21.3.tar` & `dyno_viewer-0.21.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1067 2024-02-27 03:38:39.225651 dyno_viewer-0.21.3/LICENSE
--rw-r--r--   0        0        0     2390 2024-02-27 03:38:39.225651 dyno_viewer-0.21.3/README.md
--rw-r--r--   0        0        0       58 2024-02-27 03:38:39.225651 dyno_viewer-0.21.3/dyno_viewer/__main__.py
--rw-r--r--   0        0        0    10416 2024-02-27 03:38:39.225651 dyno_viewer-0.21.3/dyno_viewer/app.py
--rw-r--r--   0        0        0      181 2024-02-27 03:38:39.225651 dyno_viewer-0.21.3/dyno_viewer/app_types.py
--rw-r--r--   0        0        0     7792 2024-02-27 03:38:39.225651 dyno_viewer-0.21.3/dyno_viewer/aws/ddb.py
--rw-r--r--   0        0        0      211 2024-02-27 03:38:39.225651 dyno_viewer-0.21.3/dyno_viewer/aws/session.py
--rw-r--r--   0        0        0      558 2024-02-27 03:38:39.225651 dyno_viewer-0.21.3/dyno_viewer/components/css/query.css
--rw-r--r--   0        0        0       56 2024-02-27 03:38:39.225651 dyno_viewer-0.21.3/dyno_viewer/components/css/table.css
--rw-r--r--   0        0        0      390 2024-02-27 03:38:39.225651 dyno_viewer-0.21.3/dyno_viewer/components/help/help-doc.md
--rw-r--r--   0        0        0     2233 2024-02-27 03:38:39.225651 dyno_viewer-0.21.3/dyno_viewer/components/query/filter_query.py
--rw-r--r--   0        0        0     2440 2024-02-27 03:38:39.225651 dyno_viewer-0.21.3/dyno_viewer/components/query/key_filter.py
--rw-r--r--   0        0        0     2057 2024-02-27 03:38:39.225651 dyno_viewer-0.21.3/dyno_viewer/components/query/sort_key_filter.py
--rw-r--r--   0        0        0      149 2024-02-27 03:38:39.225651 dyno_viewer-0.21.3/dyno_viewer/components/screens/__init__.py
--rw-r--r--   0        0        0      794 2024-02-27 03:38:39.225651 dyno_viewer-0.21.3/dyno_viewer/components/screens/error.py
--rw-r--r--   0        0        0      576 2024-02-27 03:38:39.225651 dyno_viewer-0.21.3/dyno_viewer/components/screens/help.py
--rw-r--r--   0        0        0      912 2024-02-27 03:38:39.229651 dyno_viewer-0.21.3/dyno_viewer/components/screens/profile_select.py
--rw-r--r--   0        0        0     6497 2024-02-27 03:38:39.229651 dyno_viewer-0.21.3/dyno_viewer/components/screens/query.py
--rw-r--r--   0        0        0      857 2024-02-27 03:38:39.229651 dyno_viewer-0.21.3/dyno_viewer/components/screens/region_select.py
--rw-r--r--   0        0        0     4341 2024-02-27 03:38:39.229651 dyno_viewer-0.21.3/dyno_viewer/components/screens/table_select.py
--rw-r--r--   0        0        0     2177 2024-02-27 03:38:39.229651 dyno_viewer-0.21.3/dyno_viewer/components/table.py
--rw-r--r--   0        0        0       20 2024-02-27 03:38:39.229651 dyno_viewer-0.21.3/dyno_viewer/util/__init__.py
--rw-r--r--   0        0        0      565 2024-02-27 03:38:39.229651 dyno_viewer-0.21.3/dyno_viewer/util/util.py
--rw-r--r--   0        0        0     1085 2024-02-27 03:39:00.393632 dyno_viewer-0.21.3/pyproject.toml
--rw-r--r--   0        0        0     3040 1970-01-01 00:00:00.000000 dyno_viewer-0.21.3/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-13 00:58:15.717985 dyno_viewer-0.21.4/LICENSE
+-rw-r--r--   0        0        0     2390 2024-05-13 00:58:15.717985 dyno_viewer-0.21.4/README.md
+-rw-r--r--   0        0        0       58 2024-05-13 00:58:15.717985 dyno_viewer-0.21.4/dyno_viewer/__main__.py
+-rw-r--r--   0        0        0    10418 2024-05-13 00:58:15.717985 dyno_viewer-0.21.4/dyno_viewer/app.py
+-rw-r--r--   0        0        0      181 2024-05-13 00:58:15.717985 dyno_viewer-0.21.4/dyno_viewer/app_types.py
+-rw-r--r--   0        0        0     7792 2024-05-13 00:58:15.717985 dyno_viewer-0.21.4/dyno_viewer/aws/ddb.py
+-rw-r--r--   0        0        0      211 2024-05-13 00:58:15.717985 dyno_viewer-0.21.4/dyno_viewer/aws/session.py
+-rw-r--r--   0        0        0      558 2024-05-13 00:58:15.721985 dyno_viewer-0.21.4/dyno_viewer/components/css/query.tcss
+-rw-r--r--   0        0        0       56 2024-05-13 00:58:15.721985 dyno_viewer-0.21.4/dyno_viewer/components/css/table.tcss
+-rw-r--r--   0        0        0      390 2024-05-13 00:58:15.721985 dyno_viewer-0.21.4/dyno_viewer/components/help/help-doc.md
+-rw-r--r--   0        0        0     2233 2024-05-13 00:58:15.721985 dyno_viewer-0.21.4/dyno_viewer/components/query/filter_query.py
+-rw-r--r--   0        0        0     2440 2024-05-13 00:58:15.721985 dyno_viewer-0.21.4/dyno_viewer/components/query/key_filter.py
+-rw-r--r--   0        0        0     2057 2024-05-13 00:58:15.721985 dyno_viewer-0.21.4/dyno_viewer/components/query/sort_key_filter.py
+-rw-r--r--   0        0        0      149 2024-05-13 00:58:15.721985 dyno_viewer-0.21.4/dyno_viewer/components/screens/__init__.py
+-rw-r--r--   0        0        0      794 2024-05-13 00:58:15.721985 dyno_viewer-0.21.4/dyno_viewer/components/screens/error.py
+-rw-r--r--   0        0        0      576 2024-05-13 00:58:15.721985 dyno_viewer-0.21.4/dyno_viewer/components/screens/help.py
+-rw-r--r--   0        0        0      912 2024-05-13 00:58:15.721985 dyno_viewer-0.21.4/dyno_viewer/components/screens/profile_select.py
+-rw-r--r--   0        0        0     6497 2024-05-13 00:58:15.721985 dyno_viewer-0.21.4/dyno_viewer/components/screens/query.py
+-rw-r--r--   0        0        0      857 2024-05-13 00:58:15.721985 dyno_viewer-0.21.4/dyno_viewer/components/screens/region_select.py
+-rw-r--r--   0        0        0     4341 2024-05-13 00:58:15.721985 dyno_viewer-0.21.4/dyno_viewer/components/screens/table_select.py
+-rw-r--r--   0        0        0     2177 2024-05-13 00:58:15.721985 dyno_viewer-0.21.4/dyno_viewer/components/table.py
+-rw-r--r--   0        0        0       20 2024-05-13 00:58:15.721985 dyno_viewer-0.21.4/dyno_viewer/util/__init__.py
+-rw-r--r--   0        0        0      565 2024-05-13 00:58:15.721985 dyno_viewer-0.21.4/dyno_viewer/util/util.py
+-rw-r--r--   0        0        0     1085 2024-05-13 00:58:37.117987 dyno_viewer-0.21.4/pyproject.toml
+-rw-r--r--   0        0        0     3040 1970-01-01 00:00:00.000000 dyno_viewer-0.21.4/PKG-INFO
```

### Comparing `dyno_viewer-0.21.3/LICENSE` & `dyno_viewer-0.21.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dyno_viewer-0.21.3/README.md` & `dyno_viewer-0.21.4/README.md`

 * *Files identical despite different names*

### Comparing `dyno_viewer-0.21.3/dyno_viewer/app.py` & `dyno_viewer-0.21.4/dyno_viewer/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         "tableSelect": TableSelectScreen(),
         "regionSelect": RegionSelectScreen(),
         "profile": ProfileSelectScreen(),
         "query": QueryScreen(),
         "help": HelpMenu(),
     }
 
-    CSS_PATH = ["components/css/query.css", "components/css/table.css"]
+    CSS_PATH = ["components/css/query.tcss", "components/css/table.tcss"]
 
     profiles = reactive(get_available_profiles())
 
     aws_profile = reactive(None)
 
     table_name = reactive("")
```

### Comparing `dyno_viewer-0.21.3/dyno_viewer/aws/ddb.py` & `dyno_viewer-0.21.4/dyno_viewer/aws/ddb.py`

 * *Files identical despite different names*

### Comparing `dyno_viewer-0.21.3/dyno_viewer/components/css/query.css` & `dyno_viewer-0.21.4/dyno_viewer/components/css/query.tcss`

 * *Files identical despite different names*

### Comparing `dyno_viewer-0.21.3/dyno_viewer/components/query/filter_query.py` & `dyno_viewer-0.21.4/dyno_viewer/components/query/filter_query.py`

 * *Files identical despite different names*

### Comparing `dyno_viewer-0.21.3/dyno_viewer/components/query/key_filter.py` & `dyno_viewer-0.21.4/dyno_viewer/components/query/key_filter.py`

 * *Files identical despite different names*

### Comparing `dyno_viewer-0.21.3/dyno_viewer/components/query/sort_key_filter.py` & `dyno_viewer-0.21.4/dyno_viewer/components/query/sort_key_filter.py`

 * *Files identical despite different names*

### Comparing `dyno_viewer-0.21.3/dyno_viewer/components/screens/error.py` & `dyno_viewer-0.21.4/dyno_viewer/components/screens/error.py`

 * *Files identical despite different names*

### Comparing `dyno_viewer-0.21.3/dyno_viewer/components/screens/help.py` & `dyno_viewer-0.21.4/dyno_viewer/components/screens/help.py`

 * *Files identical despite different names*

### Comparing `dyno_viewer-0.21.3/dyno_viewer/components/screens/profile_select.py` & `dyno_viewer-0.21.4/dyno_viewer/components/screens/profile_select.py`

 * *Files identical despite different names*

### Comparing `dyno_viewer-0.21.3/dyno_viewer/components/screens/query.py` & `dyno_viewer-0.21.4/dyno_viewer/components/screens/query.py`

 * *Files identical despite different names*

### Comparing `dyno_viewer-0.21.3/dyno_viewer/components/screens/region_select.py` & `dyno_viewer-0.21.4/dyno_viewer/components/screens/region_select.py`

 * *Files identical despite different names*

### Comparing `dyno_viewer-0.21.3/dyno_viewer/components/screens/table_select.py` & `dyno_viewer-0.21.4/dyno_viewer/components/screens/table_select.py`

 * *Files identical despite different names*

### Comparing `dyno_viewer-0.21.3/dyno_viewer/components/table.py` & `dyno_viewer-0.21.4/dyno_viewer/components/table.py`

 * *Files identical despite different names*

### Comparing `dyno_viewer-0.21.3/dyno_viewer/util/util.py` & `dyno_viewer-0.21.4/dyno_viewer/util/util.py`

 * *Files identical despite different names*

### Comparing `dyno_viewer-0.21.3/pyproject.toml` & `dyno_viewer-0.21.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "dyno-viewer"
-version = "0.21.3"
+version = "0.21.4"
 description = ""
 authors = ["Rowan Self <piesrule123@gmail.com>"]
 readme = "README.md"
 packages = [{include = "dyno_viewer"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 boto3 = "^1.26.135"
 simplejson = "^3.19.1"
 dynamodb-json = "^1.3"
 pyclip = "^0.7.0"
-textual = ">=0.24.1,<0.53.0"
+textual = ">=0.24.1,<0.60.0"
 
 
 [tool.poetry.group.dev.dependencies]
 black = ">=23.3,<25.0"
 ipykernel = "^6.22.0"
 pytest = ">=7.3.1,<9.0.0"
 moto = {extras = ["all"], version = "^4.1.9"}
```

### Comparing `dyno_viewer-0.21.3/PKG-INFO` & `dyno_viewer-0.21.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: dyno-viewer
-Version: 0.21.3
+Version: 0.21.4
 Summary: 
 Author: Rowan Self
 Author-email: piesrule123@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: boto3 (>=1.26.135,<2.0.0)
 Requires-Dist: dynamodb-json (>=1.3,<2.0)
 Requires-Dist: pyclip (>=0.7.0,<0.8.0)
 Requires-Dist: simplejson (>=3.19.1,<4.0.0)
-Requires-Dist: textual (>=0.24.1,<0.53.0)
+Requires-Dist: textual (>=0.24.1,<0.60.0)
 Description-Content-Type: text/markdown
 
 ![screenshot](dyno-viewer-screenshot.png)
 # Dyno-viewer
 
 Dyno-viewer is dynamodb table viewer for your terminal build using [textual](https://github.com/Textualize/textual).
```

