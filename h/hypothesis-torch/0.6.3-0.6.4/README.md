# Comparing `tmp/hypothesis_torch-0.6.3.tar.gz` & `tmp/hypothesis_torch-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypothesis_torch-0.6.3.tar", last modified: Sun May 12 02:19:21 2024, max compression
+gzip compressed data, was "hypothesis_torch-0.6.4.tar", last modified: Mon May 13 15:10:43 2024, max compression
```

## Comparing `hypothesis_torch-0.6.3.tar` & `hypothesis_torch-0.6.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 02:19:21.289204 hypothesis_torch-0.6.3/
--rw-r--r--   0 root         (0) root         (0)     1070 2024-05-12 02:18:47.000000 hypothesis_torch-0.6.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     9045 2024-05-12 02:19:21.289204 hypothesis_torch-0.6.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5465 2024-05-12 02:18:47.000000 hypothesis_torch-0.6.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 02:19:21.285204 hypothesis_torch-0.6.3/hypothesis_torch/
--rw-r--r--   0 root         (0) root         (0)     2168 2024-05-12 02:19:17.000000 hypothesis_torch-0.6.3/hypothesis_torch/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1408 2024-05-12 02:18:47.000000 hypothesis_torch-0.6.3/hypothesis_torch/device.py
--rw-r--r--   0 root         (0) root         (0)     2757 2024-05-12 02:18:47.000000 hypothesis_torch-0.6.3/hypothesis_torch/dtype.py
--rw-r--r--   0 root         (0) root         (0)    11506 2024-05-12 02:18:47.000000 hypothesis_torch-0.6.3/hypothesis_torch/huggingface.py
--rw-r--r--   0 root         (0) root         (0)     2841 2024-05-12 02:18:47.000000 hypothesis_torch-0.6.3/hypothesis_torch/inspection_util.py
--rw-r--r--   0 root         (0) root         (0)      735 2024-05-12 02:18:47.000000 hypothesis_torch-0.6.3/hypothesis_torch/layout.py
--rw-r--r--   0 root         (0) root         (0)      846 2024-05-12 02:18:47.000000 hypothesis_torch-0.6.3/hypothesis_torch/memory_format.py
--rw-r--r--   0 root         (0) root         (0)    11178 2024-05-12 02:18:47.000000 hypothesis_torch-0.6.3/hypothesis_torch/module.py
--rw-r--r--   0 root         (0) root         (0)     4873 2024-05-12 02:18:47.000000 hypothesis_torch-0.6.3/hypothesis_torch/optim.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-12 02:18:47.000000 hypothesis_torch-0.6.3/hypothesis_torch/py.typed
--rw-r--r--   0 root         (0) root         (0)      866 2024-05-12 02:18:47.000000 hypothesis_torch-0.6.3/hypothesis_torch/register_random_torch_state.py
--rw-r--r--   0 root         (0) root         (0)     9464 2024-05-12 02:18:47.000000 hypothesis_torch-0.6.3/hypothesis_torch/tensor.py
--rw-r--r--   0 root         (0) root         (0)     1442 2024-05-12 02:18:47.000000 hypothesis_torch-0.6.3/hypothesis_torch/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 02:19:21.285204 hypothesis_torch-0.6.3/hypothesis_torch.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9045 2024-05-12 02:19:21.000000 hypothesis_torch-0.6.3/hypothesis_torch.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      665 2024-05-12 02:19:21.000000 hypothesis_torch-0.6.3/hypothesis_torch.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-12 02:19:21.000000 hypothesis_torch-0.6.3/hypothesis_torch.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2024-05-12 02:19:21.000000 hypothesis_torch-0.6.3/hypothesis_torch.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      294 2024-05-12 02:19:21.000000 hypothesis_torch-0.6.3/hypothesis_torch.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-05-12 02:19:21.000000 hypothesis_torch-0.6.3/hypothesis_torch.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2903 2024-05-12 02:18:47.000000 hypothesis_torch-0.6.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-12 02:19:21.289204 hypothesis_torch-0.6.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 15:10:43.943974 hypothesis_torch-0.6.4/
+-rw-r--r--   0 root         (0) root         (0)     1070 2024-05-13 15:09:56.000000 hypothesis_torch-0.6.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     9029 2024-05-13 15:10:43.943974 hypothesis_torch-0.6.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5465 2024-05-13 15:09:56.000000 hypothesis_torch-0.6.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 15:10:43.939974 hypothesis_torch-0.6.4/hypothesis_torch/
+-rw-r--r--   0 root         (0) root         (0)     2168 2024-05-13 15:10:40.000000 hypothesis_torch-0.6.4/hypothesis_torch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1408 2024-05-13 15:09:56.000000 hypothesis_torch-0.6.4/hypothesis_torch/device.py
+-rw-r--r--   0 root         (0) root         (0)     2757 2024-05-13 15:09:56.000000 hypothesis_torch-0.6.4/hypothesis_torch/dtype.py
+-rw-r--r--   0 root         (0) root         (0)    11506 2024-05-13 15:09:56.000000 hypothesis_torch-0.6.4/hypothesis_torch/huggingface.py
+-rw-r--r--   0 root         (0) root         (0)     2841 2024-05-13 15:09:56.000000 hypothesis_torch-0.6.4/hypothesis_torch/inspection_util.py
+-rw-r--r--   0 root         (0) root         (0)      735 2024-05-13 15:09:56.000000 hypothesis_torch-0.6.4/hypothesis_torch/layout.py
+-rw-r--r--   0 root         (0) root         (0)      846 2024-05-13 15:09:56.000000 hypothesis_torch-0.6.4/hypothesis_torch/memory_format.py
+-rw-r--r--   0 root         (0) root         (0)    11178 2024-05-13 15:09:56.000000 hypothesis_torch-0.6.4/hypothesis_torch/module.py
+-rw-r--r--   0 root         (0) root         (0)     4873 2024-05-13 15:09:56.000000 hypothesis_torch-0.6.4/hypothesis_torch/optim.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 15:09:56.000000 hypothesis_torch-0.6.4/hypothesis_torch/py.typed
+-rw-r--r--   0 root         (0) root         (0)      866 2024-05-13 15:09:56.000000 hypothesis_torch-0.6.4/hypothesis_torch/register_random_torch_state.py
+-rw-r--r--   0 root         (0) root         (0)     9464 2024-05-13 15:09:56.000000 hypothesis_torch-0.6.4/hypothesis_torch/tensor.py
+-rw-r--r--   0 root         (0) root         (0)     1442 2024-05-13 15:09:56.000000 hypothesis_torch-0.6.4/hypothesis_torch/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 15:10:43.939974 hypothesis_torch-0.6.4/hypothesis_torch.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9029 2024-05-13 15:10:43.000000 hypothesis_torch-0.6.4/hypothesis_torch.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      665 2024-05-13 15:10:43.000000 hypothesis_torch-0.6.4/hypothesis_torch.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-13 15:10:43.000000 hypothesis_torch-0.6.4/hypothesis_torch.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       91 2024-05-13 15:10:43.000000 hypothesis_torch-0.6.4/hypothesis_torch.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      278 2024-05-13 15:10:43.000000 hypothesis_torch-0.6.4/hypothesis_torch.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-05-13 15:10:43.000000 hypothesis_torch-0.6.4/hypothesis_torch.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2887 2024-05-13 15:09:56.000000 hypothesis_torch-0.6.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-13 15:10:43.943974 hypothesis_torch-0.6.4/setup.cfg
```

### Comparing `hypothesis_torch-0.6.3/LICENSE` & `hypothesis_torch-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.6.3/PKG-INFO` & `hypothesis_torch-0.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypothesis-torch
-Version: 0.6.3
+Version: 0.6.4
 Summary: Hypothesis strategies for various Pytorch structures, including tensors and modules.
 Author-email: "Andrew P. Sansom" <andrew@euleriancircuit.com>
 License: MIT License
         
         Copyright (c) 2024 Andrew Sansom
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -46,27 +46,27 @@
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: hypothesis<=6.98.8,>=6.0.0
-Requires-Dist: torch<=2.3.0,>=1.13.0
+Requires-Dist: hypothesis>=6.0.0
+Requires-Dist: torch>=1.13.0
 Provides-Extra: huggingface
-Requires-Dist: transformers<=4.40.0,>=4.0.0; extra == "huggingface"
+Requires-Dist: transformers<=4.40.2,>=4.0.0; extra == "huggingface"
 Provides-Extra: dev
-Requires-Dist: ruff==0.4.3; extra == "dev"
+Requires-Dist: ruff==0.4.4; extra == "dev"
 Requires-Dist: pytest==8.2.0; extra == "dev"
 Requires-Dist: pytest-cov==5.0.0; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: mkdocs==1.6.0; extra == "docs"
 Requires-Dist: mkdocstrings[python]==0.25.1; extra == "docs"
 Requires-Dist: mkdocs-autolinks-plugin==0.7.1; extra == "docs"
-Requires-Dist: mkdocs-material==9.4.6; extra == "docs"
+Requires-Dist: mkdocs-material==9.5.22; extra == "docs"
 Requires-Dist: mkdocs-snippets==1.3.0; extra == "docs"
 Requires-Dist: mkdocs-exclude==1.0.2; extra == "docs"
 
 [![PyPI version](https://img.shields.io/pypi/v/hypothesis-torch.svg)](https://pypi.org/project/hypothesis-torch) ![PyPI - Downloads](https://img.shields.io/pypi/dm/hypothesis-torch)
 
 # hypothesis-torch
 Hypothesis strategies for various Pytorch structures (including tensors and modules).
```

### Comparing `hypothesis_torch-0.6.3/README.md` & `hypothesis_torch-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.6.3/hypothesis_torch/__init__.py` & `hypothesis_torch-0.6.4/hypothesis_torch/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Hypothesis strategies for various Pytorch structures (including tensors and modules).
 
 [Hypothesis](https://hypothesis.readthedocs.io/en/latest/) is a powerful property-based testing library for Python. It
 lacks built-in support for Pytorch tensors and modules, so this library provides strategies for generating them.
 """
 
-__version__ = "0.6.3"
+__version__ = "0.6.4"
 import importlib.util
 
 from hypothesis_torch.device import (
     device_strategy,
     AVAILABLE_CPU_DEVICES,
     AVAILABLE_CUDA_DEVICES,
     AVAILABLE_MPS_DEVICES,
```

### Comparing `hypothesis_torch-0.6.3/hypothesis_torch/device.py` & `hypothesis_torch-0.6.4/hypothesis_torch/device.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.6.3/hypothesis_torch/dtype.py` & `hypothesis_torch-0.6.4/hypothesis_torch/dtype.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.6.3/hypothesis_torch/huggingface.py` & `hypothesis_torch-0.6.4/hypothesis_torch/huggingface.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.6.3/hypothesis_torch/inspection_util.py` & `hypothesis_torch-0.6.4/hypothesis_torch/inspection_util.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.6.3/hypothesis_torch/layout.py` & `hypothesis_torch-0.6.4/hypothesis_torch/layout.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.6.3/hypothesis_torch/memory_format.py` & `hypothesis_torch-0.6.4/hypothesis_torch/memory_format.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.6.3/hypothesis_torch/module.py` & `hypothesis_torch-0.6.4/hypothesis_torch/module.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.6.3/hypothesis_torch/optim.py` & `hypothesis_torch-0.6.4/hypothesis_torch/optim.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.6.3/hypothesis_torch/register_random_torch_state.py` & `hypothesis_torch-0.6.4/hypothesis_torch/register_random_torch_state.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.6.3/hypothesis_torch/tensor.py` & `hypothesis_torch-0.6.4/hypothesis_torch/tensor.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.6.3/hypothesis_torch/utils.py` & `hypothesis_torch-0.6.4/hypothesis_torch/utils.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.6.3/hypothesis_torch.egg-info/PKG-INFO` & `hypothesis_torch-0.6.4/hypothesis_torch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypothesis-torch
-Version: 0.6.3
+Version: 0.6.4
 Summary: Hypothesis strategies for various Pytorch structures, including tensors and modules.
 Author-email: "Andrew P. Sansom" <andrew@euleriancircuit.com>
 License: MIT License
         
         Copyright (c) 2024 Andrew Sansom
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -46,27 +46,27 @@
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: hypothesis<=6.98.8,>=6.0.0
-Requires-Dist: torch<=2.3.0,>=1.13.0
+Requires-Dist: hypothesis>=6.0.0
+Requires-Dist: torch>=1.13.0
 Provides-Extra: huggingface
-Requires-Dist: transformers<=4.40.0,>=4.0.0; extra == "huggingface"
+Requires-Dist: transformers<=4.40.2,>=4.0.0; extra == "huggingface"
 Provides-Extra: dev
-Requires-Dist: ruff==0.4.3; extra == "dev"
+Requires-Dist: ruff==0.4.4; extra == "dev"
 Requires-Dist: pytest==8.2.0; extra == "dev"
 Requires-Dist: pytest-cov==5.0.0; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: mkdocs==1.6.0; extra == "docs"
 Requires-Dist: mkdocstrings[python]==0.25.1; extra == "docs"
 Requires-Dist: mkdocs-autolinks-plugin==0.7.1; extra == "docs"
-Requires-Dist: mkdocs-material==9.4.6; extra == "docs"
+Requires-Dist: mkdocs-material==9.5.22; extra == "docs"
 Requires-Dist: mkdocs-snippets==1.3.0; extra == "docs"
 Requires-Dist: mkdocs-exclude==1.0.2; extra == "docs"
 
 [![PyPI version](https://img.shields.io/pypi/v/hypothesis-torch.svg)](https://pypi.org/project/hypothesis-torch) ![PyPI - Downloads](https://img.shields.io/pypi/dm/hypothesis-torch)
 
 # hypothesis-torch
 Hypothesis strategies for various Pytorch structures (including tensors and modules).
```

### Comparing `hypothesis_torch-0.6.3/hypothesis_torch.egg-info/SOURCES.txt` & `hypothesis_torch-0.6.4/hypothesis_torch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.6.3/pyproject.toml` & `hypothesis_torch-0.6.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 [project]
 name = "hypothesis-torch"
 description = "Hypothesis strategies for various Pytorch structures, including tensors and modules."
 
 dynamic = ["version"]
 dependencies = [
-    "hypothesis>=6.0.0,<=6.98.8",
-    "torch>=1.13.0,<=2.3.0",
+    "hypothesis>=6.0.0",
+    "torch>=1.13.0",
 ]
 requires-python = ">=3.9"
 authors=[{name="Andrew P. Sansom", email="andrew@euleriancircuit.com"}]
 readme="README.md"
 license={file="LICENSE"}
 keywords = ["hypothesis", "torch", "pytorch", "testing", "property-based testing", "deep learning", "tensor", "neural network", "artificial intelligence", "machine learning"]
 classifiers = [
@@ -40,26 +40,26 @@
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 [project.entry-points."hypothesis"]
 _ = "hypothesis_torch.register_random_torch_state:_register_random_torch_state"
 
 [project.optional-dependencies]
 huggingface = [
-  "transformers<=4.40.0,>=4.0.0",
+  "transformers>=4.0.0,<=4.40.2",
 ]
 dev = [
-  "ruff==0.4.3",
+  "ruff==0.4.4",
   "pytest==8.2.0",
   "pytest-cov==5.0.0"
 ]
 docs = [
   "mkdocs==1.6.0",
   "mkdocstrings[python]==0.25.1",
   "mkdocs-autolinks-plugin==0.7.1",
-  "mkdocs-material==9.4.6",
+  "mkdocs-material==9.5.22",
   "mkdocs-snippets==1.3.0",
   "mkdocs-exclude==1.0.2",
 ]
 
 [project.urls]
 Homepage = "https://github.com/qthequartermasterman/hypothesis-torch"
 Documentation = "https://hypothesis-torch.readthedocs.io/en/stable/"
```

