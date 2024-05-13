# Comparing `tmp/pinned_import_linter-1.0.1.tar.gz` & `tmp/pinned_import_linter-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinned_import_linter-1.0.1.tar", last modified: Mon May 13 12:34:10 2024, max compression
+gzip compressed data, was "pinned_import_linter-1.1.0.tar", last modified: Mon May 13 15:37:53 2024, max compression
```

## Comparing `pinned_import_linter-1.0.1.tar` & `pinned_import_linter-1.1.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:34:10.791742 pinned_import_linter-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-13 12:34:07.000000 pinned_import_linter-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6433 2024-05-13 12:34:10.791742 pinned_import_linter-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5393 2024-05-13 12:34:07.000000 pinned_import_linter-1.0.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-13 12:34:07.000000 pinned_import_linter-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 12:34:10.791742 pinned_import_linter-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:34:10.787742 pinned_import_linter-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:34:10.791742 pinned_import_linter-1.0.1/src/pinned_import_linter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6433 2024-05-13 12:34:10.000000 pinned_import_linter-1.0.1/src/pinned_import_linter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-13 12:34:10.000000 pinned_import_linter-1.0.1/src/pinned_import_linter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 12:34:10.000000 pinned_import_linter-1.0.1/src/pinned_import_linter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-13 12:34:10.000000 pinned_import_linter-1.0.1/src/pinned_import_linter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 12:34:10.000000 pinned_import_linter-1.0.1/src/pinned_import_linter.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-13 12:34:10.000000 pinned_import_linter-1.0.1/src/pinned_import_linter.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:34:10.791742 pinned_import_linter-1.0.1/src/pinnedimportlinter/
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-13 12:34:07.000000 pinned_import_linter-1.0.1/src/pinnedimportlinter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:34:10.791742 pinned_import_linter-1.0.1/src/pinnedimportlinter/application/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-13 12:34:07.000000 pinned_import_linter-1.0.1/src/pinnedimportlinter/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-05-13 12:34:07.000000 pinned_import_linter-1.0.1/src/pinnedimportlinter/application/config_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-13 12:34:07.000000 pinned_import_linter-1.0.1/src/pinnedimportlinter/application/printer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-05-13 12:34:07.000000 pinned_import_linter-1.0.1/src/pinnedimportlinter/application/rule_checker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:34:10.791742 pinned_import_linter-1.0.1/src/pinnedimportlinter/application/use_cases/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 12:34:07.000000 pinned_import_linter-1.0.1/src/pinnedimportlinter/application/use_cases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-13 12:34:07.000000 pinned_import_linter-1.0.1/src/pinnedimportlinter/application/use_cases/checker_files_content.py
--rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-05-13 12:34:07.000000 pinned_import_linter-1.0.1/src/pinnedimportlinter/application/use_cases/walk.py
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-13 12:34:07.000000 pinned_import_linter-1.0.1/src/pinnedimportlinter/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:34:10.791742 pinned_import_linter-1.0.1/src/pinnedimportlinter/domain/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 12:34:07.000000 pinned_import_linter-1.0.1/src/pinnedimportlinter/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-13 12:34:07.000000 pinned_import_linter-1.0.1/src/pinnedimportlinter/domain/constant.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-13 12:34:07.000000 pinned_import_linter-1.0.1/src/pinnedimportlinter/domain/linter.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 12:34:07.000000 pinned_import_linter-1.0.1/src/pinnedimportlinter/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:37:53.667987 pinned_import_linter-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-13 15:37:48.000000 pinned_import_linter-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6433 2024-05-13 15:37:53.667987 pinned_import_linter-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5393 2024-05-13 15:37:48.000000 pinned_import_linter-1.1.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-13 15:37:48.000000 pinned_import_linter-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 15:37:53.667987 pinned_import_linter-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:37:53.659987 pinned_import_linter-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:37:53.667987 pinned_import_linter-1.1.0/src/pinned_import_linter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6433 2024-05-13 15:37:53.000000 pinned_import_linter-1.1.0/src/pinned_import_linter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-13 15:37:53.000000 pinned_import_linter-1.1.0/src/pinned_import_linter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 15:37:53.000000 pinned_import_linter-1.1.0/src/pinned_import_linter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-13 15:37:53.000000 pinned_import_linter-1.1.0/src/pinned_import_linter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 15:37:53.000000 pinned_import_linter-1.1.0/src/pinned_import_linter.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-13 15:37:53.000000 pinned_import_linter-1.1.0/src/pinned_import_linter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:37:53.663987 pinned_import_linter-1.1.0/src/pinnedimportlinter/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-13 15:37:48.000000 pinned_import_linter-1.1.0/src/pinnedimportlinter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:37:53.663987 pinned_import_linter-1.1.0/src/pinnedimportlinter/application/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-13 15:37:48.000000 pinned_import_linter-1.1.0/src/pinnedimportlinter/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-05-13 15:37:48.000000 pinned_import_linter-1.1.0/src/pinnedimportlinter/application/config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-13 15:37:48.000000 pinned_import_linter-1.1.0/src/pinnedimportlinter/application/printer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-05-13 15:37:48.000000 pinned_import_linter-1.1.0/src/pinnedimportlinter/application/rule_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:37:53.663987 pinned_import_linter-1.1.0/src/pinnedimportlinter/application/use_cases/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:37:48.000000 pinned_import_linter-1.1.0/src/pinnedimportlinter/application/use_cases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-13 15:37:48.000000 pinned_import_linter-1.1.0/src/pinnedimportlinter/application/use_cases/checker_files_content.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-05-13 15:37:48.000000 pinned_import_linter-1.1.0/src/pinnedimportlinter/application/use_cases/walk.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-13 15:37:48.000000 pinned_import_linter-1.1.0/src/pinnedimportlinter/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:37:53.667987 pinned_import_linter-1.1.0/src/pinnedimportlinter/domain/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:37:48.000000 pinned_import_linter-1.1.0/src/pinnedimportlinter/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-13 15:37:48.000000 pinned_import_linter-1.1.0/src/pinnedimportlinter/domain/constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-13 15:37:48.000000 pinned_import_linter-1.1.0/src/pinnedimportlinter/domain/linter.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:37:48.000000 pinned_import_linter-1.1.0/src/pinnedimportlinter/py.typed
```

### Comparing `pinned_import_linter-1.0.1/LICENSE` & `pinned_import_linter-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pinned_import_linter-1.0.1/PKG-INFO` & `pinned_import_linter-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinned-import-linter
-Version: 1.0.1
+Version: 1.1.0
 Summary: A plugin for python that will help you standardize imports from any libraries.
 Author-email: Danil Gubanov <20949800+maintainer64@users.noreply.github.com>
 License: MIT LICENSE
 Project-URL: Source-code, https://github.com/maintainer64/pinned-import-linter/
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
```

### Comparing `pinned_import_linter-1.0.1/README.rst` & `pinned_import_linter-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `pinned_import_linter-1.0.1/pyproject.toml` & `pinned_import_linter-1.1.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 build-backend = "setuptools.build_meta"
 requires = [
   "setuptools>=61.2",
 ]
 
 [project]
 name = "pinned-import-linter"
-version = "1.0.1"
+version = "1.1.0"
 description = "A plugin for python that will help you standardize imports from any libraries."
 license = { text = "MIT LICENSE" }
 authors = [
     { name = "Danil Gubanov", email = "20949800+maintainer64@users.noreply.github.com" },
 ]
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `pinned_import_linter-1.0.1/src/pinned_import_linter.egg-info/PKG-INFO` & `pinned_import_linter-1.1.0/src/pinned_import_linter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinned-import-linter
-Version: 1.0.1
+Version: 1.1.0
 Summary: A plugin for python that will help you standardize imports from any libraries.
 Author-email: Danil Gubanov <20949800+maintainer64@users.noreply.github.com>
 License: MIT LICENSE
 Project-URL: Source-code, https://github.com/maintainer64/pinned-import-linter/
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
```

### Comparing `pinned_import_linter-1.0.1/src/pinned_import_linter.egg-info/SOURCES.txt` & `pinned_import_linter-1.1.0/src/pinned_import_linter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pinned_import_linter-1.0.1/src/pinnedimportlinter/application/config_parser.py` & `pinned_import_linter-1.1.0/src/pinnedimportlinter/application/config_parser.py`

 * *Files identical despite different names*

### Comparing `pinned_import_linter-1.0.1/src/pinnedimportlinter/application/printer.py` & `pinned_import_linter-1.1.0/src/pinnedimportlinter/application/printer.py`

 * *Files identical despite different names*

### Comparing `pinned_import_linter-1.0.1/src/pinnedimportlinter/application/rule_checker.py` & `pinned_import_linter-1.1.0/src/pinnedimportlinter/application/rule_checker.py`

 * *Files identical despite different names*

### Comparing `pinned_import_linter-1.0.1/src/pinnedimportlinter/application/use_cases/checker_files_content.py` & `pinned_import_linter-1.1.0/src/pinnedimportlinter/application/use_cases/checker_files_content.py`

 * *Files identical despite different names*

### Comparing `pinned_import_linter-1.0.1/src/pinnedimportlinter/application/use_cases/walk.py` & `pinned_import_linter-1.1.0/src/pinnedimportlinter/application/use_cases/walk.py`

 * *Files identical despite different names*

### Comparing `pinned_import_linter-1.0.1/src/pinnedimportlinter/cli.py` & `pinned_import_linter-1.1.0/src/pinnedimportlinter/cli.py`

 * *Files identical despite different names*

