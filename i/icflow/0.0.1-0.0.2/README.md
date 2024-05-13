# Comparing `tmp/icflow-0.0.1.tar.gz` & `tmp/icflow-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icflow-0.0.1.tar", last modified: Wed May  1 16:19:27 2024, max compression
+gzip compressed data, was "icflow-0.0.2.tar", last modified: Mon May 13 16:32:44 2024, max compression
```

## Comparing `icflow-0.0.1.tar` & `icflow-0.0.2.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxr-xr-x   0 jgrogan    (503) staff       (20)        0 2024-05-01 16:19:27.367578 icflow-0.0.1/
--rw-r--r--   0 jgrogan    (503) staff       (20)    34621 2024-03-14 10:55:47.000000 icflow-0.0.1/LICENSE
--rw-r--r--   0 jgrogan    (503) staff       (20)     2200 2024-05-01 16:19:27.367448 icflow-0.0.1/PKG-INFO
--rw-r--r--   0 jgrogan    (503) staff       (20)     1086 2024-05-01 14:18:00.000000 icflow-0.0.1/README.md
--rw-r--r--   0 jgrogan    (503) staff       (20)     1962 2024-05-01 16:16:40.000000 icflow-0.0.1/pyproject.toml
--rw-r--r--   0 jgrogan    (503) staff       (20)       93 2024-05-01 16:19:27.369297 icflow-0.0.1/setup.cfg
-drwxr-xr-x   0 jgrogan    (503) staff       (20)        0 2024-05-01 16:19:27.280194 icflow-0.0.1/src/
-drwxr-xr-x   0 jgrogan    (503) staff       (20)        0 2024-05-01 16:19:27.295310 icflow-0.0.1/src/icflow/
--rw-r--r--   0 jgrogan    (503) staff       (20)        0 2024-02-07 16:10:25.000000 icflow-0.0.1/src/icflow/__init__.py
-drwxr-xr-x   0 jgrogan    (503) staff       (20)        0 2024-05-01 16:19:27.320006 icflow-0.0.1/src/icflow/data/
--rw-r--r--   0 jgrogan    (503) staff       (20)       41 2024-05-01 15:49:54.000000 icflow-0.0.1/src/icflow/data/__init__.py
--rw-r--r--   0 jgrogan    (503) staff       (20)     3234 2024-05-01 14:26:50.000000 icflow-0.0.1/src/icflow/data/dataloaders.py
--rw-r--r--   0 jgrogan    (503) staff       (20)     2375 2024-05-01 15:34:53.000000 icflow-0.0.1/src/icflow/data/dataset.py
-drwxr-xr-x   0 jgrogan    (503) staff       (20)        0 2024-05-01 16:19:27.321870 icflow-0.0.1/src/icflow/data/datasets/
--rw-r--r--   0 jgrogan    (503) staff       (20)       62 2024-05-01 15:49:50.000000 icflow-0.0.1/src/icflow/data/datasets/__init__.py
--rw-r--r--   0 jgrogan    (503) staff       (20)     1850 2024-05-01 15:49:20.000000 icflow-0.0.1/src/icflow/data/datasets/dataset_collection.py
--rw-r--r--   0 jgrogan    (503) staff       (20)     1188 2024-05-01 15:59:06.000000 icflow-0.0.1/src/icflow/data/datasets/hitl.py
--rw-r--r--   0 jgrogan    (503) staff       (20)     1566 2024-05-01 14:26:50.000000 icflow-0.0.1/src/icflow/data/image_dataloaders.py
-drwxr-xr-x   0 jgrogan    (503) staff       (20)        0 2024-05-01 16:19:27.326999 icflow-0.0.1/src/icflow/models/
--rw-r--r--   0 jgrogan    (503) staff       (20)       49 2024-05-01 15:51:07.000000 icflow-0.0.1/src/icflow/models/__init__.py
--rw-r--r--   0 jgrogan    (503) staff       (20)     4275 2024-05-01 15:35:44.000000 icflow-0.0.1/src/icflow/models/metrics.py
--rw-r--r--   0 jgrogan    (503) staff       (20)      667 2024-05-01 15:36:09.000000 icflow-0.0.1/src/icflow/models/model.py
--rw-r--r--   0 jgrogan    (503) staff       (20)     1094 2024-05-01 15:36:31.000000 icflow-0.0.1/src/icflow/models/models.py
--rw-r--r--   0 jgrogan    (503) staff       (20)     7065 2024-05-01 15:45:49.000000 icflow-0.0.1/src/icflow/models/torch_models.py
-drwxr-xr-x   0 jgrogan    (503) staff       (20)        0 2024-05-01 16:19:27.331102 icflow-0.0.1/src/icflow/output/
--rw-r--r--   0 jgrogan    (503) staff       (20)       43 2024-05-01 15:50:53.000000 icflow-0.0.1/src/icflow/output/__init__.py
--rw-r--r--   0 jgrogan    (503) staff       (20)     1700 2024-05-01 16:00:05.000000 icflow-0.0.1/src/icflow/output/output.py
--rw-r--r--   0 jgrogan    (503) staff       (20)     1314 2024-04-11 07:24:18.000000 icflow-0.0.1/src/icflow/output/plot.py
--rw-r--r--   0 jgrogan    (503) staff       (20)     2236 2024-05-01 15:51:07.000000 icflow-0.0.1/src/icflow/output/visualization.py
-drwxr-xr-x   0 jgrogan    (503) staff       (20)        0 2024-05-01 16:19:27.343047 icflow-0.0.1/src/icflow/session/
--rw-r--r--   0 jgrogan    (503) staff       (20)       91 2024-05-01 15:51:07.000000 icflow-0.0.1/src/icflow/session/__init__.py
--rw-r--r--   0 jgrogan    (503) staff       (20)     2473 2024-05-01 15:53:03.000000 icflow-0.0.1/src/icflow/session/ml_session.py
--rw-r--r--   0 jgrogan    (503) staff       (20)     1535 2024-05-01 15:45:49.000000 icflow-0.0.1/src/icflow/session/session.py
--rw-r--r--   0 jgrogan    (503) staff       (20)     1083 2024-05-01 14:26:50.000000 icflow-0.0.1/src/icflow/session/settings.py
--rw-r--r--   0 jgrogan    (503) staff       (20)      267 2024-05-01 14:26:50.000000 icflow-0.0.1/src/icflow/session/task.py
-drwxr-xr-x   0 jgrogan    (503) staff       (20)        0 2024-05-01 16:19:27.366367 icflow-0.0.1/src/icflow/utils/
--rw-r--r--   0 jgrogan    (503) staff       (20)      140 2024-05-01 15:51:07.000000 icflow-0.0.1/src/icflow/utils/__init__.py
--rw-r--r--   0 jgrogan    (503) staff       (20)      458 2024-04-11 07:24:18.000000 icflow-0.0.1/src/icflow/utils/cli_utils.py
--rw-r--r--   0 jgrogan    (503) staff       (20)     3992 2024-05-01 15:41:24.000000 icflow-0.0.1/src/icflow/utils/devices.py
--rw-r--r--   0 jgrogan    (503) staff       (20)      440 2024-05-01 15:42:21.000000 icflow-0.0.1/src/icflow/utils/filesystem.py
--rw-r--r--   0 jgrogan    (503) staff       (20)      313 2024-05-01 15:43:00.000000 icflow-0.0.1/src/icflow/utils/logging_utils.py
--rw-r--r--   0 jgrogan    (503) staff       (20)      197 2024-04-11 07:24:18.000000 icflow-0.0.1/src/icflow/utils/runtime_ctx.py
--rw-r--r--   0 jgrogan    (503) staff       (20)      865 2024-05-01 15:52:21.000000 icflow-0.0.1/src/icflow/utils/scheduler.py
--rw-r--r--   0 jgrogan    (503) staff       (20)      868 2024-05-01 15:44:52.000000 icflow-0.0.1/src/icflow/utils/serialization.py
--rw-r--r--   0 jgrogan    (503) staff       (20)      126 2024-04-11 07:24:18.000000 icflow-0.0.1/src/icflow/utils/time_utils.py
--rw-r--r--   0 jgrogan    (503) staff       (20)     1706 2024-05-01 15:45:42.000000 icflow-0.0.1/src/icflow/utils/transforms.py
-drwxr-xr-x   0 jgrogan    (503) staff       (20)        0 2024-05-01 16:19:27.366928 icflow-0.0.1/src/icflow.egg-info/
--rw-r--r--   0 jgrogan    (503) staff       (20)     2200 2024-05-01 16:19:27.000000 icflow-0.0.1/src/icflow.egg-info/PKG-INFO
--rw-r--r--   0 jgrogan    (503) staff       (20)     1203 2024-05-01 16:19:27.000000 icflow-0.0.1/src/icflow.egg-info/SOURCES.txt
--rw-r--r--   0 jgrogan    (503) staff       (20)        1 2024-05-01 16:19:27.000000 icflow-0.0.1/src/icflow.egg-info/dependency_links.txt
--rw-r--r--   0 jgrogan    (503) staff       (20)      154 2024-05-01 16:19:27.000000 icflow-0.0.1/src/icflow.egg-info/requires.txt
--rw-r--r--   0 jgrogan    (503) staff       (20)        7 2024-05-01 16:19:27.000000 icflow-0.0.1/src/icflow.egg-info/top_level.txt
+drwxr-xr-x   0 jgrogan    (503) staff       (20)        0 2024-05-13 16:32:44.707134 icflow-0.0.2/
+-rw-r--r--   0 jgrogan    (503) staff       (20)    34621 2024-03-14 10:55:47.000000 icflow-0.0.2/LICENSE
+-rw-r--r--   0 jgrogan    (503) staff       (20)     2175 2024-05-13 16:32:44.706844 icflow-0.0.2/PKG-INFO
+-rw-r--r--   0 jgrogan    (503) staff       (20)     1086 2024-05-09 07:26:53.000000 icflow-0.0.2/README.md
+-rw-r--r--   0 jgrogan    (503) staff       (20)     2054 2024-05-13 16:26:27.000000 icflow-0.0.2/pyproject.toml
+-rw-r--r--   0 jgrogan    (503) staff       (20)       93 2024-05-13 16:32:44.752425 icflow-0.0.2/setup.cfg
+drwxr-xr-x   0 jgrogan    (503) staff       (20)        0 2024-05-13 16:32:44.338957 icflow-0.0.2/src/
+drwxr-xr-x   0 jgrogan    (503) staff       (20)        0 2024-05-13 16:32:44.445356 icflow-0.0.2/src/icflow/
+-rw-r--r--   0 jgrogan    (503) staff       (20)        0 2024-02-07 16:10:25.000000 icflow-0.0.2/src/icflow/__init__.py
+drwxr-xr-x   0 jgrogan    (503) staff       (20)        0 2024-05-13 16:32:44.473460 icflow-0.0.2/src/icflow/data/
+-rw-r--r--   0 jgrogan    (503) staff       (20)       41 2024-05-09 07:26:53.000000 icflow-0.0.2/src/icflow/data/__init__.py
+-rw-r--r--   0 jgrogan    (503) staff       (20)     3234 2024-05-09 07:26:53.000000 icflow-0.0.2/src/icflow/data/dataloaders.py
+-rw-r--r--   0 jgrogan    (503) staff       (20)     2375 2024-05-09 07:26:53.000000 icflow-0.0.2/src/icflow/data/dataset.py
+drwxr-xr-x   0 jgrogan    (503) staff       (20)        0 2024-05-13 16:32:44.476049 icflow-0.0.2/src/icflow/data/datasets/
+-rw-r--r--   0 jgrogan    (503) staff       (20)       62 2024-05-09 07:26:53.000000 icflow-0.0.2/src/icflow/data/datasets/__init__.py
+-rw-r--r--   0 jgrogan    (503) staff       (20)     1850 2024-05-09 07:26:53.000000 icflow-0.0.2/src/icflow/data/datasets/dataset_collection.py
+-rw-r--r--   0 jgrogan    (503) staff       (20)     1188 2024-05-09 07:26:53.000000 icflow-0.0.2/src/icflow/data/datasets/hitl.py
+-rw-r--r--   0 jgrogan    (503) staff       (20)     1566 2024-05-09 07:26:53.000000 icflow-0.0.2/src/icflow/data/image_dataloaders.py
+drwxr-xr-x   0 jgrogan    (503) staff       (20)        0 2024-05-13 16:32:44.485169 icflow-0.0.2/src/icflow/models/
+-rw-r--r--   0 jgrogan    (503) staff       (20)       49 2024-05-09 07:26:53.000000 icflow-0.0.2/src/icflow/models/__init__.py
+-rw-r--r--   0 jgrogan    (503) staff       (20)     4275 2024-05-09 07:26:53.000000 icflow-0.0.2/src/icflow/models/metrics.py
+-rw-r--r--   0 jgrogan    (503) staff       (20)      667 2024-05-09 07:26:53.000000 icflow-0.0.2/src/icflow/models/model.py
+-rw-r--r--   0 jgrogan    (503) staff       (20)     1094 2024-05-09 07:26:53.000000 icflow-0.0.2/src/icflow/models/models.py
+-rw-r--r--   0 jgrogan    (503) staff       (20)     7065 2024-05-09 07:26:53.000000 icflow-0.0.2/src/icflow/models/torch_models.py
+drwxr-xr-x   0 jgrogan    (503) staff       (20)        0 2024-05-13 16:32:44.489239 icflow-0.0.2/src/icflow/output/
+-rw-r--r--   0 jgrogan    (503) staff       (20)       43 2024-05-09 07:26:53.000000 icflow-0.0.2/src/icflow/output/__init__.py
+-rw-r--r--   0 jgrogan    (503) staff       (20)     1700 2024-05-09 07:26:53.000000 icflow-0.0.2/src/icflow/output/output.py
+-rw-r--r--   0 jgrogan    (503) staff       (20)     1314 2024-04-11 07:24:18.000000 icflow-0.0.2/src/icflow/output/plot.py
+-rw-r--r--   0 jgrogan    (503) staff       (20)     2236 2024-05-09 07:26:53.000000 icflow-0.0.2/src/icflow/output/visualization.py
+-rw-r--r--   0 jgrogan    (503) staff       (20)        0 2024-05-13 16:25:42.000000 icflow-0.0.2/src/icflow/py.typed
+drwxr-xr-x   0 jgrogan    (503) staff       (20)        0 2024-05-13 16:32:44.693301 icflow-0.0.2/src/icflow/session/
+-rw-r--r--   0 jgrogan    (503) staff       (20)      139 2024-05-13 16:25:42.000000 icflow-0.0.2/src/icflow/session/__init__.py
+-rw-r--r--   0 jgrogan    (503) staff       (20)     2473 2024-05-09 07:26:53.000000 icflow-0.0.2/src/icflow/session/ml_session.py
+-rw-r--r--   0 jgrogan    (503) staff       (20)     1570 2024-05-13 16:25:42.000000 icflow-0.0.2/src/icflow/session/session.py
+-rw-r--r--   0 jgrogan    (503) staff       (20)     1083 2024-05-09 07:26:53.000000 icflow-0.0.2/src/icflow/session/settings.py
+-rw-r--r--   0 jgrogan    (503) staff       (20)      267 2024-05-09 07:26:53.000000 icflow-0.0.2/src/icflow/session/task.py
+drwxr-xr-x   0 jgrogan    (503) staff       (20)        0 2024-05-13 16:32:44.704526 icflow-0.0.2/src/icflow/utils/
+-rw-r--r--   0 jgrogan    (503) staff       (20)      140 2024-05-09 07:26:53.000000 icflow-0.0.2/src/icflow/utils/__init__.py
+-rw-r--r--   0 jgrogan    (503) staff       (20)      458 2024-04-11 07:24:18.000000 icflow-0.0.2/src/icflow/utils/cli_utils.py
+-rw-r--r--   0 jgrogan    (503) staff       (20)     3992 2024-05-09 07:26:53.000000 icflow-0.0.2/src/icflow/utils/devices.py
+-rw-r--r--   0 jgrogan    (503) staff       (20)      440 2024-05-09 07:26:53.000000 icflow-0.0.2/src/icflow/utils/filesystem.py
+-rw-r--r--   0 jgrogan    (503) staff       (20)      313 2024-05-09 07:26:53.000000 icflow-0.0.2/src/icflow/utils/logging_utils.py
+-rw-r--r--   0 jgrogan    (503) staff       (20)      197 2024-04-11 07:24:18.000000 icflow-0.0.2/src/icflow/utils/runtime_ctx.py
+-rw-r--r--   0 jgrogan    (503) staff       (20)      865 2024-05-09 07:26:53.000000 icflow-0.0.2/src/icflow/utils/scheduler.py
+-rw-r--r--   0 jgrogan    (503) staff       (20)      868 2024-05-09 07:26:53.000000 icflow-0.0.2/src/icflow/utils/serialization.py
+-rw-r--r--   0 jgrogan    (503) staff       (20)      126 2024-04-11 07:24:18.000000 icflow-0.0.2/src/icflow/utils/time_utils.py
+-rw-r--r--   0 jgrogan    (503) staff       (20)     1706 2024-05-09 07:26:53.000000 icflow-0.0.2/src/icflow/utils/transforms.py
+drwxr-xr-x   0 jgrogan    (503) staff       (20)        0 2024-05-13 16:32:44.705505 icflow-0.0.2/src/icflow.egg-info/
+-rw-r--r--   0 jgrogan    (503) staff       (20)     2175 2024-05-13 16:32:44.000000 icflow-0.0.2/src/icflow.egg-info/PKG-INFO
+-rw-r--r--   0 jgrogan    (503) staff       (20)     1223 2024-05-13 16:32:44.000000 icflow-0.0.2/src/icflow.egg-info/SOURCES.txt
+-rw-r--r--   0 jgrogan    (503) staff       (20)        1 2024-05-13 16:32:44.000000 icflow-0.0.2/src/icflow.egg-info/dependency_links.txt
+-rw-r--r--   0 jgrogan    (503) staff       (20)      144 2024-05-13 16:32:44.000000 icflow-0.0.2/src/icflow.egg-info/requires.txt
+-rw-r--r--   0 jgrogan    (503) staff       (20)        7 2024-05-13 16:32:44.000000 icflow-0.0.2/src/icflow.egg-info/top_level.txt
```

### Comparing `icflow-0.0.1/LICENSE` & `icflow-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `icflow-0.0.1/PKG-INFO` & `icflow-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icflow
-Version: 0.0.1
+Version: 0.0.2
 Summary: A collection of simple utilities for machine learning workflows.
 Author-email: "James Grogan, Irish Centre for High End Computing" <james.grogan@ichec.ie>
 Project-URL: Repository, https://git.ichec.ie/performance/toolshed/icflow
 Project-URL: Homepage, https://git.ichec.ie/performance/toolshed/icflow
 Keywords: Machine Learning,Workflow,HPC
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
@@ -16,15 +16,14 @@
 License-File: LICENSE
 Requires-Dist: icsystemutils
 Requires-Dist: PyYAML
 Requires-Dist: types-PyYAML
 Requires-Dist: albumentations
 Requires-Dist: numpy
 Requires-Dist: opencv-python
-Requires-Dist: patchwork
 Requires-Dist: segmentation_models_pytorch
 Requires-Dist: tqdm
 Requires-Dist: tensorboard
 Requires-Dist: torch
 Requires-Dist: torchvision
 Requires-Dist: ultralytics
```

### Comparing `icflow-0.0.1/README.md` & `icflow-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `icflow-0.0.1/pyproject.toml` & `icflow-0.0.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "icflow"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="James Grogan, Irish Centre for High End Computing", email="james.grogan@ichec.ie" },
 ]
 description = "A collection of simple utilities for machine learning workflows."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -13,29 +13,35 @@
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Operating System :: OS Independent",
     "Topic :: System :: Distributed Computing"
 ]
 keywords = ["Machine Learning", "Workflow", "HPC"]
 
 dependencies = ["icsystemutils", "PyYAML", "types-PyYAML",
-                "albumentations", "numpy", "opencv-python", "patchwork",
+                "albumentations", "numpy", "opencv-python",
                 "segmentation_models_pytorch", "tqdm",
                 "tensorboard", "torch", "torchvision", "ultralytics"]
             
 [project.urls]
 Repository = "https://git.ichec.ie/performance/toolshed/icflow"
 Homepage = "https://git.ichec.ie/performance/toolshed/icflow"
 
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.mypy]
 ignore_missing_imports = true
 
+[tool.setuptools.package-data]
+"icflow" = ["py.typed"]
+
+[tool.setuptools.packages.find]
+where = ["src"]
+
 [tool.pytest.ini_options]
 testpaths = ["test",]
 log_cli = 1
 log_cli_level = "debug"
 
 [tool.tox]
 legacy_tox_ini = """
```

### Comparing `icflow-0.0.1/src/icflow/data/dataloaders.py` & `icflow-0.0.2/src/icflow/data/dataloaders.py`

 * *Files identical despite different names*

### Comparing `icflow-0.0.1/src/icflow/data/dataset.py` & `icflow-0.0.2/src/icflow/data/dataset.py`

 * *Files identical despite different names*

### Comparing `icflow-0.0.1/src/icflow/data/datasets/dataset_collection.py` & `icflow-0.0.2/src/icflow/data/datasets/dataset_collection.py`

 * *Files identical despite different names*

### Comparing `icflow-0.0.1/src/icflow/data/datasets/hitl.py` & `icflow-0.0.2/src/icflow/data/datasets/hitl.py`

 * *Files identical despite different names*

### Comparing `icflow-0.0.1/src/icflow/data/image_dataloaders.py` & `icflow-0.0.2/src/icflow/data/image_dataloaders.py`

 * *Files identical despite different names*

### Comparing `icflow-0.0.1/src/icflow/models/metrics.py` & `icflow-0.0.2/src/icflow/models/metrics.py`

 * *Files identical despite different names*

### Comparing `icflow-0.0.1/src/icflow/models/model.py` & `icflow-0.0.2/src/icflow/models/model.py`

 * *Files identical despite different names*

### Comparing `icflow-0.0.1/src/icflow/models/models.py` & `icflow-0.0.2/src/icflow/models/models.py`

 * *Files identical despite different names*

### Comparing `icflow-0.0.1/src/icflow/models/torch_models.py` & `icflow-0.0.2/src/icflow/models/torch_models.py`

 * *Files identical despite different names*

### Comparing `icflow-0.0.1/src/icflow/output/output.py` & `icflow-0.0.2/src/icflow/output/output.py`

 * *Files identical despite different names*

### Comparing `icflow-0.0.1/src/icflow/output/plot.py` & `icflow-0.0.2/src/icflow/output/plot.py`

 * *Files identical despite different names*

### Comparing `icflow-0.0.1/src/icflow/output/visualization.py` & `icflow-0.0.2/src/icflow/output/visualization.py`

 * *Files identical despite different names*

### Comparing `icflow-0.0.1/src/icflow/session/ml_session.py` & `icflow-0.0.2/src/icflow/session/ml_session.py`

 * *Files identical despite different names*

### Comparing `icflow-0.0.1/src/icflow/session/session.py` & `icflow-0.0.2/src/icflow/session/session.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 from pathlib import Path
 import logging
 
 import icflow.utils
 from icflow.session.settings import SessionSettings
 
 
+logger = logging.getLogger(__name__)
+
+
 class WorkflowSession:
     def __init__(
         self, settings: SessionSettings, result_dir: None | Path = None
     ) -> None:
 
         if result_dir is None:
             self.result_dir = Path(os.getcwd())
@@ -39,17 +42,17 @@
 
     def run_tasks(self):
 
         if not self.tasks_initialized:
             self.init_tasks()
 
         if not self.tasks:
-            logging.info("No tasks available to launch")
+            logger.info("No tasks available to launch")
             return
 
-        logging.info(f"Launching {len(self.tasks)} tasks")
+        logger.info(f"Launching {len(self.tasks)} tasks")
 
         for idx, task in enumerate(self.tasks):
-            logging.info(f"Launching {idx} of {len(self.tasks)} tasks: {task.name}")
+            logger.info(f"Launching {idx} of {len(self.tasks)} tasks: {task.name}")
             task.launch()
 
-        logging.info("Finished launching tasks")
+        logger.info("Finished launching tasks")
```

### Comparing `icflow-0.0.1/src/icflow/session/settings.py` & `icflow-0.0.2/src/icflow/session/settings.py`

 * *Files identical despite different names*

### Comparing `icflow-0.0.1/src/icflow/utils/devices.py` & `icflow-0.0.2/src/icflow/utils/devices.py`

 * *Files identical despite different names*

### Comparing `icflow-0.0.1/src/icflow/utils/scheduler.py` & `icflow-0.0.2/src/icflow/utils/scheduler.py`

 * *Files identical despite different names*

### Comparing `icflow-0.0.1/src/icflow/utils/serialization.py` & `icflow-0.0.2/src/icflow/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `icflow-0.0.1/src/icflow/utils/transforms.py` & `icflow-0.0.2/src/icflow/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `icflow-0.0.1/src/icflow.egg-info/PKG-INFO` & `icflow-0.0.2/src/icflow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icflow
-Version: 0.0.1
+Version: 0.0.2
 Summary: A collection of simple utilities for machine learning workflows.
 Author-email: "James Grogan, Irish Centre for High End Computing" <james.grogan@ichec.ie>
 Project-URL: Repository, https://git.ichec.ie/performance/toolshed/icflow
 Project-URL: Homepage, https://git.ichec.ie/performance/toolshed/icflow
 Keywords: Machine Learning,Workflow,HPC
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
@@ -16,15 +16,14 @@
 License-File: LICENSE
 Requires-Dist: icsystemutils
 Requires-Dist: PyYAML
 Requires-Dist: types-PyYAML
 Requires-Dist: albumentations
 Requires-Dist: numpy
 Requires-Dist: opencv-python
-Requires-Dist: patchwork
 Requires-Dist: segmentation_models_pytorch
 Requires-Dist: tqdm
 Requires-Dist: tensorboard
 Requires-Dist: torch
 Requires-Dist: torchvision
 Requires-Dist: ultralytics
```

### Comparing `icflow-0.0.1/src/icflow.egg-info/SOURCES.txt` & `icflow-0.0.2/src/icflow.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 src/icflow/__init__.py
+src/icflow/py.typed
 src/icflow.egg-info/PKG-INFO
 src/icflow.egg-info/SOURCES.txt
 src/icflow.egg-info/dependency_links.txt
 src/icflow.egg-info/requires.txt
 src/icflow.egg-info/top_level.txt
 src/icflow/data/__init__.py
 src/icflow/data/dataloaders.py
```

