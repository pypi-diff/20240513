# Comparing `tmp/shellcrafter-1.1.5.tar.gz` & `tmp/shellcrafter-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shellcrafter-1.1.5.tar", last modified: Mon May 13 16:59:09 2024, max compression
+gzip compressed data, was "shellcrafter-1.1.6.tar", last modified: Mon May 13 17:02:48 2024, max compression
```

## Comparing `shellcrafter-1.1.5.tar` & `shellcrafter-1.1.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:59:09.277474 shellcrafter-1.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-05-13 16:59:09.277474 shellcrafter-1.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5705 2024-05-13 16:58:56.000000 shellcrafter-1.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-13 16:58:56.000000 shellcrafter-1.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 16:59:09.277474 shellcrafter-1.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-13 16:58:56.000000 shellcrafter-1.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:59:09.273474 shellcrafter-1.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:59:09.277474 shellcrafter-1.1.5/src/shellcrafter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 16:58:56.000000 shellcrafter-1.1.5/src/shellcrafter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12470 2024-05-13 16:58:56.000000 shellcrafter-1.1.5/src/shellcrafter/cli.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13367 2024-05-13 16:58:56.000000 shellcrafter-1.1.5/src/shellcrafter/find_gadgets.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11174 2024-05-13 16:58:56.000000 shellcrafter-1.1.5/src/shellcrafter/keyst_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     8714 2024-05-13 16:58:56.000000 shellcrafter-1.1.5/src/shellcrafter/peutils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10063 2024-05-13 16:58:56.000000 shellcrafter-1.1.5/src/shellcrafter/shellcode_procedure_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:59:09.277474 shellcrafter-1.1.5/src/shellcrafter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-05-13 16:59:09.000000 shellcrafter-1.1.5/src/shellcrafter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-13 16:59:09.000000 shellcrafter-1.1.5/src/shellcrafter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 16:59:09.000000 shellcrafter-1.1.5/src/shellcrafter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-13 16:59:09.000000 shellcrafter-1.1.5/src/shellcrafter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-13 16:59:09.000000 shellcrafter-1.1.5/src/shellcrafter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-13 16:59:09.000000 shellcrafter-1.1.5/src/shellcrafter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:02:48.521830 shellcrafter-1.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-05-13 17:02:48.521830 shellcrafter-1.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5705 2024-05-13 17:02:37.000000 shellcrafter-1.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-13 17:02:37.000000 shellcrafter-1.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 17:02:48.521830 shellcrafter-1.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-13 17:02:37.000000 shellcrafter-1.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:02:48.517830 shellcrafter-1.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:02:48.517830 shellcrafter-1.1.6/src/shellcrafter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 17:02:37.000000 shellcrafter-1.1.6/src/shellcrafter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12498 2024-05-13 17:02:37.000000 shellcrafter-1.1.6/src/shellcrafter/cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13367 2024-05-13 17:02:37.000000 shellcrafter-1.1.6/src/shellcrafter/find_gadgets.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11174 2024-05-13 17:02:37.000000 shellcrafter-1.1.6/src/shellcrafter/keyst_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8714 2024-05-13 17:02:37.000000 shellcrafter-1.1.6/src/shellcrafter/peutils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10063 2024-05-13 17:02:37.000000 shellcrafter-1.1.6/src/shellcrafter/shellcode_procedure_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:02:48.521830 shellcrafter-1.1.6/src/shellcrafter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-05-13 17:02:48.000000 shellcrafter-1.1.6/src/shellcrafter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-13 17:02:48.000000 shellcrafter-1.1.6/src/shellcrafter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 17:02:48.000000 shellcrafter-1.1.6/src/shellcrafter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-13 17:02:48.000000 shellcrafter-1.1.6/src/shellcrafter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-13 17:02:48.000000 shellcrafter-1.1.6/src/shellcrafter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-13 17:02:48.000000 shellcrafter-1.1.6/src/shellcrafter.egg-info/top_level.txt
```

### Comparing `shellcrafter-1.1.5/PKG-INFO` & `shellcrafter-1.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shellcrafter
-Version: 1.1.5
+Version: 1.1.6
 Summary: A package containing scripts for developing and generating shellcode
 Home-page: https://github.com/totekuh/shellcrafter
 Author: totekuh
 Author-email: totekuh@protonmail.com
 Project-URL: Bug Reports, https://github.com/totekuh/shellcrafter/issues
 Project-URL: Source, https://github.com/totekuh/shellcrafter
 Description-Content-Type: text/markdown
```

### Comparing `shellcrafter-1.1.5/README.md` & `shellcrafter-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `shellcrafter-1.1.5/setup.py` & `shellcrafter-1.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-version = "1.1.5"
+version = "1.1.6"
 
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 REPO_URL = 'https://github.com/totekuh/shellcrafter'
```

### Comparing `shellcrafter-1.1.5/src/shellcrafter/cli.py` & `shellcrafter-1.1.6/src/shellcrafter/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from shellcode_procedure_generator import str_to_hex_little_endian_push, \
     data_types, \
     print_hash_algorithm, \
     compute_hash, \
     generate_load_library, \
     write_to_memory
 from find_gadgets import do_find_gadgets
+from typing import Optional
 from peutils import *
 
 app = Typer(help="Shellcrafter: A tool for shellcode development and gadget finding.", add_completion=False)
 
 shellcode_app = Typer(add_completion=False)
 app.add_typer(shellcode_app, name="shellcode", help="Shellcode-related operations.")
```

### Comparing `shellcrafter-1.1.5/src/shellcrafter/find_gadgets.py` & `shellcrafter-1.1.6/src/shellcrafter/find_gadgets.py`

 * *Files identical despite different names*

### Comparing `shellcrafter-1.1.5/src/shellcrafter/keyst_api.py` & `shellcrafter-1.1.6/src/shellcrafter/keyst_api.py`

 * *Files identical despite different names*

### Comparing `shellcrafter-1.1.5/src/shellcrafter/peutils.py` & `shellcrafter-1.1.6/src/shellcrafter/peutils.py`

 * *Files identical despite different names*

### Comparing `shellcrafter-1.1.5/src/shellcrafter/shellcode_procedure_generator.py` & `shellcrafter-1.1.6/src/shellcrafter/shellcode_procedure_generator.py`

 * *Files identical despite different names*

### Comparing `shellcrafter-1.1.5/src/shellcrafter.egg-info/PKG-INFO` & `shellcrafter-1.1.6/src/shellcrafter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shellcrafter
-Version: 1.1.5
+Version: 1.1.6
 Summary: A package containing scripts for developing and generating shellcode
 Home-page: https://github.com/totekuh/shellcrafter
 Author: totekuh
 Author-email: totekuh@protonmail.com
 Project-URL: Bug Reports, https://github.com/totekuh/shellcrafter/issues
 Project-URL: Source, https://github.com/totekuh/shellcrafter
 Description-Content-Type: text/markdown
```

