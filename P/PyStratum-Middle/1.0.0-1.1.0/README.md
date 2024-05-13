# Comparing `tmp/PyStratum-Middle-1.0.0.tar.gz` & `tmp/pystratum_middle-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PyStratum-Middle-1.0.0.tar", last modified: Fri Oct 16 00:25:31 2020, max compression
+gzip compressed data, was "pystratum_middle-1.1.0.tar", last modified: Mon May 13 05:46:56 2024, max compression
```

## Comparing `PyStratum-Middle-1.0.0.tar` & `pystratum_middle-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,8 @@
-drwxrwxr-x   0 water     (1000) water     (1000)        0 2020-10-16 00:25:31.498803 PyStratum-Middle-1.0.0/
--rw-rw-r--   0 water     (1000) water     (1000)     4091 2020-10-16 00:25:31.498803 PyStratum-Middle-1.0.0/PKG-INFO
-drwxrwxr-x   0 water     (1000) water     (1000)        0 2020-10-16 00:25:31.497803 PyStratum-Middle-1.0.0/PyStratum_Middle.egg-info/
--rw-rw-r--   0 water     (1000) water     (1000)     4091 2020-10-16 00:25:31.000000 PyStratum-Middle-1.0.0/PyStratum_Middle.egg-info/PKG-INFO
--rw-rw-r--   0 water     (1000) water     (1000)      325 2020-10-16 00:25:31.000000 PyStratum-Middle-1.0.0/PyStratum_Middle.egg-info/SOURCES.txt
--rw-rw-r--   0 water     (1000) water     (1000)        1 2020-10-16 00:25:31.000000 PyStratum-Middle-1.0.0/PyStratum_Middle.egg-info/dependency_links.txt
--rw-rw-r--   0 water     (1000) water     (1000)       17 2020-10-16 00:25:31.000000 PyStratum-Middle-1.0.0/PyStratum_Middle.egg-info/top_level.txt
--rw-rw-r--   0 water     (1000) water     (1000)     3101 2020-10-15 23:19:05.000000 PyStratum-Middle-1.0.0/README.rst
-drwxrwxr-x   0 water     (1000) water     (1000)        0 2020-10-16 00:25:31.497803 PyStratum-Middle-1.0.0/pystratum_middle/
--rw-rw-r--   0 water     (1000) water     (1000)     1170 2020-10-15 23:23:34.000000 PyStratum-Middle-1.0.0/pystratum_middle/BulkHandler.py
--rw-rw-r--   0 water     (1000) water     (1000)        0 2020-10-15 21:32:51.000000 PyStratum-Middle-1.0.0/pystratum_middle/__init__.py
-drwxrwxr-x   0 water     (1000) water     (1000)        0 2020-10-16 00:25:31.497803 PyStratum-Middle-1.0.0/pystratum_middle/exception/
--rw-rw-r--   0 water     (1000) water     (1000)     2987 2020-10-15 23:23:34.000000 PyStratum-Middle-1.0.0/pystratum_middle/exception/ResultException.py
--rw-rw-r--   0 water     (1000) water     (1000)        0 2020-10-15 16:55:08.000000 PyStratum-Middle-1.0.0/pystratum_middle/exception/__init__.py
--rw-rw-r--   0 water     (1000) water     (1000)       38 2020-10-16 00:25:31.498803 PyStratum-Middle-1.0.0/setup.cfg
--rw-rw-r--   0 water     (1000) water     (1000)     1244 2020-10-16 00:25:17.000000 PyStratum-Middle-1.0.0/setup.py
+-rw-r--r--   0        0        0     1091 2020-10-15 23:05:00.000000 pystratum_middle-1.1.0/LICENSE.md
+-rw-r--r--   0        0        0     3101 2020-10-15 23:19:05.000000 pystratum_middle-1.1.0/README.rst
+-rw-r--r--   0        0        0     1062 2024-05-13 05:46:56.688999 pystratum_middle-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1170 2020-10-15 23:23:34.000000 pystratum_middle-1.1.0/pystratum_middle/BulkHandler.py
+-rw-r--r--   0        0        0        0 2020-10-15 21:32:51.000000 pystratum_middle-1.1.0/pystratum_middle/__init__.py
+-rw-r--r--   0        0        0     2987 2020-10-15 23:23:34.000000 pystratum_middle-1.1.0/pystratum_middle/exception/ResultException.py
+-rw-r--r--   0        0        0        0 2020-10-15 16:55:08.000000 pystratum_middle-1.1.0/pystratum_middle/exception/__init__.py
+-rw-r--r--   0        0        0     4030 1970-01-01 00:00:00.000000 pystratum_middle-1.1.0/PKG-INFO
```

### Comparing `PyStratum-Middle-1.0.0/README.rst` & `pystratum_middle-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `PyStratum-Middle-1.0.0/pystratum_middle/BulkHandler.py` & `pystratum_middle-1.1.0/pystratum_middle/BulkHandler.py`

 * *Files identical despite different names*

### Comparing `PyStratum-Middle-1.0.0/pystratum_middle/exception/ResultException.py` & `pystratum_middle-1.1.0/pystratum_middle/exception/ResultException.py`

 * *Files identical despite different names*

