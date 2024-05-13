# Comparing `tmp/submititnow-0.9.5.tar.gz` & `tmp/submititnow-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "submititnow-0.9.5.tar", last modified: Tue Dec  5 18:22:46 2023, max compression
+gzip compressed data, was "submititnow-0.9.6.tar", last modified: Mon May 13 10:35:07 2024, max compression
```

## Comparing `submititnow-0.9.5.tar` & `submititnow-0.9.6.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 18:22:46.867682 submititnow-0.9.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2023-12-05 18:22:41.000000 submititnow-0.9.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6973 2023-12-05 18:22:46.863682 submititnow-0.9.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5431 2023-12-05 18:22:41.000000 submititnow-0.9.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 18:22:46.863682 submititnow-0.9.5/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)     5166 2023-12-05 18:22:41.000000 submititnow-0.9.5/bin/jt
--rwxr-xr-x   0 runner    (1001) docker     (127)     2071 2023-12-05 18:22:41.000000 submititnow-0.9.5/bin/py-srun
--rwxr-xr-x   0 runner    (1001) docker     (127)     4629 2023-12-05 18:22:41.000000 submititnow-0.9.5/bin/slaunch
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-05 18:22:46.867682 submititnow-0.9.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      973 2023-12-05 18:22:41.000000 submititnow-0.9.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 18:22:46.863682 submititnow-0.9.5/submititnow/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2023-12-05 18:22:41.000000 submititnow-0.9.5/submititnow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3866 2023-12-05 18:22:41.000000 submititnow-0.9.5/submititnow/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4795 2023-12-05 18:22:41.000000 submititnow-0.9.5/submititnow/experiment_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 18:22:46.863682 submititnow-0.9.5/submititnow/jt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-05 18:22:41.000000 submititnow-0.9.5/submititnow/jt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2023-12-05 18:22:41.000000 submititnow-0.9.5/submititnow/jt/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4819 2023-12-05 18:22:41.000000 submititnow-0.9.5/submititnow/options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 18:22:46.863682 submititnow-0.9.5/submititnow/umiacs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-05 18:22:41.000000 submititnow-0.9.5/submititnow/umiacs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2023-12-05 18:22:41.000000 submititnow-0.9.5/submititnow/umiacs/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 18:22:46.863682 submititnow-0.9.5/submititnow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6973 2023-12-05 18:22:46.000000 submititnow-0.9.5/submititnow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      440 2023-12-05 18:22:46.000000 submititnow-0.9.5/submititnow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-05 18:22:46.000000 submititnow-0.9.5/submititnow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      105 2023-12-05 18:22:46.000000 submititnow-0.9.5/submititnow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-12-05 18:22:46.000000 submititnow-0.9.5/submititnow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:35:07.588326 submititnow-0.9.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-13 10:35:04.000000 submititnow-0.9.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6973 2024-05-13 10:35:07.588326 submititnow-0.9.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5431 2024-05-13 10:35:04.000000 submititnow-0.9.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:35:07.584325 submititnow-0.9.6/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5166 2024-05-13 10:35:04.000000 submititnow-0.9.6/bin/jt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2071 2024-05-13 10:35:04.000000 submititnow-0.9.6/bin/py-srun
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4629 2024-05-13 10:35:04.000000 submititnow-0.9.6/bin/slaunch
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 10:35:07.588326 submititnow-0.9.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-13 10:35:04.000000 submititnow-0.9.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:35:07.588326 submititnow-0.9.6/submititnow/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-13 10:35:04.000000 submititnow-0.9.6/submititnow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-05-13 10:35:04.000000 submititnow-0.9.6/submititnow/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5096 2024-05-13 10:35:04.000000 submititnow-0.9.6/submititnow/experiment_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-13 10:35:04.000000 submititnow-0.9.6/submititnow/experiment_lib_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:35:07.588326 submititnow-0.9.6/submititnow/jt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 10:35:04.000000 submititnow-0.9.6/submititnow/jt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-05-13 10:35:04.000000 submititnow-0.9.6/submititnow/jt/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-05-13 10:35:04.000000 submititnow-0.9.6/submititnow/options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:35:07.588326 submititnow-0.9.6/submititnow/umiacs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 10:35:04.000000 submititnow-0.9.6/submititnow/umiacs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-13 10:35:04.000000 submititnow-0.9.6/submititnow/umiacs/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:35:07.588326 submititnow-0.9.6/submititnow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6973 2024-05-13 10:35:07.000000 submititnow-0.9.6/submititnow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-13 10:35:07.000000 submititnow-0.9.6/submititnow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 10:35:07.000000 submititnow-0.9.6/submititnow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-13 10:35:07.000000 submititnow-0.9.6/submititnow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-13 10:35:07.000000 submititnow-0.9.6/submititnow.egg-info/top_level.txt
```

### Comparing `submititnow-0.9.5/LICENSE` & `submititnow-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `submititnow-0.9.5/PKG-INFO` & `submititnow-0.9.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: submititnow
-Version: 0.9.5
+Version: 0.9.6
 Summary: A package to make submitit easier to use
 Home-page: https://github.com/maharshi95/submititnow
 Author: Maharshi Gor
 Author-email: maharshigor@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/maharshi95/submititnow/issues
 Description: # :rocket: Submit it Now! :rocket:
```

### Comparing `submititnow-0.9.5/README.md` & `submititnow-0.9.6/README.md`

 * *Files identical despite different names*

### Comparing `submititnow-0.9.5/bin/jt` & `submititnow-0.9.6/bin/jt`

 * *Files identical despite different names*

### Comparing `submititnow-0.9.5/bin/py-srun` & `submititnow-0.9.6/bin/py-srun`

 * *Files identical despite different names*

### Comparing `submititnow-0.9.5/bin/slaunch` & `submititnow-0.9.6/bin/slaunch`

 * *Files identical despite different names*

### Comparing `submititnow-0.9.5/setup.py` & `submititnow-0.9.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 packages = filter(lambda x: x.startswith("submititnow"), setuptools.find_packages())
 
 setuptools.setup(
     name="submititnow",
-    version="0.9.5",
+    version="0.9.6",
     author="Maharshi Gor",
     author_email="maharshigor@gmail.com",
     description="A package to make submitit easier to use",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/maharshi95/submititnow",
     project_urls={
```

### Comparing `submititnow-0.9.5/submititnow/cli.py` & `submititnow-0.9.6/submititnow/cli.py`

 * *Files identical despite different names*

### Comparing `submititnow-0.9.5/submititnow/experiment_lib.py` & `submititnow-0.9.6/submititnow/experiment_lib.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,45 @@
 import argparse
 import datetime as dt
 from pathlib import Path
-from typing import List, Iterable, Optional, Callable, Any, Dict
+from typing import List, Iterable, Optional, Callable, Any, Dict, Sequence
 
 import submitit
 
 from submititnow import cli
 from submititnow.jt import utils
 
 
 def _job_start_time(job: submitit.Job):
     return dt.datetime.fromtimestamp(job._start_time)
 
 
+def _extract_common_params(
+    list_of_params: Sequence[argparse.Namespace],
+) -> Dict[str, Any]:
+    if not list_of_params:
+        return {}
+
+    common_params = vars(list_of_params[0])
+    for params in list_of_params[1:]:
+        params = vars(params)
+        for k, v in tuple(common_params.items()):
+            if k not in params or v != params[k]:
+                del common_params[k]
+        if not common_params:
+            break
+    return common_params
+
+
 class Experiment:
     def __init__(
         self,
         name: str,
         job_func: Callable,
-        job_params: Iterable[argparse.Namespace],
+        job_params: Sequence[argparse.Namespace],
         job_desc_function: Optional[Callable] = None,
         submititnow_dir: Optional[str] = None,
     ):
         self.submititnow_dir = (
             Path(submititnow_dir) if submititnow_dir else utils.SUBMITITNOW_ROOT_DIR
         )
         self.exp_name = name
@@ -33,19 +50,15 @@
         self.job_descriptions = {}
         self.profile_handlers = {}
 
     @property
     def job_function_description(self):
         func_name = self.job_func.__module__ + "." + self.job_func.__qualname__
 
-        common_params = vars(self.job_params[0])
-        for param in self.job_params[1:]:
-            for k, v in vars(param).items():
-                if k in common_params and v != common_params[k]:
-                    del common_params[k]
+        common_params = _extract_common_params(self.job_params)
 
         tokens = []
         for k, v in common_params.items():
             token = f"{k}='{v}'" if isinstance(v, str) else f"{k}={v}"
             tokens.append(token)
         return f"{func_name}( {', '.join(tokens)} )"
```

### Comparing `submititnow-0.9.5/submititnow/jt/utils.py` & `submititnow-0.9.6/submititnow/jt/utils.py`

 * *Files identical despite different names*

### Comparing `submititnow-0.9.5/submititnow/options.py` & `submititnow-0.9.6/submititnow/options.py`

 * *Files identical despite different names*

### Comparing `submititnow-0.9.5/submititnow/umiacs/handlers.py` & `submititnow-0.9.6/submititnow/umiacs/handlers.py`

 * *Files identical despite different names*

### Comparing `submititnow-0.9.5/submititnow.egg-info/PKG-INFO` & `submititnow-0.9.6/submititnow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: submititnow
-Version: 0.9.5
+Version: 0.9.6
 Summary: A package to make submitit easier to use
 Home-page: https://github.com/maharshi95/submititnow
 Author: Maharshi Gor
 Author-email: maharshigor@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/maharshi95/submititnow/issues
 Description: # :rocket: Submit it Now! :rocket:
```

