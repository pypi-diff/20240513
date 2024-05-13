# Comparing `tmp/lptlib-0.0.1a0.tar.gz` & `tmp/lptlib-0.0.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lptlib-0.0.1a0.tar", last modified: Mon May 13 17:32:37 2024, max compression
+gzip compressed data, was "lptlib-0.0.1a1.tar", last modified: Mon May 13 17:34:56 2024, max compression
```

## Comparing `lptlib-0.0.1a0.tar` & `lptlib-0.0.1a1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 17:32:37.328472 lptlib-0.0.1a0/
--rwx------   0 kal        (501) staff       (20)     1093 2024-05-10 20:01:36.000000 lptlib-0.0.1a0/LICENSE
--rw-r--r--   0 kal        (501) staff       (20)     1563 2024-05-13 17:32:37.328004 lptlib-0.0.1a0/PKG-INFO
--rw-r--r--   0 kal        (501) staff       (20)      579 2024-05-13 17:06:24.000000 lptlib-0.0.1a0/README.md
--rw-r--r--   0 kal        (501) staff       (20)     1094 2024-05-13 17:31:37.000000 lptlib-0.0.1a0/pyproject.toml
--rw-r--r--   0 kal        (501) staff       (20)       38 2024-05-13 17:32:37.328576 lptlib-0.0.1a0/setup.cfg
-drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 17:32:37.296744 lptlib-0.0.1a0/src/
--rw-r--r--   0 kal        (501) staff       (20)      127 2024-05-13 16:33:20.000000 lptlib-0.0.1a0/src/__init__.py
-drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 17:32:37.299686 lptlib-0.0.1a0/src/function/
--rw-r--r--   0 kal        (501) staff       (20)      109 2024-01-23 01:40:32.000000 lptlib-0.0.1a0/src/function/__init__.py
--rwx------   0 kal        (501) staff       (20)    12638 2024-05-13 17:24:07.000000 lptlib-0.0.1a0/src/function/plots.py
--rw-r--r--   0 kal        (501) staff       (20)     2034 2024-01-23 01:40:32.000000 lptlib-0.0.1a0/src/function/timer.py
--rw-r--r--   0 kal        (501) staff       (20)    11932 2024-05-13 17:24:06.000000 lptlib-0.0.1a0/src/function/variables.py
-drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 17:32:37.302574 lptlib-0.0.1a0/src/io/
--rw-r--r--   0 kal        (501) staff       (20)       91 2024-01-23 01:40:32.000000 lptlib-0.0.1a0/src/io/__init__.py
--rw-r--r--   0 kal        (501) staff       (20)    14881 2024-05-13 17:24:06.000000 lptlib-0.0.1a0/src/io/dataio.py
--rw-r--r--   0 kal        (501) staff       (20)    24440 2024-04-22 21:46:04.000000 lptlib-0.0.1a0/src/io/plot3dio.py
-drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 17:32:37.327406 lptlib-0.0.1a0/src/lptlib.egg-info/
--rw-r--r--   0 kal        (501) staff       (20)     1563 2024-05-13 17:32:37.000000 lptlib-0.0.1a0/src/lptlib.egg-info/PKG-INFO
--rw-r--r--   0 kal        (501) staff       (20)      898 2024-05-13 17:32:37.000000 lptlib-0.0.1a0/src/lptlib.egg-info/SOURCES.txt
--rw-r--r--   0 kal        (501) staff       (20)        1 2024-05-13 17:32:37.000000 lptlib-0.0.1a0/src/lptlib.egg-info/dependency_links.txt
--rw-r--r--   0 kal        (501) staff       (20)       46 2024-05-13 17:32:37.000000 lptlib-0.0.1a0/src/lptlib.egg-info/requires.txt
--rw-r--r--   0 kal        (501) staff       (20)       44 2024-05-13 17:32:37.000000 lptlib-0.0.1a0/src/lptlib.egg-info/top_level.txt
-drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 17:32:37.313092 lptlib-0.0.1a0/src/streamlines/
--rw-r--r--   0 kal        (501) staff       (20)      257 2024-01-23 01:40:32.000000 lptlib-0.0.1a0/src/streamlines/__init__.py
--rw-r--r--   0 kal        (501) staff       (20)    34475 2024-05-13 17:24:06.000000 lptlib-0.0.1a0/src/streamlines/integration.py
--rw-r--r--   0 kal        (501) staff       (20)    47345 2024-05-13 17:24:06.000000 lptlib-0.0.1a0/src/streamlines/interpolation.py
--rwxr-xr-x   0 kal        (501) staff       (20)    15615 2024-05-13 17:24:06.000000 lptlib-0.0.1a0/src/streamlines/search.py
--rw-r--r--   0 kal        (501) staff       (20)     7539 2024-05-13 17:24:06.000000 lptlib-0.0.1a0/src/streamlines/stochastic_model.py
--rw-r--r--   0 kal        (501) staff       (20)    39741 2024-05-13 17:24:07.000000 lptlib-0.0.1a0/src/streamlines/streamlines.py
-drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 17:32:37.315258 lptlib-0.0.1a0/src/test_cases/
--rwx------   0 kal        (501) staff       (20)       89 2024-01-23 01:40:32.000000 lptlib-0.0.1a0/src/test_cases/__init__.py
--rwx------   0 kal        (501) staff       (20)    10011 2024-05-13 17:24:06.000000 lptlib-0.0.1a0/src/test_cases/oblique_shock_data.py
-drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 17:32:37.326604 lptlib-0.0.1a0/test/
--rw-r--r--   0 kal        (501) staff       (20)     1019 2024-05-13 17:21:40.000000 lptlib-0.0.1a0/test/test_dataio.py
--rwx------   0 kal        (501) staff       (20)      576 2024-05-13 17:21:48.000000 lptlib-0.0.1a0/test/test_import.py
--rwx------   0 kal        (501) staff       (20)     2446 2024-05-13 17:24:07.000000 lptlib-0.0.1a0/test/test_integration.py
--rw-r--r--   0 kal        (501) staff       (20)     2103 2024-05-13 17:24:06.000000 lptlib-0.0.1a0/test/test_interpolation.py
--rwx------   0 kal        (501) staff       (20)     1238 2024-05-13 17:24:06.000000 lptlib-0.0.1a0/test/test_oblique_shock_data.py
--rw-r--r--   0 kal        (501) staff       (20)     2059 2023-08-17 08:22:42.000000 lptlib-0.0.1a0/test/test_plot.py
--rw-r--r--   0 kal        (501) staff       (20)     7327 2024-05-13 17:24:06.000000 lptlib-0.0.1a0/test/test_plot3dio.py
--rwx------   0 kal        (501) staff       (20)     2637 2024-05-13 17:24:07.000000 lptlib-0.0.1a0/test/test_plots.py
--rw-r--r--   0 kal        (501) staff       (20)     3306 2024-05-13 17:24:06.000000 lptlib-0.0.1a0/test/test_search.py
--rw-r--r--   0 kal        (501) staff       (20)     1955 2024-05-13 17:24:06.000000 lptlib-0.0.1a0/test/test_stochastic_model.py
--rw-r--r--   0 kal        (501) staff       (20)     1440 2024-05-13 17:24:06.000000 lptlib-0.0.1a0/test/test_terminal_run.py
--rwx------   0 kal        (501) staff       (20)     2829 2024-05-13 17:24:06.000000 lptlib-0.0.1a0/test/test_variables.py
+drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 17:34:56.673932 lptlib-0.0.1a1/
+-rwx------   0 kal        (501) staff       (20)     1093 2024-05-10 20:01:36.000000 lptlib-0.0.1a1/LICENSE
+-rw-r--r--   0 kal        (501) staff       (20)     1545 2024-05-13 17:34:56.673202 lptlib-0.0.1a1/PKG-INFO
+-rw-r--r--   0 kal        (501) staff       (20)      579 2024-05-13 17:06:24.000000 lptlib-0.0.1a1/README.md
+-rw-r--r--   0 kal        (501) staff       (20)     1085 2024-05-13 17:34:50.000000 lptlib-0.0.1a1/pyproject.toml
+-rw-r--r--   0 kal        (501) staff       (20)       38 2024-05-13 17:34:56.674099 lptlib-0.0.1a1/setup.cfg
+drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 17:34:56.641452 lptlib-0.0.1a1/src/
+-rw-r--r--   0 kal        (501) staff       (20)      127 2024-05-13 16:33:20.000000 lptlib-0.0.1a1/src/__init__.py
+drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 17:34:56.646139 lptlib-0.0.1a1/src/function/
+-rw-r--r--   0 kal        (501) staff       (20)      109 2024-01-23 01:40:32.000000 lptlib-0.0.1a1/src/function/__init__.py
+-rwx------   0 kal        (501) staff       (20)    12638 2024-05-13 17:24:07.000000 lptlib-0.0.1a1/src/function/plots.py
+-rw-r--r--   0 kal        (501) staff       (20)     2034 2024-01-23 01:40:32.000000 lptlib-0.0.1a1/src/function/timer.py
+-rw-r--r--   0 kal        (501) staff       (20)    11932 2024-05-13 17:24:06.000000 lptlib-0.0.1a1/src/function/variables.py
+drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 17:34:56.648888 lptlib-0.0.1a1/src/io/
+-rw-r--r--   0 kal        (501) staff       (20)       91 2024-01-23 01:40:32.000000 lptlib-0.0.1a1/src/io/__init__.py
+-rw-r--r--   0 kal        (501) staff       (20)    14881 2024-05-13 17:24:06.000000 lptlib-0.0.1a1/src/io/dataio.py
+-rw-r--r--   0 kal        (501) staff       (20)    24440 2024-04-22 21:46:04.000000 lptlib-0.0.1a1/src/io/plot3dio.py
+drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 17:34:56.672292 lptlib-0.0.1a1/src/lptlib.egg-info/
+-rw-r--r--   0 kal        (501) staff       (20)     1545 2024-05-13 17:34:56.000000 lptlib-0.0.1a1/src/lptlib.egg-info/PKG-INFO
+-rw-r--r--   0 kal        (501) staff       (20)      898 2024-05-13 17:34:56.000000 lptlib-0.0.1a1/src/lptlib.egg-info/SOURCES.txt
+-rw-r--r--   0 kal        (501) staff       (20)        1 2024-05-13 17:34:56.000000 lptlib-0.0.1a1/src/lptlib.egg-info/dependency_links.txt
+-rw-r--r--   0 kal        (501) staff       (20)       43 2024-05-13 17:34:56.000000 lptlib-0.0.1a1/src/lptlib.egg-info/requires.txt
+-rw-r--r--   0 kal        (501) staff       (20)       44 2024-05-13 17:34:56.000000 lptlib-0.0.1a1/src/lptlib.egg-info/top_level.txt
+drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 17:34:56.657368 lptlib-0.0.1a1/src/streamlines/
+-rw-r--r--   0 kal        (501) staff       (20)      257 2024-01-23 01:40:32.000000 lptlib-0.0.1a1/src/streamlines/__init__.py
+-rw-r--r--   0 kal        (501) staff       (20)    34475 2024-05-13 17:24:06.000000 lptlib-0.0.1a1/src/streamlines/integration.py
+-rw-r--r--   0 kal        (501) staff       (20)    47345 2024-05-13 17:24:06.000000 lptlib-0.0.1a1/src/streamlines/interpolation.py
+-rwxr-xr-x   0 kal        (501) staff       (20)    15615 2024-05-13 17:24:06.000000 lptlib-0.0.1a1/src/streamlines/search.py
+-rw-r--r--   0 kal        (501) staff       (20)     7539 2024-05-13 17:24:06.000000 lptlib-0.0.1a1/src/streamlines/stochastic_model.py
+-rw-r--r--   0 kal        (501) staff       (20)    39741 2024-05-13 17:24:07.000000 lptlib-0.0.1a1/src/streamlines/streamlines.py
+drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 17:34:56.660008 lptlib-0.0.1a1/src/test_cases/
+-rwx------   0 kal        (501) staff       (20)       89 2024-01-23 01:40:32.000000 lptlib-0.0.1a1/src/test_cases/__init__.py
+-rwx------   0 kal        (501) staff       (20)    10011 2024-05-13 17:24:06.000000 lptlib-0.0.1a1/src/test_cases/oblique_shock_data.py
+drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 17:34:56.671100 lptlib-0.0.1a1/test/
+-rw-r--r--   0 kal        (501) staff       (20)     1019 2024-05-13 17:21:40.000000 lptlib-0.0.1a1/test/test_dataio.py
+-rwx------   0 kal        (501) staff       (20)      576 2024-05-13 17:21:48.000000 lptlib-0.0.1a1/test/test_import.py
+-rwx------   0 kal        (501) staff       (20)     2446 2024-05-13 17:24:07.000000 lptlib-0.0.1a1/test/test_integration.py
+-rw-r--r--   0 kal        (501) staff       (20)     2103 2024-05-13 17:24:06.000000 lptlib-0.0.1a1/test/test_interpolation.py
+-rwx------   0 kal        (501) staff       (20)     1238 2024-05-13 17:24:06.000000 lptlib-0.0.1a1/test/test_oblique_shock_data.py
+-rw-r--r--   0 kal        (501) staff       (20)     2059 2023-08-17 08:22:42.000000 lptlib-0.0.1a1/test/test_plot.py
+-rw-r--r--   0 kal        (501) staff       (20)     7327 2024-05-13 17:24:06.000000 lptlib-0.0.1a1/test/test_plot3dio.py
+-rwx------   0 kal        (501) staff       (20)     2637 2024-05-13 17:24:07.000000 lptlib-0.0.1a1/test/test_plots.py
+-rw-r--r--   0 kal        (501) staff       (20)     3306 2024-05-13 17:24:06.000000 lptlib-0.0.1a1/test/test_search.py
+-rw-r--r--   0 kal        (501) staff       (20)     1955 2024-05-13 17:24:06.000000 lptlib-0.0.1a1/test/test_stochastic_model.py
+-rw-r--r--   0 kal        (501) staff       (20)     1440 2024-05-13 17:24:06.000000 lptlib-0.0.1a1/test/test_terminal_run.py
+-rwx------   0 kal        (501) staff       (20)     2829 2024-05-13 17:24:06.000000 lptlib-0.0.1a1/test/test_variables.py
```

### Comparing `lptlib-0.0.1a0/LICENSE` & `lptlib-0.0.1a1/LICENSE`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a0/PKG-INFO` & `lptlib-0.0.1a1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lptlib
-Version: 0.0.1a0
+Version: 0.0.1a1
 Summary: One-way coupled Lagrangian Particle Tracking algorithms.
 Author: Dilip Kalagotla
 Author-email: dilipkalagotla@gmail.com
 Project-URL: homepage, https://github.com/kalagotla/project-arrakis
 Project-URL: issues, https://github.com/kalagotla/project-arrakis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -20,15 +20,14 @@
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: matplotlib
 Requires-Dist: pandas
 Requires-Dist: seaborn
 Requires-Dist: tqdm
-Requires-Dist: re
 
 # lptlib (Lagrangian Particle Tracking Library)
 ### Previously project-arrakis
 
 Python based particle tracking algorithms for CFD data
 
 A highly parallelized set of Lagrangian Particle Tracking (LPT) algorithms based on Python to post-process steady and unsteady CFD data. An advanced programming interface (API) is developed for uncertainty quantification of optical velocimetry data.
```

### Comparing `lptlib-0.0.1a0/README.md` & `lptlib-0.0.1a1/README.md`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a0/pyproject.toml` & `lptlib-0.0.1a1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lptlib"
-version = "0.0.1a0"
+version = "0.0.1a1"
 authors = [
     {name="Dilip Kalagotla"},
     {email="dilipkalagotla@gmail.com"},
     ]
 description = "One-way coupled Lagrangian Particle Tracking algorithms."
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = [
     "numpy",
     "scipy",
     "matplotlib",
     "pandas",
     "seaborn",
     "tqdm",
-    "re"
     ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "License :: OSI Approved :: MIT License",
```

### Comparing `lptlib-0.0.1a0/src/function/plots.py` & `lptlib-0.0.1a1/src/function/plots.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a0/src/function/timer.py` & `lptlib-0.0.1a1/src/function/timer.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a0/src/function/variables.py` & `lptlib-0.0.1a1/src/function/variables.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a0/src/io/dataio.py` & `lptlib-0.0.1a1/src/io/dataio.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a0/src/io/plot3dio.py` & `lptlib-0.0.1a1/src/io/plot3dio.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a0/src/lptlib.egg-info/PKG-INFO` & `lptlib-0.0.1a1/src/lptlib.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lptlib
-Version: 0.0.1a0
+Version: 0.0.1a1
 Summary: One-way coupled Lagrangian Particle Tracking algorithms.
 Author: Dilip Kalagotla
 Author-email: dilipkalagotla@gmail.com
 Project-URL: homepage, https://github.com/kalagotla/project-arrakis
 Project-URL: issues, https://github.com/kalagotla/project-arrakis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -20,15 +20,14 @@
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: matplotlib
 Requires-Dist: pandas
 Requires-Dist: seaborn
 Requires-Dist: tqdm
-Requires-Dist: re
 
 # lptlib (Lagrangian Particle Tracking Library)
 ### Previously project-arrakis
 
 Python based particle tracking algorithms for CFD data
 
 A highly parallelized set of Lagrangian Particle Tracking (LPT) algorithms based on Python to post-process steady and unsteady CFD data. An advanced programming interface (API) is developed for uncertainty quantification of optical velocimetry data.
```

### Comparing `lptlib-0.0.1a0/src/lptlib.egg-info/SOURCES.txt` & `lptlib-0.0.1a1/src/lptlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a0/src/streamlines/integration.py` & `lptlib-0.0.1a1/src/streamlines/integration.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a0/src/streamlines/interpolation.py` & `lptlib-0.0.1a1/src/streamlines/interpolation.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a0/src/streamlines/search.py` & `lptlib-0.0.1a1/src/streamlines/search.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a0/src/streamlines/stochastic_model.py` & `lptlib-0.0.1a1/src/streamlines/stochastic_model.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a0/src/streamlines/streamlines.py` & `lptlib-0.0.1a1/src/streamlines/streamlines.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a0/src/test_cases/oblique_shock_data.py` & `lptlib-0.0.1a1/src/test_cases/oblique_shock_data.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a0/test/test_dataio.py` & `lptlib-0.0.1a1/test/test_dataio.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a0/test/test_import.py` & `lptlib-0.0.1a1/test/test_import.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a0/test/test_integration.py` & `lptlib-0.0.1a1/test/test_integration.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a0/test/test_interpolation.py` & `lptlib-0.0.1a1/test/test_interpolation.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a0/test/test_oblique_shock_data.py` & `lptlib-0.0.1a1/test/test_oblique_shock_data.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a0/test/test_plot.py` & `lptlib-0.0.1a1/test/test_plot.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a0/test/test_plot3dio.py` & `lptlib-0.0.1a1/test/test_plot3dio.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a0/test/test_plots.py` & `lptlib-0.0.1a1/test/test_plots.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a0/test/test_search.py` & `lptlib-0.0.1a1/test/test_search.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a0/test/test_stochastic_model.py` & `lptlib-0.0.1a1/test/test_stochastic_model.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a0/test/test_terminal_run.py` & `lptlib-0.0.1a1/test/test_terminal_run.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a0/test/test_variables.py` & `lptlib-0.0.1a1/test/test_variables.py`

 * *Files identical despite different names*

