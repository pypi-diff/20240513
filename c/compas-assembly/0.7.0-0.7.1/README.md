# Comparing `tmp/compas_assembly-0.7.0.tar.gz` & `tmp/compas_assembly-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compas_assembly-0.7.0.tar", last modified: Fri Mar  1 22:23:41 2024, max compression
+gzip compressed data, was "compas_assembly-0.7.1.tar", last modified: Mon May 13 21:29:37 2024, max compression
```

## Comparing `compas_assembly-0.7.0.tar` & `compas_assembly-0.7.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 22:23:41.490677 compas_assembly-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-03-01 22:23:28.000000 compas_assembly-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-03-01 22:23:41.490677 compas_assembly-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-03-01 22:23:28.000000 compas_assembly-0.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3482 2024-03-01 22:23:28.000000 compas_assembly-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-01 22:23:28.000000 compas_assembly-0.7.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-01 22:23:28.000000 compas_assembly-0.7.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-01 22:23:41.490677 compas_assembly-0.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 22:23:41.482677 compas_assembly-0.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 22:23:41.486677 compas_assembly-0.7.0/src/compas_assembly/
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-03-01 22:23:28.000000 compas_assembly-0.7.0/src/compas_assembly/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 22:23:41.486677 compas_assembly-0.7.0/src/compas_assembly/algorithms/
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-03-01 22:23:28.000000 compas_assembly-0.7.0/src/compas_assembly/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-03-01 22:23:28.000000 compas_assembly-0.7.0/src/compas_assembly/algorithms/hull.py
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-03-01 22:23:28.000000 compas_assembly-0.7.0/src/compas_assembly/algorithms/hull_numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     7081 2024-03-01 22:23:28.000000 compas_assembly-0.7.0/src/compas_assembly/algorithms/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     4523 2024-03-01 22:23:28.000000 compas_assembly-0.7.0/src/compas_assembly/algorithms/interfaces_numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-03-01 22:23:28.000000 compas_assembly-0.7.0/src/compas_assembly/algorithms/nnbrs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 22:23:41.486677 compas_assembly-0.7.0/src/compas_assembly/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 22:23:28.000000 compas_assembly-0.7.0/src/compas_assembly/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 22:23:41.490677 compas_assembly-0.7.0/src/compas_assembly/datastructures/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-03-01 22:23:28.000000 compas_assembly-0.7.0/src/compas_assembly/datastructures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16275 2024-03-01 22:23:28.000000 compas_assembly-0.7.0/src/compas_assembly/datastructures/assembly.py
--rw-r--r--   0 runner    (1001) docker     (127)     4791 2024-03-01 22:23:28.000000 compas_assembly-0.7.0/src/compas_assembly/datastructures/block.py
--rw-r--r--   0 runner    (1001) docker     (127)     9810 2024-03-01 22:23:28.000000 compas_assembly-0.7.0/src/compas_assembly/datastructures/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 22:23:41.490677 compas_assembly-0.7.0/src/compas_assembly/geometry/
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-03-01 22:23:28.000000 compas_assembly-0.7.0/src/compas_assembly/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-03-01 22:23:28.000000 compas_assembly-0.7.0/src/compas_assembly/geometry/_geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-03-01 22:23:28.000000 compas_assembly-0.7.0/src/compas_assembly/geometry/arch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-03-01 22:23:28.000000 compas_assembly-0.7.0/src/compas_assembly/geometry/dome.py
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-03-01 22:23:28.000000 compas_assembly-0.7.0/src/compas_assembly/geometry/wall.py
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-01 22:23:28.000000 compas_assembly-0.7.0/src/compas_assembly/install.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 22:23:41.490677 compas_assembly-0.7.0/src/compas_assembly/rhino/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 22:23:28.000000 compas_assembly-0.7.0/src/compas_assembly/rhino/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-01 22:23:28.000000 compas_assembly-0.7.0/src/compas_assembly/rhino/install.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 22:23:41.490677 compas_assembly-0.7.0/src/compas_assembly/viewer/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-01 22:23:28.000000 compas_assembly-0.7.0/src/compas_assembly/viewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9369 2024-03-01 22:23:28.000000 compas_assembly-0.7.0/src/compas_assembly/viewer/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 22:23:41.490677 compas_assembly-0.7.0/src/compas_assembly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-03-01 22:23:41.000000 compas_assembly-0.7.0/src/compas_assembly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-03-01 22:23:41.000000 compas_assembly-0.7.0/src/compas_assembly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 22:23:41.000000 compas_assembly-0.7.0/src/compas_assembly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 22:23:41.000000 compas_assembly-0.7.0/src/compas_assembly.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-03-01 22:23:41.000000 compas_assembly-0.7.0/src/compas_assembly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-01 22:23:41.000000 compas_assembly-0.7.0/src/compas_assembly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 22:23:41.490677 compas_assembly-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-01 22:23:28.000000 compas_assembly-0.7.0/tests/test_placeholder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:29:37.087358 compas_assembly-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-13 21:29:26.000000 compas_assembly-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-05-13 21:29:37.087358 compas_assembly-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-13 21:29:26.000000 compas_assembly-0.7.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-05-13 21:29:26.000000 compas_assembly-0.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-13 21:29:26.000000 compas_assembly-0.7.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-13 21:29:26.000000 compas_assembly-0.7.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 21:29:37.087358 compas_assembly-0.7.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:29:37.079358 compas_assembly-0.7.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:29:37.083358 compas_assembly-0.7.1/src/compas_assembly/
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-13 21:29:26.000000 compas_assembly-0.7.1/src/compas_assembly/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:29:37.083358 compas_assembly-0.7.1/src/compas_assembly/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-13 21:29:26.000000 compas_assembly-0.7.1/src/compas_assembly/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-13 21:29:26.000000 compas_assembly-0.7.1/src/compas_assembly/algorithms/hull.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-13 21:29:26.000000 compas_assembly-0.7.1/src/compas_assembly/algorithms/hull_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7081 2024-05-13 21:29:26.000000 compas_assembly-0.7.1/src/compas_assembly/algorithms/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4523 2024-05-13 21:29:26.000000 compas_assembly-0.7.1/src/compas_assembly/algorithms/interfaces_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-13 21:29:26.000000 compas_assembly-0.7.1/src/compas_assembly/algorithms/nnbrs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:29:37.083358 compas_assembly-0.7.1/src/compas_assembly/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 21:29:26.000000 compas_assembly-0.7.1/src/compas_assembly/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:29:37.083358 compas_assembly-0.7.1/src/compas_assembly/datastructures/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-13 21:29:26.000000 compas_assembly-0.7.1/src/compas_assembly/datastructures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16275 2024-05-13 21:29:26.000000 compas_assembly-0.7.1/src/compas_assembly/datastructures/assembly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4791 2024-05-13 21:29:26.000000 compas_assembly-0.7.1/src/compas_assembly/datastructures/block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9810 2024-05-13 21:29:26.000000 compas_assembly-0.7.1/src/compas_assembly/datastructures/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:29:37.087358 compas_assembly-0.7.1/src/compas_assembly/geometry/
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-13 21:29:26.000000 compas_assembly-0.7.1/src/compas_assembly/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-13 21:29:26.000000 compas_assembly-0.7.1/src/compas_assembly/geometry/_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-13 21:29:26.000000 compas_assembly-0.7.1/src/compas_assembly/geometry/arch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-05-13 21:29:26.000000 compas_assembly-0.7.1/src/compas_assembly/geometry/dome.py
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-13 21:29:26.000000 compas_assembly-0.7.1/src/compas_assembly/geometry/wall.py
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-13 21:29:26.000000 compas_assembly-0.7.1/src/compas_assembly/install.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:29:37.087358 compas_assembly-0.7.1/src/compas_assembly/rhino/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 21:29:26.000000 compas_assembly-0.7.1/src/compas_assembly/rhino/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-13 21:29:26.000000 compas_assembly-0.7.1/src/compas_assembly/rhino/install.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:29:37.087358 compas_assembly-0.7.1/src/compas_assembly/viewer/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-13 21:29:26.000000 compas_assembly-0.7.1/src/compas_assembly/viewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9369 2024-05-13 21:29:26.000000 compas_assembly-0.7.1/src/compas_assembly/viewer/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:29:37.087358 compas_assembly-0.7.1/src/compas_assembly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-05-13 21:29:37.000000 compas_assembly-0.7.1/src/compas_assembly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-13 21:29:37.000000 compas_assembly-0.7.1/src/compas_assembly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 21:29:37.000000 compas_assembly-0.7.1/src/compas_assembly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 21:29:36.000000 compas_assembly-0.7.1/src/compas_assembly.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-13 21:29:37.000000 compas_assembly-0.7.1/src/compas_assembly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-13 21:29:37.000000 compas_assembly-0.7.1/src/compas_assembly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:29:37.087358 compas_assembly-0.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-13 21:29:26.000000 compas_assembly-0.7.1/tests/test_placeholder.py
```

### Comparing `compas_assembly-0.7.0/LICENSE` & `compas_assembly-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `compas_assembly-0.7.0/PKG-INFO` & `compas_assembly-0.7.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compas_assembly
-Version: 0.7.0
+Version: 0.7.1
 Author-email: tom van mele <tom.v.mele@gmail.com>
 License: MIT License
         
         Copyright (c) 2018-2021 Block Research Group - ETH Zurich
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -31,25 +31,27 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Scientific/Engineering
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: compas>=2.0
 Requires-Dist: shapely
 Provides-Extra: dev
 Requires-Dist: attrs>=17.4; extra == "dev"
 Requires-Dist: black>=22.12.0; extra == "dev"
 Requires-Dist: bump-my-version; extra == "dev"
 Requires-Dist: compas_invocations2; extra == "dev"
 Requires-Dist: compas_notebook; extra == "dev"
+Requires-Dist: compas_viewer; extra == "dev"
 Requires-Dist: invoke>=0.14; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: sphinx_compas2_theme; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: wheel; extra == "dev"
 
 # COMPAS Assembly
```

### Comparing `compas_assembly-0.7.0/README.md` & `compas_assembly-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `compas_assembly-0.7.0/pyproject.toml` & `compas_assembly-0.7.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     "Development Status :: 4 - Beta",
     "Topic :: Scientific/Engineering",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
 ]
 
 [project.urls]
 Homepage = "https://blockresearchgroup.github.io/compas_assembly"
 Documentation = "https://blockresearchgroup.github.io/compas_assembly"
 Repository = "https://github.com/blockresearchgroup/compas_assembly.git"
 Changelog = "https://github.com/blockresearchgroup/compas_assembly/blob/main/CHANGELOG.md"
@@ -66,15 +67,15 @@
 ]
 
 # ============================================================================
 # replace bumpversion.cfg
 # ============================================================================
 
 [tool.bumpversion]
-current_version = "0.7.0"
+current_version = "0.7.1"
 message = "Bump version to {new_version}"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "src/compas_assembly/__init__.py"
 search = "{current_version}"
@@ -86,18 +87,18 @@
 replace = "[{new_version}] {now:%Y-%m-%d}"
 
 # ============================================================================
 # replace setup.cfg
 # ============================================================================
 
 [tool.black]
-line-length = 119
+line-length = 179
 
 [tool.ruff]
-line-length = 119
+line-length = 179
 indent-width = 4
 target-version = "py39"
 
 [tool.ruff.lint]
 select = ["E", "F", "I"]
 
 [tool.ruff.lint.per-file-ignores]
```

### Comparing `compas_assembly-0.7.0/src/compas_assembly/__init__.py` & `compas_assembly-0.7.1/src/compas_assembly/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import os
 
 __author__ = ["Tom Van Mele"]
 __copyright__ = "ETH Zurich - Block Research Group"
 __license__ = "MIT License"
 __email__ = "tom.v.mele@gmail.com"
-__version__ = "0.7.0"
+__version__ = "0.7.1"
 
 
 HERE = os.path.dirname(__file__)
 HOME = os.path.abspath(os.path.join(HERE, "../../"))
 DATA = os.path.abspath(os.path.join(HOME, "data"))
 TEMP = os.path.abspath(os.path.join(HERE, "__temp"))
 SAMPLES = os.path.abspath(os.path.join(HERE, "data/samples"))
```

### Comparing `compas_assembly-0.7.0/src/compas_assembly/algorithms/__init__.py` & `compas_assembly-0.7.1/src/compas_assembly/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `compas_assembly-0.7.0/src/compas_assembly/algorithms/hull.py` & `compas_assembly-0.7.1/src/compas_assembly/algorithms/hull.py`

 * *Files identical despite different names*

### Comparing `compas_assembly-0.7.0/src/compas_assembly/algorithms/hull_numpy.py` & `compas_assembly-0.7.1/src/compas_assembly/algorithms/hull_numpy.py`

 * *Files identical despite different names*

### Comparing `compas_assembly-0.7.0/src/compas_assembly/algorithms/interfaces.py` & `compas_assembly-0.7.1/src/compas_assembly/algorithms/interfaces.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from compas.geometry import Plane
 from compas.geometry import Polygon
 from compas.geometry import Transformation
 from compas.geometry import centroid_polygon
 from compas.geometry import is_colinear
 from compas.geometry import is_coplanar
 from compas.geometry import transform_points
-from compas.utilities import window
+from compas.itertools import window
 from compas_assembly.algorithms.nnbrs import find_nearest_neighbours
 from compas_assembly.datastructures import Assembly
 from compas_assembly.datastructures import Block
 from compas_assembly.datastructures import Interface
 
 
 def assembly_interfaces(
```

### Comparing `compas_assembly-0.7.0/src/compas_assembly/algorithms/interfaces_numpy.py` & `compas_assembly-0.7.1/src/compas_assembly/algorithms/interfaces_numpy.py`

 * *Files identical despite different names*

### Comparing `compas_assembly-0.7.0/src/compas_assembly/datastructures/assembly.py` & `compas_assembly-0.7.1/src/compas_assembly/datastructures/assembly.py`

 * *Files identical despite different names*

### Comparing `compas_assembly-0.7.0/src/compas_assembly/datastructures/block.py` & `compas_assembly-0.7.1/src/compas_assembly/datastructures/block.py`

 * *Files identical despite different names*

### Comparing `compas_assembly-0.7.0/src/compas_assembly/datastructures/interface.py` & `compas_assembly-0.7.1/src/compas_assembly/datastructures/interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from compas.geometry import Line
 from compas.geometry import Point
 from compas.geometry import Polygon
 from compas.geometry import Transformation
 from compas.geometry import centroid_points_weighted
 from compas.geometry import dot_vectors
 from compas.geometry import transform_points
-from compas.utilities import pairwise
+from compas.itertools import pairwise
 
 
 def outer_product(u, v):
     return [[ui * vi for vi in v] for ui in u]
 
 
 def scale_matrix(M, scale):
```

### Comparing `compas_assembly-0.7.0/src/compas_assembly/geometry/_geometry.py` & `compas_assembly-0.7.1/src/compas_assembly/geometry/_geometry.py`

 * *Files identical despite different names*

### Comparing `compas_assembly-0.7.0/src/compas_assembly/geometry/arch.py` & `compas_assembly-0.7.1/src/compas_assembly/geometry/arch.py`

 * *Files identical despite different names*

### Comparing `compas_assembly-0.7.0/src/compas_assembly/geometry/dome.py` & `compas_assembly-0.7.1/src/compas_assembly/geometry/dome.py`

 * *Files identical despite different names*

### Comparing `compas_assembly-0.7.0/src/compas_assembly/geometry/wall.py` & `compas_assembly-0.7.1/src/compas_assembly/geometry/wall.py`

 * *Files identical despite different names*

### Comparing `compas_assembly-0.7.0/src/compas_assembly/viewer/app.py` & `compas_assembly-0.7.1/src/compas_assembly/viewer/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from compas_view2.app import App
 from compas_view2.app import Controller
 from compas_view2.objects import Collection
 from qt_material import apply_stylesheet
 
 from compas.colors import Color
 from compas.geometry import Line
-from compas.utilities import remap_values
+from compas.itertools import remap_values
 from compas_assembly.datastructures import Interface
 
 HERE = os.path.dirname(__file__)
 CONFIG = os.path.join(HERE, "config.json")
 
 
 class DEMController(Controller):
```

### Comparing `compas_assembly-0.7.0/src/compas_assembly.egg-info/PKG-INFO` & `compas_assembly-0.7.1/src/compas_assembly.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compas_assembly
-Version: 0.7.0
+Version: 0.7.1
 Author-email: tom van mele <tom.v.mele@gmail.com>
 License: MIT License
         
         Copyright (c) 2018-2021 Block Research Group - ETH Zurich
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -31,25 +31,27 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Scientific/Engineering
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: compas>=2.0
 Requires-Dist: shapely
 Provides-Extra: dev
 Requires-Dist: attrs>=17.4; extra == "dev"
 Requires-Dist: black>=22.12.0; extra == "dev"
 Requires-Dist: bump-my-version; extra == "dev"
 Requires-Dist: compas_invocations2; extra == "dev"
 Requires-Dist: compas_notebook; extra == "dev"
+Requires-Dist: compas_viewer; extra == "dev"
 Requires-Dist: invoke>=0.14; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: sphinx_compas2_theme; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: wheel; extra == "dev"
 
 # COMPAS Assembly
```

### Comparing `compas_assembly-0.7.0/src/compas_assembly.egg-info/SOURCES.txt` & `compas_assembly-0.7.1/src/compas_assembly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

