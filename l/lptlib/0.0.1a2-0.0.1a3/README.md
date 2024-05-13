# Comparing `tmp/lptlib-0.0.1a2.tar.gz` & `tmp/lptlib-0.0.1a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lptlib-0.0.1a2.tar", last modified: Mon May 13 17:40:52 2024, max compression
+gzip compressed data, was "lptlib-0.0.1a3.tar", last modified: Mon May 13 17:51:53 2024, max compression
```

## Comparing `lptlib-0.0.1a2.tar` & `lptlib-0.0.1a3.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 17:40:52.476982 lptlib-0.0.1a2/
--rwx------   0 kal        (501) staff       (20)     1093 2024-05-10 20:01:36.000000 lptlib-0.0.1a2/LICENSE
--rw-r--r--   0 kal        (501) staff       (20)     1545 2024-05-13 17:40:52.476262 lptlib-0.0.1a2/PKG-INFO
--rw-r--r--   0 kal        (501) staff       (20)      579 2024-05-13 17:06:24.000000 lptlib-0.0.1a2/README.md
--rw-r--r--   0 kal        (501) staff       (20)     1085 2024-05-13 17:40:45.000000 lptlib-0.0.1a2/pyproject.toml
--rw-r--r--   0 kal        (501) staff       (20)       38 2024-05-13 17:40:52.477150 lptlib-0.0.1a2/setup.cfg
-drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 17:40:52.447578 lptlib-0.0.1a2/src/
-drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 17:40:52.450987 lptlib-0.0.1a2/src/lptlib/
--rw-r--r--   0 kal        (501) staff       (20)      122 2024-05-13 17:40:07.000000 lptlib-0.0.1a2/src/lptlib/__init__.py
-drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 17:40:52.455987 lptlib-0.0.1a2/src/lptlib/function/
--rw-r--r--   0 kal        (501) staff       (20)      109 2024-01-23 01:40:32.000000 lptlib-0.0.1a2/src/lptlib/function/__init__.py
--rwx------   0 kal        (501) staff       (20)    12638 2024-05-13 17:24:07.000000 lptlib-0.0.1a2/src/lptlib/function/plots.py
--rw-r--r--   0 kal        (501) staff       (20)     2034 2024-01-23 01:40:32.000000 lptlib-0.0.1a2/src/lptlib/function/timer.py
--rw-r--r--   0 kal        (501) staff       (20)    11932 2024-05-13 17:24:06.000000 lptlib-0.0.1a2/src/lptlib/function/variables.py
-drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 17:40:52.458242 lptlib-0.0.1a2/src/lptlib/io/
--rw-r--r--   0 kal        (501) staff       (20)       91 2024-01-23 01:40:32.000000 lptlib-0.0.1a2/src/lptlib/io/__init__.py
--rw-r--r--   0 kal        (501) staff       (20)    14881 2024-05-13 17:24:06.000000 lptlib-0.0.1a2/src/lptlib/io/dataio.py
--rw-r--r--   0 kal        (501) staff       (20)    24440 2024-04-22 21:46:04.000000 lptlib-0.0.1a2/src/lptlib/io/plot3dio.py
-drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 17:40:52.464994 lptlib-0.0.1a2/src/lptlib/streamlines/
--rw-r--r--   0 kal        (501) staff       (20)      257 2024-01-23 01:40:32.000000 lptlib-0.0.1a2/src/lptlib/streamlines/__init__.py
--rw-r--r--   0 kal        (501) staff       (20)    34475 2024-05-13 17:24:06.000000 lptlib-0.0.1a2/src/lptlib/streamlines/integration.py
--rw-r--r--   0 kal        (501) staff       (20)    47345 2024-05-13 17:24:06.000000 lptlib-0.0.1a2/src/lptlib/streamlines/interpolation.py
--rwxr-xr-x   0 kal        (501) staff       (20)    15615 2024-05-13 17:24:06.000000 lptlib-0.0.1a2/src/lptlib/streamlines/search.py
--rw-r--r--   0 kal        (501) staff       (20)     7539 2024-05-13 17:24:06.000000 lptlib-0.0.1a2/src/lptlib/streamlines/stochastic_model.py
--rw-r--r--   0 kal        (501) staff       (20)    39741 2024-05-13 17:24:07.000000 lptlib-0.0.1a2/src/lptlib/streamlines/streamlines.py
-drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 17:40:52.467522 lptlib-0.0.1a2/src/lptlib/test_cases/
--rwx------   0 kal        (501) staff       (20)       89 2024-01-23 01:40:32.000000 lptlib-0.0.1a2/src/lptlib/test_cases/__init__.py
--rwx------   0 kal        (501) staff       (20)    10011 2024-05-13 17:24:06.000000 lptlib-0.0.1a2/src/lptlib/test_cases/oblique_shock_data.py
-drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 17:40:52.475381 lptlib-0.0.1a2/src/lptlib.egg-info/
--rw-r--r--   0 kal        (501) staff       (20)     1545 2024-05-13 17:40:52.000000 lptlib-0.0.1a2/src/lptlib.egg-info/PKG-INFO
--rw-r--r--   0 kal        (501) staff       (20)     1010 2024-05-13 17:40:52.000000 lptlib-0.0.1a2/src/lptlib.egg-info/SOURCES.txt
--rw-r--r--   0 kal        (501) staff       (20)        1 2024-05-13 17:40:52.000000 lptlib-0.0.1a2/src/lptlib.egg-info/dependency_links.txt
--rw-r--r--   0 kal        (501) staff       (20)       43 2024-05-13 17:40:52.000000 lptlib-0.0.1a2/src/lptlib.egg-info/requires.txt
--rw-r--r--   0 kal        (501) staff       (20)        7 2024-05-13 17:40:52.000000 lptlib-0.0.1a2/src/lptlib.egg-info/top_level.txt
-drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 17:40:52.474625 lptlib-0.0.1a2/test/
--rw-r--r--   0 kal        (501) staff       (20)      997 2024-05-13 17:40:07.000000 lptlib-0.0.1a2/test/test_dataio.py
--rwx------   0 kal        (501) staff       (20)      446 2024-05-13 17:40:07.000000 lptlib-0.0.1a2/test/test_import.py
--rwx------   0 kal        (501) staff       (20)     2350 2024-05-13 17:40:07.000000 lptlib-0.0.1a2/test/test_integration.py
--rw-r--r--   0 kal        (501) staff       (20)     2016 2024-05-13 17:40:07.000000 lptlib-0.0.1a2/test/test_interpolation.py
--rwx------   0 kal        (501) staff       (20)     1148 2024-05-13 17:40:08.000000 lptlib-0.0.1a2/test/test_oblique_shock_data.py
--rw-r--r--   0 kal        (501) staff       (20)     2059 2023-08-17 08:22:42.000000 lptlib-0.0.1a2/test/test_plot.py
--rw-r--r--   0 kal        (501) staff       (20)     7324 2024-05-13 17:40:08.000000 lptlib-0.0.1a2/test/test_plot3dio.py
--rwx------   0 kal        (501) staff       (20)     2607 2024-05-13 17:40:08.000000 lptlib-0.0.1a2/test/test_plots.py
--rw-r--r--   0 kal        (501) staff       (20)     3260 2024-05-13 17:40:07.000000 lptlib-0.0.1a2/test/test_search.py
--rw-r--r--   0 kal        (501) staff       (20)     1914 2024-05-13 17:40:07.000000 lptlib-0.0.1a2/test/test_stochastic_model.py
--rw-r--r--   0 kal        (501) staff       (20)     1399 2024-05-13 17:40:07.000000 lptlib-0.0.1a2/test/test_terminal_run.py
--rwx------   0 kal        (501) staff       (20)     2696 2024-05-13 17:40:07.000000 lptlib-0.0.1a2/test/test_variables.py
+drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 17:51:53.774287 lptlib-0.0.1a3/
+-rwx------   0 kal        (501) staff       (20)     1093 2024-05-10 20:01:36.000000 lptlib-0.0.1a3/LICENSE
+-rw-r--r--   0 kal        (501) staff       (20)     1545 2024-05-13 17:51:53.773424 lptlib-0.0.1a3/PKG-INFO
+-rw-r--r--   0 kal        (501) staff       (20)      579 2024-05-13 17:06:24.000000 lptlib-0.0.1a3/README.md
+-rw-r--r--   0 kal        (501) staff       (20)     1085 2024-05-13 17:51:47.000000 lptlib-0.0.1a3/pyproject.toml
+-rw-r--r--   0 kal        (501) staff       (20)       38 2024-05-13 17:51:53.774507 lptlib-0.0.1a3/setup.cfg
+drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 17:51:53.744452 lptlib-0.0.1a3/src/
+-rw-r--r--   0 kal        (501) staff       (20)       22 2024-05-13 17:51:47.000000 lptlib-0.0.1a3/src/__init__.py
+drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 17:51:53.745011 lptlib-0.0.1a3/src/lptlib/
+-rw-r--r--   0 kal        (501) staff       (20)      122 2024-05-13 17:40:07.000000 lptlib-0.0.1a3/src/lptlib/__init__.py
+drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 17:51:53.750343 lptlib-0.0.1a3/src/lptlib/function/
+-rw-r--r--   0 kal        (501) staff       (20)      109 2024-01-23 01:40:32.000000 lptlib-0.0.1a3/src/lptlib/function/__init__.py
+-rwx------   0 kal        (501) staff       (20)    12631 2024-05-13 17:51:47.000000 lptlib-0.0.1a3/src/lptlib/function/plots.py
+-rw-r--r--   0 kal        (501) staff       (20)     2034 2024-01-23 01:40:32.000000 lptlib-0.0.1a3/src/lptlib/function/timer.py
+-rw-r--r--   0 kal        (501) staff       (20)    11932 2024-05-13 17:24:06.000000 lptlib-0.0.1a3/src/lptlib/function/variables.py
+drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 17:51:53.753336 lptlib-0.0.1a3/src/lptlib/io/
+-rw-r--r--   0 kal        (501) staff       (20)       91 2024-01-23 01:40:32.000000 lptlib-0.0.1a3/src/lptlib/io/__init__.py
+-rw-r--r--   0 kal        (501) staff       (20)    14895 2024-05-13 17:51:47.000000 lptlib-0.0.1a3/src/lptlib/io/dataio.py
+-rw-r--r--   0 kal        (501) staff       (20)    24440 2024-04-22 21:46:04.000000 lptlib-0.0.1a3/src/lptlib/io/plot3dio.py
+drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 17:51:53.759254 lptlib-0.0.1a3/src/lptlib/streamlines/
+-rw-r--r--   0 kal        (501) staff       (20)      257 2024-01-23 01:40:32.000000 lptlib-0.0.1a3/src/lptlib/streamlines/__init__.py
+-rw-r--r--   0 kal        (501) staff       (20)    34496 2024-05-13 17:51:47.000000 lptlib-0.0.1a3/src/lptlib/streamlines/integration.py
+-rw-r--r--   0 kal        (501) staff       (20)    47345 2024-05-13 17:24:06.000000 lptlib-0.0.1a3/src/lptlib/streamlines/interpolation.py
+-rwxr-xr-x   0 kal        (501) staff       (20)    15615 2024-05-13 17:24:06.000000 lptlib-0.0.1a3/src/lptlib/streamlines/search.py
+-rw-r--r--   0 kal        (501) staff       (20)     7546 2024-05-13 17:51:47.000000 lptlib-0.0.1a3/src/lptlib/streamlines/stochastic_model.py
+-rw-r--r--   0 kal        (501) staff       (20)    39790 2024-05-13 17:51:47.000000 lptlib-0.0.1a3/src/lptlib/streamlines/streamlines.py
+drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 17:51:53.760745 lptlib-0.0.1a3/src/lptlib/test_cases/
+-rwx------   0 kal        (501) staff       (20)       89 2024-01-23 01:40:32.000000 lptlib-0.0.1a3/src/lptlib/test_cases/__init__.py
+-rwx------   0 kal        (501) staff       (20)    10018 2024-05-13 17:51:47.000000 lptlib-0.0.1a3/src/lptlib/test_cases/oblique_shock_data.py
+drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 17:51:53.772575 lptlib-0.0.1a3/src/lptlib.egg-info/
+-rw-r--r--   0 kal        (501) staff       (20)     1545 2024-05-13 17:51:53.000000 lptlib-0.0.1a3/src/lptlib.egg-info/PKG-INFO
+-rw-r--r--   0 kal        (501) staff       (20)     1026 2024-05-13 17:51:53.000000 lptlib-0.0.1a3/src/lptlib.egg-info/SOURCES.txt
+-rw-r--r--   0 kal        (501) staff       (20)        1 2024-05-13 17:51:53.000000 lptlib-0.0.1a3/src/lptlib.egg-info/dependency_links.txt
+-rw-r--r--   0 kal        (501) staff       (20)       43 2024-05-13 17:51:53.000000 lptlib-0.0.1a3/src/lptlib.egg-info/requires.txt
+-rw-r--r--   0 kal        (501) staff       (20)       16 2024-05-13 17:51:53.000000 lptlib-0.0.1a3/src/lptlib.egg-info/top_level.txt
+drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-13 17:51:53.771639 lptlib-0.0.1a3/test/
+-rw-r--r--   0 kal        (501) staff       (20)     1011 2024-05-13 17:51:47.000000 lptlib-0.0.1a3/test/test_dataio.py
+-rwx------   0 kal        (501) staff       (20)      468 2024-05-13 17:51:47.000000 lptlib-0.0.1a3/test/test_import.py
+-rwx------   0 kal        (501) staff       (20)     2350 2024-05-13 17:40:07.000000 lptlib-0.0.1a3/test/test_integration.py
+-rw-r--r--   0 kal        (501) staff       (20)     2016 2024-05-13 17:40:07.000000 lptlib-0.0.1a3/test/test_interpolation.py
+-rwx------   0 kal        (501) staff       (20)     1148 2024-05-13 17:40:08.000000 lptlib-0.0.1a3/test/test_oblique_shock_data.py
+-rw-r--r--   0 kal        (501) staff       (20)     2059 2023-08-17 08:22:42.000000 lptlib-0.0.1a3/test/test_plot.py
+-rw-r--r--   0 kal        (501) staff       (20)     7324 2024-05-13 17:40:08.000000 lptlib-0.0.1a3/test/test_plot3dio.py
+-rwx------   0 kal        (501) staff       (20)     2607 2024-05-13 17:40:08.000000 lptlib-0.0.1a3/test/test_plots.py
+-rw-r--r--   0 kal        (501) staff       (20)     3260 2024-05-13 17:40:07.000000 lptlib-0.0.1a3/test/test_search.py
+-rw-r--r--   0 kal        (501) staff       (20)     1914 2024-05-13 17:40:07.000000 lptlib-0.0.1a3/test/test_stochastic_model.py
+-rw-r--r--   0 kal        (501) staff       (20)     1399 2024-05-13 17:40:07.000000 lptlib-0.0.1a3/test/test_terminal_run.py
+-rwx------   0 kal        (501) staff       (20)     2696 2024-05-13 17:40:07.000000 lptlib-0.0.1a3/test/test_variables.py
```

### Comparing `lptlib-0.0.1a2/LICENSE` & `lptlib-0.0.1a3/LICENSE`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a2/PKG-INFO` & `lptlib-0.0.1a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lptlib
-Version: 0.0.1a2
+Version: 0.0.1a3
 Summary: One-way coupled Lagrangian Particle Tracking algorithms.
 Author: Dilip Kalagotla
 Author-email: dilipkalagotla@gmail.com
 Project-URL: homepage, https://github.com/kalagotla/project-arrakis
 Project-URL: issues, https://github.com/kalagotla/project-arrakis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `lptlib-0.0.1a2/README.md` & `lptlib-0.0.1a3/README.md`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a2/pyproject.toml` & `lptlib-0.0.1a3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lptlib"
-version = "0.0.1a2"
+version = "0.0.1a3"
 authors = [
     {name="Dilip Kalagotla"},
     {email="dilipkalagotla@gmail.com"},
     ]
 description = "One-way coupled Lagrangian Particle Tracking algorithms."
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `lptlib-0.0.1a2/src/lptlib/function/plots.py` & `lptlib-0.0.1a3/src/lptlib/function/plots.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 import matplotlib.pyplot as plt
 import matplotlib.colors as colors
 import matplotlib.patches as patches
 import matplotlib.gridspec as gridspec
 import seaborn as sns
 import re
 import pandas as pd
-from src.streamlines import Search, Interpolation
-from src.function import Variables
+from src.lptlib import Search, Interpolation
+from src.lptlib import Variables
 
 
 class Plots:
     """
     Module to plot data
     """
     def __init__(self, file, grid=None, flow=None):
```

### Comparing `lptlib-0.0.1a2/src/lptlib/function/timer.py` & `lptlib-0.0.1a3/src/lptlib/function/timer.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a2/src/lptlib/function/variables.py` & `lptlib-0.0.1a3/src/lptlib/function/variables.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a2/src/lptlib/io/dataio.py` & `lptlib-0.0.1a3/src/lptlib/io/dataio.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # This file contains DataIO class to read and write particle data
 
 import numpy as np
-from src.streamlines.search import Search
-from src.streamlines.interpolation import Interpolation
+from src.lptlib.streamlines.search import Search
+from src.lptlib.streamlines.interpolation import Interpolation
 from multiprocessing import Pool
 import multiprocessing as mp
 from scipy.interpolate import griddata
 import os
 import re
 from tqdm import tqdm
 rng = np.random.default_rng()
```

### Comparing `lptlib-0.0.1a2/src/lptlib/io/plot3dio.py` & `lptlib-0.0.1a3/src/lptlib/io/plot3dio.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a2/src/lptlib/streamlines/integration.py` & `lptlib-0.0.1a3/src/lptlib/streamlines/integration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Integrate from given point to produce streamlines
 import numpy as np
-from src.streamlines.interpolation import Interpolation
-from src.streamlines.search import Search
-from src.function.variables import Variables
+from src.lptlib.streamlines.interpolation import Interpolation
+from src.lptlib.streamlines.search import Search
+from src.lptlib.function.variables import Variables
 from scipy.optimize import fsolve
 
 
 class Integration:
 
     def __init__(self, interp):
         self.interp = interp
```

### Comparing `lptlib-0.0.1a2/src/lptlib/streamlines/interpolation.py` & `lptlib-0.0.1a3/src/lptlib/streamlines/interpolation.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a2/src/lptlib/streamlines/search.py` & `lptlib-0.0.1a3/src/lptlib/streamlines/search.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a2/src/lptlib/streamlines/stochastic_model.py` & `lptlib-0.0.1a3/src/lptlib/streamlines/stochastic_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Class to run streamlines script in parallel
 # Stochastic model for tracers is implemented
 
 import numpy as np
 from multiprocessing.pool import ThreadPool as Pool
 import multiprocessing as mp
-from src.streamlines.streamlines import Streamlines
+from src.lptlib.streamlines.streamlines import Streamlines
 from scipy.stats import skewnorm, lognorm
 from tqdm import tqdm
 
 rng = np.random.default_rng(7)
 
 
 class StochasticModel(Streamlines):
```

### Comparing `lptlib-0.0.1a2/src/lptlib/streamlines/streamlines.py` & `lptlib-0.0.1a3/src/lptlib/streamlines/streamlines.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # Uses the program API to extract streamlines
 import numpy as np
-from src.function.timer import Timer
-from src.io.plot3dio import GridIO
-from src.io.plot3dio import FlowIO
-from src.streamlines.search import Search
-from src.streamlines.interpolation import Interpolation
-from src.streamlines.integration import Integration
-from src.function.variables import Variables
+from src.lptlib.function.timer import Timer
+from src.lptlib.io.plot3dio import GridIO
+from src.lptlib.io.plot3dio import FlowIO
+from src.lptlib.streamlines.search import Search
+from src.lptlib.streamlines.interpolation import Interpolation
+from src.lptlib.streamlines.integration import Integration
+from src.lptlib.function.variables import Variables
 import matplotlib.pyplot as plt
 import functools
 
 
 class Streamlines:
     """
     Module to extract particle path information
```

### Comparing `lptlib-0.0.1a2/src/lptlib/test_cases/oblique_shock_data.py` & `lptlib-0.0.1a3/src/lptlib/test_cases/oblique_shock_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Class to calculate particle response across an oblique shock
 
 import numpy as np
 from scipy.optimize import newton
-from src.streamlines.stochastic_model import StochasticModel, Particle, SpawnLocations
+from src.lptlib.streamlines.stochastic_model import StochasticModel, Particle, SpawnLocations
 import matplotlib.pyplot as plt
 import os
 import glob
 
 
 # Create a class to calculate oblique shock properties from given mach and deflection angle
 class ObliqueShock:
```

### Comparing `lptlib-0.0.1a2/src/lptlib.egg-info/PKG-INFO` & `lptlib-0.0.1a3/src/lptlib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lptlib
-Version: 0.0.1a2
+Version: 0.0.1a3
 Summary: One-way coupled Lagrangian Particle Tracking algorithms.
 Author: Dilip Kalagotla
 Author-email: dilipkalagotla@gmail.com
 Project-URL: homepage, https://github.com/kalagotla/project-arrakis
 Project-URL: issues, https://github.com/kalagotla/project-arrakis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `lptlib-0.0.1a2/src/lptlib.egg-info/SOURCES.txt` & `lptlib-0.0.1a3/src/lptlib.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 README.md
 pyproject.toml
+src/__init__.py
 src/lptlib/__init__.py
 src/lptlib.egg-info/PKG-INFO
 src/lptlib.egg-info/SOURCES.txt
 src/lptlib.egg-info/dependency_links.txt
 src/lptlib.egg-info/requires.txt
 src/lptlib.egg-info/top_level.txt
 src/lptlib/function/__init__.py
```

### Comparing `lptlib-0.0.1a2/test/test_dataio.py` & `lptlib-0.0.1a3/test/test_dataio.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import unittest
 
 
 class TestDataIO(unittest.TestCase):
     def test_dataio(self):
-        from src import DataIO
-        from src import GridIO, FlowIO
+        from src.lptlib import DataIO
+        from src.lptlib import GridIO, FlowIO
         # grid object
         grid = GridIO('../data/shocks/shock_test.sb.sp.x')
         grid.read_grid()
         grid.compute_metrics()
 
         # flow object
         flow = FlowIO('../data/shocks/shock_test.sb.sp.q')
```

### Comparing `lptlib-0.0.1a2/test/test_integration.py` & `lptlib-0.0.1a3/test/test_integration.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a2/test/test_interpolation.py` & `lptlib-0.0.1a3/test/test_interpolation.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a2/test/test_oblique_shock_data.py` & `lptlib-0.0.1a3/test/test_oblique_shock_data.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a2/test/test_plot.py` & `lptlib-0.0.1a3/test/test_plot.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a2/test/test_plot3dio.py` & `lptlib-0.0.1a3/test/test_plot3dio.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a2/test/test_plots.py` & `lptlib-0.0.1a3/test/test_plots.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a2/test/test_search.py` & `lptlib-0.0.1a3/test/test_search.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a2/test/test_stochastic_model.py` & `lptlib-0.0.1a3/test/test_stochastic_model.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a2/test/test_terminal_run.py` & `lptlib-0.0.1a3/test/test_terminal_run.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a2/test/test_variables.py` & `lptlib-0.0.1a3/test/test_variables.py`

 * *Files identical despite different names*

