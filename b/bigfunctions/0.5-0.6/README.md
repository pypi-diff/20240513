# Comparing `tmp/bigfunctions-0.5.tar.gz` & `tmp/bigfunctions-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigfunctions-0.5.tar", last modified: Mon May 13 12:50:19 2024, max compression
+gzip compressed data, was "bigfunctions-0.6.tar", last modified: Mon May 13 14:59:48 2024, max compression
```

## Comparing `bigfunctions-0.5.tar` & `bigfunctions-0.6.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-05-13 12:50:19.496251 bigfunctions-0.5/
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     1064 2023-11-08 21:20:23.000000 bigfunctions-0.5/LICENSE
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     9822 2024-05-13 12:50:19.495251 bigfunctions-0.5/PKG-INFO
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     9097 2024-02-22 22:16:20.000000 bigfunctions-0.5/README.md
-drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-05-13 12:50:19.151225 bigfunctions-0.5/bigfun/
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2023-11-08 21:20:23.000000 bigfunctions-0.5/bigfun/__init__.py
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     8507 2024-05-10 19:42:48.000000 bigfunctions-0.5/bigfun/bigfunctions.py
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     9663 2024-05-10 19:32:19.000000 bigfunctions-0.5/bigfun/cli.py
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      844 2023-12-01 17:33:50.000000 bigfunctions-0.5/bigfun/load_table.py
-drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-05-13 12:50:19.302236 bigfunctions-0.5/bigfun/templates/
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     1086 2023-11-08 21:20:23.000000 bigfunctions-0.5/bigfun/templates/Dockerfile
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)    11722 2024-05-10 19:28:43.000000 bigfunctions-0.5/bigfun/templates/bigfunction.md
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     3784 2024-01-19 20:34:23.000000 bigfunctions-0.5/bigfun/templates/bookmarklet.js
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     1618 2024-05-10 09:49:39.000000 bigfunctions-0.5/bigfun/templates/categories.md
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     4164 2024-01-24 23:20:01.000000 bigfunctions-0.5/bigfun/templates/data.md
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      554 2024-02-23 19:54:09.000000 bigfunctions-0.5/bigfun/templates/function_js.sql
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     7724 2024-02-23 21:48:51.000000 bigfunctions-0.5/bigfun/templates/function_py.py
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      316 2024-02-23 19:48:03.000000 bigfunctions-0.5/bigfun/templates/function_py.sql
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      212 2024-02-23 21:42:39.000000 bigfunctions-0.5/bigfun/templates/function_py_test.py
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      410 2024-02-23 19:54:09.000000 bigfunctions-0.5/bigfun/templates/function_sql.sql
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      251 2024-02-23 22:59:01.000000 bigfunctions-0.5/bigfun/templates/function_sql_test.sql
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      702 2024-02-23 19:54:09.000000 bigfunctions-0.5/bigfun/templates/procedure.sql
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      717 2024-02-23 22:23:06.000000 bigfunctions-0.5/bigfun/templates/procedure_test.sql
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      345 2024-02-23 19:54:09.000000 bigfunctions-0.5/bigfun/templates/table_function.sql
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)    13269 2024-05-10 19:41:56.000000 bigfunctions-0.5/bigfun/utils.py
-drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-05-13 12:50:19.303236 bigfunctions-0.5/bigfun/website/
-drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-05-13 12:50:19.468249 bigfunctions-0.5/bigfun/website/assets/
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     1714 2023-11-29 13:48:58.000000 bigfunctions-0.5/bigfun/website/assets/GitHub-Mark-32px.png
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)  1353755 2024-01-19 20:34:23.000000 bigfunctions-0.5/bigfun/website/assets/bookmarklet_usage.gif
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)    23806 2023-11-29 13:48:58.000000 bigfunctions-0.5/bigfun/website/assets/logo.png
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)    73519 2023-11-29 13:48:58.000000 bigfunctions-0.5/bigfun/website/assets/logo_and_name.png
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)    49771 2023-11-29 13:48:58.000000 bigfunctions-0.5/bigfun/website/assets/logo_and_name_wo_supercharge.png
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     1712 2024-05-10 18:53:52.000000 bigfunctions-0.5/bigfun/website/mkdocs.yml
-drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-05-13 12:50:19.476249 bigfunctions-0.5/bigfun/website/theme_overrides/
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     6185 2024-05-10 12:11:21.000000 bigfunctions-0.5/bigfun/website/theme_overrides/main.html
-drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-05-13 12:50:19.495251 bigfunctions-0.5/bigfunctions.egg-info/
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     9822 2024-05-13 12:50:19.000000 bigfunctions-0.5/bigfunctions.egg-info/PKG-INFO
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     1076 2024-05-13 12:50:19.000000 bigfunctions-0.5/bigfunctions.egg-info/SOURCES.txt
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)        1 2024-05-13 12:50:19.000000 bigfunctions-0.5/bigfunctions.egg-info/dependency_links.txt
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)       42 2024-05-13 12:50:19.000000 bigfunctions-0.5/bigfunctions.egg-info/entry_points.txt
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      130 2024-05-13 12:50:19.000000 bigfunctions-0.5/bigfunctions.egg-info/requires.txt
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)        7 2024-05-13 12:50:19.000000 bigfunctions-0.5/bigfunctions.egg-info/top_level.txt
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)       38 2024-05-13 12:50:19.496251 bigfunctions-0.5/setup.cfg
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     1112 2024-05-13 12:49:39.000000 bigfunctions-0.5/setup.py
+drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-05-13 14:59:48.478641 bigfunctions-0.6/
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     1064 2023-11-08 21:20:23.000000 bigfunctions-0.6/LICENSE
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     9821 2024-05-13 14:59:48.477641 bigfunctions-0.6/PKG-INFO
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     9097 2024-02-22 22:16:20.000000 bigfunctions-0.6/README.md
+drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-05-13 14:59:48.466640 bigfunctions-0.6/bigfun/
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2023-11-08 21:20:23.000000 bigfunctions-0.6/bigfun/__init__.py
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     8507 2024-05-10 19:42:48.000000 bigfunctions-0.6/bigfun/bigfunctions.py
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     9663 2024-05-10 19:32:19.000000 bigfunctions-0.6/bigfun/cli.py
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      844 2023-12-01 17:33:50.000000 bigfunctions-0.6/bigfun/load_table.py
+drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-05-13 14:59:48.470641 bigfunctions-0.6/bigfun/templates/
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     1086 2023-11-08 21:20:23.000000 bigfunctions-0.6/bigfun/templates/Dockerfile
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)    11722 2024-05-10 19:28:43.000000 bigfunctions-0.6/bigfun/templates/bigfunction.md
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     3784 2024-01-19 20:34:23.000000 bigfunctions-0.6/bigfun/templates/bookmarklet.js
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     1618 2024-05-10 09:49:39.000000 bigfunctions-0.6/bigfun/templates/categories.md
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     4164 2024-01-24 23:20:01.000000 bigfunctions-0.6/bigfun/templates/data.md
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      554 2024-02-23 19:54:09.000000 bigfunctions-0.6/bigfun/templates/function_js.sql
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     7724 2024-02-23 21:48:51.000000 bigfunctions-0.6/bigfun/templates/function_py.py
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      403 2024-05-13 13:22:43.000000 bigfunctions-0.6/bigfun/templates/function_py.sql
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      212 2024-02-23 21:42:39.000000 bigfunctions-0.6/bigfun/templates/function_py_test.py
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      410 2024-02-23 19:54:09.000000 bigfunctions-0.6/bigfun/templates/function_sql.sql
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      251 2024-02-23 22:59:01.000000 bigfunctions-0.6/bigfun/templates/function_sql_test.sql
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      702 2024-02-23 19:54:09.000000 bigfunctions-0.6/bigfun/templates/procedure.sql
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      717 2024-02-23 22:23:06.000000 bigfunctions-0.6/bigfun/templates/procedure_test.sql
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      345 2024-02-23 19:54:09.000000 bigfunctions-0.6/bigfun/templates/table_function.sql
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)    13269 2024-05-10 19:41:56.000000 bigfunctions-0.6/bigfun/utils.py
+drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-05-13 14:59:48.471641 bigfunctions-0.6/bigfun/website/
+drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-05-13 14:59:48.475641 bigfunctions-0.6/bigfun/website/assets/
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     1714 2023-11-29 13:48:58.000000 bigfunctions-0.6/bigfun/website/assets/GitHub-Mark-32px.png
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)  1353755 2024-01-19 20:34:23.000000 bigfunctions-0.6/bigfun/website/assets/bookmarklet_usage.gif
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)    23806 2023-11-29 13:48:58.000000 bigfunctions-0.6/bigfun/website/assets/logo.png
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)    73519 2023-11-29 13:48:58.000000 bigfunctions-0.6/bigfun/website/assets/logo_and_name.png
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)    49771 2023-11-29 13:48:58.000000 bigfunctions-0.6/bigfun/website/assets/logo_and_name_wo_supercharge.png
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     1712 2024-05-10 18:53:52.000000 bigfunctions-0.6/bigfun/website/mkdocs.yml
+drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-05-13 14:59:48.475641 bigfunctions-0.6/bigfun/website/theme_overrides/
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     6185 2024-05-10 12:11:21.000000 bigfunctions-0.6/bigfun/website/theme_overrides/main.html
+drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-05-13 14:59:48.477641 bigfunctions-0.6/bigfunctions.egg-info/
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     9821 2024-05-13 14:59:48.000000 bigfunctions-0.6/bigfunctions.egg-info/PKG-INFO
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     1076 2024-05-13 14:59:48.000000 bigfunctions-0.6/bigfunctions.egg-info/SOURCES.txt
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)        1 2024-05-13 14:59:48.000000 bigfunctions-0.6/bigfunctions.egg-info/dependency_links.txt
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)       42 2024-05-13 14:59:48.000000 bigfunctions-0.6/bigfunctions.egg-info/entry_points.txt
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      130 2024-05-13 14:59:48.000000 bigfunctions-0.6/bigfunctions.egg-info/requires.txt
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)        7 2024-05-13 14:59:48.000000 bigfunctions-0.6/bigfunctions.egg-info/top_level.txt
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)       38 2024-05-13 14:59:48.478641 bigfunctions-0.6/setup.cfg
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     1111 2024-05-13 14:59:05.000000 bigfunctions-0.6/setup.py
```

### Comparing `bigfunctions-0.5/LICENSE` & `bigfunctions-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.5/PKG-INFO` & `bigfunctions-0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: bigfunctions
-Version: 0.5
+Version: 0.6
 Summary: Supercharge BigQuery with BigFunctions
-Download-URL: https://github.com/unytics/bigfunctions/archive/refs/tags/v0.5.tar.gz
+Download-URL: https://github.com/unytics/bigfunctions/archive/refs/tags/v0.6.tar.gz
 Author: Unytics
 Author-email: paul.marcombes@unytics.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: google-cloud-bigquery
 Requires-Dist: google-cloud-bigquery_connection
 Requires-Dist: google-cloud-storage
 Requires-Dist: pyyaml
 Requires-Dist: jinja2
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: bigfunctions Version: 0.5 Summary: Supercharge
+Metadata-Version: 2.1 Name: bigfunctions Version: 0.6 Summary: Supercharge
 BigQuery with BigFunctions Download-URL: https://github.com/unytics/
-bigfunctions/archive/refs/tags/v0.5.tar.gz Author: Unytics Author-email:
+bigfunctions/archive/refs/tags/v0.6.tar.gz Author: Unytics Author-email:
 paul.marcombes@unytics.io Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
-:: OS Independent Requires-Python: >=3.10 Description-Content-Type: text/
+:: OS Independent Requires-Python: >=3.6 Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: google-cloud-bigquery Requires-
 Dist: google-cloud-bigquery_connection Requires-Dist: google-cloud-storage
 Requires-Dist: pyyaml Requires-Dist: jinja2 Requires-Dist: mkdocs-material
 Requires-Dist: click Requires-Dist: click-help-colors
                                 [logo_and_name]
                              Supercharge BBiiggQQuueerryy
                                with BBiiggFFuunnccttiioonnss
```

### Comparing `bigfunctions-0.5/README.md` & `bigfunctions-0.6/README.md`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.5/bigfun/bigfunctions.py` & `bigfunctions-0.6/bigfun/bigfunctions.py`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.5/bigfun/cli.py` & `bigfunctions-0.6/bigfun/cli.py`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.5/bigfun/load_table.py` & `bigfunctions-0.6/bigfun/load_table.py`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.5/bigfun/templates/Dockerfile` & `bigfunctions-0.6/bigfun/templates/Dockerfile`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.5/bigfun/templates/bigfunction.md` & `bigfunctions-0.6/bigfun/templates/bigfunction.md`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.5/bigfun/templates/bookmarklet.js` & `bigfunctions-0.6/bigfun/templates/bookmarklet.js`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.5/bigfun/templates/categories.md` & `bigfunctions-0.6/bigfun/templates/categories.md`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.5/bigfun/templates/data.md` & `bigfunctions-0.6/bigfun/templates/data.md`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.5/bigfun/templates/function_js.sql` & `bigfunctions-0.6/bigfun/templates/function_js.sql`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.5/bigfun/templates/function_py.py` & `bigfunctions-0.6/bigfun/templates/function_py.py`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.5/bigfun/templates/procedure.sql` & `bigfunctions-0.6/bigfun/templates/procedure.sql`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.5/bigfun/templates/procedure_test.sql` & `bigfunctions-0.6/bigfun/templates/procedure_test.sql`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.5/bigfun/utils.py` & `bigfunctions-0.6/bigfun/utils.py`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.5/bigfun/website/assets/GitHub-Mark-32px.png` & `bigfunctions-0.6/bigfun/website/assets/GitHub-Mark-32px.png`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.5/bigfun/website/assets/bookmarklet_usage.gif` & `bigfunctions-0.6/bigfun/website/assets/bookmarklet_usage.gif`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.5/bigfun/website/assets/logo.png` & `bigfunctions-0.6/bigfun/website/assets/logo.png`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.5/bigfun/website/assets/logo_and_name.png` & `bigfunctions-0.6/bigfun/website/assets/logo_and_name.png`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.5/bigfun/website/assets/logo_and_name_wo_supercharge.png` & `bigfunctions-0.6/bigfun/website/assets/logo_and_name_wo_supercharge.png`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.5/bigfun/website/mkdocs.yml` & `bigfunctions-0.6/bigfun/website/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.5/bigfun/website/theme_overrides/main.html` & `bigfunctions-0.6/bigfun/website/theme_overrides/main.html`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.5/bigfunctions.egg-info/PKG-INFO` & `bigfunctions-0.6/bigfunctions.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: bigfunctions
-Version: 0.5
+Version: 0.6
 Summary: Supercharge BigQuery with BigFunctions
-Download-URL: https://github.com/unytics/bigfunctions/archive/refs/tags/v0.5.tar.gz
+Download-URL: https://github.com/unytics/bigfunctions/archive/refs/tags/v0.6.tar.gz
 Author: Unytics
 Author-email: paul.marcombes@unytics.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: google-cloud-bigquery
 Requires-Dist: google-cloud-bigquery_connection
 Requires-Dist: google-cloud-storage
 Requires-Dist: pyyaml
 Requires-Dist: jinja2
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: bigfunctions Version: 0.5 Summary: Supercharge
+Metadata-Version: 2.1 Name: bigfunctions Version: 0.6 Summary: Supercharge
 BigQuery with BigFunctions Download-URL: https://github.com/unytics/
-bigfunctions/archive/refs/tags/v0.5.tar.gz Author: Unytics Author-email:
+bigfunctions/archive/refs/tags/v0.6.tar.gz Author: Unytics Author-email:
 paul.marcombes@unytics.io Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
-:: OS Independent Requires-Python: >=3.10 Description-Content-Type: text/
+:: OS Independent Requires-Python: >=3.6 Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: google-cloud-bigquery Requires-
 Dist: google-cloud-bigquery_connection Requires-Dist: google-cloud-storage
 Requires-Dist: pyyaml Requires-Dist: jinja2 Requires-Dist: mkdocs-material
 Requires-Dist: click Requires-Dist: click-help-colors
                                 [logo_and_name]
                              Supercharge BBiiggQQuueerryy
                                with BBiiggFFuunnccttiioonnss
```

### Comparing `bigfunctions-0.5/bigfunctions.egg-info/SOURCES.txt` & `bigfunctions-0.6/bigfunctions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bigfunctions-0.5/setup.py` & `bigfunctions-0.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 
 
-VERSION = '0.5'
+VERSION = '0.6'
 
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
@@ -19,15 +19,15 @@
     long_description_content_type='text/markdown',
     download_url=f'https://github.com/unytics/bigfunctions/archive/refs/tags/v{VERSION}.tar.gz',
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
-    python_requires='>=3.10',
+    python_requires='>=3.6',
     include_package_data=True,
     install_requires=[
         'google-cloud-bigquery',
         'google-cloud-bigquery_connection',
         'google-cloud-storage',
         'pyyaml',
         'jinja2',
```

