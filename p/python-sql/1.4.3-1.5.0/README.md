# Comparing `tmp/python-sql-1.4.3.tar.gz` & `tmp/python_sql-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-sql-1.4.3.tar", last modified: Sat Dec 30 17:19:57 2023, max compression
+gzip compressed data, was "python_sql-1.5.0.tar", last modified: Mon May 13 16:52:16 2024, max compression
```

## Comparing `python-sql-1.4.3.tar` & `python_sql-1.5.0.tar`

### file list

```diff
@@ -1,49 +1,50 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-12-30 17:19:57.587252 python-sql-1.4.3/
--rw-r--r--   0 ced       (1000) ced       (1000)       41 2020-02-29 23:00:32.000000 python-sql-1.4.3/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)     1368 2023-10-07 13:08:01.000000 python-sql-1.4.3/.gitlab-ci.yml
--rw-r--r--   0 ced       (1000) ced       (1000)      828 2023-06-25 09:04:06.000000 python-sql-1.4.3/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)       31 2021-12-18 00:47:59.000000 python-sql-1.4.3/.isort.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     2911 2023-12-30 17:19:00.000000 python-sql-1.4.3/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)     1576 2023-06-25 09:03:37.000000 python-sql-1.4.3/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)       55 2023-03-02 21:12:39.000000 python-sql-1.4.3/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     8514 2023-12-30 17:19:57.587252 python-sql-1.4.3/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     7265 2021-09-10 11:50:13.000000 python-sql-1.4.3/README.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-12-30 17:19:57.580586 python-sql-1.4.3/python_sql.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     8514 2023-12-30 17:19:57.000000 python-sql-1.4.3/python_sql.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      932 2023-12-30 17:19:57.000000 python-sql-1.4.3/python_sql.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-12-30 17:19:57.000000 python-sql-1.4.3/python_sql.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        4 2023-12-30 17:19:57.000000 python-sql-1.4.3/python_sql.egg-info/top_level.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-12-30 17:19:57.587252 python-sql-1.4.3/setup.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     1922 2023-10-07 13:08:26.000000 python-sql-1.4.3/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-12-30 17:19:57.580586 python-sql-1.4.3/sql/
--rw-r--r--   0 ced       (1000) ced       (1000)    47512 2023-12-10 21:58:22.000000 python-sql-1.4.3/sql/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5241 2022-01-29 01:09:33.000000 python-sql-1.4.3/sql/aggregate.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2541 2021-12-18 00:48:19.000000 python-sql-1.4.3/sql/conditionals.py
--rw-r--r--   0 ced       (1000) ced       (1000)    12307 2021-12-18 00:48:19.000000 python-sql-1.4.3/sql/functions.py
--rw-r--r--   0 ced       (1000) ced       (1000)    10782 2022-04-27 16:39:13.000000 python-sql-1.4.3/sql/operators.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-12-30 17:19:57.587252 python-sql-1.4.3/sql/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      675 2022-04-27 16:41:54.000000 python-sql-1.4.3/sql/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2592 2022-01-28 11:56:33.000000 python-sql-1.4.3/sql/tests/test_aggregate.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1884 2021-12-18 00:48:19.000000 python-sql-1.4.3/sql/tests/test_alias.py
--rw-r--r--   0 ced       (1000) ced       (1000)      926 2021-12-18 00:48:19.000000 python-sql-1.4.3/sql/tests/test_as.py
--rw-r--r--   0 ced       (1000) ced       (1000)      653 2021-09-14 07:32:05.000000 python-sql-1.4.3/sql/tests/test_cast.py
--rw-r--r--   0 ced       (1000) ced       (1000)      842 2021-09-14 07:32:14.000000 python-sql-1.4.3/sql/tests/test_collate.py
--rw-r--r--   0 ced       (1000) ced       (1000)      866 2022-04-27 16:41:54.000000 python-sql-1.4.3/sql/tests/test_column.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2277 2023-12-10 22:48:45.000000 python-sql-1.4.3/sql/tests/test_combining_query.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2705 2021-12-18 00:48:19.000000 python-sql-1.4.3/sql/tests/test_conditionals.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1591 2021-09-14 07:32:51.000000 python-sql-1.4.3/sql/tests/test_delete.py
--rw-r--r--   0 ced       (1000) ced       (1000)      550 2021-09-14 07:33:00.000000 python-sql-1.4.3/sql/tests/test_for.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5377 2021-12-18 00:48:19.000000 python-sql-1.4.3/sql/tests/test_functions.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3972 2023-06-18 08:11:33.000000 python-sql-1.4.3/sql/tests/test_insert.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1891 2021-12-18 00:48:19.000000 python-sql-1.4.3/sql/tests/test_join.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1046 2021-12-18 00:48:19.000000 python-sql-1.4.3/sql/tests/test_lateral.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1010 2021-12-18 00:48:19.000000 python-sql-1.4.3/sql/tests/test_literal.py
--rw-r--r--   0 ced       (1000) ced       (1000)    15639 2022-04-27 16:39:13.000000 python-sql-1.4.3/sql/tests/test_operators.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1996 2021-12-18 00:48:19.000000 python-sql-1.4.3/sql/tests/test_order.py
--rw-r--r--   0 ced       (1000) ced       (1000)    18053 2021-12-18 00:49:44.000000 python-sql-1.4.3/sql/tests/test_select.py
--rw-r--r--   0 ced       (1000) ced       (1000)      758 2021-09-14 07:34:28.000000 python-sql-1.4.3/sql/tests/test_table.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3490 2023-06-18 08:11:33.000000 python-sql-1.4.3/sql/tests/test_update.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1053 2021-09-14 07:34:49.000000 python-sql-1.4.3/sql/tests/test_values.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2383 2021-12-18 00:48:19.000000 python-sql-1.4.3/sql/tests/test_window.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2256 2021-12-18 00:48:19.000000 python-sql-1.4.3/sql/tests/test_with.py
--rw-r--r--   0 ced       (1000) ced       (1000)      575 2023-10-07 13:08:14.000000 python-sql-1.4.3/tox.ini
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-13 16:52:16.977754 python_sql-1.5.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)       41 2020-02-29 23:00:32.000000 python_sql-1.5.0/.flake8
+-rw-r--r--   0 ced       (1000) ced       (1000)     1360 2024-03-07 16:01:58.000000 python_sql-1.5.0/.gitlab-ci.yml
+-rw-r--r--   0 ced       (1000) ced       (1000)      922 2024-05-13 16:51:40.000000 python_sql-1.5.0/.hgtags
+-rw-r--r--   0 ced       (1000) ced       (1000)       31 2021-12-18 00:47:59.000000 python_sql-1.5.0/.isort.cfg
+-rw-r--r--   0 ced       (1000) ced       (1000)     3109 2024-05-13 16:51:04.000000 python_sql-1.5.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)     1576 2023-06-25 09:03:37.000000 python_sql-1.5.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)       55 2023-03-02 21:12:39.000000 python_sql-1.5.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     8514 2024-05-13 16:52:16.977754 python_sql-1.5.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     7265 2021-09-10 11:50:13.000000 python_sql-1.5.0/README.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-13 16:52:16.977754 python_sql-1.5.0/python_sql.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     8514 2024-05-13 16:52:16.000000 python_sql-1.5.0/python_sql.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      956 2024-05-13 16:52:16.000000 python_sql-1.5.0/python_sql.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-05-13 16:52:16.000000 python_sql-1.5.0/python_sql.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        4 2024-05-13 16:52:16.000000 python_sql-1.5.0/python_sql.egg-info/top_level.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-05-13 16:52:16.977754 python_sql-1.5.0/setup.cfg
+-rw-r--r--   0 ced       (1000) ced       (1000)     1922 2023-10-07 13:08:26.000000 python_sql-1.5.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-13 16:52:16.974421 python_sql-1.5.0/sql/
+-rw-r--r--   0 ced       (1000) ced       (1000)    59923 2024-05-13 16:50:38.000000 python_sql-1.5.0/sql/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5241 2022-01-29 01:09:33.000000 python_sql-1.5.0/sql/aggregate.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2541 2021-12-18 00:48:19.000000 python_sql-1.5.0/sql/conditionals.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    12373 2024-05-06 07:52:59.000000 python_sql-1.5.0/sql/functions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    10788 2024-03-07 16:01:58.000000 python_sql-1.5.0/sql/operators.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-05-13 16:52:16.977754 python_sql-1.5.0/sql/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      675 2022-04-27 16:41:54.000000 python_sql-1.5.0/sql/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2592 2022-01-28 11:56:33.000000 python_sql-1.5.0/sql/tests/test_aggregate.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1884 2021-12-18 00:48:19.000000 python_sql-1.5.0/sql/tests/test_alias.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      926 2021-12-18 00:48:19.000000 python_sql-1.5.0/sql/tests/test_as.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      653 2021-09-14 07:32:05.000000 python_sql-1.5.0/sql/tests/test_cast.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      842 2021-09-14 07:32:14.000000 python_sql-1.5.0/sql/tests/test_collate.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      866 2022-04-27 16:41:54.000000 python_sql-1.5.0/sql/tests/test_column.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2277 2023-12-10 22:48:45.000000 python_sql-1.5.0/sql/tests/test_combining_query.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2705 2021-12-18 00:48:19.000000 python_sql-1.5.0/sql/tests/test_conditionals.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1591 2021-09-14 07:32:51.000000 python_sql-1.5.0/sql/tests/test_delete.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      550 2021-09-14 07:33:00.000000 python_sql-1.5.0/sql/tests/test_for.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5377 2021-12-18 00:48:19.000000 python_sql-1.5.0/sql/tests/test_functions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7378 2024-05-12 06:43:27.000000 python_sql-1.5.0/sql/tests/test_insert.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1891 2021-12-18 00:48:19.000000 python_sql-1.5.0/sql/tests/test_join.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1046 2021-12-18 00:48:19.000000 python_sql-1.5.0/sql/tests/test_lateral.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1010 2021-12-18 00:48:19.000000 python_sql-1.5.0/sql/tests/test_literal.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4074 2024-05-12 06:35:08.000000 python_sql-1.5.0/sql/tests/test_merge.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    15542 2024-03-07 16:01:58.000000 python_sql-1.5.0/sql/tests/test_operators.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1996 2021-12-18 00:48:19.000000 python_sql-1.5.0/sql/tests/test_order.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    19882 2024-03-07 16:01:58.000000 python_sql-1.5.0/sql/tests/test_select.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      758 2021-09-14 07:34:28.000000 python_sql-1.5.0/sql/tests/test_table.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3490 2023-06-18 08:11:33.000000 python_sql-1.5.0/sql/tests/test_update.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1053 2021-09-14 07:34:49.000000 python_sql-1.5.0/sql/tests/test_values.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2383 2021-12-18 00:48:19.000000 python_sql-1.5.0/sql/tests/test_window.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2256 2021-12-18 00:48:19.000000 python_sql-1.5.0/sql/tests/test_with.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      583 2024-03-07 16:01:58.000000 python_sql-1.5.0/tox.ini
```

### Comparing `python-sql-1.4.3/.gitlab-ci.yml` & `python_sql-1.5.0/.gitlab-ci.yml`

 * *Files 1% similar despite different names*

```diff
@@ -50,17 +50,17 @@
         coverage_format: cobertura
         path: coverage.xml
 
 test-tox-python:
   extends: .test-tox
   image: ${CI_DEPENDENCY_PROXY_GROUP_IMAGE_PREFIX}/python:${PYTHON_VERSION}
   script:
-    - tox -e "py${PYTHON_VERSION/./}" -vv -- -v --output-file junit.xml
+    - tox -e "py${PYTHON_VERSION/./}" -- -v --output-file junit.xml
   parallel:
     matrix:
       - PYTHON_VERSION: ["3.5", "3.6", "3.7", "3.8", "3.9", "3.10", "3.11", "3.12"]
 
 test-tox-pypy:
   extends: .test-tox
   image: ${CI_DEPENDENCY_PROXY_GROUP_IMAGE_PREFIX}/pypy:3
   script:
-    - tox -e pypy3 -vv -- -v --output-file junit.xml
+    - tox -e pypy3 -- -v --output-file junit.xml
```

### Comparing `python-sql-1.4.3/.hgtags` & `python_sql-1.5.0/.hgtags`

 * *Files 16% similar despite different names*

```diff
@@ -12,7 +12,9 @@
 de68c850bc6a809b0c88ddbe2fa99b02df07bee3 1.2.0
 b2bcc0f71f6881316c11330c07de34113f088888 1.2.1
 1c38ffeacbb82a9ff6ae3568cdc017dbbeddff5d 1.2.2
 edc03ee84f0ac96d403d8f984d59fffa3274cd2f 1.3.0
 a317c40a4d60089ba9e465fbd64b78df24f9e890 1.4.0
 e71bbae3398cb6a0e72f97a0cada9fcdee2bddea 1.4.1
 fcb64787b51db2068061eb4aa13825abc1134916 1.4.2
+111e3e86865360f83a65c04fa48c55f3d2957ee3 1.4.3
+6f9066b83fe3a8c4699a8555ad1bc406f18974ff 1.5.0
```

### Comparing `python-sql-1.4.3/CHANGELOG` & `python_sql-1.5.0/CHANGELOG`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+Version 1.5.0 - 2024-05-13
+* Skip alias on INSERT without ON CONFLICT or RETURNING
+* Add MERGE
+* Support UPSERT
+* Remove default escape char on LIKE and ILIKE
+* Add GROUPING SETS, CUBE, and ROLLUP
+
 Version 1.4.3 - 2023-12-30
 * Render common table expression in combining query
 * Add support for Python 3.12
 
 Version 1.4.2 - 2023-06-25
 * Restore usage of alias in returning expression
```

### Comparing `python-sql-1.4.3/COPYRIGHT` & `python_sql-1.5.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `python-sql-1.4.3/PKG-INFO` & `python_sql-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-sql
-Version: 1.4.3
+Version: 1.5.0
 Summary: Library to write SQL queries
 Home-page: https://pypi.org/project/python-sql/
 Download-URL: https://downloads.tryton.org/python-sql/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: BSD
 Project-URL: Bug Tracker, https://bugs.tryton.org/python-sql
```

### Comparing `python-sql-1.4.3/README.rst` & `python_sql-1.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `python-sql-1.4.3/python_sql.egg-info/PKG-INFO` & `python_sql-1.5.0/python_sql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-sql
-Version: 1.4.3
+Version: 1.5.0
 Summary: Library to write SQL queries
 Home-page: https://pypi.org/project/python-sql/
 Download-URL: https://downloads.tryton.org/python-sql/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: BSD
 Project-URL: Bug Tracker, https://bugs.tryton.org/python-sql
```

### Comparing `python-sql-1.4.3/python_sql.egg-info/SOURCES.txt` & `python_sql-1.5.0/python_sql.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 sql/tests/test_delete.py
 sql/tests/test_for.py
 sql/tests/test_functions.py
 sql/tests/test_insert.py
 sql/tests/test_join.py
 sql/tests/test_lateral.py
 sql/tests/test_literal.py
+sql/tests/test_merge.py
 sql/tests/test_operators.py
 sql/tests/test_order.py
 sql/tests/test_select.py
 sql/tests/test_table.py
 sql/tests/test_update.py
 sql/tests/test_values.py
 sql/tests/test_window.py
```

### Comparing `python-sql-1.4.3/setup.py` & `python_sql-1.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `python-sql-1.4.3/sql/__init__.py` & `python_sql-1.5.0/sql/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,17 +3,21 @@
 import numbers
 import string
 import warnings
 from collections import defaultdict
 from itertools import chain
 from threading import current_thread, local
 
-__version__ = '1.4.3'
-__all__ = ['Flavor', 'Table', 'Values', 'Literal', 'Column', 'Join',
-    'Asc', 'Desc', 'NullsFirst', 'NullsLast', 'format2numeric']
+__version__ = '1.5.0'
+__all__ = [
+    'Flavor', 'Table', 'Values', 'Literal', 'Column', 'Grouping', 'Conflict',
+    'Matched', 'MatchedUpdate', 'MatchedDelete',
+    'NotMatched', 'NotMatchedInsert',
+    'Rollup', 'Cube', 'Excluded', 'Join', 'Asc', 'Desc', 'NullsFirst',
+    'NullsLast', 'format2numeric']
 
 
 def _escape_identifier(name):
     return '"%s"' % name.replace('"', '""')
 
 
 def alias(i, letters=string.ascii_lowercase):
@@ -659,25 +663,28 @@
                 p.extend(self.having.params)
             for window in self.windows:
                 p.extend(window.params)
         return tuple(p)
 
 
 class Insert(WithQuery):
-    __slots__ = ('_table', '_columns', '_values', '_returning')
+    __slots__ = ('_table', '_columns', '_values', '_on_conflict', '_returning')
 
-    def __init__(self, table, columns=None, values=None, returning=None,
-            **kwargs):
+    def __init__(
+            self, table, columns=None, values=None, returning=None,
+            on_conflict=None, **kwargs):
         self._table = None
         self._columns = None
         self._values = None
+        self._on_conflict = None
         self._returning = None
         self.table = table
         self.columns = columns
         self.values = values
+        self.on_conflict = on_conflict
         self.returning = returning
         super(Insert, self).__init__(**kwargs)
 
     @property
     def table(self):
         return self._table
 
@@ -706,14 +713,25 @@
         if value is not None:
             assert isinstance(value, (list, Select))
         if isinstance(value, list):
             value = Values(value)
         self._values = value
 
     @property
+    def on_conflict(self):
+        return self._on_conflict
+
+    @on_conflict.setter
+    def on_conflict(self, value):
+        if value is not None:
+            assert isinstance(value, Conflict)
+            assert value.table == self.table
+        self._on_conflict = value
+
+    @property
     def returning(self):
         return self._returning
 
     @returning.setter
     def returning(self, value):
         if value is not None:
             assert isinstance(value, list)
@@ -739,34 +757,178 @@
             columns = ' (' + columns + ')'
         with AliasManager():
             if isinstance(self.values, Query):
                 values = ' %s' % str(self.values)
                 # TODO manage DEFAULT
             elif self.values is None:
                 values = ' DEFAULT VALUES'
+            on_conflict = ''
+            if self.on_conflict:
+                on_conflict = ' %s' % self.on_conflict
             returning = ''
             if self.returning:
                 returning = ' RETURNING ' + ', '.join(
                     map(self._format, self.returning))
+            if on_conflict or returning:
+                table = '%s AS "%s"' % (self.table, self.table.alias)
+            else:
+                table = str(self.table)
             return (self._with_str()
-                + 'INSERT INTO %s AS "%s"' % (self.table, self.table.alias)
-                + columns + values + returning)
+                + 'INSERT INTO %s' % table
+                + columns + values + on_conflict + returning)
 
     @property
     def params(self):
         p = []
         p.extend(self._with_params())
         if isinstance(self.values, Query):
             p.extend(self.values.params)
+        if self.on_conflict:
+            p.extend(self.on_conflict.params)
         if self.returning:
             for exp in self.returning:
                 p.extend(exp.params)
         return tuple(p)
 
 
+class Conflict(object):
+    __slots__ = (
+        '_table', '_indexed_columns', '_index_where', '_columns', '_values',
+        '_where')
+
+    def __init__(
+            self, table, indexed_columns=None, index_where=None,
+            columns=None, values=None, where=None):
+        self._table = None
+        self._indexed_columns = None
+        self._index_where = None
+        self._columns = None
+        self._values = None
+        self._where = None
+        self.table = table
+        self.indexed_columns = indexed_columns
+        self.index_where = index_where
+        self.columns = columns
+        self.values = values
+        self.where = where
+
+    @property
+    def table(self):
+        return self._table
+
+    @table.setter
+    def table(self, value):
+        assert isinstance(value, Table)
+        self._table = value
+
+    @property
+    def indexed_columns(self):
+        return self._indexed_columns
+
+    @indexed_columns.setter
+    def indexed_columns(self, value):
+        if value is not None:
+            assert all(isinstance(col, Column) for col in value)
+            assert all(col.table == self.table for col in value)
+        self._indexed_columns = value
+
+    @property
+    def index_where(self):
+        return self._index_where
+
+    @index_where.setter
+    def index_where(self, value):
+        from sql.operators import And, Or
+        if value is not None:
+            assert isinstance(value, (Expression, And, Or))
+        self._index_where = value
+
+    @property
+    def columns(self):
+        return self._columns
+
+    @columns.setter
+    def columns(self, value):
+        if value is not None:
+            assert all(isinstance(col, Column) for col in value)
+            assert all(col.table == self.table for col in value)
+        self._columns = value
+
+    @property
+    def values(self):
+        return self._values
+
+    @values.setter
+    def values(self, value):
+        if value is not None:
+            assert isinstance(value, (list, Select))
+        if isinstance(value, list):
+            value = Values([value])
+        self._values = value
+
+    @property
+    def where(self):
+        return self._where
+
+    @where.setter
+    def where(self, value):
+        from sql.operators import And, Or
+        if value is not None:
+            assert isinstance(value, (Expression, And, Or))
+        self._where = value
+
+    def __str__(self):
+        indexed_columns = ''
+        if self.indexed_columns:
+            assert all(c.table == self.table for c in self.indexed_columns)
+            # Get columns without alias
+            indexed_columns = ', '.join(
+                c.column_name for c in self.indexed_columns)
+            indexed_columns = ' (' + indexed_columns + ')'
+            if self.index_where:
+                indexed_columns += ' WHERE ' + str(self.index_where)
+        else:
+            assert not self.index_where
+        do = ''
+        if not self.columns:
+            assert not self.values
+            assert not self.where
+            do = 'NOTHING'
+        else:
+            assert all(c.table == self.table for c in self.columns)
+            # Get columns without alias
+            do = ', '.join(c.column_name for c in self.columns)
+            # TODO manage DEFAULT
+            values = str(self.values)
+            if values.startswith('VALUES'):
+                values = values[len('VALUES'):]
+            else:
+                values = ' (' + values + ')'
+            if len(self.columns) == 1:
+                # PostgreSQL would require ROW expression
+                # with single column with parenthesis
+                do = 'UPDATE SET ' + do + ' =' + values
+            else:
+                do = 'UPDATE SET (' + do + ') =' + values
+            if self.where:
+                do += ' WHERE %s' % self.where
+        return 'ON CONFLICT' + indexed_columns + ' DO ' + do
+
+    @property
+    def params(self):
+        p = []
+        if self.index_where:
+            p.extend(self.index_where.params)
+        if self.values:
+            p.extend(self.values.params)
+        if self.where:
+            p.extend(self.where.params)
+        return p
+
+
 class Update(Insert):
     __slots__ = ('_where', '_values', 'from_')
 
     def __init__(self, table, columns, values, from_=None, where=None,
             returning=None, **kwargs):
         super(Update, self).__init__(table, columns=columns, values=values,
             returning=returning, **kwargs)
@@ -915,14 +1077,215 @@
             p.extend(self.where.params)
         if self.returning:
             for exp in self.returning:
                 p.extend(exp.params)
         return tuple(p)
 
 
+class Merge(WithQuery):
+    __slots__ = ('_target', '_source', '_condition', '_whens')
+
+    def __init__(self, target, source, condition, *whens, **kwargs):
+        self._target = None
+        self._source = None
+        self._condition = None
+        self._whens = None
+        self.target = target
+        self.source = source
+        self.condition = condition
+        self.whens = whens
+        super().__init__(**kwargs)
+
+    @property
+    def target(self):
+        return self._target
+
+    @target.setter
+    def target(self, value):
+        assert isinstance(value, Table)
+        self._target = value
+
+    @property
+    def source(self):
+        return self._source
+
+    @source.setter
+    def source(self, value):
+        assert isinstance(value, (Table, SelectQuery, Values))
+        self._source = value
+
+    @property
+    def condition(self):
+        return self._condition
+
+    @condition.setter
+    def condition(self, value):
+        assert isinstance(value, Expression)
+        self._condition = value
+
+    @property
+    def whens(self):
+        return self._whens
+
+    @whens.setter
+    def whens(self, value):
+        assert all(isinstance(w, Matched) for w in value)
+        self._whens = tuple(value)
+
+    def __str__(self):
+        with AliasManager():
+            if isinstance(self.source, (Select, Values)):
+                source = '(%s)' % self.source
+            else:
+                source = self.source
+            if self.condition:
+                condition = 'ON %s' % self.condition
+            else:
+                condition = ''
+            return (self._with_str()
+                + 'MERGE INTO %s AS "%s" ' % (self.target, self.target.alias)
+                + 'USING %s AS "%s" ' % (source, self.source.alias)
+                + condition + ' ' + ' '.join(map(str, self.whens)))
+
+    @property
+    def params(self):
+        p = []
+        p.extend(self._with_params())
+        if isinstance(self.source, (SelectQuery, Values)):
+            p.extend(self.source.params)
+        if self.condition:
+            p.extend(self.condition.params)
+        for match in self.whens:
+            p.extend(match.params)
+        return tuple(p)
+
+
+class Matched(object):
+    __slots__ = ('_condition',)
+    _when = 'MATCHED'
+
+    def __init__(self, condition=None):
+        self._condition = None
+        self.condition = condition
+
+    @property
+    def condition(self):
+        return self._condition
+
+    @condition.setter
+    def condition(self, value):
+        if value is not None:
+            assert isinstance(value, Expression)
+        self._condition = value
+
+    def _then_str(self):
+        return 'DO NOTHING'
+
+    def __str__(self):
+        if self.condition is not None:
+            condition = ' AND ' + str(self.condition)
+        else:
+            condition = ''
+        return 'WHEN ' + self._when + condition + ' THEN ' + self._then_str()
+
+    @property
+    def params(self):
+        p = []
+        if self.condition:
+            p.extend(self.condition.params)
+        return tuple(p)
+
+
+class _MatchedValues(Matched):
+    __slots__ = ('_columns', '_values')
+
+    def __init__(self, columns, values, **kwargs):
+        self._columns = columns
+        self._values = values
+        self.columns = columns
+        self.values = values
+        super().__init__(**kwargs)
+
+    @property
+    def columns(self):
+        return self._columns
+
+    @columns.setter
+    def columns(self, value):
+        assert all(isinstance(col, Column) for col in value)
+        self._columns = value
+
+
+class MatchedUpdate(_MatchedValues, Matched):
+    __slots__ = ()
+
+    @property
+    def values(self):
+        return self._values
+
+    @values.setter
+    def values(self, value):
+        self._values = value
+
+    def _then_str(self):
+        columns = [c.column_name for c in self.columns]
+        return 'UPDATE SET ' + ', '.join(
+            '%s = %s' % (c, Update._format(v))
+            for c, v in zip(columns, self.values))
+
+    @property
+    def params(self):
+        p = list(super().params)
+        for value in self.values:
+            if isinstance(value, (Expression, Select)):
+                p.extend(value.params)
+            else:
+                p.append(value)
+        return tuple(p)
+
+
+class MatchedDelete(Matched):
+    __slots__ = ()
+
+    def _then_str(self):
+        return 'DELETE'
+
+
+class NotMatched(Matched):
+    __slots__ = ()
+    _when = 'NOT MATCHED'
+
+
+class NotMatchedInsert(_MatchedValues, NotMatched):
+    __slots__ = ()
+
+    @property
+    def values(self):
+        return self._values
+
+    @values.setter
+    def values(self, value):
+        self._values = Values([value])
+
+    def _then_str(self):
+        columns = ', '.join(c.column_name for c in self.columns)
+        columns = '(' + columns + ')'
+        if self.values is None:
+            values = ' DEFAULT VALUES '
+        else:
+            values = ' ' + str(self.values)
+        return 'INSERT ' + columns + values
+
+    @property
+    def params(self):
+        p = list(super().params)
+        p.extend(self.values.params)
+        return tuple(p)
+
+
 class CombiningQuery(FromItem, SelectQuery):
     __slots__ = ('queries', 'all_')
     _operator = ''
 
     def __init__(self, *queries, **kwargs):
         assert all(isinstance(q, Query) for q in queries)
         self.queries = queries
@@ -985,28 +1348,49 @@
         return '.'.join(map(_escape_identifier, filter(None,
                     (self._database, self._schema, self._name))))
 
     @property
     def params(self):
         return ()
 
-    def insert(self, columns=None, values=None, returning=None, with_=None):
+    def insert(
+            self, columns=None, values=None, returning=None, with_=None,
+            on_conflict=None):
         return Insert(self, columns=columns, values=values,
-            returning=returning, with_=with_)
+            on_conflict=on_conflict, returning=returning, with_=with_)
 
     def update(self, columns, values, from_=None, where=None, returning=None,
             with_=None):
         return Update(self, columns=columns, values=values, from_=from_,
             where=where, returning=returning, with_=with_)
 
     def delete(self, only=False, using=None, where=None, returning=None,
             with_=None):
         return Delete(self, only=only, using=using, where=where,
             returning=returning, with_=with_)
 
+    def merge(self, source, condition, *whens, with_=None):
+        return Merge(self, source, condition, *whens, with_=with_)
+
+
+class _Excluded(Table):
+    def __init__(self):
+        super().__init__('EXCLUDED')
+
+    @property
+    def alias(self):
+        return 'EXCLUDED'
+
+    @property
+    def has_alias(self):
+        return False
+
+
+Excluded = _Excluded()
+
 
 class Join(FromItem):
     __slots__ = ('_left', '_right', '_condition', '_type_')
 
     def __init__(self, left, right, type_='INNER', condition=None):
         super(Join, self).__init__()
         self._left, self._right = None, None
@@ -1066,18 +1450,22 @@
             condition = ''
         return join + condition
 
     @property
     def params(self):
         p = []
         for item in (self.left, self.right):
-            if hasattr(item, 'params'):
+            try:
                 p.extend(item.params)
-        if hasattr(self.condition, 'params'):
+            except AttributeError:
+                pass
+        try:
             p.extend(self.condition.params)
+        except AttributeError:
+            pass
         return tuple(p)
 
     @property
     def alias(self):
         raise AttributeError
 
     @property
@@ -1438,14 +1826,87 @@
     def params(self):
         if isinstance(self.expression, Expression):
             return self.expression.params
         else:
             return (self.expression,)
 
 
+class Grouping(Expression):
+    __slots__ = ('_sets',)
+
+    def __init__(self, *sets):
+        super().__init__()
+        self.sets = sets
+
+    @property
+    def sets(self):
+        return self._sets
+
+    @sets.setter
+    def sets(self, value):
+        assert all(
+            isinstance(col, Expression) for cols in value for col in cols)
+        self._sets = tuple(tuple(cols) for cols in value)
+
+    def __str__(self):
+        return 'GROUPING SETS (%s)' % (
+            ', '.join(
+                '(%s)' % ', '.join(str(col) for col in cols)
+                for cols in self.sets))
+
+    @property
+    def params(self):
+        return sum((col.params for cols in self.sets for col in cols), ())
+
+
+class Rollup(Expression):
+    __slots__ = ('_expressions',)
+
+    def __init__(self, *expressions):
+        super().__init__()
+        self.expressions = expressions
+
+    @property
+    def expressions(self):
+        return self._expressions
+
+    @expressions.setter
+    def expressions(self, value):
+        assert all(
+            isinstance(col, Expression)
+            or all(isinstance(c, Expression) for c in col)
+            for col in value)
+        self._expressions = tuple(value)
+
+    def __str__(self):
+        def format(col):
+            if isinstance(col, Expression):
+                return str(col)
+            else:
+                return '(%s)' % ', '.join(str(c) for c in col)
+        return '%s (%s)' % (
+            self.__class__.__name__.upper(),
+            ', '.join(format(col) for col in self.expressions))
+
+    @property
+    def params(self):
+        p = []
+        for col in self.expressions:
+            if isinstance(col, Expression):
+                p.extend(col.params)
+            else:
+                for c in col:
+                    p.extend(c.params)
+        return tuple(p)
+
+
+class Cube(Rollup):
+    pass
+
+
 class Window(object):
     __slots__ = (
         '_partition', '_order_by', '_frame', '_start', '_end', '_exclude')
 
     def __init__(self, partition, order_by=None,
             frame=None, start=None, end=0, exclude=None):
         super(Window, self).__init__()
```

### Comparing `python-sql-1.4.3/sql/aggregate.py` & `python_sql-1.5.0/sql/aggregate.py`

 * *Files identical despite different names*

### Comparing `python-sql-1.4.3/sql/conditionals.py` & `python_sql-1.5.0/sql/conditionals.py`

 * *Files identical despite different names*

### Comparing `python-sql-1.4.3/sql/functions.py` & `python_sql-1.5.0/sql/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -311,16 +311,19 @@
         Mapping = Flavor.get().function_mapping.get(self.__class__)
         if Mapping:
             return Mapping(self.string, self.position, self.characters).params
         p = []
         for arg in (self.characters, self.string):
             if isinstance(arg, str):
                 p.append(arg)
-            elif hasattr(arg, 'params'):
-                p.extend(arg.params)
+            else:
+                try:
+                    p.extend(arg.params)
+                except AttributeError:
+                    pass
         return tuple(p)
 
 
 class Upper(Function):
     __slots__ = ()
     _function = 'UPPER'
```

### Comparing `python-sql-1.4.3/sql/operators.py` & `python_sql-1.5.0/sql/operators.py`

 * *Files 0% similar despite different names*

```diff
@@ -373,24 +373,24 @@
     _operator = '||'
 
 
 class Like(BinaryOperator):
     __slots__ = 'escape'
     _operator = 'LIKE'
 
-    def __init__(self, left, right, escape='\\'):
+    def __init__(self, left, right, escape=None):
         super().__init__(left, right)
         assert not escape or len(escape) == 1
         self.escape = escape
 
     @property
     def params(self):
         params = super().params
         if self.escape or Flavor().get().escape_empty:
-            params += (self.escape,)
+            params += (self.escape or '',)
         return params
 
     def __str__(self):
         left, right = self._operands
         if self.escape or Flavor().get().escape_empty:
             return '(%s %s %s ESCAPE %s)' % (
                 self._format(left), self._operator, self._format(right),
```

### Comparing `python-sql-1.4.3/sql/tests/__init__.py` & `python_sql-1.5.0/sql/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `python-sql-1.4.3/sql/tests/test_aggregate.py` & `python_sql-1.5.0/sql/tests/test_aggregate.py`

 * *Files identical despite different names*

### Comparing `python-sql-1.4.3/sql/tests/test_alias.py` & `python_sql-1.5.0/sql/tests/test_alias.py`

 * *Files identical despite different names*

### Comparing `python-sql-1.4.3/sql/tests/test_as.py` & `python_sql-1.5.0/sql/tests/test_as.py`

 * *Files identical despite different names*

### Comparing `python-sql-1.4.3/sql/tests/test_cast.py` & `python_sql-1.5.0/sql/tests/test_cast.py`

 * *Files identical despite different names*

### Comparing `python-sql-1.4.3/sql/tests/test_collate.py` & `python_sql-1.5.0/sql/tests/test_collate.py`

 * *Files identical despite different names*

### Comparing `python-sql-1.4.3/sql/tests/test_column.py` & `python_sql-1.5.0/sql/tests/test_column.py`

 * *Files identical despite different names*

### Comparing `python-sql-1.4.3/sql/tests/test_combining_query.py` & `python_sql-1.5.0/sql/tests/test_combining_query.py`

 * *Files identical despite different names*

### Comparing `python-sql-1.4.3/sql/tests/test_conditionals.py` & `python_sql-1.5.0/sql/tests/test_conditionals.py`

 * *Files identical despite different names*

### Comparing `python-sql-1.4.3/sql/tests/test_delete.py` & `python_sql-1.5.0/sql/tests/test_delete.py`

 * *Files identical despite different names*

### Comparing `python-sql-1.4.3/sql/tests/test_for.py` & `python_sql-1.5.0/sql/tests/test_for.py`

 * *Files identical despite different names*

### Comparing `python-sql-1.4.3/sql/tests/test_functions.py` & `python_sql-1.5.0/sql/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `python-sql-1.4.3/sql/tests/test_insert.py` & `python_sql-1.5.0/sql/tests/test_merge.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,105 +1,111 @@
 # This file is part of python-sql.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
-import unittest
-
-from sql import Table, With
-from sql.functions import Abs
-
 
-class TestInsert(unittest.TestCase):
-    table = Table('t')
-
-    def test_insert_default(self):
-        query = self.table.insert()
-        self.assertEqual(str(query), 'INSERT INTO "t" AS "a" DEFAULT VALUES')
-        self.assertEqual(tuple(query.params), ())
-
-    def test_insert_values(self):
-        query = self.table.insert([self.table.c1, self.table.c2],
-            [['foo', 'bar']])
-        self.assertEqual(str(query),
-            'INSERT INTO "t" AS "a" ("c1", "c2") VALUES (%s, %s)')
-        self.assertEqual(tuple(query.params), ('foo', 'bar'))
-
-    def test_insert_many_values(self):
-        query = self.table.insert([self.table.c1, self.table.c2],
-            [['foo', 'bar'], ['spam', 'eggs']])
-        self.assertEqual(str(query),
-            'INSERT INTO "t" AS "a" ("c1", "c2") VALUES (%s, %s), (%s, %s)')
-        self.assertEqual(tuple(query.params), ('foo', 'bar', 'spam', 'eggs'))
-
-    def test_insert_subselect(self):
-        t1 = Table('t1')
-        t2 = Table('t2')
-        subquery = t2.select(t2.c1, t2.c2)
-        query = t1.insert([t1.c1, t1.c2], subquery)
-        self.assertEqual(str(query),
-            'INSERT INTO "t1" AS "b" ("c1", "c2") '
-            'SELECT "a"."c1", "a"."c2" FROM "t2" AS "a"')
-        self.assertEqual(tuple(query.params), ())
-
-    def test_insert_function(self):
-        query = self.table.insert([self.table.c], [[Abs(-1)]])
-        self.assertEqual(str(query),
-            'INSERT INTO "t" AS "a" ("c") VALUES (ABS(%s))')
-        self.assertEqual(tuple(query.params), (-1,))
-
-    def test_insert_returning(self):
-        query = self.table.insert([self.table.c1, self.table.c2],
-            [['foo', 'bar']], returning=[self.table.c1, self.table.c2])
-        self.assertEqual(str(query),
-            'INSERT INTO "t" AS "a" ("c1", "c2") VALUES (%s, %s) '
-            'RETURNING "a"."c1", "a"."c2"')
-        self.assertEqual(tuple(query.params), ('foo', 'bar'))
+import unittest
 
-    def test_insert_returning_select(self):
-        t1 = Table('t1')
-        t2 = Table('t2')
-        query = t1.insert([t1.c], [['foo']],
-            returning=[
-                t2.select(t2.c, where=(t2.c1 == t1.c) & (t2.c2 == 'bar'))])
-        self.assertEqual(str(query),
-            'INSERT INTO "t1" AS "b" ("c") VALUES (%s) '
-            'RETURNING (SELECT "a"."c" FROM "t2" AS "a" '
-            'WHERE (("a"."c1" = "b"."c") AND ("a"."c2" = %s)))')
-        self.assertEqual(tuple(query.params), ('foo', 'bar'))
+from sql import (
+    Matched, MatchedDelete, MatchedUpdate, NotMatched, NotMatchedInsert, Table,
+    With)
+
+
+class TestMerge(unittest.TestCase):
+    target = Table('t')
+    source = Table('s')
+
+    def test_merge(self):
+        query = self.target.merge(
+            self.source, self.target.c1 == self.source.c2, Matched())
+        self.assertEqual(
+            str(query),
+            'MERGE INTO "t" AS "a" USING "s" AS "b" '
+            'ON ("a"."c1" = "b"."c2") '
+            'WHEN MATCHED THEN DO NOTHING')
+        self.assertEqual(query.params, ())
+
+    def test_condition(self):
+        query = self.target.merge(
+            self.source,
+            (self.target.c1 == self.source.c2) & (self.target.c3 == 42),
+            Matched())
+        self.assertEqual(
+            str(query),
+            'MERGE INTO "t" AS "a" USING "s" AS "b" '
+            'ON (("a"."c1" = "b"."c2") AND ("a"."c3" = %s)) '
+            'WHEN MATCHED THEN DO NOTHING')
+        self.assertEqual(query.params, (42,))
+
+    def test_matched(self):
+        query = self.target.merge(
+            self.source, self.target.c1 == self.source.c2,
+            Matched((self.source.c3 == 42)
+                & (self.target.c4 == self.source.c5)))
+        self.assertEqual(
+            str(query),
+            'MERGE INTO "t" AS "a" USING "s" AS "b" '
+            'ON ("a"."c1" = "b"."c2") '
+            'WHEN MATCHED '
+            'AND (("b"."c3" = %s) AND ("a"."c4" = "b"."c5")) '
+            'THEN DO NOTHING')
+        self.assertEqual(query.params, (42,))
+
+    def test_matched_update(self):
+        query = self.target.merge(
+            self.source, self.target.c1 == self.source.c2,
+            MatchedUpdate([self.target.c1], [self.target.c1 + self.source.c2]))
+        self.assertEqual(
+            str(query),
+            'MERGE INTO "t" AS "a" USING "s" AS "b" '
+            'ON ("a"."c1" = "b"."c2") '
+            'WHEN MATCHED THEN '
+            'UPDATE SET "c1" = ("a"."c1" + "b"."c2")')
+        self.assertEqual(query.params, ())
+
+    def test_matched_delete(self):
+        query = self.target.merge(
+            self.source, self.target.c1 == self.source.c2, MatchedDelete())
+        self.assertEqual(
+            str(query),
+            'MERGE INTO "t" AS "a" USING "s" AS "b" '
+            'ON ("a"."c1" = "b"."c2") '
+            'WHEN MATCHED THEN DELETE')
+        self.assertEqual(query.params, ())
+
+    def test_not_matched(self):
+        query = self.target.merge(
+            self.source, self.target.c1 == self.source.c2, NotMatched())
+        self.assertEqual(
+            str(query),
+            'MERGE INTO "t" AS "a" USING "s" AS "b" '
+            'ON ("a"."c1" = "b"."c2") '
+            'WHEN NOT MATCHED THEN DO NOTHING')
+        self.assertEqual(query.params, ())
+
+    def test_not_matched_insert(self):
+        query = self.target.merge(
+            self.source, self.target.c1 == self.source.c2,
+            NotMatchedInsert(
+                [self.target.c1, self.target.c2],
+                [self.source.c3, self.source.c4]))
+        self.assertEqual(
+            str(query),
+            'MERGE INTO "t" AS "a" USING "s" AS "b" '
+            'ON ("a"."c1" = "b"."c2") '
+            'WHEN NOT MATCHED THEN '
+            'INSERT ("c1", "c2") VALUES ("b"."c3", "b"."c4")')
+        self.assertEqual(query.params, ())
 
     def test_with(self):
         t1 = Table('t1')
-        w = With(query=t1.select())
-
-        query = self.table.insert(
-            [self.table.c1],
-            with_=[w],
-            values=w.select())
-        self.assertEqual(str(query),
-            'WITH "a" AS (SELECT * FROM "t1" AS "b") '
-            'INSERT INTO "t" AS "c" ("c1") SELECT * FROM "a" AS "a"')
-        self.assertEqual(tuple(query.params), ())
-
-    def test_insert_in_with(self):
-        t1 = Table('t1')
+        w = With(query=t1.select(where=t1.c2 == 42))
+        source = w.select()
 
-        w = With(query=self.table.insert(
-                [self.table.c1],
-                values=[['foo']],
-                returning=[self.table.id]))
-        query = t1.update(
-            [t1.c],
-            [w.id],
-            from_=[w],
-            with_=[w])
-        self.assertEqual(str(query),
-            'WITH "a" AS ('
-                'INSERT INTO "t" AS "b" ("c1") VALUES (%s) '
-                'RETURNING "b"."id") '
-            'UPDATE "t1" AS "c" SET "c" = "a"."id" FROM "a" AS "a"')
-        self.assertEqual(tuple(query.params), ('foo',))
-
-    def test_schema(self):
-        t1 = Table('t1', 'default')
-        query = t1.insert([t1.c1], [['foo']])
-
-        self.assertEqual(str(query),
-            'INSERT INTO "default"."t1" AS "a" ("c1") VALUES (%s)')
-        self.assertEqual(tuple(query.params), ('foo',))
+        query = self.target.merge(
+            source, self.target.c1 == source.c2, Matched(), with_=[w])
+        self.assertEqual(
+            str(query),
+            'WITH "a" AS (SELECT * FROM "t1" AS "d" WHERE ("d"."c2" = %s)) '
+            'MERGE INTO "t" AS "b" '
+            'USING (SELECT * FROM "a" AS "a") AS "c" '
+            'ON ("b"."c1" = "c"."c2") '
+            'WHEN MATCHED THEN DO NOTHING')
+        self.assertEqual(query.params, (42,))
```

### Comparing `python-sql-1.4.3/sql/tests/test_join.py` & `python_sql-1.5.0/sql/tests/test_join.py`

 * *Files identical despite different names*

### Comparing `python-sql-1.4.3/sql/tests/test_lateral.py` & `python_sql-1.5.0/sql/tests/test_lateral.py`

 * *Files identical despite different names*

### Comparing `python-sql-1.4.3/sql/tests/test_literal.py` & `python_sql-1.5.0/sql/tests/test_literal.py`

 * *Files identical despite different names*

### Comparing `python-sql-1.4.3/sql/tests/test_operators.py` & `python_sql-1.5.0/sql/tests/test_operators.py`

 * *Files 1% similar despite different names*

```diff
@@ -283,82 +283,82 @@
             self.assertEqual(rshift.params, (2,))
 
     def test_like(self):
         for like in [Like(self.table.c1, 'foo'),
                 self.table.c1.like('foo'),
                 ~NotLike(self.table.c1, 'foo'),
                 ~~Like(self.table.c1, 'foo')]:
-            self.assertEqual(str(like), '("c1" LIKE %s ESCAPE %s)')
-            self.assertEqual(like.params, ('foo', '\\'))
+            self.assertEqual(str(like), '("c1" LIKE %s)')
+            self.assertEqual(like.params, ('foo',))
 
     def test_like_escape(self):
         like = Like(self.table.c1, 'foo', escape='$')
         self.assertEqual(str(like), '("c1" LIKE %s ESCAPE %s)')
         self.assertEqual(like.params, ('foo', '$'))
 
     def test_like_escape_empty_false(self):
         flavor = Flavor(escape_empty=False)
         Flavor.set(flavor)
         try:
-            like = Like(self.table.c1, 'foo', escape='')
+            like = Like(self.table.c1, 'foo')
             self.assertEqual(str(like), '("c1" LIKE %s)')
             self.assertEqual(like.params, ('foo',))
         finally:
             Flavor.set(Flavor())
 
     def test_like_escape_empty_true(self):
         flavor = Flavor(escape_empty=True)
         Flavor.set(flavor)
         try:
-            like = Like(self.table.c1, 'foo', escape='')
+            like = Like(self.table.c1, 'foo')
             self.assertEqual(str(like), '("c1" LIKE %s ESCAPE %s)')
             self.assertEqual(like.params, ('foo', ''))
         finally:
             Flavor.set(Flavor())
 
     def test_ilike(self):
         flavor = Flavor(ilike=True)
         Flavor.set(flavor)
         try:
             for like in [ILike(self.table.c1, 'foo'),
                     self.table.c1.ilike('foo'),
                     ~NotILike(self.table.c1, 'foo')]:
-                self.assertEqual(str(like), '("c1" ILIKE %s ESCAPE %s)')
-                self.assertEqual(like.params, ('foo', '\\'))
+                self.assertEqual(str(like), '("c1" ILIKE %s)')
+                self.assertEqual(like.params, ('foo',))
         finally:
             Flavor.set(Flavor())
 
         flavor = Flavor(ilike=False)
         Flavor.set(flavor)
         try:
             like = ILike(self.table.c1, 'foo')
             self.assertEqual(
-                str(like), '(UPPER("c1") LIKE UPPER(%s) ESCAPE %s)')
-            self.assertEqual(like.params, ('foo', '\\'))
+                str(like), '(UPPER("c1") LIKE UPPER(%s))')
+            self.assertEqual(like.params, ('foo',))
         finally:
             Flavor.set(Flavor())
 
     def test_not_ilike(self):
         flavor = Flavor(ilike=True)
         Flavor.set(flavor)
         try:
             for like in [NotILike(self.table.c1, 'foo'),
                     ~self.table.c1.ilike('foo')]:
-                self.assertEqual(str(like), '("c1" NOT ILIKE %s ESCAPE %s)')
-                self.assertEqual(like.params, ('foo', '\\'))
+                self.assertEqual(str(like), '("c1" NOT ILIKE %s)')
+                self.assertEqual(like.params, ('foo',))
         finally:
             Flavor.set(Flavor())
 
         flavor = Flavor(ilike=False)
         Flavor.set(flavor)
         try:
             like = NotILike(self.table.c1, 'foo')
             self.assertEqual(
-                str(like), '(UPPER("c1") NOT LIKE UPPER(%s) ESCAPE %s)')
-            self.assertEqual(like.params, ('foo', '\\'))
+                str(like), '(UPPER("c1") NOT LIKE UPPER(%s))')
+            self.assertEqual(like.params, ('foo',))
         finally:
             Flavor.set(Flavor())
 
     def test_in(self):
         for in_ in [In(self.table.c1, [self.table.c2, 1, Null]),
                 ~NotIn(self.table.c1, [self.table.c2, 1, Null]),
                 ~~In(self.table.c1, [self.table.c2, 1, Null])]:
```

### Comparing `python-sql-1.4.3/sql/tests/test_order.py` & `python_sql-1.5.0/sql/tests/test_order.py`

 * *Files identical despite different names*

### Comparing `python-sql-1.4.3/sql/tests/test_select.py` & `python_sql-1.5.0/sql/tests/test_select.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # This file is part of python-sql.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 import unittest
 import warnings
 from copy import deepcopy
 
-from sql import Flavor, For, Join, Literal, Select, Table, Union, Window, With
+from sql import (
+    Cube, Flavor, For, Grouping, Join, Literal, Rollup, Select, Table, Union,
+    Window, With)
 from sql.aggregate import Max, Min
 from sql.functions import DatePart, Function, Now, Rank
 
 
 class TestSelect(unittest.TestCase):
     table = Table('t')
 
@@ -181,14 +183,58 @@
         self.assertEqual(tuple(query.params), ())
 
         query = self.table.select(Literal('foo'), group_by=Literal('foo'))
         self.assertEqual(str(query),
             'SELECT %s FROM "t" AS "a" GROUP BY %s')
         self.assertEqual(tuple(query.params), ('foo', 'foo'))
 
+    def test_select_group_by_grouping_sets(self):
+        query = self.table.select(
+            Literal('*'),
+            group_by=Grouping((self.table.a, self.table.b), (Literal('foo'),)))
+        self.assertEqual(str(query),
+            'SELECT %s FROM "t" AS "a" '
+            'GROUP BY GROUPING SETS (("a"."a", "a"."b"), (%s))')
+        self.assertEqual(tuple(query.params), ('*', 'foo',))
+
+        query = self.table.select(
+            Literal('*'),
+            group_by=[
+                self.table.a, Grouping((self.table.b,), (self.table.c,))])
+        self.assertEqual(str(query),
+            'SELECT %s FROM "t" AS "a" '
+            'GROUP BY "a"."a", GROUPING SETS (("a"."b"), ("a"."c"))')
+        self.assertEqual(tuple(query.params), ('*',))
+
+    def test_select_group_by_rollup(self):
+        query = self.table.select(
+            Literal('*'),
+            group_by=Rollup(self.table.a, self.table.b, Literal('foo')))
+        self.assertEqual(str(query),
+            'SELECT %s FROM "t" AS "a" '
+            'GROUP BY ROLLUP ("a"."a", "a"."b", %s)')
+        self.assertEqual(tuple(query.params), ('*', 'foo'))
+
+        query = self.table.select(
+            Literal('*'),
+            group_by=Rollup((self.table.a, self.table.b), self.table.c))
+        self.assertEqual(str(query),
+            'SELECT %s FROM "t" AS "a" '
+            'GROUP BY ROLLUP (("a"."a", "a"."b"), "a"."c")')
+        self.assertEqual(tuple(query.params), ('*',))
+
+    def test_select_group_by_cube(self):
+        query = self.table.select(
+            Literal('*'),
+            group_by=Cube(self.table.a, self.table.b))
+        self.assertEqual(str(query),
+            'SELECT %s FROM "t" AS "a" '
+            'GROUP BY CUBE ("a"."a", "a"."b")')
+        self.assertEqual(tuple(query.params), ('*',))
+
     def test_select_having(self):
         col1 = self.table.col1
         col2 = self.table.col2
         query = self.table.select(col1, Min(col2),
             having=(Min(col2) > 3))
         self.assertEqual(str(query),
             'SELECT "a"."col1", MIN("a"."col2") FROM "t" AS "a" '
```

### Comparing `python-sql-1.4.3/sql/tests/test_table.py` & `python_sql-1.5.0/sql/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `python-sql-1.4.3/sql/tests/test_update.py` & `python_sql-1.5.0/sql/tests/test_update.py`

 * *Files identical despite different names*

### Comparing `python-sql-1.4.3/sql/tests/test_values.py` & `python_sql-1.5.0/sql/tests/test_values.py`

 * *Files identical despite different names*

### Comparing `python-sql-1.4.3/sql/tests/test_window.py` & `python_sql-1.5.0/sql/tests/test_window.py`

 * *Files identical despite different names*

### Comparing `python-sql-1.4.3/sql/tests/test_with.py` & `python_sql-1.5.0/sql/tests/test_with.py`

 * *Files identical despite different names*

### Comparing `python-sql-1.4.3/tox.ini` & `python_sql-1.5.0/tox.ini`

 * *Files 25% similar despite different names*

```diff
@@ -7,13 +7,13 @@
 envlist = py35, py36, py37, py38, py39, py310, py311, py312, pypy3
 
 [testenv]
 usedevelop = true
 commands =
     coverage run --omit=*/tests/* -m xmlrunner discover -s sql.tests {posargs}
 commands_post =
-    coverage report --omit=README
-    coverage xml --omit=README
+    coverage report --omit=README.rst
+    coverage xml --omit=README.rst
 deps =
     coverage
     unittest-xml-reporting
 passenv = *
```

