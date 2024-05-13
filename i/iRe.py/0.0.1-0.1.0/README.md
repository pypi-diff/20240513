# Comparing `tmp/iRe.py-0.0.1.tar.gz` & `tmp/iRe.py-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iRe.py-0.0.1.tar", last modified: Mon Apr  1 00:15:03 2024, max compression
+gzip compressed data, was "iRe.py-0.1.0.tar", last modified: Mon May 13 02:05:39 2024, max compression
```

## Comparing `iRe.py-0.0.1.tar` & `iRe.py-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 00:15:03.642484 iRe.py-0.0.1/
--rw-rw-rw-   0 root         (0) root         (0)     1061 2024-04-01 00:14:47.000000 iRe.py-0.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      920 2024-04-01 00:15:03.642484 iRe.py-0.0.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      514 2024-04-01 00:14:47.000000 iRe.py-0.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 00:15:03.641568 iRe.py-0.0.1/iRe.py.egg-info/
--rw-r--r--   0 root         (0) root         (0)      920 2024-04-01 00:15:03.000000 iRe.py-0.0.1/iRe.py.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      237 2024-04-01 00:15:03.000000 iRe.py-0.0.1/iRe.py.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-01 00:15:03.000000 iRe.py-0.0.1/iRe.py.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      195 2024-04-01 00:15:03.000000 iRe.py-0.0.1/iRe.py.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2024-04-01 00:15:03.000000 iRe.py-0.0.1/iRe.py.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 00:15:03.642484 iRe.py-0.0.1/ire/
--rw-rw-rw-   0 root         (0) root         (0)       38 2024-04-01 00:14:47.000000 iRe.py-0.0.1/ire/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      790 2024-04-01 00:14:47.000000 iRe.py-0.0.1/ire/dvc.py
--rw-rw-rw-   0 root         (0) root         (0)     2613 2024-04-01 00:14:47.000000 iRe.py-0.0.1/ire/git.py
--rw-rw-rw-   0 root         (0) root         (0)     6337 2024-04-01 00:14:47.000000 iRe.py-0.0.1/ire/ire.py
--rw-rw-rw-   0 root         (0) root         (0)     1747 2024-04-01 00:14:47.000000 iRe.py-0.0.1/ire/utils.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-01 00:15:03.642484 iRe.py-0.0.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      677 2024-04-01 00:14:47.000000 iRe.py-0.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 02:05:39.180495 iRe.py-0.1.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1061 2024-05-13 02:05:22.000000 iRe.py-0.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      920 2024-05-13 02:05:39.180495 iRe.py-0.1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      514 2024-05-13 02:05:22.000000 iRe.py-0.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 02:05:39.178495 iRe.py-0.1.0/iRe.py.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      920 2024-05-13 02:05:39.000000 iRe.py-0.1.0/iRe.py.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      237 2024-05-13 02:05:39.000000 iRe.py-0.1.0/iRe.py.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-13 02:05:39.000000 iRe.py-0.1.0/iRe.py.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      195 2024-05-13 02:05:39.000000 iRe.py-0.1.0/iRe.py.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2024-05-13 02:05:39.000000 iRe.py-0.1.0/iRe.py.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 02:05:39.179495 iRe.py-0.1.0/ire/
+-rw-rw-rw-   0 root         (0) root         (0)       61 2024-05-13 02:05:22.000000 iRe.py-0.1.0/ire/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      790 2024-05-13 02:05:22.000000 iRe.py-0.1.0/ire/dvc.py
+-rw-rw-rw-   0 root         (0) root         (0)     2613 2024-05-13 02:05:22.000000 iRe.py-0.1.0/ire/git.py
+-rw-rw-rw-   0 root         (0) root         (0)     6447 2024-05-13 02:05:22.000000 iRe.py-0.1.0/ire/ire.py
+-rw-rw-rw-   0 root         (0) root         (0)     1747 2024-05-13 02:05:22.000000 iRe.py-0.1.0/ire/utils.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-13 02:05:39.180495 iRe.py-0.1.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      677 2024-05-13 02:05:22.000000 iRe.py-0.1.0/setup.py
```

### Comparing `iRe.py-0.0.1/LICENSE` & `iRe.py-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `iRe.py-0.0.1/PKG-INFO` & `iRe.py-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iRe.py
-Version: 0.0.1
+Version: 0.1.0
 Summary: Export tables and plots from Jupyter notebooks, along with metadata for embedding interactive tables in downstream apps.
 Home-page: https://gitlab.com/runsascoded/ire/py
 Author: Ryan Williams
 Author-email: ryan@runsascoded.com
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: plotly
```

### Comparing `iRe.py-0.0.1/README.md` & `iRe.py-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `iRe.py-0.0.1/iRe.py.egg-info/PKG-INFO` & `iRe.py-0.1.0/iRe.py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iRe.py
-Version: 0.0.1
+Version: 0.1.0
 Summary: Export tables and plots from Jupyter notebooks, along with metadata for embedding interactive tables in downstream apps.
 Home-page: https://gitlab.com/runsascoded/ire/py
 Author: Ryan Williams
 Author-email: ryan@runsascoded.com
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: plotly
```

### Comparing `iRe.py-0.0.1/ire/dvc.py` & `iRe.py-0.1.0/ire/dvc.py`

 * *Files identical despite different names*

### Comparing `iRe.py-0.0.1/ire/git.py` & `iRe.py-0.1.0/ire/git.py`

 * *Files identical despite different names*

### Comparing `iRe.py-0.0.1/ire/ire.py` & `iRe.py-0.1.0/ire/ire.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 import os
 from dataclasses import dataclass
 from inspect import getfullargspec
 from os import getcwd, makedirs, rename
-from os.path import exists, islink, join
-import shlex
-import sys
+from os.path import islink, join
 from tempfile import TemporaryDirectory
 from typing import Literal, Optional, Union, TypeVar, Callable
-from utz import process
 
 import pandas as pd
 from IPython.display import display, HTML, Image
 from utz import err
 
 from ire.dvc import DvcConfig, is_dvc_repo, process_dvc_config
-from ire.git import CommitConfig, GitConfig, has_unpushed_commits, PushConfig, process_git_config
+from ire.git import GitConfig, has_unpushed_commits, process_git_config
 from ire.utils import md5_file, run
 
+
 DEFAULT_ARTIFACTS_DIR = ".ire"
 METADATA_KEY = 'iRe'
 
 ParquetEngine = Optional[Literal['fastparquet', 'pyarrow', 'auto']]
 
 
 @dataclass
@@ -41,21 +39,28 @@
 @dataclass
 class Output:
     path: str
     md5: str
 
 
 Fmt = Union[Literal['parquet'], Literal['plotly'], Literal['png']]
+ShowPlot = Union[None, 'png', 'html']
+
 
 T = TypeVar("T")
 DEFAULT_EXTENSION_OVERRIDES = {
     'plotly': 'json',
 }
 
 
+def chdir(path):
+    os.chdir(path)
+    config.dir = join(path, DEFAULT_ARTIFACTS_DIR)
+
+
 def write_obj(
         obj: T,
         write: Callable,
         fmt: Fmt,
         name: str = None,
         dir: str = DEFAULT_ARTIFACTS_DIR,
         extension: str = None,
@@ -122,26 +127,28 @@
         f.write(fig_json)
 
 
 def write_matplotlib(fig: 'plt.Figure', path: str):
     fig.savefig(path)
 
 
-def maybe_handle_plotly(obj, kwargs, show: Optional[Literal['png']] = None):
+def maybe_handle_plotly(obj, kwargs, show: ShowPlot = None):
     try:
         from plotly.graph_objs import Figure
         if isinstance(obj, Figure):
             fig = obj
             metadata = write_obj(fig, write=write_plotly, fmt='plotly', **kwargs)
             if show == 'png':
                 img_bytes = fig.to_image(format='png')
                 display(Image(img_bytes), metadata=metadata)
-            else:
+            elif show == 'html':
                 html = fig.to_html()
                 display(HTML(html), metadata=metadata)
+            else:
+                display(fig, metadata=metadata)
             return True
     except ImportError:
         pass
     return False
 
 
 def maybe_handle_matplotlib(obj, kwargs):
@@ -161,25 +168,25 @@
 def export(
         obj,
         name: str = None,
         dir: str = None,
         git: Optional[GitConfig] = None,
         dvc: Optional[DvcConfig] = None,
         verbose: bool = False,
-        show: Optional[Literal['png']] = None,
+        show: ShowPlot = None,
         engine: ParquetEngine = None,
 ):
     if git is None:
         git = config.git
     if dvc is None:
         dvc = config.dvc
     if dir is None:
         dir = config.dir
     if show:
-        if show != 'png':
+        if show not in ['html', 'png']:
             raise ValueError(f"Unrecognized `show` param: {show}")
 
     kwargs = dict(dir=dir, name=name, git=git, dvc=dvc, verbose=verbose)
     if isinstance(obj, pd.DataFrame):
         df = obj
         metadata = write_obj(obj=obj, write=write_parquet, fmt='parquet', **kwargs)
         html = df._repr_html_()
```

### Comparing `iRe.py-0.0.1/ire/utils.py` & `iRe.py-0.1.0/ire/utils.py`

 * *Files identical despite different names*

### Comparing `iRe.py-0.0.1/setup.py` & `iRe.py-0.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="iRe.py",
-    version="0.0.1",
+    version="0.1.0",
     description="Export tables and plots from Jupyter notebooks, along with metadata for embedding interactive tables in downstream apps.",
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=open("requirements.txt", "r").read(),
     extras_require={
         "plotly": "plotly",
```

