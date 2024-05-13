# Comparing `tmp/imt_ikarus-1.1.2.tar.gz` & `tmp/imt_ikarus-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imt_ikarus-1.1.2.tar", last modified: Wed Apr 24 11:20:56 2024, max compression
+gzip compressed data, was "imt_ikarus-1.2.0.tar", last modified: Mon May 13 09:25:14 2024, max compression
```

## Comparing `imt_ikarus-1.1.2.tar` & `imt_ikarus-1.2.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:20:56.270224 imt_ikarus-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     5387 2024-04-24 11:20:56.270224 imt_ikarus-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-24 11:20:24.000000 imt_ikarus-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     4567 2024-04-24 11:20:24.000000 imt_ikarus-1.1.2/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-24 11:20:56.270224 imt_ikarus-1.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:20:56.262224 imt_ikarus-1.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:20:56.266224 imt_ikarus-1.1.2/src/ikarus/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-24 11:20:24.000000 imt_ikarus-1.1.2/src/ikarus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-04-24 11:20:24.000000 imt_ikarus-1.1.2/src/ikarus/_src.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:20:56.266224 imt_ikarus-1.1.2/src/ikarus/baselines/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-24 11:20:24.000000 imt_ikarus-1.1.2/src/ikarus/baselines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-04-24 11:20:24.000000 imt_ikarus-1.1.2/src/ikarus/baselines/qmt_baselines.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:20:56.266224 imt_ikarus-1.1.2/src/ikarus/baselines/riann/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-24 11:20:24.000000 imt_ikarus-1.1.2/src/ikarus/baselines/riann/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  1471345 2024-04-24 11:20:24.000000 imt_ikarus-1.1.2/src/ikarus/baselines/riann/riann.onnx
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-24 11:20:24.000000 imt_ikarus-1.1.2/src/ikarus/baselines/riann/riann.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:20:56.270224 imt_ikarus-1.1.2/src/ikarus/benchmark/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-24 11:20:24.000000 imt_ikarus-1.1.2/src/ikarus/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-04-24 11:20:24.000000 imt_ikarus-1.1.2/src/ikarus/benchmark/_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:20:56.270224 imt_ikarus-1.1.2/src/ikarus/benchmark/xmls/
--rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-04-24 11:20:24.000000 imt_ikarus-1.1.2/src/ikarus/benchmark/xmls/arm.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-04-24 11:20:24.000000 imt_ikarus-1.1.2/src/ikarus/benchmark/xmls/gait.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-04-24 11:20:24.000000 imt_ikarus-1.1.2/src/ikarus/dataverse_github.py
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-24 11:20:24.000000 imt_ikarus-1.1.2/src/ikarus/test_dataverse_github.py
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-24 11:20:24.000000 imt_ikarus-1.1.2/src/ikarus/test_src.py
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-04-24 11:20:24.000000 imt_ikarus-1.1.2/src/ikarus/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9671 2024-04-24 11:20:24.000000 imt_ikarus-1.1.2/src/ikarus/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:20:56.270224 imt_ikarus-1.1.2/src/imt_ikarus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5387 2024-04-24 11:20:56.000000 imt_ikarus-1.1.2/src/imt_ikarus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-24 11:20:56.000000 imt_ikarus-1.1.2/src/imt_ikarus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 11:20:56.000000 imt_ikarus-1.1.2/src/imt_ikarus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-24 11:20:56.000000 imt_ikarus-1.1.2/src/imt_ikarus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-24 11:20:56.000000 imt_ikarus-1.1.2/src/imt_ikarus.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:25:14.258148 imt_ikarus-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     5387 2024-05-13 09:25:14.258148 imt_ikarus-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-13 09:25:10.000000 imt_ikarus-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     4567 2024-05-13 09:25:10.000000 imt_ikarus-1.2.0/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-13 09:25:14.258148 imt_ikarus-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:25:14.250148 imt_ikarus-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:25:14.250148 imt_ikarus-1.2.0/src/ikarus/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-13 09:25:10.000000 imt_ikarus-1.2.0/src/ikarus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-05-13 09:25:10.000000 imt_ikarus-1.2.0/src/ikarus/_src.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:25:14.250148 imt_ikarus-1.2.0/src/ikarus/baselines/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-13 09:25:10.000000 imt_ikarus-1.2.0/src/ikarus/baselines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-05-13 09:25:10.000000 imt_ikarus-1.2.0/src/ikarus/baselines/qmt_baselines.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:25:14.254148 imt_ikarus-1.2.0/src/ikarus/baselines/riann/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-13 09:25:10.000000 imt_ikarus-1.2.0/src/ikarus/baselines/riann/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1471345 2024-05-13 09:25:10.000000 imt_ikarus-1.2.0/src/ikarus/baselines/riann/riann.onnx
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-13 09:25:10.000000 imt_ikarus-1.2.0/src/ikarus/baselines/riann/riann.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:25:14.254148 imt_ikarus-1.2.0/src/ikarus/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-13 09:25:10.000000 imt_ikarus-1.2.0/src/ikarus/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-05-13 09:25:10.000000 imt_ikarus-1.2.0/src/ikarus/benchmark/_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:25:14.254148 imt_ikarus-1.2.0/src/ikarus/benchmark/xmls/
+-rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-05-13 09:25:10.000000 imt_ikarus-1.2.0/src/ikarus/benchmark/xmls/arm.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-05-13 09:25:10.000000 imt_ikarus-1.2.0/src/ikarus/benchmark/xmls/gait.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3572 2024-05-13 09:25:10.000000 imt_ikarus-1.2.0/src/ikarus/dataverse_github.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-13 09:25:10.000000 imt_ikarus-1.2.0/src/ikarus/test_dataverse_github.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-13 09:25:10.000000 imt_ikarus-1.2.0/src/ikarus/test_src.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-05-13 09:25:10.000000 imt_ikarus-1.2.0/src/ikarus/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9671 2024-05-13 09:25:10.000000 imt_ikarus-1.2.0/src/ikarus/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:25:14.254148 imt_ikarus-1.2.0/src/imt_ikarus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5387 2024-05-13 09:25:14.000000 imt_ikarus-1.2.0/src/imt_ikarus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-13 09:25:14.000000 imt_ikarus-1.2.0/src/imt_ikarus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 09:25:14.000000 imt_ikarus-1.2.0/src/imt_ikarus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-13 09:25:14.000000 imt_ikarus-1.2.0/src/imt_ikarus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-13 09:25:14.000000 imt_ikarus-1.2.0/src/imt_ikarus.egg-info/top_level.txt
```

### Comparing `imt_ikarus-1.1.2/PKG-INFO` & `imt_ikarus-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imt-ikarus
-Version: 1.1.2
+Version: 1.2.0
 Summary: IKArus - Inertial and Optical Data of Kinematic ChAin Motion
 Author-email: Simon Bachhuber <simon.bachhuber@fau.de>
 Project-URL: Homepage, https://github.com/SimiPixel/ikarus
 Project-URL: Issues, https://github.com/SimiPixel/ikarus/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `imt_ikarus-1.1.2/pyproject.toml` & `imt_ikarus-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=69.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "imt-ikarus"
-version = "1.1.2"
+version = "1.2.0"
 authors = [
   { name="Simon Bachhuber", email="simon.bachhuber@fau.de" },
 ]
 description = "IKArus - Inertial and Optical Data of Kinematic ChAin Motion"
 readme = "readme.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `imt_ikarus-1.1.2/readme.md` & `imt_ikarus-1.2.0/readme.md`

 * *Files identical despite different names*

### Comparing `imt_ikarus-1.1.2/src/ikarus/_src.py` & `imt_ikarus-1.2.0/src/ikarus/_src.py`

 * *Files identical despite different names*

### Comparing `imt_ikarus-1.1.2/src/ikarus/baselines/qmt_baselines.py` & `imt_ikarus-1.2.0/src/ikarus/baselines/qmt_baselines.py`

 * *Files identical despite different names*

### Comparing `imt_ikarus-1.1.2/src/ikarus/baselines/riann/riann.onnx` & `imt_ikarus-1.2.0/src/ikarus/baselines/riann/riann.onnx`

 * *Files identical despite different names*

### Comparing `imt_ikarus-1.1.2/src/ikarus/baselines/riann/riann.py` & `imt_ikarus-1.2.0/src/ikarus/baselines/riann/riann.py`

 * *Files identical despite different names*

### Comparing `imt_ikarus-1.1.2/src/ikarus/benchmark/_benchmark.py` & `imt_ikarus-1.2.0/src/ikarus/benchmark/_benchmark.py`

 * *Files identical despite different names*

### Comparing `imt_ikarus-1.1.2/src/ikarus/benchmark/xmls/arm.xml` & `imt_ikarus-1.2.0/src/ikarus/benchmark/xmls/arm.xml`

 * *Files identical despite different names*

### Comparing `imt_ikarus-1.1.2/src/ikarus/benchmark/xmls/gait.xml` & `imt_ikarus-1.2.0/src/ikarus/benchmark/xmls/gait.xml`

 * *Files identical despite different names*

### Comparing `imt_ikarus-1.1.2/src/ikarus/dataverse_github.py` & `imt_ikarus-1.2.0/src/ikarus/dataverse_github.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from functools import cache
 from pathlib import Path
 from typing import NamedTuple, Optional
 
 import requests
 
+_default_backend = "dataverse"
+
 
 def listdir(
     filter_prefix: Optional[str] = None,
     filter_suffix: Optional[str] = None,
-    backend: str = "github",
+    backend: str = _default_backend,
 ) -> list[str]:
 
     if backend == "github":
         files = _listdir_github()
     elif backend == "dataverse":
         files = _listdir_dataverse()
     else:
@@ -28,17 +30,19 @@
             if file[-len(filter_suffix) :] == filter_suffix  # noqa: E203
         ]
 
     return files
 
 
 def download(
-    path_in_repo: str, path_to_cache: str = "~/.ikarus_cache", backend: str = "github"
+    path_in_repo: str,
+    path_to_cache: str = "~/.ikarus_cache",
+    backend: str = _default_backend,
 ) -> Path:
-    "Download file from Github repo. Returns path on disk."
+    "Download file from Github/Dataverse repo. Returns path on disk."
     path_on_disk = Path(path_to_cache).expanduser().joinpath(path_in_repo)
     if not path_on_disk.exists():
         path_on_disk.parent.mkdir(parents=True, exist_ok=True)
 
         if backend == "github":
             url = _url_github(path_in_repo)
         elif backend == "dataverse":
@@ -57,15 +61,15 @@
 
 class DataverseFile(NamedTuple):
     path: str
     id: int
 
 
 _dataverse_url = "https://dataverse.harvard.edu/api"
-_dataset_doi = "doi:10.7910/DVN/M0NKN9"
+_dataset_doi = "doi:10.7910/DVN/SGJLZA"
 
 
 @cache
 def _dataverse_files() -> list[DataverseFile]:
 
     url = f"{_dataverse_url}/datasets/:persistentId/versions/:latest/files?persistentId={_dataset_doi}"  # noqa: E501
     response = requests.get(url)
```

### Comparing `imt_ikarus-1.1.2/src/ikarus/test_src.py` & `imt_ikarus-1.2.0/src/ikarus/test_src.py`

 * *Files identical despite different names*

### Comparing `imt_ikarus-1.1.2/src/ikarus/test_utils.py` & `imt_ikarus-1.2.0/src/ikarus/test_utils.py`

 * *Files identical despite different names*

### Comparing `imt_ikarus-1.1.2/src/ikarus/utils.py` & `imt_ikarus-1.2.0/src/ikarus/utils.py`

 * *Files identical despite different names*

### Comparing `imt_ikarus-1.1.2/src/imt_ikarus.egg-info/PKG-INFO` & `imt_ikarus-1.2.0/src/imt_ikarus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imt-ikarus
-Version: 1.1.2
+Version: 1.2.0
 Summary: IKArus - Inertial and Optical Data of Kinematic ChAin Motion
 Author-email: Simon Bachhuber <simon.bachhuber@fau.de>
 Project-URL: Homepage, https://github.com/SimiPixel/ikarus
 Project-URL: Issues, https://github.com/SimiPixel/ikarus/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `imt_ikarus-1.1.2/src/imt_ikarus.egg-info/SOURCES.txt` & `imt_ikarus-1.2.0/src/imt_ikarus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

