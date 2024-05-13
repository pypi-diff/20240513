# Comparing `tmp/ziptimezone-1.0.4.tar.gz` & `tmp/ziptimezone-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ziptimezone-1.0.4.tar", max compression
+gzip compressed data, was "ziptimezone-1.1.0.tar", max compression
```

## Comparing `ziptimezone-1.0.4.tar` & `ziptimezone-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        2 2024-04-20 11:29:25.216037 ziptimezone-1.0.4/LICENSE
--rw-r--r--   0        0        0      846 2024-04-24 22:35:20.171518 ziptimezone-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     1818 2024-04-24 12:24:15.572521 ziptimezone-1.0.4/README.rst
--rw-r--r--   0        0        0     1334 2024-04-24 12:20:02.715620 ziptimezone-1.0.4/ziptimezone/__init__.py
--rw-r--r--   0        0        0     3598 2024-04-24 12:28:21.581939 ziptimezone-1.0.4/ziptimezone/batch_processor.py
--rw-r--r--   0        0        0     1801 2024-04-21 13:54:36.748759 ziptimezone-1.0.4/ziptimezone/core.py
--rw-r--r--   0        0        0     2780 2024-04-21 13:54:36.749759 ziptimezone-1.0.4/ziptimezone/data_manager.py
--rw-r--r--   0        0        0     1101 2024-04-21 13:54:36.749759 ziptimezone-1.0.4/ziptimezone/geocode.py
--rw-r--r--   0        0        0     1645 2024-04-21 13:54:36.749759 ziptimezone-1.0.4/ziptimezone/globals.py
--rw-r--r--   0        0        0     1874 2024-04-21 13:54:36.749759 ziptimezone-1.0.4/ziptimezone/mappings.py
--rw-r--r--   0        0        0     2490 1970-01-01 00:00:00.000000 ziptimezone-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0        2 2024-04-20 11:29:25.216037 ziptimezone-1.1.0/LICENSE
+-rw-r--r--   0        0        0      846 2024-05-13 09:50:20.104321 ziptimezone-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1818 2024-04-24 12:24:15.572521 ziptimezone-1.1.0/README.rst
+-rw-r--r--   0        0        0     1368 2024-05-13 10:03:51.537325 ziptimezone-1.1.0/ziptimezone/__init__.py
+-rw-r--r--   0        0        0     3598 2024-04-24 12:28:21.581939 ziptimezone-1.1.0/ziptimezone/batch_processor.py
+-rw-r--r--   0        0        0     3101 2024-05-13 09:55:00.835217 ziptimezone-1.1.0/ziptimezone/core.py
+-rw-r--r--   0        0        0     2780 2024-04-21 13:54:36.749759 ziptimezone-1.1.0/ziptimezone/data_manager.py
+-rw-r--r--   0        0        0     1101 2024-04-21 13:54:36.749759 ziptimezone-1.1.0/ziptimezone/geocode.py
+-rw-r--r--   0        0        0     1645 2024-04-21 13:54:36.749759 ziptimezone-1.1.0/ziptimezone/globals.py
+-rw-r--r--   0        0        0     1874 2024-04-21 13:54:36.749759 ziptimezone-1.1.0/ziptimezone/mappings.py
+-rw-r--r--   0        0        0     2490 1970-01-01 00:00:00.000000 ziptimezone-1.1.0/PKG-INFO
```

### Comparing `ziptimezone-1.0.4/pyproject.toml` & `ziptimezone-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ziptimezone"
-version = "1.0.4"
+version = "1.1.0"
 description = "A package to convert ZIP codes to time zones and get geographic coordinates."
 readme = "README.rst"
 authors = ["Manjunath Bettadapura <manjunathbettadapura412@gmail.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = ">=3.9, <4.0"
```

### Comparing `ziptimezone-1.0.4/README.rst` & `ziptimezone-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `ziptimezone-1.0.4/ziptimezone/__init__.py` & `ziptimezone-1.1.0/ziptimezone/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,13 +23,14 @@
 from .data_manager import refresh_data_if_needed
 from .batch_processor import get_timezone_for_many_zips, get_lat_long_for_many_zips
 
 ##from .mappings import map_timezone_to_region
 # from .geocode import get_lat_long_for_zip
 
 __all__ = [
+    "get_lat_long_for_zip",
     "get_timezone_by_zip",
+    "calculate_time_difference",
     "refresh_data_if_needed",
-    "get_lat_long_for_zip",
     "get_timezone_for_many_zips",
     "get_lat_long_for_many_zips",
 ]
```

### Comparing `ziptimezone-1.0.4/ziptimezone/batch_processor.py` & `ziptimezone-1.1.0/ziptimezone/batch_processor.py`

 * *Files identical despite different names*

### Comparing `ziptimezone-1.0.4/ziptimezone/data_manager.py` & `ziptimezone-1.1.0/ziptimezone/data_manager.py`

 * *Files identical despite different names*

### Comparing `ziptimezone-1.0.4/ziptimezone/geocode.py` & `ziptimezone-1.1.0/ziptimezone/geocode.py`

 * *Files identical despite different names*

### Comparing `ziptimezone-1.0.4/ziptimezone/globals.py` & `ziptimezone-1.1.0/ziptimezone/globals.py`

 * *Files identical despite different names*

### Comparing `ziptimezone-1.0.4/ziptimezone/mappings.py` & `ziptimezone-1.1.0/ziptimezone/mappings.py`

 * *Files identical despite different names*

### Comparing `ziptimezone-1.0.4/PKG-INFO` & `ziptimezone-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ziptimezone
-Version: 1.0.4
+Version: 1.1.0
 Summary: A package to convert ZIP codes to time zones and get geographic coordinates.
 License: MIT
 Author: Manjunath Bettadapura
 Author-email: manjunathbettadapura412@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

