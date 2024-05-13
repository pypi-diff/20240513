# Comparing `tmp/hackerargs-0.0.1.tar.gz` & `tmp/hackerargs-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hackerargs-0.0.1.tar", last modified: Mon May 13 18:57:02 2024, max compression
+gzip compressed data, was "hackerargs-1.0.0.tar", last modified: Mon May 13 18:58:17 2024, max compression
```

## Comparing `hackerargs-0.0.1.tar` & `hackerargs-1.0.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)        0 2024-05-13 18:57:02.609883 hackerargs-0.0.1/
--rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)     1055 2024-05-11 21:31:25.000000 hackerargs-0.0.1/LICENSE
--rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)     7804 2024-05-13 18:57:02.601882 hackerargs-0.0.1/PKG-INFO
--rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)     7476 2024-05-13 18:47:12.000000 hackerargs-0.0.1/README.md
-drwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)        0 2024-05-13 18:57:02.276929 hackerargs-0.0.1/hackerargs/
--rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)       55 2024-05-12 02:54:31.000000 hackerargs-0.0.1/hackerargs/__init__.py
--rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)      380 2024-05-12 19:36:14.000000 hackerargs-0.0.1/hackerargs/argparse_access.py
--rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)     8924 2024-05-12 21:11:53.000000 hackerargs-0.0.1/hackerargs/args.py
--rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)     1185 2024-05-12 00:25:18.000000 hackerargs-0.0.1/hackerargs/strict_bool_yaml.py
-drwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)        0 2024-05-13 18:57:02.585864 hackerargs-0.0.1/hackerargs.egg-info/
--rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)     7804 2024-05-13 18:57:01.000000 hackerargs-0.0.1/hackerargs.egg-info/PKG-INFO
--rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)      373 2024-05-13 18:57:02.000000 hackerargs-0.0.1/hackerargs.egg-info/SOURCES.txt
--rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)        1 2024-05-13 18:57:01.000000 hackerargs-0.0.1/hackerargs.egg-info/dependency_links.txt
--rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)        7 2024-05-13 18:57:01.000000 hackerargs-0.0.1/hackerargs.egg-info/requires.txt
--rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)       11 2024-05-13 18:57:01.000000 hackerargs-0.0.1/hackerargs.egg-info/top_level.txt
--rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)      394 2024-05-12 20:15:50.000000 hackerargs-0.0.1/pyproject.toml
--rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)       38 2024-05-13 18:57:02.617871 hackerargs-0.0.1/setup.cfg
-drwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)        0 2024-05-13 18:57:02.552692 hackerargs-0.0.1/tests/
--rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)      492 2024-05-12 21:02:44.000000 hackerargs-0.0.1/tests/test_access.py
--rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)      776 2024-05-12 21:02:22.000000 hackerargs-0.0.1/tests/test_positional.py
--rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)      913 2024-05-12 21:02:25.000000 hackerargs-0.0.1/tests/test_priority.py
+drwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)        0 2024-05-13 18:58:17.262904 hackerargs-1.0.0/
+-rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)     1055 2024-05-11 21:31:25.000000 hackerargs-1.0.0/LICENSE
+-rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)     7804 2024-05-13 18:58:17.251710 hackerargs-1.0.0/PKG-INFO
+-rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)     7476 2024-05-13 18:47:12.000000 hackerargs-1.0.0/README.md
+drwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)        0 2024-05-13 18:58:16.887506 hackerargs-1.0.0/hackerargs/
+-rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)       55 2024-05-12 02:54:31.000000 hackerargs-1.0.0/hackerargs/__init__.py
+-rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)      380 2024-05-12 19:36:14.000000 hackerargs-1.0.0/hackerargs/argparse_access.py
+-rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)     8924 2024-05-12 21:11:53.000000 hackerargs-1.0.0/hackerargs/args.py
+-rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)     1185 2024-05-12 00:25:18.000000 hackerargs-1.0.0/hackerargs/strict_bool_yaml.py
+drwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)        0 2024-05-13 18:58:17.226528 hackerargs-1.0.0/hackerargs.egg-info/
+-rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)     7804 2024-05-13 18:58:16.000000 hackerargs-1.0.0/hackerargs.egg-info/PKG-INFO
+-rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)      373 2024-05-13 18:58:16.000000 hackerargs-1.0.0/hackerargs.egg-info/SOURCES.txt
+-rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)        1 2024-05-13 18:58:16.000000 hackerargs-1.0.0/hackerargs.egg-info/dependency_links.txt
+-rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)        7 2024-05-13 18:58:16.000000 hackerargs-1.0.0/hackerargs.egg-info/requires.txt
+-rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)       11 2024-05-13 18:58:16.000000 hackerargs-1.0.0/hackerargs.egg-info/top_level.txt
+-rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)      394 2024-05-13 18:58:00.000000 hackerargs-1.0.0/pyproject.toml
+-rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)       38 2024-05-13 18:58:17.267944 hackerargs-1.0.0/setup.cfg
+drwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)        0 2024-05-13 18:58:17.172559 hackerargs-1.0.0/tests/
+-rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)      492 2024-05-12 21:02:44.000000 hackerargs-1.0.0/tests/test_access.py
+-rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)      776 2024-05-12 21:02:22.000000 hackerargs-1.0.0/tests/test_positional.py
+-rwxrwxrwx   0 maxwshen  (1000) maxwshen  (1000)      913 2024-05-12 21:02:25.000000 hackerargs-1.0.0/tests/test_priority.py
```

### Comparing `hackerargs-0.0.1/LICENSE` & `hackerargs-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hackerargs-0.0.1/PKG-INFO` & `hackerargs-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hackerargs
-Version: 0.0.1
+Version: 1.0.0
 Summary: Simple config and argument system
 Author: Max Shen
 Project-URL: Homepage, https://github.com/maxwshen/hackerargs
 Project-URL: Issues, https://github.com/maxwshen/hackerargs/issues
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: PyYAML
```

### Comparing `hackerargs-0.0.1/README.md` & `hackerargs-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `hackerargs-0.0.1/hackerargs/args.py` & `hackerargs-1.0.0/hackerargs/args.py`

 * *Files identical despite different names*

### Comparing `hackerargs-0.0.1/hackerargs/strict_bool_yaml.py` & `hackerargs-1.0.0/hackerargs/strict_bool_yaml.py`

 * *Files identical despite different names*

### Comparing `hackerargs-0.0.1/hackerargs.egg-info/PKG-INFO` & `hackerargs-1.0.0/hackerargs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hackerargs
-Version: 0.0.1
+Version: 1.0.0
 Summary: Simple config and argument system
 Author: Max Shen
 Project-URL: Homepage, https://github.com/maxwshen/hackerargs
 Project-URL: Issues, https://github.com/maxwshen/hackerargs/issues
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: PyYAML
```

### Comparing `hackerargs-0.0.1/tests/test_positional.py` & `hackerargs-1.0.0/tests/test_positional.py`

 * *Files identical despite different names*

### Comparing `hackerargs-0.0.1/tests/test_priority.py` & `hackerargs-1.0.0/tests/test_priority.py`

 * *Files identical despite different names*

