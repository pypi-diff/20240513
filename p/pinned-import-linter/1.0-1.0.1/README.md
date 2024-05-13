# Comparing `tmp/pinned_import_linter-1.0.tar.gz` & `tmp/pinned_import_linter-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinned_import_linter-1.0.tar", last modified: Mon May 13 07:53:13 2024, max compression
+gzip compressed data, was "pinned_import_linter-1.0.1.tar", last modified: Mon May 13 12:34:10 2024, max compression
```

## Comparing `pinned_import_linter-1.0.tar` & `pinned_import_linter-1.0.1.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:53:13.827222 pinned_import_linter-1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-13 07:53:09.000000 pinned_import_linter-1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6006 2024-05-13 07:53:13.827222 pinned_import_linter-1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4968 2024-05-13 07:53:09.000000 pinned_import_linter-1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-13 07:53:09.000000 pinned_import_linter-1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 07:53:13.827222 pinned_import_linter-1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:53:13.823222 pinned_import_linter-1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:53:13.827222 pinned_import_linter-1.0/src/pinned_import_linter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6006 2024-05-13 07:53:13.000000 pinned_import_linter-1.0/src/pinned_import_linter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-13 07:53:13.000000 pinned_import_linter-1.0/src/pinned_import_linter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 07:53:13.000000 pinned_import_linter-1.0/src/pinned_import_linter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-13 07:53:13.000000 pinned_import_linter-1.0/src/pinned_import_linter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 07:53:13.000000 pinned_import_linter-1.0/src/pinned_import_linter.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-13 07:53:13.000000 pinned_import_linter-1.0/src/pinned_import_linter.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:53:13.823222 pinned_import_linter-1.0/src/pinnedimportlinter/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-13 07:53:09.000000 pinned_import_linter-1.0/src/pinnedimportlinter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:53:13.823222 pinned_import_linter-1.0/src/pinnedimportlinter/application/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-13 07:53:09.000000 pinned_import_linter-1.0/src/pinnedimportlinter/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-05-13 07:53:09.000000 pinned_import_linter-1.0/src/pinnedimportlinter/application/config_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-13 07:53:09.000000 pinned_import_linter-1.0/src/pinnedimportlinter/application/printer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-05-13 07:53:09.000000 pinned_import_linter-1.0/src/pinnedimportlinter/application/rule_checker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:53:13.827222 pinned_import_linter-1.0/src/pinnedimportlinter/application/use_cases/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 07:53:09.000000 pinned_import_linter-1.0/src/pinnedimportlinter/application/use_cases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-13 07:53:09.000000 pinned_import_linter-1.0/src/pinnedimportlinter/application/use_cases/checker_files_content.py
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-13 07:53:09.000000 pinned_import_linter-1.0/src/pinnedimportlinter/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:53:13.827222 pinned_import_linter-1.0/src/pinnedimportlinter/domain/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 07:53:09.000000 pinned_import_linter-1.0/src/pinnedimportlinter/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-13 07:53:09.000000 pinned_import_linter-1.0/src/pinnedimportlinter/domain/constant.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-13 07:53:09.000000 pinned_import_linter-1.0/src/pinnedimportlinter/domain/linter.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 07:53:09.000000 pinned_import_linter-1.0/src/pinnedimportlinter/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:34:10.791742 pinned_import_linter-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-13 12:34:07.000000 pinned_import_linter-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6433 2024-05-13 12:34:10.791742 pinned_import_linter-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5393 2024-05-13 12:34:07.000000 pinned_import_linter-1.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-13 12:34:07.000000 pinned_import_linter-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 12:34:10.791742 pinned_import_linter-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:34:10.787742 pinned_import_linter-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:34:10.791742 pinned_import_linter-1.0.1/src/pinned_import_linter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6433 2024-05-13 12:34:10.000000 pinned_import_linter-1.0.1/src/pinned_import_linter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-13 12:34:10.000000 pinned_import_linter-1.0.1/src/pinned_import_linter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 12:34:10.000000 pinned_import_linter-1.0.1/src/pinned_import_linter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-13 12:34:10.000000 pinned_import_linter-1.0.1/src/pinned_import_linter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 12:34:10.000000 pinned_import_linter-1.0.1/src/pinned_import_linter.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-13 12:34:10.000000 pinned_import_linter-1.0.1/src/pinned_import_linter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:34:10.791742 pinned_import_linter-1.0.1/src/pinnedimportlinter/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-13 12:34:07.000000 pinned_import_linter-1.0.1/src/pinnedimportlinter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:34:10.791742 pinned_import_linter-1.0.1/src/pinnedimportlinter/application/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-13 12:34:07.000000 pinned_import_linter-1.0.1/src/pinnedimportlinter/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-05-13 12:34:07.000000 pinned_import_linter-1.0.1/src/pinnedimportlinter/application/config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-13 12:34:07.000000 pinned_import_linter-1.0.1/src/pinnedimportlinter/application/printer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-05-13 12:34:07.000000 pinned_import_linter-1.0.1/src/pinnedimportlinter/application/rule_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:34:10.791742 pinned_import_linter-1.0.1/src/pinnedimportlinter/application/use_cases/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 12:34:07.000000 pinned_import_linter-1.0.1/src/pinnedimportlinter/application/use_cases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-13 12:34:07.000000 pinned_import_linter-1.0.1/src/pinnedimportlinter/application/use_cases/checker_files_content.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-05-13 12:34:07.000000 pinned_import_linter-1.0.1/src/pinnedimportlinter/application/use_cases/walk.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-13 12:34:07.000000 pinned_import_linter-1.0.1/src/pinnedimportlinter/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:34:10.791742 pinned_import_linter-1.0.1/src/pinnedimportlinter/domain/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 12:34:07.000000 pinned_import_linter-1.0.1/src/pinnedimportlinter/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-13 12:34:07.000000 pinned_import_linter-1.0.1/src/pinnedimportlinter/domain/constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-13 12:34:07.000000 pinned_import_linter-1.0.1/src/pinnedimportlinter/domain/linter.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 12:34:07.000000 pinned_import_linter-1.0.1/src/pinnedimportlinter/py.typed
```

### Comparing `pinned_import_linter-1.0/LICENSE` & `pinned_import_linter-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pinned_import_linter-1.0/PKG-INFO` & `pinned_import_linter-1.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinned-import-linter
-Version: 1.0
+Version: 1.0.1
 Summary: A plugin for python that will help you standardize imports from any libraries.
 Author-email: Danil Gubanov <20949800+maintainer64@users.noreply.github.com>
 License: MIT LICENSE
 Project-URL: Source-code, https://github.com/maintainer64/pinned-import-linter/
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
@@ -29,16 +29,16 @@
 .. image:: https://img.shields.io/pypi/v/pinned-import-linter.svg
     :target: https://pypi.org/project/pinned-import-linter
 
 .. image:: https://img.shields.io/pypi/pyversions/pinned-import-linter.svg
     :alt: Python versions
     :target: https://pypi.org/project/pinned-import-linter/
 
-.. image:: https://github.com/maintainer64/pinned-import-linter/workflows/CI/badge.svg?branch=main
-     :target: https://github.com/maintainer64/pinned-import-linter/actions?workflow=CI
+.. image:: https://github.com/maintainer64/pinned-import-linter/actions/workflows/main.yml/badge.svg?branch=main
+     :target: https://github.com/maintainer64/pinned-import-linter/actions/workflows/main.yml
      :alt: CI Status
 
 ⚡ A plugin for python that will help you standardize imports from any libraries.
 
 * Free software: MIT License
 
 Overview
@@ -77,14 +77,16 @@
 (then it will need to be connected via the ``--config`` parameter in the *CLI*)
 with similar contents:
 
 .. code-block:: ini
 
     [pinned_import_linter]
     package_names = typing,itertools,datetime,sys,pathlib
+    file_extensions = py,pyi
+    exclude = ^(venv|.venv)
 
     [pinned_import_linter.typing]
     allow_alias = true
     alias_names = t
     allow_from = false
     allow_package = false
 
@@ -132,15 +134,15 @@
 4. For the other Libraries (not described) in
 the configuration can be imported in any way.
 
 
 Now, from your project root, run::
 
 
-    lint-pinned-imports --config tox.ini main.py
+    lint-pinned-imports --config tox.ini main.py your_folder .
 
 For a file with this configuration:
 
 .. code-block:: python
 
     from typing import Callable, List
     from itertools import product
@@ -159,18 +161,33 @@
 
 Connect all files on pre-commit
 -------------------------------
 
 1. Add package on dev-dependency in your project on Python
 2. Add step into your .pre-commit-config.yaml
 
+Check all files on directories:
+
+.. code-block:: yml
+
+    repos:
+      - repo: local
+        hooks:
+          - id: lint-pinned-imports
+            name: Restricted imports
+            entry: lint-pinned-imports --config tox.ini .
+            language: system
+            pass_filenames: false
+
+
+Alternative .pre-commit-config.yaml checked only changed files:
+
 .. code-block:: yml
 
     repos:
       - repo: local
         hooks:
           - id: lint-pinned-imports
             name: Restricted imports
             entry: lint-pinned-imports --config tox.ini
             language: system
-            files: \.py$
-            pass_filenames: true
+            types: [ python ]
```

### Comparing `pinned_import_linter-1.0/README.rst` & `pinned_import_linter-1.0.1/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 .. image:: https://img.shields.io/pypi/v/pinned-import-linter.svg
     :target: https://pypi.org/project/pinned-import-linter
 
 .. image:: https://img.shields.io/pypi/pyversions/pinned-import-linter.svg
     :alt: Python versions
     :target: https://pypi.org/project/pinned-import-linter/
 
-.. image:: https://github.com/maintainer64/pinned-import-linter/workflows/CI/badge.svg?branch=main
-     :target: https://github.com/maintainer64/pinned-import-linter/actions?workflow=CI
+.. image:: https://github.com/maintainer64/pinned-import-linter/actions/workflows/main.yml/badge.svg?branch=main
+     :target: https://github.com/maintainer64/pinned-import-linter/actions/workflows/main.yml
      :alt: CI Status
 
 ⚡ A plugin for python that will help you standardize imports from any libraries.
 
 * Free software: MIT License
 
 Overview
@@ -53,14 +53,16 @@
 (then it will need to be connected via the ``--config`` parameter in the *CLI*)
 with similar contents:
 
 .. code-block:: ini
 
     [pinned_import_linter]
     package_names = typing,itertools,datetime,sys,pathlib
+    file_extensions = py,pyi
+    exclude = ^(venv|.venv)
 
     [pinned_import_linter.typing]
     allow_alias = true
     alias_names = t
     allow_from = false
     allow_package = false
 
@@ -108,15 +110,15 @@
 4. For the other Libraries (not described) in
 the configuration can be imported in any way.
 
 
 Now, from your project root, run::
 
 
-    lint-pinned-imports --config tox.ini main.py
+    lint-pinned-imports --config tox.ini main.py your_folder .
 
 For a file with this configuration:
 
 .. code-block:: python
 
     from typing import Callable, List
     from itertools import product
@@ -135,18 +137,33 @@
 
 Connect all files on pre-commit
 -------------------------------
 
 1. Add package on dev-dependency in your project on Python
 2. Add step into your .pre-commit-config.yaml
 
+Check all files on directories:
+
+.. code-block:: yml
+
+    repos:
+      - repo: local
+        hooks:
+          - id: lint-pinned-imports
+            name: Restricted imports
+            entry: lint-pinned-imports --config tox.ini .
+            language: system
+            pass_filenames: false
+
+
+Alternative .pre-commit-config.yaml checked only changed files:
+
 .. code-block:: yml
 
     repos:
       - repo: local
         hooks:
           - id: lint-pinned-imports
             name: Restricted imports
             entry: lint-pinned-imports --config tox.ini
             language: system
-            files: \.py$
-            pass_filenames: true
+            types: [ python ]
```

### Comparing `pinned_import_linter-1.0/pyproject.toml` & `pinned_import_linter-1.0.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 build-backend = "setuptools.build_meta"
 requires = [
   "setuptools>=61.2",
 ]
 
 [project]
 name = "pinned-import-linter"
-version = "1.0"
+version = "1.0.1"
 description = "A plugin for python that will help you standardize imports from any libraries."
 license = { text = "MIT LICENSE" }
 authors = [
     { name = "Danil Gubanov", email = "20949800+maintainer64@users.noreply.github.com" },
 ]
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `pinned_import_linter-1.0/src/pinned_import_linter.egg-info/PKG-INFO` & `pinned_import_linter-1.0.1/src/pinned_import_linter.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinned-import-linter
-Version: 1.0
+Version: 1.0.1
 Summary: A plugin for python that will help you standardize imports from any libraries.
 Author-email: Danil Gubanov <20949800+maintainer64@users.noreply.github.com>
 License: MIT LICENSE
 Project-URL: Source-code, https://github.com/maintainer64/pinned-import-linter/
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
@@ -29,16 +29,16 @@
 .. image:: https://img.shields.io/pypi/v/pinned-import-linter.svg
     :target: https://pypi.org/project/pinned-import-linter
 
 .. image:: https://img.shields.io/pypi/pyversions/pinned-import-linter.svg
     :alt: Python versions
     :target: https://pypi.org/project/pinned-import-linter/
 
-.. image:: https://github.com/maintainer64/pinned-import-linter/workflows/CI/badge.svg?branch=main
-     :target: https://github.com/maintainer64/pinned-import-linter/actions?workflow=CI
+.. image:: https://github.com/maintainer64/pinned-import-linter/actions/workflows/main.yml/badge.svg?branch=main
+     :target: https://github.com/maintainer64/pinned-import-linter/actions/workflows/main.yml
      :alt: CI Status
 
 ⚡ A plugin for python that will help you standardize imports from any libraries.
 
 * Free software: MIT License
 
 Overview
@@ -77,14 +77,16 @@
 (then it will need to be connected via the ``--config`` parameter in the *CLI*)
 with similar contents:
 
 .. code-block:: ini
 
     [pinned_import_linter]
     package_names = typing,itertools,datetime,sys,pathlib
+    file_extensions = py,pyi
+    exclude = ^(venv|.venv)
 
     [pinned_import_linter.typing]
     allow_alias = true
     alias_names = t
     allow_from = false
     allow_package = false
 
@@ -132,15 +134,15 @@
 4. For the other Libraries (not described) in
 the configuration can be imported in any way.
 
 
 Now, from your project root, run::
 
 
-    lint-pinned-imports --config tox.ini main.py
+    lint-pinned-imports --config tox.ini main.py your_folder .
 
 For a file with this configuration:
 
 .. code-block:: python
 
     from typing import Callable, List
     from itertools import product
@@ -159,18 +161,33 @@
 
 Connect all files on pre-commit
 -------------------------------
 
 1. Add package on dev-dependency in your project on Python
 2. Add step into your .pre-commit-config.yaml
 
+Check all files on directories:
+
+.. code-block:: yml
+
+    repos:
+      - repo: local
+        hooks:
+          - id: lint-pinned-imports
+            name: Restricted imports
+            entry: lint-pinned-imports --config tox.ini .
+            language: system
+            pass_filenames: false
+
+
+Alternative .pre-commit-config.yaml checked only changed files:
+
 .. code-block:: yml
 
     repos:
       - repo: local
         hooks:
           - id: lint-pinned-imports
             name: Restricted imports
             entry: lint-pinned-imports --config tox.ini
             language: system
-            files: \.py$
-            pass_filenames: true
+            types: [ python ]
```

### Comparing `pinned_import_linter-1.0/src/pinned_import_linter.egg-info/SOURCES.txt` & `pinned_import_linter-1.0.1/src/pinned_import_linter.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,10 +13,11 @@
 src/pinnedimportlinter/py.typed
 src/pinnedimportlinter/application/__init__.py
 src/pinnedimportlinter/application/config_parser.py
 src/pinnedimportlinter/application/printer.py
 src/pinnedimportlinter/application/rule_checker.py
 src/pinnedimportlinter/application/use_cases/__init__.py
 src/pinnedimportlinter/application/use_cases/checker_files_content.py
+src/pinnedimportlinter/application/use_cases/walk.py
 src/pinnedimportlinter/domain/__init__.py
 src/pinnedimportlinter/domain/constant.py
 src/pinnedimportlinter/domain/linter.py
```

### Comparing `pinned_import_linter-1.0/src/pinnedimportlinter/application/config_parser.py` & `pinned_import_linter-1.0.1/src/pinnedimportlinter/application/config_parser.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 from __future__ import annotations
 
 import configparser
 import dataclasses
+import re
 import typing as t
 
 from ..domain.constant import CONFIG_BLOCK_NAME
 
 
-def _string_spit(string: str) -> t.List[str]:
+def _string_spit(string: str | list[str]) -> list[str]:
+    if isinstance(string, list):
+        return string
     return [name.strip() for name in string.split(",") if name.strip()]
 
 
 @dataclasses.dataclass
 class PackageNameSettingsBlock:
     allow_alias: bool
-    alias_names: t.Set[str]
+    alias_names: set[str]
     allow_from: bool
     allow_package: bool
 
     @classmethod
     def from_dict(cls, value: configparser.SectionProxy) -> t.Self:
         return cls(
             allow_alias=value.getboolean("allow_alias", fallback=True),
@@ -44,32 +47,43 @@
         allow_alias=True,
         alias_names=set(),
         allow_from=True,
         allow_package=True,
     )
 
     def __init__(
-        self, config_path: str, packages: dict[str, PackageNameSettingsBlock] | None = None
+        self,
+        config_path: str,
+        file_extensions: set[str] | None = None,
+        exclude: str | None = None,
+        packages: dict[str, PackageNameSettingsBlock] | None = None,
     ):
         self.config_path = config_path
+        self.file_extensions: set[str] = file_extensions or {"py"}
+        self.exclude: t.Pattern[str] | None = re.compile(exclude) if exclude else None
         self._packages = packages or {}
 
     def get(self, package_name: str | None) -> PackageNameSettingsBlock:
         if not package_name:
             return self.__default__
         return self._packages.get(package_name) or self.__default__
 
     @classmethod
     def read_config(cls, config_path: str) -> t.Self:
         config = configparser.ConfigParser()
         config.read(config_path)
         if CONFIG_BLOCK_NAME not in config:
             return cls(config_path=config_path)
-        package_names = _string_spit(config[CONFIG_BLOCK_NAME].get("package_names") or "")
+        main_block = config[CONFIG_BLOCK_NAME]
+        package_names = _string_spit(main_block.get("package_names") or "")
+        file_extensions = _string_spit(main_block.get("file_extensions") or "")
+        exclude = main_block.get("exclude", None)
         return cls(
             config_path=config_path,
+            file_extensions=set(file_extensions),
+            exclude=exclude,
             packages={
                 package_name: PackageNameSettingsBlock.from_dict(config[block_name])
                 for package_name in package_names
                 if (block_name := f"{CONFIG_BLOCK_NAME}.{package_name}") in config
             },
         )
```

### Comparing `pinned_import_linter-1.0/src/pinnedimportlinter/application/printer.py` & `pinned_import_linter-1.0.1/src/pinnedimportlinter/application/printer.py`

 * *Files identical despite different names*

### Comparing `pinned_import_linter-1.0/src/pinnedimportlinter/application/rule_checker.py` & `pinned_import_linter-1.0.1/src/pinnedimportlinter/application/rule_checker.py`

 * *Files identical despite different names*

### Comparing `pinned_import_linter-1.0/src/pinnedimportlinter/application/use_cases/checker_files_content.py` & `pinned_import_linter-1.0.1/src/pinnedimportlinter/application/use_cases/checker_files_content.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,35 +3,40 @@
 import sys
 
 from ...domain.constant import EXIT_STATUS_ERROR
 from ...domain.constant import EXIT_STATUS_SUCCESS
 from ..config_parser import LinterConfig
 from ..printer import Printer
 from ..rule_checker import RuleCheckerService
+from .walk import search_python_files
 
 
 def read_file(filename: str) -> str:
     with open(filename, encoding="utf-8") as file:
         return file.read()
 
 
 def checker_files_content_uc(
     configure_path: str,
-    file_path_to_check: list[str],
+    paths_to_check: list[str],
 ) -> None:
     """
     Load configure and check files
     :param configure_path: Path on ini file
-    :param file_path_to_check: List of files to check
+    :param paths_to_check: List of files or directories to check
     :return: system exit code
     """
     config = LinterConfig.read_config(config_path=configure_path)
     printer = Printer()
     errors = 0
-    for filename in file_path_to_check:
+    for file_path in search_python_files(
+        paths_to_check=paths_to_check,
+        config=config,
+    ):
+        filename = str(file_path)
         file_content = read_file(filename=filename)
-        errors = RuleCheckerService(
+        errors += RuleCheckerService(
             filename=filename, config=config, printer=printer
         ).check_content(file_content=file_content)
     printer.print()
     exit_code = EXIT_STATUS_ERROR if errors else EXIT_STATUS_SUCCESS
     sys.exit(exit_code)
```

### Comparing `pinned_import_linter-1.0/src/pinnedimportlinter/cli.py` & `pinned_import_linter-1.0.1/src/pinnedimportlinter/cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,24 +3,26 @@
 import argparse
 
 from .application.use_cases.checker_files_content import checker_files_content_uc
 
 
 def argument_parser() -> argparse.Namespace:
     parser = argparse.ArgumentParser(description="Check for restricted imports in Python files.")
-    parser.add_argument("files", metavar="FILE", type=str, nargs="+", help="Files to be checked")
+    parser.add_argument(
+        "files", metavar="FILE", type=str, nargs="+", help="Files or directories to be checked"
+    )
     parser.add_argument(
         "--config", type=str, default="tox.ini", help="Path to config file (default: tox.ini)"
     )
     return parser.parse_args()
 
 
 def main() -> None:
     args = argument_parser()
     checker_files_content_uc(
         configure_path=args.config,
-        file_path_to_check=args.files,
+        paths_to_check=args.files,
     )
 
 
 if __name__ == "__main__":
     main()
```

