# Comparing `tmp/gridappsd_python-2024.4.0a0.tar.gz` & `tmp/gridappsd_python-2024.4.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gridappsd_python-2024.4.0a0.tar", max compression
+gzip compressed data, was "gridappsd_python-2024.4.1a0.tar", max compression
```

## Comparing `gridappsd_python-2024.4.0a0.tar` & `gridappsd_python-2024.4.1a0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    10489 2024-05-02 16:40:43.790433 gridappsd_python-2024.4.0a0/README.md
--rw-r--r--   0        0        0     3794 2024-05-02 16:40:43.790433 gridappsd_python-2024.4.0a0/gridappsd/__init__.py
--rw-r--r--   0        0        0     4685 2024-05-02 16:40:43.790433 gridappsd_python-2024.4.0a0/gridappsd/__main__.py
--rw-r--r--   0        0        0     7012 2024-05-02 16:40:43.790433 gridappsd_python-2024.4.0a0/gridappsd/app_registration.py
--rw-r--r--   0        0        0     4687 2024-05-02 16:40:43.790433 gridappsd_python-2024.4.0a0/gridappsd/difference_builder.py
--rw-r--r--   0        0        0    30366 2024-05-02 16:40:43.790433 gridappsd_python-2024.4.0a0/gridappsd/docker_handler.py
--rw-r--r--   0        0        0    17354 2024-05-02 16:40:43.790433 gridappsd_python-2024.4.0a0/gridappsd/goss.py
--rw-r--r--   0        0        0    12737 2024-05-02 16:40:43.790433 gridappsd_python-2024.4.0a0/gridappsd/gridappsd.py
--rw-r--r--   0        0        0     3275 2024-05-02 16:40:43.790433 gridappsd_python-2024.4.0a0/gridappsd/houses.py
--rw-r--r--   0        0        0     3388 2024-05-02 16:40:43.790433 gridappsd_python-2024.4.0a0/gridappsd/json_extension.py
--rw-r--r--   0        0        0     2703 2024-05-02 16:40:43.794433 gridappsd_python-2024.4.0a0/gridappsd/loghandler.py
--rw-r--r--   0        0        0     2570 2024-05-02 16:40:43.794433 gridappsd_python-2024.4.0a0/gridappsd/register_app.py
--rw-r--r--   0        0        0    12234 2024-05-02 16:40:43.794433 gridappsd_python-2024.4.0a0/gridappsd/simulation.py
--rw-r--r--   0        0        0     3201 2024-05-02 16:40:43.794433 gridappsd_python-2024.4.0a0/gridappsd/timeseries.py
--rw-r--r--   0        0        0    12128 2024-05-02 16:40:43.794433 gridappsd_python-2024.4.0a0/gridappsd/topics.py
--rw-r--r--   0        0        0     3167 2024-05-02 16:40:43.794433 gridappsd_python-2024.4.0a0/gridappsd/utils.py
--rw-r--r--   0        0        0     1383 2024-05-02 16:41:41.478312 gridappsd_python-2024.4.0a0/pyproject.toml
--rw-r--r--   0        0        0    11473 1970-01-01 00:00:00.000000 gridappsd_python-2024.4.0a0/PKG-INFO
+-rw-r--r--   0        0        0    10489 2024-05-13 20:14:27.056062 gridappsd_python-2024.4.1a0/README.md
+-rw-r--r--   0        0        0     3794 2024-05-13 20:14:27.056062 gridappsd_python-2024.4.1a0/gridappsd/__init__.py
+-rw-r--r--   0        0        0     4685 2024-05-13 20:14:27.056062 gridappsd_python-2024.4.1a0/gridappsd/__main__.py
+-rw-r--r--   0        0        0     7012 2024-05-13 20:14:27.056062 gridappsd_python-2024.4.1a0/gridappsd/app_registration.py
+-rw-r--r--   0        0        0     4687 2024-05-13 20:14:27.056062 gridappsd_python-2024.4.1a0/gridappsd/difference_builder.py
+-rw-r--r--   0        0        0    30366 2024-05-13 20:14:27.056062 gridappsd_python-2024.4.1a0/gridappsd/docker_handler.py
+-rw-r--r--   0        0        0    17354 2024-05-13 20:14:27.056062 gridappsd_python-2024.4.1a0/gridappsd/goss.py
+-rw-r--r--   0        0        0    12737 2024-05-13 20:14:27.056062 gridappsd_python-2024.4.1a0/gridappsd/gridappsd.py
+-rw-r--r--   0        0        0     3275 2024-05-13 20:14:27.056062 gridappsd_python-2024.4.1a0/gridappsd/houses.py
+-rw-r--r--   0        0        0     3388 2024-05-13 20:14:27.056062 gridappsd_python-2024.4.1a0/gridappsd/json_extension.py
+-rw-r--r--   0        0        0     2703 2024-05-13 20:14:27.056062 gridappsd_python-2024.4.1a0/gridappsd/loghandler.py
+-rw-r--r--   0        0        0     2570 2024-05-13 20:14:27.056062 gridappsd_python-2024.4.1a0/gridappsd/register_app.py
+-rw-r--r--   0        0        0    12234 2024-05-13 20:14:27.056062 gridappsd_python-2024.4.1a0/gridappsd/simulation.py
+-rw-r--r--   0        0        0     3201 2024-05-13 20:14:27.056062 gridappsd_python-2024.4.1a0/gridappsd/timeseries.py
+-rw-r--r--   0        0        0    12128 2024-05-13 20:14:27.056062 gridappsd_python-2024.4.1a0/gridappsd/topics.py
+-rw-r--r--   0        0        0     3167 2024-05-13 20:14:27.056062 gridappsd_python-2024.4.1a0/gridappsd/utils.py
+-rw-r--r--   0        0        0     1383 2024-05-13 20:15:47.364606 gridappsd_python-2024.4.1a0/pyproject.toml
+-rw-r--r--   0        0        0    11473 1970-01-01 00:00:00.000000 gridappsd_python-2024.4.1a0/PKG-INFO
```

### Comparing `gridappsd_python-2024.4.0a0/README.md` & `gridappsd_python-2024.4.1a0/README.md`

 * *Files identical despite different names*

### Comparing `gridappsd_python-2024.4.0a0/gridappsd/__init__.py` & `gridappsd_python-2024.4.1a0/gridappsd/__init__.py`

 * *Files identical despite different names*

### Comparing `gridappsd_python-2024.4.0a0/gridappsd/__main__.py` & `gridappsd_python-2024.4.1a0/gridappsd/__main__.py`

 * *Files identical despite different names*

### Comparing `gridappsd_python-2024.4.0a0/gridappsd/app_registration.py` & `gridappsd_python-2024.4.1a0/gridappsd/app_registration.py`

 * *Files identical despite different names*

### Comparing `gridappsd_python-2024.4.0a0/gridappsd/difference_builder.py` & `gridappsd_python-2024.4.1a0/gridappsd/difference_builder.py`

 * *Files identical despite different names*

### Comparing `gridappsd_python-2024.4.0a0/gridappsd/docker_handler.py` & `gridappsd_python-2024.4.1a0/gridappsd/docker_handler.py`

 * *Files identical despite different names*

### Comparing `gridappsd_python-2024.4.0a0/gridappsd/goss.py` & `gridappsd_python-2024.4.1a0/gridappsd/goss.py`

 * *Files identical despite different names*

### Comparing `gridappsd_python-2024.4.0a0/gridappsd/gridappsd.py` & `gridappsd_python-2024.4.1a0/gridappsd/gridappsd.py`

 * *Files identical despite different names*

### Comparing `gridappsd_python-2024.4.0a0/gridappsd/houses.py` & `gridappsd_python-2024.4.1a0/gridappsd/houses.py`

 * *Files identical despite different names*

### Comparing `gridappsd_python-2024.4.0a0/gridappsd/json_extension.py` & `gridappsd_python-2024.4.1a0/gridappsd/json_extension.py`

 * *Files identical despite different names*

### Comparing `gridappsd_python-2024.4.0a0/gridappsd/loghandler.py` & `gridappsd_python-2024.4.1a0/gridappsd/loghandler.py`

 * *Files identical despite different names*

### Comparing `gridappsd_python-2024.4.0a0/gridappsd/register_app.py` & `gridappsd_python-2024.4.1a0/gridappsd/register_app.py`

 * *Files identical despite different names*

### Comparing `gridappsd_python-2024.4.0a0/gridappsd/simulation.py` & `gridappsd_python-2024.4.1a0/gridappsd/simulation.py`

 * *Files identical despite different names*

### Comparing `gridappsd_python-2024.4.0a0/gridappsd/timeseries.py` & `gridappsd_python-2024.4.1a0/gridappsd/timeseries.py`

 * *Files identical despite different names*

### Comparing `gridappsd_python-2024.4.0a0/gridappsd/topics.py` & `gridappsd_python-2024.4.1a0/gridappsd/topics.py`

 * *Files identical despite different names*

### Comparing `gridappsd_python-2024.4.0a0/gridappsd/utils.py` & `gridappsd_python-2024.4.1a0/gridappsd/utils.py`

 * *Files identical despite different names*

### Comparing `gridappsd_python-2024.4.0a0/pyproject.toml` & `gridappsd_python-2024.4.1a0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gridappsd-python"
-version = "2024.4.0a0"
+version = "2024.4.1a0"
 description = "A GridAPPS-D Python Adapter"
 authors = [
     "C. Allwardt <3979063+craig8@users.noreply.github.com>",
     "P. Sharma <poorva.sharma@pnnl.gov",
     "A. Fisher <andrew.fisher@pnnl.gov"
 ]
 license = "BSD-3-Clause"
```

### Comparing `gridappsd_python-2024.4.0a0/PKG-INFO` & `gridappsd_python-2024.4.1a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gridappsd-python
-Version: 2024.4.0a0
+Version: 2024.4.1a0
 Summary: A GridAPPS-D Python Adapter
 Home-page: https://gridappsd.readthedocs.io
 License: BSD-3-Clause
 Keywords: gridappsd,grid,activmq,powergrid,simulation,library
 Author: C. Allwardt
 Author-email: 3979063+craig8@users.noreply.github.com
 Requires-Python: >=3.7.9,<4.0
```

