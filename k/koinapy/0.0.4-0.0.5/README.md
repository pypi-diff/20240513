# Comparing `tmp/koinapy-0.0.4.tar.gz` & `tmp/koinapy-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "koinapy-0.0.4.tar", max compression
+gzip compressed data, was "koinapy-0.0.5.tar", max compression
```

## Comparing `koinapy-0.0.4.tar` & `koinapy-0.0.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       37 2024-05-10 11:43:41.840293 koinapy-0.0.4/README.md
--rw-r--r--   0        0        0       24 2024-05-10 11:43:41.840293 koinapy-0.0.4/koinapy/__init__.py
--rw-r--r--   0        0        0      930 2024-05-10 11:43:41.840293 koinapy-0.0.4/koinapy/__main__.py
--rw-r--r--   0        0        0    28557 2024-05-10 11:43:41.840293 koinapy-0.0.4/koinapy/grpc.py
--rw-r--r--   0        0        0      783 2024-05-10 11:43:41.840293 koinapy-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      963 1970-01-01 00:00:00.000000 koinapy-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       37 2024-05-13 17:21:36.425215 koinapy-0.0.5/README.md
+-rw-r--r--   0        0        0       24 2024-05-13 17:21:36.425215 koinapy-0.0.5/koinapy/__init__.py
+-rw-r--r--   0        0        0      930 2024-05-13 17:21:36.425215 koinapy-0.0.5/koinapy/__main__.py
+-rw-r--r--   0        0        0    28615 2024-05-13 17:21:36.425215 koinapy-0.0.5/koinapy/grpc.py
+-rw-r--r--   0        0        0      783 2024-05-13 17:21:36.425215 koinapy-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      963 1970-01-01 00:00:00.000000 koinapy-0.0.5/PKG-INFO
```

### Comparing `koinapy-0.0.4/koinapy/__main__.py` & `koinapy-0.0.5/koinapy/__main__.py`

 * *Files identical despite different names*

### Comparing `koinapy-0.0.4/koinapy/grpc.py` & `koinapy-0.0.5/koinapy/grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import time
 import warnings
 from functools import partial
 from typing import Dict, Generator, KeysView, List, Optional, Union
+from math import ceil
+
 
 import numpy as np
 import pandas as pd
 from tqdm.auto import tqdm
 from tritonclient.grpc import (
     InferenceServerClient,
     InferenceServerException,
@@ -513,15 +515,15 @@
         else:
             raise ValueError(f"mode must be one of 'semi_async', 'async' or 'sync'")
 
     def __predict_semi_async(self, data, debug=False, disable_progress_bar=False):
         results = []
         data_subsets = list(self.__slice_dict(data, self.batchsize * 10))
         pbar = tqdm(
-            total=len(data_subsets) * 10,
+            total=ceil(next(iter(data.values())).shape[0] / self.batchsize),
             desc=f"{self.model_name}:",
             disable=disable_progress_bar,
         )
         for data_batch in data_subsets:
             results.append(
                 self.__predict_async(data_batch, debug=debug, pbar_input=pbar)
             )
```

### Comparing `koinapy-0.0.4/pyproject.toml` & `koinapy-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "koinapy"
-version = "0.0.4"
+version = "0.0.5"
 description = "Python client to communicate with Koina."
 authors = ["Ludwig Lautenbacher <Ludwig.Lautenbacher@tum.de>"]
 license = "Apache 2.0"
 homepage = "https://koina.wilhelmlab.org/"
 repository = "https://github.com/wilhelm-lab/koina"
 documentation = "https://koina.wilhelmlab.org/docs"
 readme = "README.md"
```

### Comparing `koinapy-0.0.4/PKG-INFO` & `koinapy-0.0.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: koinapy
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python client to communicate with Koina.
 Home-page: https://koina.wilhelmlab.org/
 License: Apache 2.0
 Author: Ludwig Lautenbacher
 Author-email: Ludwig.Lautenbacher@tum.de
 Requires-Python: >=3.8,<3.11
 Classifier: License :: Other/Proprietary License
```

