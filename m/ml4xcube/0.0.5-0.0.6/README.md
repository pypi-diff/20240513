# Comparing `tmp/ml4xcube-0.0.5.tar.gz` & `tmp/ml4xcube-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml4xcube-0.0.5.tar", last modified: Thu May  2 23:57:16 2024, max compression
+gzip compressed data, was "ml4xcube-0.0.6.tar", last modified: Mon May 13 13:52:08 2024, max compression
```

## Comparing `ml4xcube-0.0.5.tar` & `ml4xcube-0.0.6.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 julia     (1000) julia     (1000)        0 2024-05-02 23:57:16.827259 ml4xcube-0.0.5/
--rw-rw-r--   0 julia     (1000) julia     (1000)     1113 2024-04-23 08:43:03.000000 ml4xcube-0.0.5/LICENSE
--rw-rw-r--   0 julia     (1000) julia     (1000)       70 2024-05-02 18:14:05.000000 ml4xcube-0.0.5/MANIFEST.in
--rw-r--r--   0 julia     (1000) julia     (1000)     3690 2024-05-02 23:57:16.827259 ml4xcube-0.0.5/PKG-INFO
--rw-rw-r--   0 julia     (1000) julia     (1000)     1726 2024-05-02 19:14:55.000000 ml4xcube-0.0.5/README.md
-drwxrwxr-x   0 julia     (1000) julia     (1000)        0 2024-05-02 23:57:16.815259 ml4xcube-0.0.5/mltools/
-drwxrwxr-x   0 julia     (1000) julia     (1000)        0 2024-05-02 23:57:16.819259 ml4xcube-0.0.5/mltools/ml4xcube/
--rw-rw-r--   0 julia     (1000) julia     (1000)        0 2024-04-23 11:53:26.000000 ml4xcube-0.0.5/mltools/ml4xcube/__init__.py
--rw-rw-r--   0 julia     (1000) julia     (1000)     5544 2024-05-02 16:06:56.000000 ml4xcube-0.0.5/mltools/ml4xcube/cube_utilities.py
--rw-rw-r--   0 julia     (1000) julia     (1000)     2377 2024-05-02 23:27:38.000000 ml4xcube-0.0.5/mltools/ml4xcube/data_assignment.py
-drwxrwxr-x   0 julia     (1000) julia     (1000)        0 2024-05-02 23:57:16.819259 ml4xcube-0.0.5/mltools/ml4xcube/datasets/
--rw-rw-r--   0 julia     (1000) julia     (1000)        0 2024-05-02 10:14:25.000000 ml4xcube-0.0.5/mltools/ml4xcube/datasets/__init__.py
--rw-rw-r--   0 julia     (1000) julia     (1000)     2765 2024-05-02 16:06:56.000000 ml4xcube-0.0.5/mltools/ml4xcube/datasets/pytorch_xr.py
--rw-rw-r--   0 julia     (1000) julia     (1000)     3734 2024-05-02 23:38:35.000000 ml4xcube-0.0.5/mltools/ml4xcube/datasets/tensorflow_xr.py
--rw-rw-r--   0 julia     (1000) julia     (1000)     4242 2024-05-02 23:27:38.000000 ml4xcube-0.0.5/mltools/ml4xcube/datasets/xr_dataset.py
-drwxrwxr-x   0 julia     (1000) julia     (1000)        0 2024-05-02 23:57:16.819259 ml4xcube-0.0.5/mltools/ml4xcube/gapfilling/
--rw-rw-r--   0 julia     (1000) julia     (1000)        0 2024-05-01 15:35:17.000000 ml4xcube-0.0.5/mltools/ml4xcube/gapfilling/__init__.py
--rw-rw-r--   0 julia     (1000) julia     (1000)    14356 2024-05-02 16:06:56.000000 ml4xcube-0.0.5/mltools/ml4xcube/gapfilling/gap_dataset.py
--rw-rw-r--   0 julia     (1000) julia     (1000)    31651 2024-05-02 16:06:56.000000 ml4xcube-0.0.5/mltools/ml4xcube/gapfilling/gap_filling.py
-drwxrwxr-x   0 julia     (1000) julia     (1000)        0 2024-05-02 23:57:16.827259 ml4xcube-0.0.5/mltools/ml4xcube/gapfilling/helper/
--rw-rw-r--   0 julia     (1000) julia     (1000)        0 2024-05-01 15:36:00.000000 ml4xcube-0.0.5/mltools/ml4xcube/gapfilling/helper/__init__.py
--rw-rw-r--   0 julia     (1000) julia     (1000)  9401362 2024-04-23 11:53:26.000000 ml4xcube-0.0.5/mltools/ml4xcube/gapfilling/helper/global_lcc.nc
--rw-rw-r--   0 julia     (1000) julia     (1000)     4441 2024-05-01 14:21:50.000000 ml4xcube-0.0.5/mltools/ml4xcube/gapfilling/helper/lcc.py
--rw-rw-r--   0 julia     (1000) julia     (1000)     2365 2024-05-01 13:43:43.000000 ml4xcube-0.0.5/mltools/ml4xcube/geo_plots.py
--rw-rw-r--   0 julia     (1000) julia     (1000)      389 2024-05-01 13:43:43.000000 ml4xcube-0.0.5/mltools/ml4xcube/preprocessing.py
--rw-rw-r--   0 julia     (1000) julia     (1000)     1384 2024-05-01 14:33:44.000000 ml4xcube-0.0.5/mltools/ml4xcube/statistics.py
-drwxrwxr-x   0 julia     (1000) julia     (1000)        0 2024-05-02 23:57:16.827259 ml4xcube-0.0.5/mltools/ml4xcube/training/
--rw-rw-r--   0 julia     (1000) julia     (1000)        0 2024-05-01 15:23:29.000000 ml4xcube-0.0.5/mltools/ml4xcube/training/__init__.py
--rw-rw-r--   0 julia     (1000) julia     (1000)     4560 2024-05-01 13:43:43.000000 ml4xcube-0.0.5/mltools/ml4xcube/training/pytorch.py
--rw-rw-r--   0 julia     (1000) julia     (1000)     8840 2024-05-01 14:01:45.000000 ml4xcube-0.0.5/mltools/ml4xcube/training/pytorch_distributed.py
--rw-rw-r--   0 julia     (1000) julia     (1000)     3776 2024-05-02 11:04:54.000000 ml4xcube-0.0.5/mltools/ml4xcube/training/sklearn.py
--rw-rw-r--   0 julia     (1000) julia     (1000)     2946 2024-05-01 13:43:43.000000 ml4xcube-0.0.5/mltools/ml4xcube/training/tensorflow.py
-drwxrwxr-x   0 julia     (1000) julia     (1000)        0 2024-05-02 23:57:16.827259 ml4xcube-0.0.5/mltools/ml4xcube.egg-info/
--rw-r--r--   0 julia     (1000) julia     (1000)     3690 2024-05-02 23:57:16.000000 ml4xcube-0.0.5/mltools/ml4xcube.egg-info/PKG-INFO
--rw-rw-r--   0 julia     (1000) julia     (1000)     1085 2024-05-02 23:57:16.000000 ml4xcube-0.0.5/mltools/ml4xcube.egg-info/SOURCES.txt
--rw-rw-r--   0 julia     (1000) julia     (1000)        1 2024-05-02 23:57:16.000000 ml4xcube-0.0.5/mltools/ml4xcube.egg-info/dependency_links.txt
--rw-rw-r--   0 julia     (1000) julia     (1000)      163 2024-05-02 23:57:16.000000 ml4xcube-0.0.5/mltools/ml4xcube.egg-info/requires.txt
--rw-rw-r--   0 julia     (1000) julia     (1000)        9 2024-05-02 23:57:16.000000 ml4xcube-0.0.5/mltools/ml4xcube.egg-info/top_level.txt
--rw-rw-r--   0 julia     (1000) julia     (1000)      628 2024-05-02 23:54:56.000000 ml4xcube-0.0.5/pyproject.toml
--rw-rw-r--   0 julia     (1000) julia     (1000)       38 2024-05-02 23:57:16.827259 ml4xcube-0.0.5/setup.cfg
--rw-rw-r--   0 julia     (1000) julia     (1000)      619 2024-05-02 23:54:56.000000 ml4xcube-0.0.5/setup.py
+drwxrwxr-x   0 julia     (1000) julia     (1000)        0 2024-05-13 13:52:08.028173 ml4xcube-0.0.6/
+-rw-rw-r--   0 julia     (1000) julia     (1000)     1113 2024-04-23 08:43:03.000000 ml4xcube-0.0.6/LICENSE
+-rw-rw-r--   0 julia     (1000) julia     (1000)       70 2024-05-02 18:14:05.000000 ml4xcube-0.0.6/MANIFEST.in
+-rw-r--r--   0 julia     (1000) julia     (1000)     3904 2024-05-13 13:52:08.028173 ml4xcube-0.0.6/PKG-INFO
+-rw-rw-r--   0 julia     (1000) julia     (1000)     2007 2024-05-13 13:51:42.000000 ml4xcube-0.0.6/README.md
+drwxrwxr-x   0 julia     (1000) julia     (1000)        0 2024-05-13 13:52:08.020173 ml4xcube-0.0.6/mltools/
+drwxrwxr-x   0 julia     (1000) julia     (1000)        0 2024-05-13 13:52:08.020173 ml4xcube-0.0.6/mltools/ml4xcube/
+-rw-rw-r--   0 julia     (1000) julia     (1000)        0 2024-04-23 11:53:26.000000 ml4xcube-0.0.6/mltools/ml4xcube/__init__.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)     5544 2024-05-02 16:06:56.000000 ml4xcube-0.0.6/mltools/ml4xcube/cube_utilities.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)     2377 2024-05-02 23:27:38.000000 ml4xcube-0.0.6/mltools/ml4xcube/data_assignment.py
+drwxrwxr-x   0 julia     (1000) julia     (1000)        0 2024-05-13 13:52:08.020173 ml4xcube-0.0.6/mltools/ml4xcube/datasets/
+-rw-rw-r--   0 julia     (1000) julia     (1000)        0 2024-05-02 10:14:25.000000 ml4xcube-0.0.6/mltools/ml4xcube/datasets/__init__.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)     2765 2024-05-02 16:06:56.000000 ml4xcube-0.0.6/mltools/ml4xcube/datasets/pytorch_xr.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)     3734 2024-05-02 23:38:35.000000 ml4xcube-0.0.6/mltools/ml4xcube/datasets/tensorflow_xr.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)     4242 2024-05-02 23:27:38.000000 ml4xcube-0.0.6/mltools/ml4xcube/datasets/xr_dataset.py
+drwxrwxr-x   0 julia     (1000) julia     (1000)        0 2024-05-13 13:52:08.020173 ml4xcube-0.0.6/mltools/ml4xcube/gapfilling/
+-rw-rw-r--   0 julia     (1000) julia     (1000)        0 2024-05-01 15:35:17.000000 ml4xcube-0.0.6/mltools/ml4xcube/gapfilling/__init__.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)    14356 2024-05-02 16:06:56.000000 ml4xcube-0.0.6/mltools/ml4xcube/gapfilling/gap_dataset.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)    31651 2024-05-02 16:06:56.000000 ml4xcube-0.0.6/mltools/ml4xcube/gapfilling/gap_filling.py
+drwxrwxr-x   0 julia     (1000) julia     (1000)        0 2024-05-13 13:52:08.028173 ml4xcube-0.0.6/mltools/ml4xcube/gapfilling/helper/
+-rw-rw-r--   0 julia     (1000) julia     (1000)        0 2024-05-01 15:36:00.000000 ml4xcube-0.0.6/mltools/ml4xcube/gapfilling/helper/__init__.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)  9401362 2024-04-23 11:53:26.000000 ml4xcube-0.0.6/mltools/ml4xcube/gapfilling/helper/global_lcc.nc
+-rw-rw-r--   0 julia     (1000) julia     (1000)     4441 2024-05-01 14:21:50.000000 ml4xcube-0.0.6/mltools/ml4xcube/gapfilling/helper/lcc.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)     2365 2024-05-01 13:43:43.000000 ml4xcube-0.0.6/mltools/ml4xcube/geo_plots.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)      389 2024-05-01 13:43:43.000000 ml4xcube-0.0.6/mltools/ml4xcube/preprocessing.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)     1384 2024-05-01 14:33:44.000000 ml4xcube-0.0.6/mltools/ml4xcube/statistics.py
+drwxrwxr-x   0 julia     (1000) julia     (1000)        0 2024-05-13 13:52:08.028173 ml4xcube-0.0.6/mltools/ml4xcube/training/
+-rw-rw-r--   0 julia     (1000) julia     (1000)        0 2024-05-01 15:23:29.000000 ml4xcube-0.0.6/mltools/ml4xcube/training/__init__.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)     4560 2024-05-01 13:43:43.000000 ml4xcube-0.0.6/mltools/ml4xcube/training/pytorch.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)     8840 2024-05-01 14:01:45.000000 ml4xcube-0.0.6/mltools/ml4xcube/training/pytorch_distributed.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)     3776 2024-05-02 11:04:54.000000 ml4xcube-0.0.6/mltools/ml4xcube/training/sklearn.py
+-rw-rw-r--   0 julia     (1000) julia     (1000)     2946 2024-05-01 13:43:43.000000 ml4xcube-0.0.6/mltools/ml4xcube/training/tensorflow.py
+drwxrwxr-x   0 julia     (1000) julia     (1000)        0 2024-05-13 13:52:08.028173 ml4xcube-0.0.6/mltools/ml4xcube.egg-info/
+-rw-r--r--   0 julia     (1000) julia     (1000)     3904 2024-05-13 13:52:08.000000 ml4xcube-0.0.6/mltools/ml4xcube.egg-info/PKG-INFO
+-rw-rw-r--   0 julia     (1000) julia     (1000)     1085 2024-05-13 13:52:08.000000 ml4xcube-0.0.6/mltools/ml4xcube.egg-info/SOURCES.txt
+-rw-rw-r--   0 julia     (1000) julia     (1000)        1 2024-05-13 13:52:08.000000 ml4xcube-0.0.6/mltools/ml4xcube.egg-info/dependency_links.txt
+-rw-rw-r--   0 julia     (1000) julia     (1000)      126 2024-05-13 13:52:08.000000 ml4xcube-0.0.6/mltools/ml4xcube.egg-info/requires.txt
+-rw-rw-r--   0 julia     (1000) julia     (1000)        9 2024-05-13 13:52:08.000000 ml4xcube-0.0.6/mltools/ml4xcube.egg-info/top_level.txt
+-rw-rw-r--   0 julia     (1000) julia     (1000)      628 2024-05-13 13:00:46.000000 ml4xcube-0.0.6/pyproject.toml
+-rw-rw-r--   0 julia     (1000) julia     (1000)       38 2024-05-13 13:52:08.028173 ml4xcube-0.0.6/setup.cfg
+-rw-rw-r--   0 julia     (1000) julia     (1000)      558 2024-05-13 13:00:46.000000 ml4xcube-0.0.6/setup.py
```

### Comparing `ml4xcube-0.0.5/LICENSE` & `ml4xcube-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ml4xcube-0.0.5/PKG-INFO` & `ml4xcube-0.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml4xcube
-Version: 0.0.5
+Version: 0.0.6
 Summary: ML package for data cubes
 Author-email: Julia Peters <julia.peters@informatik.uni-leipzig.de>
 License: MIT License
         
         Copyright (c) 2022 by ScaDS.AI, the xcube development team and contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -28,34 +28,36 @@
 Keywords: machine learning,tools,data cube utilities
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: bokeh>=2.4.3
 Requires-Dist: dask>=2023.2.0
-Requires-Dist: jinja2==3.1.3
-Requires-Dist: mypy_extensions==1.0.0
 Requires-Dist: numpy>=1.24
 Requires-Dist: pandas>=2.2
 Requires-Dist: scikit-learn>1.3.1
 Requires-Dist: xarray>2023.8.0
 Requires-Dist: zarr>2.11
 Requires-Dist: rechunker>=0.5.1
 Requires-Dist: sentinelhub
 
-# ML-Toolkits
+# ml4xcube: Machine Learning Toolkits for Data Cubes
 
-The ML Toolkits provide a set of best practice Python-based Jupyter Notebooks that showcase the implementation of the three start-of-the-art Machine Learning libraries (1) scikit-learn, (2) PyTorch and (3) TensorFlow based on the Earth System Data Cube.
+Welcome to `ml4xcube`, a comprehensive Python-based toolkit designed for researchers and developers in the field of machine learning with an emphasis on `xarray` data cubes. Our toolkit is engineered to provide specialized and robust support for data cube management and analysis, operating with the state-of-the-art machine learning libraries (1) `scikit-learn`, (2) `PyTorch` and (3) `TensorFlow`. 
 
 ## Installation
 
-You can install `ml4xcube` directly via pip:
+Get started with `ml4xcube` effortlessly by installing it directly through pip:
 ```bash
 pip install ml4xcube
 ```
+or Conda:
+```bash
+conda install -c conda-forge ml4xcube
+```
 
 Make sure you have Python version 3.8 or higher.
 
 If you're planning to use `ml4xcube` with TensorFlow or PyTorch, set up these frameworks properly in your Conda environment. 
 
 ## Features
```

### Comparing `ml4xcube-0.0.5/README.md` & `ml4xcube-0.0.6/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,21 @@
-# ML-Toolkits
+# ml4xcube: Machine Learning Toolkits for Data Cubes
 
-The ML Toolkits provide a set of best practice Python-based Jupyter Notebooks that showcase the implementation of the three start-of-the-art Machine Learning libraries (1) scikit-learn, (2) PyTorch and (3) TensorFlow based on the Earth System Data Cube.
+Welcome to `ml4xcube`, a comprehensive Python-based toolkit designed for researchers and developers in the field of machine learning with an emphasis on `xarray` data cubes. Our toolkit is engineered to provide specialized and robust support for data cube management and analysis, operating with the state-of-the-art machine learning libraries (1) `scikit-learn`, (2) `PyTorch` and (3) `TensorFlow`. 
 
 ## Installation
 
-You can install `ml4xcube` directly via pip:
+Get started with `ml4xcube` effortlessly by installing it directly through pip:
 ```bash
 pip install ml4xcube
 ```
+or Conda:
+```bash
+conda install -c conda-forge ml4xcube
+```
 
 Make sure you have Python version 3.8 or higher.
 
 If you're planning to use `ml4xcube` with TensorFlow or PyTorch, set up these frameworks properly in your Conda environment. 
 
 ## Features
```

### Comparing `ml4xcube-0.0.5/mltools/ml4xcube/cube_utilities.py` & `ml4xcube-0.0.6/mltools/ml4xcube/cube_utilities.py`

 * *Files identical despite different names*

### Comparing `ml4xcube-0.0.5/mltools/ml4xcube/data_assignment.py` & `ml4xcube-0.0.6/mltools/ml4xcube/data_assignment.py`

 * *Files identical despite different names*

### Comparing `ml4xcube-0.0.5/mltools/ml4xcube/datasets/pytorch_xr.py` & `ml4xcube-0.0.6/mltools/ml4xcube/datasets/pytorch_xr.py`

 * *Files identical despite different names*

### Comparing `ml4xcube-0.0.5/mltools/ml4xcube/datasets/tensorflow_xr.py` & `ml4xcube-0.0.6/mltools/ml4xcube/datasets/tensorflow_xr.py`

 * *Files identical despite different names*

### Comparing `ml4xcube-0.0.5/mltools/ml4xcube/datasets/xr_dataset.py` & `ml4xcube-0.0.6/mltools/ml4xcube/datasets/xr_dataset.py`

 * *Files identical despite different names*

### Comparing `ml4xcube-0.0.5/mltools/ml4xcube/gapfilling/gap_dataset.py` & `ml4xcube-0.0.6/mltools/ml4xcube/gapfilling/gap_dataset.py`

 * *Files identical despite different names*

### Comparing `ml4xcube-0.0.5/mltools/ml4xcube/gapfilling/gap_filling.py` & `ml4xcube-0.0.6/mltools/ml4xcube/gapfilling/gap_filling.py`

 * *Files identical despite different names*

### Comparing `ml4xcube-0.0.5/mltools/ml4xcube/gapfilling/helper/global_lcc.nc` & `ml4xcube-0.0.6/mltools/ml4xcube/gapfilling/helper/global_lcc.nc`

 * *Files identical despite different names*

### Comparing `ml4xcube-0.0.5/mltools/ml4xcube/gapfilling/helper/lcc.py` & `ml4xcube-0.0.6/mltools/ml4xcube/gapfilling/helper/lcc.py`

 * *Files identical despite different names*

### Comparing `ml4xcube-0.0.5/mltools/ml4xcube/geo_plots.py` & `ml4xcube-0.0.6/mltools/ml4xcube/geo_plots.py`

 * *Files identical despite different names*

### Comparing `ml4xcube-0.0.5/mltools/ml4xcube/statistics.py` & `ml4xcube-0.0.6/mltools/ml4xcube/statistics.py`

 * *Files identical despite different names*

### Comparing `ml4xcube-0.0.5/mltools/ml4xcube/training/pytorch.py` & `ml4xcube-0.0.6/mltools/ml4xcube/training/pytorch.py`

 * *Files identical despite different names*

### Comparing `ml4xcube-0.0.5/mltools/ml4xcube/training/pytorch_distributed.py` & `ml4xcube-0.0.6/mltools/ml4xcube/training/pytorch_distributed.py`

 * *Files identical despite different names*

### Comparing `ml4xcube-0.0.5/mltools/ml4xcube/training/sklearn.py` & `ml4xcube-0.0.6/mltools/ml4xcube/training/sklearn.py`

 * *Files identical despite different names*

### Comparing `ml4xcube-0.0.5/mltools/ml4xcube/training/tensorflow.py` & `ml4xcube-0.0.6/mltools/ml4xcube/training/tensorflow.py`

 * *Files identical despite different names*

### Comparing `ml4xcube-0.0.5/mltools/ml4xcube.egg-info/PKG-INFO` & `ml4xcube-0.0.6/mltools/ml4xcube.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml4xcube
-Version: 0.0.5
+Version: 0.0.6
 Summary: ML package for data cubes
 Author-email: Julia Peters <julia.peters@informatik.uni-leipzig.de>
 License: MIT License
         
         Copyright (c) 2022 by ScaDS.AI, the xcube development team and contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -28,34 +28,36 @@
 Keywords: machine learning,tools,data cube utilities
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: bokeh>=2.4.3
 Requires-Dist: dask>=2023.2.0
-Requires-Dist: jinja2==3.1.3
-Requires-Dist: mypy_extensions==1.0.0
 Requires-Dist: numpy>=1.24
 Requires-Dist: pandas>=2.2
 Requires-Dist: scikit-learn>1.3.1
 Requires-Dist: xarray>2023.8.0
 Requires-Dist: zarr>2.11
 Requires-Dist: rechunker>=0.5.1
 Requires-Dist: sentinelhub
 
-# ML-Toolkits
+# ml4xcube: Machine Learning Toolkits for Data Cubes
 
-The ML Toolkits provide a set of best practice Python-based Jupyter Notebooks that showcase the implementation of the three start-of-the-art Machine Learning libraries (1) scikit-learn, (2) PyTorch and (3) TensorFlow based on the Earth System Data Cube.
+Welcome to `ml4xcube`, a comprehensive Python-based toolkit designed for researchers and developers in the field of machine learning with an emphasis on `xarray` data cubes. Our toolkit is engineered to provide specialized and robust support for data cube management and analysis, operating with the state-of-the-art machine learning libraries (1) `scikit-learn`, (2) `PyTorch` and (3) `TensorFlow`. 
 
 ## Installation
 
-You can install `ml4xcube` directly via pip:
+Get started with `ml4xcube` effortlessly by installing it directly through pip:
 ```bash
 pip install ml4xcube
 ```
+or Conda:
+```bash
+conda install -c conda-forge ml4xcube
+```
 
 Make sure you have Python version 3.8 or higher.
 
 If you're planning to use `ml4xcube` with TensorFlow or PyTorch, set up these frameworks properly in your Conda environment. 
 
 ## Features
```

### Comparing `ml4xcube-0.0.5/mltools/ml4xcube.egg-info/SOURCES.txt` & `ml4xcube-0.0.6/mltools/ml4xcube.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ml4xcube-0.0.5/pyproject.toml` & `ml4xcube-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ml4xcube"
-version = "0.0.5"
+version = "0.0.6"
 dynamic = ["dependencies"]
 description = "ML package for data cubes"
 authors = [{ name = "Julia Peters", email = "julia.peters@informatik.uni-leipzig.de" }]
 readme = "./README.md"
 license = { file = "LICENSE" }
 keywords = ["machine learning", "tools", "data cube utilities"]
 classifiers = [
```

### Comparing `ml4xcube-0.0.5/setup.py` & `ml4xcube-0.0.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ml4xcube',
-    version='0.0.5',
+    version='0.0.6',
     package_dir={'': 'mltools'},
     packages=find_packages(where='mltools'),
     package_data={
         'ml4xcube': ['gapfilling/helper/*'],  # Include all files within the 'helper' directory
     },
     install_requires=[
         'bokeh >=2.4.3',
         'dask >=2023.2.0',
-        'jinja2 ==3.1.3',
-        'mypy_extensions ==1.0.0',
         'numpy >=1.24',
         'pandas >=2.2',
         'scikit-learn >1.3.1',
         'xarray >2023.8.0',
         'zarr >2.11',
         'rechunker >=0.5.1',
         'sentinelhub'
```

