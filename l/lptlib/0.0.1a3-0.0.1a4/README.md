# Comparing `tmp/lptlib-0.0.1a3.tar.gz` & `tmp/lptlib-0.0.1a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lptlib-0.0.1a3.tar", last modified: Mon May 13 17:51:53 2024, max compression
+gzip compressed data, was "lptlib-0.0.1a4.tar", last modified: Mon May 13 21:50:26 2024, max compression
```

## Comparing `lptlib-0.0.1a3.tar` & `lptlib-0.0.1a4.tar`

### file list

```diff
@@ -1,48 +1,47 @@
-drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 17:51:53.774287 lptlib-0.0.1a3/
--rwx------   0 kal        (501) staff       (20)     1093 2024-05-10 20:01:36.000000 lptlib-0.0.1a3/LICENSE
--rw-r--r--   0 kal        (501) staff       (20)     1545 2024-05-13 17:51:53.773424 lptlib-0.0.1a3/PKG-INFO
--rw-r--r--   0 kal        (501) staff       (20)      579 2024-05-13 17:06:24.000000 lptlib-0.0.1a3/README.md
--rw-r--r--   0 kal        (501) staff       (20)     1085 2024-05-13 17:51:47.000000 lptlib-0.0.1a3/pyproject.toml
--rw-r--r--   0 kal        (501) staff       (20)       38 2024-05-13 17:51:53.774507 lptlib-0.0.1a3/setup.cfg
-drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 17:51:53.744452 lptlib-0.0.1a3/src/
--rw-r--r--   0 kal        (501) staff       (20)       22 2024-05-13 17:51:47.000000 lptlib-0.0.1a3/src/__init__.py
-drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 17:51:53.745011 lptlib-0.0.1a3/src/lptlib/
--rw-r--r--   0 kal        (501) staff       (20)      122 2024-05-13 17:40:07.000000 lptlib-0.0.1a3/src/lptlib/__init__.py
-drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 17:51:53.750343 lptlib-0.0.1a3/src/lptlib/function/
--rw-r--r--   0 kal        (501) staff       (20)      109 2024-01-23 01:40:32.000000 lptlib-0.0.1a3/src/lptlib/function/__init__.py
--rwx------   0 kal        (501) staff       (20)    12631 2024-05-13 17:51:47.000000 lptlib-0.0.1a3/src/lptlib/function/plots.py
--rw-r--r--   0 kal        (501) staff       (20)     2034 2024-01-23 01:40:32.000000 lptlib-0.0.1a3/src/lptlib/function/timer.py
--rw-r--r--   0 kal        (501) staff       (20)    11932 2024-05-13 17:24:06.000000 lptlib-0.0.1a3/src/lptlib/function/variables.py
-drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 17:51:53.753336 lptlib-0.0.1a3/src/lptlib/io/
--rw-r--r--   0 kal        (501) staff       (20)       91 2024-01-23 01:40:32.000000 lptlib-0.0.1a3/src/lptlib/io/__init__.py
--rw-r--r--   0 kal        (501) staff       (20)    14895 2024-05-13 17:51:47.000000 lptlib-0.0.1a3/src/lptlib/io/dataio.py
--rw-r--r--   0 kal        (501) staff       (20)    24440 2024-04-22 21:46:04.000000 lptlib-0.0.1a3/src/lptlib/io/plot3dio.py
-drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 17:51:53.759254 lptlib-0.0.1a3/src/lptlib/streamlines/
--rw-r--r--   0 kal        (501) staff       (20)      257 2024-01-23 01:40:32.000000 lptlib-0.0.1a3/src/lptlib/streamlines/__init__.py
--rw-r--r--   0 kal        (501) staff       (20)    34496 2024-05-13 17:51:47.000000 lptlib-0.0.1a3/src/lptlib/streamlines/integration.py
--rw-r--r--   0 kal        (501) staff       (20)    47345 2024-05-13 17:24:06.000000 lptlib-0.0.1a3/src/lptlib/streamlines/interpolation.py
--rwxr-xr-x   0 kal        (501) staff       (20)    15615 2024-05-13 17:24:06.000000 lptlib-0.0.1a3/src/lptlib/streamlines/search.py
--rw-r--r--   0 kal        (501) staff       (20)     7546 2024-05-13 17:51:47.000000 lptlib-0.0.1a3/src/lptlib/streamlines/stochastic_model.py
--rw-r--r--   0 kal        (501) staff       (20)    39790 2024-05-13 17:51:47.000000 lptlib-0.0.1a3/src/lptlib/streamlines/streamlines.py
-drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 17:51:53.760745 lptlib-0.0.1a3/src/lptlib/test_cases/
--rwx------   0 kal        (501) staff       (20)       89 2024-01-23 01:40:32.000000 lptlib-0.0.1a3/src/lptlib/test_cases/__init__.py
--rwx------   0 kal        (501) staff       (20)    10018 2024-05-13 17:51:47.000000 lptlib-0.0.1a3/src/lptlib/test_cases/oblique_shock_data.py
-drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 17:51:53.772575 lptlib-0.0.1a3/src/lptlib.egg-info/
--rw-r--r--   0 kal        (501) staff       (20)     1545 2024-05-13 17:51:53.000000 lptlib-0.0.1a3/src/lptlib.egg-info/PKG-INFO
--rw-r--r--   0 kal        (501) staff       (20)     1026 2024-05-13 17:51:53.000000 lptlib-0.0.1a3/src/lptlib.egg-info/SOURCES.txt
--rw-r--r--   0 kal        (501) staff       (20)        1 2024-05-13 17:51:53.000000 lptlib-0.0.1a3/src/lptlib.egg-info/dependency_links.txt
--rw-r--r--   0 kal        (501) staff       (20)       43 2024-05-13 17:51:53.000000 lptlib-0.0.1a3/src/lptlib.egg-info/requires.txt
--rw-r--r--   0 kal        (501) staff       (20)       16 2024-05-13 17:51:53.000000 lptlib-0.0.1a3/src/lptlib.egg-info/top_level.txt
-drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 17:51:53.771639 lptlib-0.0.1a3/test/
--rw-r--r--   0 kal        (501) staff       (20)     1011 2024-05-13 17:51:47.000000 lptlib-0.0.1a3/test/test_dataio.py
--rwx------   0 kal        (501) staff       (20)      468 2024-05-13 17:51:47.000000 lptlib-0.0.1a3/test/test_import.py
--rwx------   0 kal        (501) staff       (20)     2350 2024-05-13 17:40:07.000000 lptlib-0.0.1a3/test/test_integration.py
--rw-r--r--   0 kal        (501) staff       (20)     2016 2024-05-13 17:40:07.000000 lptlib-0.0.1a3/test/test_interpolation.py
--rwx------   0 kal        (501) staff       (20)     1148 2024-05-13 17:40:08.000000 lptlib-0.0.1a3/test/test_oblique_shock_data.py
--rw-r--r--   0 kal        (501) staff       (20)     2059 2023-08-17 08:22:42.000000 lptlib-0.0.1a3/test/test_plot.py
--rw-r--r--   0 kal        (501) staff       (20)     7324 2024-05-13 17:40:08.000000 lptlib-0.0.1a3/test/test_plot3dio.py
--rwx------   0 kal        (501) staff       (20)     2607 2024-05-13 17:40:08.000000 lptlib-0.0.1a3/test/test_plots.py
--rw-r--r--   0 kal        (501) staff       (20)     3260 2024-05-13 17:40:07.000000 lptlib-0.0.1a3/test/test_search.py
--rw-r--r--   0 kal        (501) staff       (20)     1914 2024-05-13 17:40:07.000000 lptlib-0.0.1a3/test/test_stochastic_model.py
--rw-r--r--   0 kal        (501) staff       (20)     1399 2024-05-13 17:40:07.000000 lptlib-0.0.1a3/test/test_terminal_run.py
--rwx------   0 kal        (501) staff       (20)     2696 2024-05-13 17:40:07.000000 lptlib-0.0.1a3/test/test_variables.py
+drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 21:50:26.745878 lptlib-0.0.1a4/
+-rwx------   0 kal        (501) staff       (20)     1093 2024-05-10 20:01:36.000000 lptlib-0.0.1a4/LICENSE
+-rw-r--r--   0 kal        (501) staff       (20)     1545 2024-05-13 21:50:26.745379 lptlib-0.0.1a4/PKG-INFO
+-rw-r--r--   0 kal        (501) staff       (20)      579 2024-05-13 17:06:24.000000 lptlib-0.0.1a4/README.md
+-rw-r--r--   0 kal        (501) staff       (20)     1085 2024-05-13 21:50:21.000000 lptlib-0.0.1a4/pyproject.toml
+-rw-r--r--   0 kal        (501) staff       (20)       38 2024-05-13 21:50:26.745988 lptlib-0.0.1a4/setup.cfg
+drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 21:50:26.714978 lptlib-0.0.1a4/src/
+drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 21:50:26.718124 lptlib-0.0.1a4/src/lptlib/
+-rw-r--r--   0 kal        (501) staff       (20)        0 2024-05-13 21:32:10.000000 lptlib-0.0.1a4/src/lptlib/__init__.py
+drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 21:50:26.721669 lptlib-0.0.1a4/src/lptlib/function/
+-rw-r--r--   0 kal        (501) staff       (20)      109 2024-01-23 01:40:32.000000 lptlib-0.0.1a4/src/lptlib/function/__init__.py
+-rwx------   0 kal        (501) staff       (20)    12533 2024-05-13 21:39:16.000000 lptlib-0.0.1a4/src/lptlib/function/plots.py
+-rw-r--r--   0 kal        (501) staff       (20)     2034 2024-01-23 01:40:32.000000 lptlib-0.0.1a4/src/lptlib/function/timer.py
+-rw-r--r--   0 kal        (501) staff       (20)    11932 2024-05-13 17:24:06.000000 lptlib-0.0.1a4/src/lptlib/function/variables.py
+drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 21:50:26.724163 lptlib-0.0.1a4/src/lptlib/io/
+-rw-r--r--   0 kal        (501) staff       (20)       91 2024-01-23 01:40:32.000000 lptlib-0.0.1a4/src/lptlib/io/__init__.py
+-rw-r--r--   0 kal        (501) staff       (20)    14895 2024-05-13 17:51:47.000000 lptlib-0.0.1a4/src/lptlib/io/dataio.py
+-rw-r--r--   0 kal        (501) staff       (20)    24440 2024-04-22 21:46:04.000000 lptlib-0.0.1a4/src/lptlib/io/plot3dio.py
+drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 21:50:26.731560 lptlib-0.0.1a4/src/lptlib/streamlines/
+-rw-r--r--   0 kal        (501) staff       (20)      257 2024-01-23 01:40:32.000000 lptlib-0.0.1a4/src/lptlib/streamlines/__init__.py
+-rw-r--r--   0 kal        (501) staff       (20)    34496 2024-05-13 17:51:47.000000 lptlib-0.0.1a4/src/lptlib/streamlines/integration.py
+-rw-r--r--   0 kal        (501) staff       (20)    47345 2024-05-13 17:24:06.000000 lptlib-0.0.1a4/src/lptlib/streamlines/interpolation.py
+-rwxr-xr-x   0 kal        (501) staff       (20)    15615 2024-05-13 17:24:06.000000 lptlib-0.0.1a4/src/lptlib/streamlines/search.py
+-rw-r--r--   0 kal        (501) staff       (20)     7537 2024-05-13 21:50:14.000000 lptlib-0.0.1a4/src/lptlib/streamlines/stochastic_model.py
+-rw-r--r--   0 kal        (501) staff       (20)    39727 2024-05-13 21:49:30.000000 lptlib-0.0.1a4/src/lptlib/streamlines/streamlines.py
+drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 21:50:26.733428 lptlib-0.0.1a4/src/lptlib/test_cases/
+-rwx------   0 kal        (501) staff       (20)       89 2024-01-23 01:40:32.000000 lptlib-0.0.1a4/src/lptlib/test_cases/__init__.py
+-rwx------   0 kal        (501) staff       (20)    10018 2024-05-13 17:51:47.000000 lptlib-0.0.1a4/src/lptlib/test_cases/oblique_shock_data.py
+drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 21:50:26.744583 lptlib-0.0.1a4/src/lptlib.egg-info/
+-rw-r--r--   0 kal        (501) staff       (20)     1545 2024-05-13 21:50:26.000000 lptlib-0.0.1a4/src/lptlib.egg-info/PKG-INFO
+-rw-r--r--   0 kal        (501) staff       (20)     1010 2024-05-13 21:50:26.000000 lptlib-0.0.1a4/src/lptlib.egg-info/SOURCES.txt
+-rw-r--r--   0 kal        (501) staff       (20)        1 2024-05-13 21:50:26.000000 lptlib-0.0.1a4/src/lptlib.egg-info/dependency_links.txt
+-rw-r--r--   0 kal        (501) staff       (20)       43 2024-05-13 21:50:26.000000 lptlib-0.0.1a4/src/lptlib.egg-info/requires.txt
+-rw-r--r--   0 kal        (501) staff       (20)        7 2024-05-13 21:50:26.000000 lptlib-0.0.1a4/src/lptlib.egg-info/top_level.txt
+drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 21:50:26.743680 lptlib-0.0.1a4/test/
+-rw-r--r--   0 kal        (501) staff       (20)     1011 2024-05-13 17:51:47.000000 lptlib-0.0.1a4/test/test_dataio.py
+-rwx------   0 kal        (501) staff       (20)      468 2024-05-13 17:51:47.000000 lptlib-0.0.1a4/test/test_import.py
+-rwx------   0 kal        (501) staff       (20)     2350 2024-05-13 17:40:07.000000 lptlib-0.0.1a4/test/test_integration.py
+-rw-r--r--   0 kal        (501) staff       (20)     2016 2024-05-13 17:40:07.000000 lptlib-0.0.1a4/test/test_interpolation.py
+-rwx------   0 kal        (501) staff       (20)     1148 2024-05-13 17:40:08.000000 lptlib-0.0.1a4/test/test_oblique_shock_data.py
+-rw-r--r--   0 kal        (501) staff       (20)     2059 2023-08-17 08:22:42.000000 lptlib-0.0.1a4/test/test_plot.py
+-rw-r--r--   0 kal        (501) staff       (20)     7324 2024-05-13 17:40:08.000000 lptlib-0.0.1a4/test/test_plot3dio.py
+-rwx------   0 kal        (501) staff       (20)     2607 2024-05-13 17:40:08.000000 lptlib-0.0.1a4/test/test_plots.py
+-rw-r--r--   0 kal        (501) staff       (20)     3260 2024-05-13 17:40:07.000000 lptlib-0.0.1a4/test/test_search.py
+-rw-r--r--   0 kal        (501) staff       (20)     1914 2024-05-13 17:40:07.000000 lptlib-0.0.1a4/test/test_stochastic_model.py
+-rw-r--r--   0 kal        (501) staff       (20)     1399 2024-05-13 17:40:07.000000 lptlib-0.0.1a4/test/test_terminal_run.py
+-rwx------   0 kal        (501) staff       (20)     2696 2024-05-13 17:40:07.000000 lptlib-0.0.1a4/test/test_variables.py
```

### Comparing `lptlib-0.0.1a3/LICENSE` & `lptlib-0.0.1a4/LICENSE`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a3/PKG-INFO` & `lptlib-0.0.1a4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lptlib
-Version: 0.0.1a3
+Version: 0.0.1a4
 Summary: One-way coupled Lagrangian Particle Tracking algorithms.
 Author: Dilip Kalagotla
 Author-email: dilipkalagotla@gmail.com
 Project-URL: homepage, https://github.com/kalagotla/project-arrakis
 Project-URL: issues, https://github.com/kalagotla/project-arrakis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `lptlib-0.0.1a3/README.md` & `lptlib-0.0.1a4/README.md`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a3/pyproject.toml` & `lptlib-0.0.1a4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lptlib"
-version = "0.0.1a3"
+version = "0.0.1a4"
 authors = [
     {name="Dilip Kalagotla"},
     {email="dilipkalagotla@gmail.com"},
     ]
 description = "One-way coupled Lagrangian Particle Tracking algorithms."
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `lptlib-0.0.1a3/src/lptlib/function/plots.py` & `lptlib-0.0.1a4/src/lptlib/function/plots.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 # Create plots for the data saved from streamlines file
 
 import numpy as np
 import matplotlib.pyplot as plt
 import matplotlib.colors as colors
-import matplotlib.patches as patches
-import matplotlib.gridspec as gridspec
-import seaborn as sns
 import re
 import pandas as pd
-from src.lptlib import Search, Interpolation
-from src.lptlib import Variables
+from ..streamlines import Search, Interpolation
+from .variables import Variables
 
 
 class Plots:
     """
     Module to plot data
     """
     def __init__(self, file, grid=None, flow=None):
```

### Comparing `lptlib-0.0.1a3/src/lptlib/function/timer.py` & `lptlib-0.0.1a4/src/lptlib/function/timer.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a3/src/lptlib/function/variables.py` & `lptlib-0.0.1a4/src/lptlib/function/variables.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a3/src/lptlib/io/dataio.py` & `lptlib-0.0.1a4/src/lptlib/io/dataio.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a3/src/lptlib/io/plot3dio.py` & `lptlib-0.0.1a4/src/lptlib/io/plot3dio.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a3/src/lptlib/streamlines/integration.py` & `lptlib-0.0.1a4/src/lptlib/streamlines/integration.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a3/src/lptlib/streamlines/interpolation.py` & `lptlib-0.0.1a4/src/lptlib/streamlines/interpolation.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a3/src/lptlib/streamlines/search.py` & `lptlib-0.0.1a4/src/lptlib/streamlines/search.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a3/src/lptlib/streamlines/stochastic_model.py` & `lptlib-0.0.1a4/src/lptlib/streamlines/stochastic_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Class to run streamlines script in parallel
 # Stochastic model for tracers is implemented
 
 import numpy as np
 from multiprocessing.pool import ThreadPool as Pool
 import multiprocessing as mp
-from src.lptlib.streamlines.streamlines import Streamlines
+from ..streamlines.streamlines import Streamlines
 from scipy.stats import skewnorm, lognorm
 from tqdm import tqdm
 
 rng = np.random.default_rng(7)
 
 
 class StochasticModel(Streamlines):
```

### Comparing `lptlib-0.0.1a3/src/lptlib/streamlines/streamlines.py` & `lptlib-0.0.1a4/src/lptlib/streamlines/streamlines.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # Uses the program API to extract streamlines
 import numpy as np
-from src.lptlib.function.timer import Timer
-from src.lptlib.io.plot3dio import GridIO
-from src.lptlib.io.plot3dio import FlowIO
-from src.lptlib.streamlines.search import Search
-from src.lptlib.streamlines.interpolation import Interpolation
-from src.lptlib.streamlines.integration import Integration
-from src.lptlib.function.variables import Variables
+from ..function.timer import Timer
+from ..io.plot3dio import GridIO
+from ..io.plot3dio import FlowIO
+from ..streamlines.search import Search
+from ..streamlines.interpolation import Interpolation
+from ..streamlines.integration import Integration
+from ..function.variables import Variables
 import matplotlib.pyplot as plt
 import functools
 
 
 class Streamlines:
     """
     Module to extract particle path information
```

### Comparing `lptlib-0.0.1a3/src/lptlib/test_cases/oblique_shock_data.py` & `lptlib-0.0.1a4/src/lptlib/test_cases/oblique_shock_data.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a3/src/lptlib.egg-info/PKG-INFO` & `lptlib-0.0.1a4/src/lptlib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lptlib
-Version: 0.0.1a3
+Version: 0.0.1a4
 Summary: One-way coupled Lagrangian Particle Tracking algorithms.
 Author: Dilip Kalagotla
 Author-email: dilipkalagotla@gmail.com
 Project-URL: homepage, https://github.com/kalagotla/project-arrakis
 Project-URL: issues, https://github.com/kalagotla/project-arrakis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `lptlib-0.0.1a3/src/lptlib.egg-info/SOURCES.txt` & `lptlib-0.0.1a4/src/lptlib.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 LICENSE
 README.md
 pyproject.toml
-src/__init__.py
 src/lptlib/__init__.py
 src/lptlib.egg-info/PKG-INFO
 src/lptlib.egg-info/SOURCES.txt
 src/lptlib.egg-info/dependency_links.txt
 src/lptlib.egg-info/requires.txt
 src/lptlib.egg-info/top_level.txt
 src/lptlib/function/__init__.py
```

### Comparing `lptlib-0.0.1a3/test/test_dataio.py` & `lptlib-0.0.1a4/test/test_dataio.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a3/test/test_integration.py` & `lptlib-0.0.1a4/test/test_integration.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a3/test/test_interpolation.py` & `lptlib-0.0.1a4/test/test_interpolation.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a3/test/test_oblique_shock_data.py` & `lptlib-0.0.1a4/test/test_oblique_shock_data.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a3/test/test_plot.py` & `lptlib-0.0.1a4/test/test_plot.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a3/test/test_plot3dio.py` & `lptlib-0.0.1a4/test/test_plot3dio.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a3/test/test_plots.py` & `lptlib-0.0.1a4/test/test_plots.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a3/test/test_search.py` & `lptlib-0.0.1a4/test/test_search.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a3/test/test_stochastic_model.py` & `lptlib-0.0.1a4/test/test_stochastic_model.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a3/test/test_terminal_run.py` & `lptlib-0.0.1a4/test/test_terminal_run.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a3/test/test_variables.py` & `lptlib-0.0.1a4/test/test_variables.py`

 * *Files identical despite different names*

