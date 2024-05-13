# Comparing `tmp/uwebserver-0.1.1.tar.gz` & `tmp/uwebserver-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uwebserver-0.1.1.tar", last modified: Mon May 13 16:43:14 2024, max compression
+gzip compressed data, was "uwebserver-0.1.2.tar", last modified: Mon May 13 16:50:13 2024, max compression
```

## Comparing `uwebserver-0.1.1.tar` & `uwebserver-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 16:43:14.697778 uwebserver-0.1.1/
--rw-rw-rw-   0        0        0     1062 2024-05-12 16:25:08.000000 uwebserver-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     2352 2024-05-13 16:43:14.696779 uwebserver-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      371 2024-05-13 16:19:18.000000 uwebserver-0.1.1/README.md
--rw-rw-rw-   0        0        0      967 2024-05-13 16:42:47.000000 uwebserver-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-13 16:43:14.697778 uwebserver-0.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-13 16:43:14.674798 uwebserver-0.1.1/uwebserver/
--rw-rw-rw-   0        0        0      111 2024-05-13 16:31:00.000000 uwebserver-0.1.1/uwebserver/__init__.py
--rw-rw-rw-   0        0        0        0 2024-05-13 16:31:10.000000 uwebserver-0.1.1/uwebserver/py.typed
--rw-rw-rw-   0        0        0    10280 2024-05-13 16:41:14.000000 uwebserver-0.1.1/uwebserver/webserver.py
-drwxrwxrwx   0        0        0        0 2024-05-13 16:43:14.694782 uwebserver-0.1.1/uwebserver.egg-info/
--rw-rw-rw-   0        0        0     2352 2024-05-13 16:43:14.000000 uwebserver-0.1.1/uwebserver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      268 2024-05-13 16:43:14.000000 uwebserver-0.1.1/uwebserver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 16:43:14.000000 uwebserver-0.1.1/uwebserver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2024-05-13 16:43:14.000000 uwebserver-0.1.1/uwebserver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-13 16:43:14.000000 uwebserver-0.1.1/uwebserver.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-13 16:50:13.040815 uwebserver-0.1.2/
+-rw-rw-rw-   0        0        0     1062 2024-05-12 16:25:08.000000 uwebserver-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     2352 2024-05-13 16:50:13.038815 uwebserver-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      371 2024-05-13 16:19:18.000000 uwebserver-0.1.2/README.md
+-rw-rw-rw-   0        0        0     1015 2024-05-13 16:50:01.000000 uwebserver-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-13 16:50:13.040815 uwebserver-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-13 16:50:13.016813 uwebserver-0.1.2/uwebserver/
+-rw-rw-rw-   0        0        0      111 2024-05-13 16:31:00.000000 uwebserver-0.1.2/uwebserver/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-05-13 16:31:10.000000 uwebserver-0.1.2/uwebserver/py.typed
+-rw-rw-rw-   0        0        0    10280 2024-05-13 16:41:14.000000 uwebserver-0.1.2/uwebserver/webserver.py
+drwxrwxrwx   0        0        0        0 2024-05-13 16:50:13.037814 uwebserver-0.1.2/uwebserver.egg-info/
+-rw-rw-rw-   0        0        0     2352 2024-05-13 16:50:12.000000 uwebserver-0.1.2/uwebserver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      268 2024-05-13 16:50:12.000000 uwebserver-0.1.2/uwebserver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 16:50:12.000000 uwebserver-0.1.2/uwebserver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2024-05-13 16:50:12.000000 uwebserver-0.1.2/uwebserver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-13 16:50:12.000000 uwebserver-0.1.2/uwebserver.egg-info/top_level.txt
```

### Comparing `uwebserver-0.1.1/LICENSE` & `uwebserver-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `uwebserver-0.1.1/PKG-INFO` & `uwebserver-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uwebserver
-Version: 0.1.1
+Version: 0.1.2
 Summary: Simple web server for micropython
 Author: 0x4aK
 License: MIT License
         
         Copyright (c) 2024 0x4aK
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `uwebserver-0.1.1/pyproject.toml` & `uwebserver-0.1.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "uwebserver"
-version = "0.1.1"
+version = "0.1.2"
 authors = [{ name = "0x4aK" }]
 description = "Simple web server for micropython"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Framework :: AsyncIO",
@@ -22,14 +22,15 @@
 
 [build-system]
 requires = ["setuptools >= 69.5.1", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 packages = ["uwebserver"]
+package-data = { "uwebserver" = ["py.typed"] }
 
 [tool.pyright]
 reportMissingImports = false
 
 [tool.ruff]
 line-length = 100
 lint = { select = ["E", "F", "I", "UP", "SIM"] }
```

### Comparing `uwebserver-0.1.1/uwebserver/webserver.py` & `uwebserver-0.1.2/uwebserver/webserver.py`

 * *Files identical despite different names*

### Comparing `uwebserver-0.1.1/uwebserver.egg-info/PKG-INFO` & `uwebserver-0.1.2/uwebserver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uwebserver
-Version: 0.1.1
+Version: 0.1.2
 Summary: Simple web server for micropython
 Author: 0x4aK
 License: MIT License
         
         Copyright (c) 2024 0x4aK
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

