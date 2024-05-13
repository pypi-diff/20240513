# Comparing `tmp/lptlib-0.0.1a1.tar.gz` & `tmp/lptlib-0.0.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lptlib-0.0.1a1.tar", last modified: Mon May 13 17:34:56 2024, max compression
+gzip compressed data, was "lptlib-0.0.1a2.tar", last modified: Mon May 13 17:40:52 2024, max compression
```

## Comparing `lptlib-0.0.1a1.tar` & `lptlib-0.0.1a2.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 17:34:56.673932 lptlib-0.0.1a1/
--rwx------   0 kal        (501) staff       (20)     1093 2024-05-10 20:01:36.000000 lptlib-0.0.1a1/LICENSE
--rw-r--r--   0 kal        (501) staff       (20)     1545 2024-05-13 17:34:56.673202 lptlib-0.0.1a1/PKG-INFO
--rw-r--r--   0 kal        (501) staff       (20)      579 2024-05-13 17:06:24.000000 lptlib-0.0.1a1/README.md
--rw-r--r--   0 kal        (501) staff       (20)     1085 2024-05-13 17:34:50.000000 lptlib-0.0.1a1/pyproject.toml
--rw-r--r--   0 kal        (501) staff       (20)       38 2024-05-13 17:34:56.674099 lptlib-0.0.1a1/setup.cfg
-drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 17:34:56.641452 lptlib-0.0.1a1/src/
--rw-r--r--   0 kal        (501) staff       (20)      127 2024-05-13 16:33:20.000000 lptlib-0.0.1a1/src/__init__.py
-drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 17:34:56.646139 lptlib-0.0.1a1/src/function/
--rw-r--r--   0 kal        (501) staff       (20)      109 2024-01-23 01:40:32.000000 lptlib-0.0.1a1/src/function/__init__.py
--rwx------   0 kal        (501) staff       (20)    12638 2024-05-13 17:24:07.000000 lptlib-0.0.1a1/src/function/plots.py
--rw-r--r--   0 kal        (501) staff       (20)     2034 2024-01-23 01:40:32.000000 lptlib-0.0.1a1/src/function/timer.py
--rw-r--r--   0 kal        (501) staff       (20)    11932 2024-05-13 17:24:06.000000 lptlib-0.0.1a1/src/function/variables.py
-drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 17:34:56.648888 lptlib-0.0.1a1/src/io/
--rw-r--r--   0 kal        (501) staff       (20)       91 2024-01-23 01:40:32.000000 lptlib-0.0.1a1/src/io/__init__.py
--rw-r--r--   0 kal        (501) staff       (20)    14881 2024-05-13 17:24:06.000000 lptlib-0.0.1a1/src/io/dataio.py
--rw-r--r--   0 kal        (501) staff       (20)    24440 2024-04-22 21:46:04.000000 lptlib-0.0.1a1/src/io/plot3dio.py
-drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 17:34:56.672292 lptlib-0.0.1a1/src/lptlib.egg-info/
--rw-r--r--   0 kal        (501) staff       (20)     1545 2024-05-13 17:34:56.000000 lptlib-0.0.1a1/src/lptlib.egg-info/PKG-INFO
--rw-r--r--   0 kal        (501) staff       (20)      898 2024-05-13 17:34:56.000000 lptlib-0.0.1a1/src/lptlib.egg-info/SOURCES.txt
--rw-r--r--   0 kal        (501) staff       (20)        1 2024-05-13 17:34:56.000000 lptlib-0.0.1a1/src/lptlib.egg-info/dependency_links.txt
--rw-r--r--   0 kal        (501) staff       (20)       43 2024-05-13 17:34:56.000000 lptlib-0.0.1a1/src/lptlib.egg-info/requires.txt
--rw-r--r--   0 kal        (501) staff       (20)       44 2024-05-13 17:34:56.000000 lptlib-0.0.1a1/src/lptlib.egg-info/top_level.txt
-drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 17:34:56.657368 lptlib-0.0.1a1/src/streamlines/
--rw-r--r--   0 kal        (501) staff       (20)      257 2024-01-23 01:40:32.000000 lptlib-0.0.1a1/src/streamlines/__init__.py
--rw-r--r--   0 kal        (501) staff       (20)    34475 2024-05-13 17:24:06.000000 lptlib-0.0.1a1/src/streamlines/integration.py
--rw-r--r--   0 kal        (501) staff       (20)    47345 2024-05-13 17:24:06.000000 lptlib-0.0.1a1/src/streamlines/interpolation.py
--rwxr-xr-x   0 kal        (501) staff       (20)    15615 2024-05-13 17:24:06.000000 lptlib-0.0.1a1/src/streamlines/search.py
--rw-r--r--   0 kal        (501) staff       (20)     7539 2024-05-13 17:24:06.000000 lptlib-0.0.1a1/src/streamlines/stochastic_model.py
--rw-r--r--   0 kal        (501) staff       (20)    39741 2024-05-13 17:24:07.000000 lptlib-0.0.1a1/src/streamlines/streamlines.py
-drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 17:34:56.660008 lptlib-0.0.1a1/src/test_cases/
--rwx------   0 kal        (501) staff       (20)       89 2024-01-23 01:40:32.000000 lptlib-0.0.1a1/src/test_cases/__init__.py
--rwx------   0 kal        (501) staff       (20)    10011 2024-05-13 17:24:06.000000 lptlib-0.0.1a1/src/test_cases/oblique_shock_data.py
-drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 17:34:56.671100 lptlib-0.0.1a1/test/
--rw-r--r--   0 kal        (501) staff       (20)     1019 2024-05-13 17:21:40.000000 lptlib-0.0.1a1/test/test_dataio.py
--rwx------   0 kal        (501) staff       (20)      576 2024-05-13 17:21:48.000000 lptlib-0.0.1a1/test/test_import.py
--rwx------   0 kal        (501) staff       (20)     2446 2024-05-13 17:24:07.000000 lptlib-0.0.1a1/test/test_integration.py
--rw-r--r--   0 kal        (501) staff       (20)     2103 2024-05-13 17:24:06.000000 lptlib-0.0.1a1/test/test_interpolation.py
--rwx------   0 kal        (501) staff       (20)     1238 2024-05-13 17:24:06.000000 lptlib-0.0.1a1/test/test_oblique_shock_data.py
--rw-r--r--   0 kal        (501) staff       (20)     2059 2023-08-17 08:22:42.000000 lptlib-0.0.1a1/test/test_plot.py
--rw-r--r--   0 kal        (501) staff       (20)     7327 2024-05-13 17:24:06.000000 lptlib-0.0.1a1/test/test_plot3dio.py
--rwx------   0 kal        (501) staff       (20)     2637 2024-05-13 17:24:07.000000 lptlib-0.0.1a1/test/test_plots.py
--rw-r--r--   0 kal        (501) staff       (20)     3306 2024-05-13 17:24:06.000000 lptlib-0.0.1a1/test/test_search.py
--rw-r--r--   0 kal        (501) staff       (20)     1955 2024-05-13 17:24:06.000000 lptlib-0.0.1a1/test/test_stochastic_model.py
--rw-r--r--   0 kal        (501) staff       (20)     1440 2024-05-13 17:24:06.000000 lptlib-0.0.1a1/test/test_terminal_run.py
--rwx------   0 kal        (501) staff       (20)     2829 2024-05-13 17:24:06.000000 lptlib-0.0.1a1/test/test_variables.py
+drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 17:40:52.476982 lptlib-0.0.1a2/
+-rwx------   0 kal        (501) staff       (20)     1093 2024-05-10 20:01:36.000000 lptlib-0.0.1a2/LICENSE
+-rw-r--r--   0 kal        (501) staff       (20)     1545 2024-05-13 17:40:52.476262 lptlib-0.0.1a2/PKG-INFO
+-rw-r--r--   0 kal        (501) staff       (20)      579 2024-05-13 17:06:24.000000 lptlib-0.0.1a2/README.md
+-rw-r--r--   0 kal        (501) staff       (20)     1085 2024-05-13 17:40:45.000000 lptlib-0.0.1a2/pyproject.toml
+-rw-r--r--   0 kal        (501) staff       (20)       38 2024-05-13 17:40:52.477150 lptlib-0.0.1a2/setup.cfg
+drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 17:40:52.447578 lptlib-0.0.1a2/src/
+drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 17:40:52.450987 lptlib-0.0.1a2/src/lptlib/
+-rw-r--r--   0 kal        (501) staff       (20)      122 2024-05-13 17:40:07.000000 lptlib-0.0.1a2/src/lptlib/__init__.py
+drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 17:40:52.455987 lptlib-0.0.1a2/src/lptlib/function/
+-rw-r--r--   0 kal        (501) staff       (20)      109 2024-01-23 01:40:32.000000 lptlib-0.0.1a2/src/lptlib/function/__init__.py
+-rwx------   0 kal        (501) staff       (20)    12638 2024-05-13 17:24:07.000000 lptlib-0.0.1a2/src/lptlib/function/plots.py
+-rw-r--r--   0 kal        (501) staff       (20)     2034 2024-01-23 01:40:32.000000 lptlib-0.0.1a2/src/lptlib/function/timer.py
+-rw-r--r--   0 kal        (501) staff       (20)    11932 2024-05-13 17:24:06.000000 lptlib-0.0.1a2/src/lptlib/function/variables.py
+drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 17:40:52.458242 lptlib-0.0.1a2/src/lptlib/io/
+-rw-r--r--   0 kal        (501) staff       (20)       91 2024-01-23 01:40:32.000000 lptlib-0.0.1a2/src/lptlib/io/__init__.py
+-rw-r--r--   0 kal        (501) staff       (20)    14881 2024-05-13 17:24:06.000000 lptlib-0.0.1a2/src/lptlib/io/dataio.py
+-rw-r--r--   0 kal        (501) staff       (20)    24440 2024-04-22 21:46:04.000000 lptlib-0.0.1a2/src/lptlib/io/plot3dio.py
+drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 17:40:52.464994 lptlib-0.0.1a2/src/lptlib/streamlines/
+-rw-r--r--   0 kal        (501) staff       (20)      257 2024-01-23 01:40:32.000000 lptlib-0.0.1a2/src/lptlib/streamlines/__init__.py
+-rw-r--r--   0 kal        (501) staff       (20)    34475 2024-05-13 17:24:06.000000 lptlib-0.0.1a2/src/lptlib/streamlines/integration.py
+-rw-r--r--   0 kal        (501) staff       (20)    47345 2024-05-13 17:24:06.000000 lptlib-0.0.1a2/src/lptlib/streamlines/interpolation.py
+-rwxr-xr-x   0 kal        (501) staff       (20)    15615 2024-05-13 17:24:06.000000 lptlib-0.0.1a2/src/lptlib/streamlines/search.py
+-rw-r--r--   0 kal        (501) staff       (20)     7539 2024-05-13 17:24:06.000000 lptlib-0.0.1a2/src/lptlib/streamlines/stochastic_model.py
+-rw-r--r--   0 kal        (501) staff       (20)    39741 2024-05-13 17:24:07.000000 lptlib-0.0.1a2/src/lptlib/streamlines/streamlines.py
+drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 17:40:52.467522 lptlib-0.0.1a2/src/lptlib/test_cases/
+-rwx------   0 kal        (501) staff       (20)       89 2024-01-23 01:40:32.000000 lptlib-0.0.1a2/src/lptlib/test_cases/__init__.py
+-rwx------   0 kal        (501) staff       (20)    10011 2024-05-13 17:24:06.000000 lptlib-0.0.1a2/src/lptlib/test_cases/oblique_shock_data.py
+drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 17:40:52.475381 lptlib-0.0.1a2/src/lptlib.egg-info/
+-rw-r--r--   0 kal        (501) staff       (20)     1545 2024-05-13 17:40:52.000000 lptlib-0.0.1a2/src/lptlib.egg-info/PKG-INFO
+-rw-r--r--   0 kal        (501) staff       (20)     1010 2024-05-13 17:40:52.000000 lptlib-0.0.1a2/src/lptlib.egg-info/SOURCES.txt
+-rw-r--r--   0 kal        (501) staff       (20)        1 2024-05-13 17:40:52.000000 lptlib-0.0.1a2/src/lptlib.egg-info/dependency_links.txt
+-rw-r--r--   0 kal        (501) staff       (20)       43 2024-05-13 17:40:52.000000 lptlib-0.0.1a2/src/lptlib.egg-info/requires.txt
+-rw-r--r--   0 kal        (501) staff       (20)        7 2024-05-13 17:40:52.000000 lptlib-0.0.1a2/src/lptlib.egg-info/top_level.txt
+drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 17:40:52.474625 lptlib-0.0.1a2/test/
+-rw-r--r--   0 kal        (501) staff       (20)      997 2024-05-13 17:40:07.000000 lptlib-0.0.1a2/test/test_dataio.py
+-rwx------   0 kal        (501) staff       (20)      446 2024-05-13 17:40:07.000000 lptlib-0.0.1a2/test/test_import.py
+-rwx------   0 kal        (501) staff       (20)     2350 2024-05-13 17:40:07.000000 lptlib-0.0.1a2/test/test_integration.py
+-rw-r--r--   0 kal        (501) staff       (20)     2016 2024-05-13 17:40:07.000000 lptlib-0.0.1a2/test/test_interpolation.py
+-rwx------   0 kal        (501) staff       (20)     1148 2024-05-13 17:40:08.000000 lptlib-0.0.1a2/test/test_oblique_shock_data.py
+-rw-r--r--   0 kal        (501) staff       (20)     2059 2023-08-17 08:22:42.000000 lptlib-0.0.1a2/test/test_plot.py
+-rw-r--r--   0 kal        (501) staff       (20)     7324 2024-05-13 17:40:08.000000 lptlib-0.0.1a2/test/test_plot3dio.py
+-rwx------   0 kal        (501) staff       (20)     2607 2024-05-13 17:40:08.000000 lptlib-0.0.1a2/test/test_plots.py
+-rw-r--r--   0 kal        (501) staff       (20)     3260 2024-05-13 17:40:07.000000 lptlib-0.0.1a2/test/test_search.py
+-rw-r--r--   0 kal        (501) staff       (20)     1914 2024-05-13 17:40:07.000000 lptlib-0.0.1a2/test/test_stochastic_model.py
+-rw-r--r--   0 kal        (501) staff       (20)     1399 2024-05-13 17:40:07.000000 lptlib-0.0.1a2/test/test_terminal_run.py
+-rwx------   0 kal        (501) staff       (20)     2696 2024-05-13 17:40:07.000000 lptlib-0.0.1a2/test/test_variables.py
```

### Comparing `lptlib-0.0.1a1/LICENSE` & `lptlib-0.0.1a2/LICENSE`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a1/PKG-INFO` & `lptlib-0.0.1a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lptlib
-Version: 0.0.1a1
+Version: 0.0.1a2
 Summary: One-way coupled Lagrangian Particle Tracking algorithms.
 Author: Dilip Kalagotla
 Author-email: dilipkalagotla@gmail.com
 Project-URL: homepage, https://github.com/kalagotla/project-arrakis
 Project-URL: issues, https://github.com/kalagotla/project-arrakis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `lptlib-0.0.1a1/README.md` & `lptlib-0.0.1a2/README.md`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a1/pyproject.toml` & `lptlib-0.0.1a2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lptlib"
-version = "0.0.1a1"
+version = "0.0.1a2"
 authors = [
     {name="Dilip Kalagotla"},
     {email="dilipkalagotla@gmail.com"},
     ]
 description = "One-way coupled Lagrangian Particle Tracking algorithms."
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `lptlib-0.0.1a1/src/function/plots.py` & `lptlib-0.0.1a2/src/lptlib/function/plots.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a1/src/function/timer.py` & `lptlib-0.0.1a2/src/lptlib/function/timer.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a1/src/function/variables.py` & `lptlib-0.0.1a2/src/lptlib/function/variables.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a1/src/io/dataio.py` & `lptlib-0.0.1a2/src/lptlib/io/dataio.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a1/src/io/plot3dio.py` & `lptlib-0.0.1a2/src/lptlib/io/plot3dio.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a1/src/lptlib.egg-info/PKG-INFO` & `lptlib-0.0.1a2/src/lptlib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lptlib
-Version: 0.0.1a1
+Version: 0.0.1a2
 Summary: One-way coupled Lagrangian Particle Tracking algorithms.
 Author: Dilip Kalagotla
 Author-email: dilipkalagotla@gmail.com
 Project-URL: homepage, https://github.com/kalagotla/project-arrakis
 Project-URL: issues, https://github.com/kalagotla/project-arrakis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `lptlib-0.0.1a1/src/lptlib.egg-info/SOURCES.txt` & `lptlib-0.0.1a2/src/lptlib.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 LICENSE
 README.md
 pyproject.toml
-src/__init__.py
-src/function/__init__.py
-src/function/plots.py
-src/function/timer.py
-src/function/variables.py
-src/io/__init__.py
-src/io/dataio.py
-src/io/plot3dio.py
+src/lptlib/__init__.py
 src/lptlib.egg-info/PKG-INFO
 src/lptlib.egg-info/SOURCES.txt
 src/lptlib.egg-info/dependency_links.txt
 src/lptlib.egg-info/requires.txt
 src/lptlib.egg-info/top_level.txt
-src/streamlines/__init__.py
-src/streamlines/integration.py
-src/streamlines/interpolation.py
-src/streamlines/search.py
-src/streamlines/stochastic_model.py
-src/streamlines/streamlines.py
-src/test_cases/__init__.py
-src/test_cases/oblique_shock_data.py
+src/lptlib/function/__init__.py
+src/lptlib/function/plots.py
+src/lptlib/function/timer.py
+src/lptlib/function/variables.py
+src/lptlib/io/__init__.py
+src/lptlib/io/dataio.py
+src/lptlib/io/plot3dio.py
+src/lptlib/streamlines/__init__.py
+src/lptlib/streamlines/integration.py
+src/lptlib/streamlines/interpolation.py
+src/lptlib/streamlines/search.py
+src/lptlib/streamlines/stochastic_model.py
+src/lptlib/streamlines/streamlines.py
+src/lptlib/test_cases/__init__.py
+src/lptlib/test_cases/oblique_shock_data.py
 test/test_dataio.py
 test/test_import.py
 test/test_integration.py
 test/test_interpolation.py
 test/test_oblique_shock_data.py
 test/test_plot.py
 test/test_plot3dio.py
```

### Comparing `lptlib-0.0.1a1/src/streamlines/integration.py` & `lptlib-0.0.1a2/src/lptlib/streamlines/integration.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a1/src/streamlines/interpolation.py` & `lptlib-0.0.1a2/src/lptlib/streamlines/interpolation.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a1/src/streamlines/search.py` & `lptlib-0.0.1a2/src/lptlib/streamlines/search.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a1/src/streamlines/stochastic_model.py` & `lptlib-0.0.1a2/src/lptlib/streamlines/stochastic_model.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a1/src/streamlines/streamlines.py` & `lptlib-0.0.1a2/src/lptlib/streamlines/streamlines.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a1/src/test_cases/oblique_shock_data.py` & `lptlib-0.0.1a2/src/lptlib/test_cases/oblique_shock_data.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a1/test/test_dataio.py` & `lptlib-0.0.1a2/test/test_dataio.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import unittest
 
 
 class TestDataIO(unittest.TestCase):
     def test_dataio(self):
-        from src.io.dataio import DataIO
-        from src.io.plot3dio import GridIO, FlowIO
+        from src import DataIO
+        from src import GridIO, FlowIO
         # grid object
         grid = GridIO('../data/shocks/shock_test.sb.sp.x')
         grid.read_grid()
         grid.compute_metrics()
 
         # flow object
         flow = FlowIO('../data/shocks/shock_test.sb.sp.q')
```

### Comparing `lptlib-0.0.1a1/test/test_integration.py` & `lptlib-0.0.1a2/test/test_integration.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import unittest
 from parameterized import parameterized
-from src.function.timer import Timer
+from src import Timer
 
 
 class TestIntegration(unittest.TestCase):
     @parameterized.expand([
         ('sb_sp_p_space', '../data/plate_data/plate.sp.x', '../data/plate_data/sol-0000010.q',
          'f4', [8.5, 0.5, 0.01], 'block_distance', 'p-space', 'p-space'),
         ('sb_sp_c_space', '../data/plate_data/plate.sp.x', '../data/plate_data/sol-0000010.q',
@@ -20,18 +20,18 @@
 
     ])
     @Timer()
     def test_integration(self, name, gridfile='../data/plate_data/plate.sp.x',
                          flowfile='../data/plate_data/sol-0000010.q', data_type='f4', point=None,
                          search_method='block_distance', interpolation_method='p-space', integration_method='RK4'):
 
-        from src.io.plot3dio import GridIO, FlowIO
-        from src.streamlines.search import Search
-        from src.streamlines.interpolation import Interpolation
-        from src.streamlines.integration import Integration
+        from src import GridIO, FlowIO
+        from src import Search
+        from src import Interpolation
+        from src import Integration
 
         if point is None:
             point = [8.5, 0.5, 0.01]
 
         # Read the grid data
         grid = GridIO(gridfile)
         grid.read_grid(data_type=data_type)
```

### Comparing `lptlib-0.0.1a1/test/test_interpolation.py` & `lptlib-0.0.1a2/test/test_interpolation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # Test the data interpolation
 
 import unittest
 
 
 class TestInterpolation(unittest.TestCase):
     def test_interpolation(self):
-        from src.io.plot3dio import GridIO, FlowIO
-        from src.streamlines.search import Search
-        from src.streamlines.interpolation import Interpolation
+        from src import GridIO, FlowIO
+        from src import Search
+        from src import Interpolation
 
         # Read the grid data
         grid = GridIO('../data/plate_data/plate.sp.x')
         flow = FlowIO('../data/plate_data/sol-0000010.q')
         idx = Search(grid, [8.5, 0.5, 0.01])
         point_data = Interpolation(flow, idx)
 
@@ -25,15 +25,15 @@
             sum(abs(point_data.q.reshape(5)
                     - [9.99767442e-01, 1.02352604e-01, -5.38538464e-06, 6.40554753e-09, 1.79096631e+00]))
             <= 1e-6,
             True)
 
 
         # Test if the point is a node interpolation
-        from src.test_cases.oblique_shock_data import ObliqueShock, ObliqueShockData
+        from src import ObliqueShock, ObliqueShockData
 
         # Create oblique shock
         os = ObliqueShock()
         os.mach = 2
         os.deflection = 9
         os.compute()
```

### Comparing `lptlib-0.0.1a1/test/test_oblique_shock_data.py` & `lptlib-0.0.1a2/test/test_oblique_shock_data.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import unittest
 import numpy as np
 
 
 class TestObliqueShockResponse(unittest.TestCase):
     def test_oblique_shock(self):
-        from src.test_cases.oblique_shock_data import ObliqueShock
+        from src import ObliqueShock
         os = ObliqueShock()
         os.mach = 2.3
         os.deflection = 10
         os.compute()
         self.assertAlmostEqual(os.shock_angle.all(), np.array([34.32642717, 85.02615188]).all(), places=4)
 
     def test_oblique_shock_relation(self):
-        from src.test_cases.oblique_shock_data import ObliqueShock
-        from src.test_cases.oblique_shock_data import ObliqueShockData
+        from src import ObliqueShock
+        from src import ObliqueShockData
         os = ObliqueShock()
         os.mach = 2.3
         os.deflection = 10
         os.compute()
 
         # Create grid and flow files
         osd = ObliqueShockData()
```

### Comparing `lptlib-0.0.1a1/test/test_plot.py` & `lptlib-0.0.1a2/test/test_plot.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a1/test/test_plot3dio.py` & `lptlib-0.0.1a2/test/test_plot3dio.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # This test case is for plate data plot3d file
 # TODO: Add the docstring test
 
 import unittest
 import doctest
 import numpy as np
-from src.io import GridIO, FlowIO
+from src import GridIO, FlowIO
 
 
 class TestIO(unittest.TestCase):
     def test_grid_io(self):
 
         # Test with the plate data
         grid = GridIO('../data/plate_data/plate.sp.x')
```

### Comparing `lptlib-0.0.1a1/test/test_plots.py` & `lptlib-0.0.1a2/test/test_plots.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from src import Plots
 import matplotlib.pyplot as plt
 path = ('/Users/kal/Library/CloudStorage/OneDrive-UniversityofCincinnati/Desktop/University of Cincinnati/'
         'DoctoralWork/Codes/project-arrakis/data/shocks/new_start/ragni_data/315e-09/')
 
 
 def get_grid_and_flow():
-    from src.test_cases.oblique_shock_data import ObliqueShock, ObliqueShockData
+    from src import ObliqueShock, ObliqueShockData
 
     # Create oblique shock
     os = ObliqueShock()
     os.mach = 2
     os.deflection = 9
     os.compute()
```

### Comparing `lptlib-0.0.1a1/test/test_search.py` & `lptlib-0.0.1a2/test/test_search.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # This test is for the search algorithm using plate plot3d data
 
 import unittest
 from parameterized import parameterized
-from src.function.timer import Timer
+from src import Timer
 
 
 # This setup only works with the plate data
 # Need to add assertions to parametrized and change them to variables in the function
 # to be able to implement
 class TestSearch(unittest.TestCase):
     # sb: single block; mb: multi block
@@ -19,16 +19,16 @@
         # ('mb_dp_block_distance', '../data/multi_block/plate/plate.mb.dp.x', 'f8', 'block_distance'),
         # ('mb_dp_c_space', '../data/multi_block/plate/plate.mb.dp.x', 'f8', 'c-space'),
         ('mb_dp_p_space', '../data/multi_block/plate/plate.mb.dp.x', 'f8', 'p-space')
 
     ])
     @Timer()
     def test_search(self, name, filename='../data/plate_data/plate.sp.x', data_type='f4', method='binary'):
-        from src.io.plot3dio import GridIO
-        from src.streamlines.search import Search
+        from src import GridIO
+        from src import Search
 
         # Read the grid data
         grid = GridIO(filename)
         grid.read_grid(data_type=data_type)
         grid.compute_metrics()
         flow = None
```

### Comparing `lptlib-0.0.1a1/test/test_stochastic_model.py` & `lptlib-0.0.1a2/test/test_stochastic_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import unittest
 import numpy as np
 import matplotlib.pyplot as plt
-from src.streamlines.stochastic_model import StochasticModel, Particle, SpawnLocations
-from src.io.plot3dio import GridIO, FlowIO
+from src import StochasticModel, Particle, SpawnLocations
+from src import GridIO, FlowIO
 
 
 class TestStochasticModel(unittest.TestCase):
     def test_stochastic_model(self):
         # Test particle class
         p = Particle()
         p.min_dia = 281e-9
```

### Comparing `lptlib-0.0.1a1/test/test_terminal_run.py` & `lptlib-0.0.1a2/test/test_terminal_run.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import numpy as np
 import sys
 
 path = '/Users/kal/Library/CloudStorage/OneDrive-UniversityofCincinnati' \
        '/Desktop/University of Cincinnati/DoctoralWork/Codes/project-arrakis'
 sys.path.append(path)
 import matplotlib.pyplot as plt
-from src.streamlines.stochastic_model import StochasticModel, Particle, SpawnLocations
-from src.io.plot3dio import GridIO, FlowIO
+from src import StochasticModel, Particle, SpawnLocations
+from src import GridIO, FlowIO
 
 
 def test_stochastic_model():
     # Test particle class
     p = Particle()
     p.min_dia = 177e-9
     p.max_dia = 573e-9
```

### Comparing `lptlib-0.0.1a1/test/test_variables.py` & `lptlib-0.0.1a2/test/test_variables.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import unittest
 
 
 class TestVariables(unittest.TestCase):
-    from src.io.plot3dio import GridIO, FlowIO
-    from src.streamlines.search import Search
-    from src.streamlines.interpolation import Interpolation
+    from src import GridIO, FlowIO
+    from src import Search
+    from src import Interpolation
 
     # Get the data at a given point
     grid = GridIO('../data/plate_data/plate.sp.x')
     flow = FlowIO('../data/plate_data/sol-0000010.q')
     idx = Search(grid, [8.5, 0.5, 0.01])
     point_data = Interpolation(flow, idx)
 
@@ -20,30 +20,30 @@
     def test_variables(self, flow=flow):
         """
         To test variables class for the whole domain
         Test each function separately
         :param flow: FlowIO object
         :return: None
         """
-        from src.function.variables import Variables
+        from src import Variables
 
         variables = Variables(flow)
         variables.compute_velocity()
         variables.compute_temperature()
 
         self.assertEqual(variables.velocity.shape, (720, 152, 129, 3, 1))
         self.assertEqual(variables.temperature.shape, (720, 152, 129, 1))
 
     def test_variables_compute(self, flow=flow):
         """
         Test "compute" method in variables class
         :param flow: FlowIO object
         :return: None
         """
-        from src.function.variables import Variables
+        from src import Variables
 
         variables = Variables(flow)
         variables.compute()
 
         self.assertEqual(variables.velocity.shape, (720, 152, 129, 3, 1))
         self.assertEqual(variables.temperature.shape, (720, 152, 129, 1))
 
@@ -62,29 +62,29 @@
 
     def test_point_variables(self, point_data=point_data):
         """
         Test variables class for a single point
         :param point_data: Interpolation object
         :return: None
         """
-        from src.function.variables import Variables
+        from src import Variables
 
         point_variables = Variables(point_data)
         point_variables.compute_velocity()
         point_variables.compute_temperature()
 
         self._test(point_variables)
 
     def test_point_variables_compute(self, point_data=point_data):
         """
         Test "compute" method in variables class for a single point
         :param point_data: Interpolation object
         :return: None
         """
-        from src.function.variables import Variables
+        from src import Variables
 
         point_variables = Variables(point_data)
         point_variables.compute()
 
         self._test(point_variables)
```

