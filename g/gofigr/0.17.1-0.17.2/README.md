# Comparing `tmp/gofigr-0.17.1.tar.gz` & `tmp/gofigr-0.17.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gofigr-0.17.1.tar", last modified: Wed Mar 27 01:47:18 2024, max compression
+gzip compressed data, was "gofigr-0.17.2.tar", last modified: Mon May 13 18:07:35 2024, max compression
```

## Comparing `gofigr-0.17.1.tar` & `gofigr-0.17.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-27 01:47:18.447345 gofigr-0.17.1/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      436 2024-03-27 01:30:21.000000 gofigr-0.17.1/CHANGELOG.rst
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1078 2024-03-27 01:30:21.000000 gofigr-0.17.1/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      194 2024-03-27 01:30:21.000000 gofigr-0.17.1/MANIFEST.in
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9058 2024-03-27 01:47:18.447345 gofigr-0.17.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6196 2024-03-27 01:30:21.000000 gofigr-0.17.1/README.rst
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-27 01:47:18.439345 gofigr-0.17.1/gofigr/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16161 2024-03-27 01:30:21.000000 gofigr-0.17.1/gofigr/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6837 2024-03-27 01:30:21.000000 gofigr-0.17.1/gofigr/annotators.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-27 01:47:18.439345 gofigr-0.17.1/gofigr/backends/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4141 2024-03-27 01:30:21.000000 gofigr-0.17.1/gofigr/backends/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2270 2024-03-27 01:30:21.000000 gofigr-0.17.1/gofigr/backends/matplotlib.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3109 2024-03-27 01:30:21.000000 gofigr-0.17.1/gofigr/backends/plotly.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4445 2024-03-27 01:30:21.000000 gofigr-0.17.1/gofigr/backends/py3dmol.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      918 2024-03-27 01:30:21.000000 gofigr-0.17.1/gofigr/context.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6127 2024-03-27 01:30:21.000000 gofigr-0.17.1/gofigr/gfconfig.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    33720 2024-03-27 01:30:21.000000 gofigr-0.17.1/gofigr/jupyter.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    51302 2024-03-27 01:30:21.000000 gofigr-0.17.1/gofigr/models.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      933 2024-03-27 01:30:21.000000 gofigr-0.17.1/gofigr/profile.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3367 2024-03-27 01:30:21.000000 gofigr-0.17.1/gofigr/proxy.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-27 01:47:18.443345 gofigr-0.17.1/gofigr/resources/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   584424 2024-03-27 01:30:21.000000 gofigr-0.17.1/gofigr/resources/FreeMono.ttf
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       76 2024-03-27 01:30:21.000000 gofigr-0.17.1/gofigr/resources/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      944 2024-03-27 01:30:21.000000 gofigr-0.17.1/gofigr/resources/copy_image.js
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      491 2024-03-27 01:30:21.000000 gofigr-0.17.1/gofigr/resources/copy_text.js
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-27 01:30:21.000000 gofigr-0.17.1/gofigr/resources/gofigr.css
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      660 2024-03-27 01:30:21.000000 gofigr-0.17.1/gofigr/resources/loader.js
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9441 2024-03-27 01:30:21.000000 gofigr-0.17.1/gofigr/resources/logo_small.png
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      874 2024-03-27 01:30:21.000000 gofigr-0.17.1/gofigr/utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5487 2024-03-27 01:30:21.000000 gofigr-0.17.1/gofigr/watermarks.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12793 2024-03-27 01:30:21.000000 gofigr-0.17.1/gofigr/widget.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-27 01:47:18.443345 gofigr-0.17.1/gofigr.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9058 2024-03-27 01:47:18.000000 gofigr-0.17.1/gofigr.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      890 2024-03-27 01:47:18.000000 gofigr-0.17.1/gofigr.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-03-27 01:47:18.000000 gofigr-0.17.1/gofigr.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       50 2024-03-27 01:47:18.000000 gofigr-0.17.1/gofigr.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      306 2024-03-27 01:47:18.000000 gofigr-0.17.1/gofigr.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        7 2024-03-27 01:47:18.000000 gofigr-0.17.1/gofigr.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1708 2024-03-27 01:30:21.000000 gofigr-0.17.1/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-03-27 01:47:18.451345 gofigr-0.17.1/setup.cfg
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-27 01:47:18.443345 gofigr-0.17.1/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    53162 2024-03-27 01:30:21.000000 gofigr-0.17.1/tests/test_client.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7062 2024-03-27 01:30:21.000000 gofigr-0.17.1/tests/test_invites.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1609 2024-03-27 01:30:21.000000 gofigr-0.17.1/tests/test_logs.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3117 2024-03-27 01:30:21.000000 gofigr-0.17.1/tests/test_metadata.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3130 2024-03-27 01:30:21.000000 gofigr-0.17.1/tests/test_models.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1007 2024-03-27 01:30:21.000000 gofigr-0.17.1/tests/test_watermarks.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-13 18:07:35.047089 gofigr-0.17.2/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      436 2024-05-13 17:50:42.000000 gofigr-0.17.2/CHANGELOG.rst
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1078 2024-05-13 17:50:42.000000 gofigr-0.17.2/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      194 2024-05-13 17:50:42.000000 gofigr-0.17.2/MANIFEST.in
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9058 2024-05-13 18:07:35.047089 gofigr-0.17.2/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6196 2024-05-13 17:50:42.000000 gofigr-0.17.2/README.rst
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-13 18:07:35.035089 gofigr-0.17.2/gofigr/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16161 2024-05-13 17:50:42.000000 gofigr-0.17.2/gofigr/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7855 2024-05-13 17:50:42.000000 gofigr-0.17.2/gofigr/annotators.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-13 18:07:35.039089 gofigr-0.17.2/gofigr/backends/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4141 2024-05-13 17:50:42.000000 gofigr-0.17.2/gofigr/backends/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2568 2024-05-13 17:50:42.000000 gofigr-0.17.2/gofigr/backends/matplotlib.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3138 2024-05-13 17:50:42.000000 gofigr-0.17.2/gofigr/backends/plotly.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4445 2024-05-13 17:50:42.000000 gofigr-0.17.2/gofigr/backends/py3dmol.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      918 2024-05-13 17:50:42.000000 gofigr-0.17.2/gofigr/context.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6127 2024-05-13 17:50:42.000000 gofigr-0.17.2/gofigr/gfconfig.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    33720 2024-05-13 17:50:42.000000 gofigr-0.17.2/gofigr/jupyter.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    51302 2024-05-13 17:50:42.000000 gofigr-0.17.2/gofigr/models.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      933 2024-05-13 17:50:42.000000 gofigr-0.17.2/gofigr/profile.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3367 2024-05-13 17:50:42.000000 gofigr-0.17.2/gofigr/proxy.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-13 18:07:35.043089 gofigr-0.17.2/gofigr/resources/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   584424 2024-05-13 17:50:42.000000 gofigr-0.17.2/gofigr/resources/FreeMono.ttf
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       76 2024-05-13 17:50:42.000000 gofigr-0.17.2/gofigr/resources/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      944 2024-05-13 17:50:42.000000 gofigr-0.17.2/gofigr/resources/copy_image.js
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      491 2024-05-13 17:50:42.000000 gofigr-0.17.2/gofigr/resources/copy_text.js
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-13 17:50:42.000000 gofigr-0.17.2/gofigr/resources/gofigr.css
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      892 2024-05-13 17:50:42.000000 gofigr-0.17.2/gofigr/resources/loader.js
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9441 2024-05-13 17:50:42.000000 gofigr-0.17.2/gofigr/resources/logo_small.png
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      874 2024-05-13 17:50:42.000000 gofigr-0.17.2/gofigr/utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5487 2024-05-13 17:50:42.000000 gofigr-0.17.2/gofigr/watermarks.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12793 2024-05-13 17:50:42.000000 gofigr-0.17.2/gofigr/widget.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-13 18:07:35.043089 gofigr-0.17.2/gofigr.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9058 2024-05-13 18:07:35.000000 gofigr-0.17.2/gofigr.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      890 2024-05-13 18:07:35.000000 gofigr-0.17.2/gofigr.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-13 18:07:35.000000 gofigr-0.17.2/gofigr.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       50 2024-05-13 18:07:35.000000 gofigr-0.17.2/gofigr.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      306 2024-05-13 18:07:35.000000 gofigr-0.17.2/gofigr.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        7 2024-05-13 18:07:35.000000 gofigr-0.17.2/gofigr.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1708 2024-05-13 17:50:42.000000 gofigr-0.17.2/pyproject.toml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-13 18:07:35.047089 gofigr-0.17.2/setup.cfg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-13 18:07:35.043089 gofigr-0.17.2/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    53162 2024-05-13 17:50:42.000000 gofigr-0.17.2/tests/test_client.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7062 2024-05-13 17:50:42.000000 gofigr-0.17.2/tests/test_invites.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1609 2024-05-13 17:50:42.000000 gofigr-0.17.2/tests/test_logs.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3117 2024-05-13 17:50:42.000000 gofigr-0.17.2/tests/test_metadata.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3130 2024-05-13 17:50:42.000000 gofigr-0.17.2/tests/test_models.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1007 2024-05-13 17:50:42.000000 gofigr-0.17.2/tests/test_watermarks.py
```

### Comparing `gofigr-0.17.1/LICENSE` & `gofigr-0.17.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gofigr-0.17.1/PKG-INFO` & `gofigr-0.17.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gofigr
-Version: 0.17.1
+Version: 0.17.2
 Summary: GoFigr client library
 Author-email: Maciej Pacula <maciej@gofigr.io>
 License: Copyright 2022-2024 Flagstaff Solutions, LLC
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the “Software”), to deal in
         the Software without restriction, including without limitation the rights to
@@ -20,15 +20,15 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
         THE SOFTWARE.
         
 Project-URL: Homepage, https://www.gofigr.io
-Project-URL: Documentation, https://gofigr.io/docs/gofigr-python/0.17.1/
+Project-URL: Documentation, https://gofigr.io/docs/gofigr-python/0.17.2/
 Keywords: science,visualization,version control,plotting,data,reproducibility
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
@@ -64,15 +64,15 @@
 Requires-Dist: py3Dmol; extra == "dev"
 Requires-Dist: html2image; extra == "dev"
 Requires-Dist: teamcity-messages; extra == "dev"
 
 .. figure:: docs/source/images/logo_wide_light.png
   :alt: GoFigr.io logo
 
-GoFigr - Python Client (0.17.1)
+GoFigr - Python Client (0.17.2)
 ====================================
 GoFigr (https://www.gofigr.io) is a service which provides sophisticated version control for figures.
 
 This repository contains the Python client for GoFigr.
 
 Account registration
 ********************
```

### Comparing `gofigr-0.17.1/README.rst` & `gofigr-0.17.2/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 .. figure:: docs/source/images/logo_wide_light.png
   :alt: GoFigr.io logo
 
-GoFigr - Python Client (0.17.1)
+GoFigr - Python Client (0.17.2)
 ====================================
 GoFigr (https://www.gofigr.io) is a service which provides sophisticated version control for figures.
 
 This repository contains the Python client for GoFigr.
 
 Account registration
 ********************
```

### Comparing `gofigr-0.17.1/gofigr/__init__.py` & `gofigr-0.17.2/gofigr/__init__.py`

 * *Files identical despite different names*

### Comparing `gofigr-0.17.1/gofigr/annotators.py` & `gofigr-0.17.2/gofigr/annotators.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """\
 Copyright (c) 2023, Flagstaff Solutions, LLC
 All rights reserved.
 
 """
 import json
 import os
+import re
 import subprocess
 import sys
 from abc import ABC
 from urllib.parse import unquote, urlparse
 
 from gofigr import CodeLanguage
 from gofigr.context import RevisionContext
@@ -108,46 +109,73 @@
 NOTEBOOK_NAME = "notebook_name"
 NOTEBOOK_URL = "url"
 NOTEBOOK_KERNEL = "kernel"
 PYTHON_VERSION = "python_version"
 BACKEND_NAME = "backend"
 
 
+_ACTIVE_TAB_TITLE = "active_tab_title"
+
+
+def _parse_path_from_tab_title(title):
+    """Parses out the notebook path from the tab/widget title"""
+    for line in title.splitlines(keepends=False):
+        m = re.match(r'Path:\s*(.*)\s*', line)
+        if m:
+            return m.group(1)
+    return None
+
+
 class NotebookMetadataAnnotator(Annotator):
     """"Annotates revisions with notebook metadata, including filename & path, as well as the full URL"""
 
     def parse_metadata(self):
         """Infers the notebook path & name from metadata passed through the WebSocket (if available)"""
         meta = self.extension.notebook_metadata
         if meta is None:
             raise RuntimeError("No Notebook metadata available")
-        if 'url' not in meta:
+        if 'url' not in meta and _ACTIVE_TAB_TITLE not in meta:
             raise RuntimeError("No URL found in Notebook metadata")
 
-        notebook_name = unquote(urlparse(meta['url']).path.rsplit('/', 1)[-1])
+        notebook_name = None
+
+        # Try parsing the name from the title first
+        if _ACTIVE_TAB_TITLE in meta and meta[_ACTIVE_TAB_TITLE] is not None:
+            notebook_name = _parse_path_from_tab_title(meta[_ACTIVE_TAB_TITLE])
+
+        # If that doesn't work, try the URL
+        if notebook_name is None:
+            notebook_name = unquote(urlparse(meta['url']).path.rsplit('/', 1)[-1])
+
         notebook_dir = self.extension.shell.starting_dir
-        full_path = os.path.join(notebook_dir, notebook_name)
+        full_path = None
+
+        for candidate_path in [os.path.join(notebook_dir, notebook_name),
+                               os.path.join(os.path.dirname(notebook_dir), notebook_name)]:
+            if os.path.exists(candidate_path):
+                full_path = candidate_path
 
-        if not os.path.exists(full_path):
+        if full_path is None:
+            full_path = os.path.join(notebook_dir, notebook_name)  # might still be helpful, even if slightly incorrect
             print(f"The inferred path for the notebook does not exist: {full_path}. {PATH_WARNING}", file=sys.stderr)
 
         return {NOTEBOOK_PATH: full_path,
                 NOTEBOOK_NAME: notebook_name,
                 NOTEBOOK_URL: meta.get('url')}
 
     def annotate(self, revision):
         if revision.metadata is None:
             revision.metadata = {}
 
         try:
             if NOTEBOOK_NAME not in revision.metadata or NOTEBOOK_PATH not in revision.metadata:
                 revision.metadata.update(self.parse_metadata())
-        except Exception:  # pylint: disable=broad-exception-caught
+        except Exception as e:  # pylint: disable=broad-exception-caught
             print(f"GoFigr could not automatically obtain the name of the currently"
-                  f" running notebook. {PATH_WARNING}",
+                  f" running notebook. {PATH_WARNING} Details: {e}",
                   file=sys.stderr)
 
             revision.metadata[NOTEBOOK_NAME] = "N/A"
             revision.metadata[NOTEBOOK_PATH] = "N/A"
 
         return revision
```

### Comparing `gofigr-0.17.1/gofigr/backends/__init__.py` & `gofigr-0.17.2/gofigr/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `gofigr-0.17.1/gofigr/backends/matplotlib.py` & `gofigr-0.17.2/gofigr/backends/matplotlib.py`

 * *Files 8% similar despite different names*

```diff
@@ -60,16 +60,25 @@
             return suptitle
         elif title is not None and title.strip() != "":
             return title
         else:
             return None
 
     def figure_to_bytes(self, fig, fmt, params):
+
+        plt_log = getattr(plt, "_log")
+        log_level = getattr(plt_log, "level") if plt_log is not None else None
+
         bio = io.BytesIO()
-        fig.savefig(bio, format=fmt, **params)
+        try:
+            plt.set_loglevel("error")
+            fig.savefig(bio, format=fmt, **params)
+        finally:
+            if plt_log is not None and log_level is not None:
+                plt_log.setLevel(log_level)
 
         bio.seek(0)
         return bio.read()
 
     def close(self, fig):
         plt.close(fig)
```

### Comparing `gofigr-0.17.1/gofigr/backends/plotly.py` & `gofigr-0.17.2/gofigr/backends/plotly.py`

 * *Files 5% similar despite different names*

```diff
@@ -74,15 +74,16 @@
 
         wfig = go.Figure(fig)
         wfig.update_layout(margin=dict(l=0, r=0, t=margin, b=margin))
         wfig.update_layout(height=new_height)
 
         wfig.add_annotation(dict(font=dict(color='black', size=15),
                                  x=0,
-                                 y=-margin / orig_height,
+                                 y=0,
+                                 yshift=-margin,
                                  showarrow=False,
                                  text=f"<a href='{rev.revision_url}'>{rev.revision_url}</a>",
                                  textangle=0,
                                  xanchor='left',
                                  xref="paper",
                                  yref="paper"))
```

### Comparing `gofigr-0.17.1/gofigr/backends/py3dmol.py` & `gofigr-0.17.2/gofigr/backends/py3dmol.py`

 * *Files identical despite different names*

### Comparing `gofigr-0.17.1/gofigr/context.py` & `gofigr-0.17.2/gofigr/context.py`

 * *Files identical despite different names*

### Comparing `gofigr-0.17.1/gofigr/gfconfig.py` & `gofigr-0.17.2/gofigr/gfconfig.py`

 * *Files identical despite different names*

### Comparing `gofigr-0.17.1/gofigr/jupyter.py` & `gofigr-0.17.2/gofigr/jupyter.py`

 * *Files identical despite different names*

### Comparing `gofigr-0.17.1/gofigr/models.py` & `gofigr-0.17.2/gofigr/models.py`

 * *Files identical despite different names*

### Comparing `gofigr-0.17.1/gofigr/profile.py` & `gofigr-0.17.2/gofigr/profile.py`

 * *Files identical despite different names*

### Comparing `gofigr-0.17.1/gofigr/proxy.py` & `gofigr-0.17.2/gofigr/proxy.py`

 * *Files identical despite different names*

### Comparing `gofigr-0.17.1/gofigr/resources/FreeMono.ttf` & `gofigr-0.17.2/gofigr/resources/FreeMono.ttf`

 * *Files identical despite different names*

### Comparing `gofigr-0.17.1/gofigr/resources/copy_image.js` & `gofigr-0.17.2/gofigr/resources/copy_image.js`

 * *Files identical despite different names*

### Comparing `gofigr-0.17.1/gofigr/resources/logo_small.png` & `gofigr-0.17.2/gofigr/resources/logo_small.png`

 * *Files identical despite different names*

### Comparing `gofigr-0.17.1/gofigr/utils.py` & `gofigr-0.17.2/gofigr/utils.py`

 * *Files identical despite different names*

### Comparing `gofigr-0.17.1/gofigr/watermarks.py` & `gofigr-0.17.2/gofigr/watermarks.py`

 * *Files identical despite different names*

### Comparing `gofigr-0.17.1/gofigr/widget.py` & `gofigr-0.17.2/gofigr/widget.py`

 * *Files identical despite different names*

### Comparing `gofigr-0.17.1/gofigr.egg-info/PKG-INFO` & `gofigr-0.17.2/gofigr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gofigr
-Version: 0.17.1
+Version: 0.17.2
 Summary: GoFigr client library
 Author-email: Maciej Pacula <maciej@gofigr.io>
 License: Copyright 2022-2024 Flagstaff Solutions, LLC
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the “Software”), to deal in
         the Software without restriction, including without limitation the rights to
@@ -20,15 +20,15 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
         THE SOFTWARE.
         
 Project-URL: Homepage, https://www.gofigr.io
-Project-URL: Documentation, https://gofigr.io/docs/gofigr-python/0.17.1/
+Project-URL: Documentation, https://gofigr.io/docs/gofigr-python/0.17.2/
 Keywords: science,visualization,version control,plotting,data,reproducibility
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
@@ -64,15 +64,15 @@
 Requires-Dist: py3Dmol; extra == "dev"
 Requires-Dist: html2image; extra == "dev"
 Requires-Dist: teamcity-messages; extra == "dev"
 
 .. figure:: docs/source/images/logo_wide_light.png
   :alt: GoFigr.io logo
 
-GoFigr - Python Client (0.17.1)
+GoFigr - Python Client (0.17.2)
 ====================================
 GoFigr (https://www.gofigr.io) is a service which provides sophisticated version control for figures.
 
 This repository contains the Python client for GoFigr.
 
 Account registration
 ********************
```

### Comparing `gofigr-0.17.1/gofigr.egg-info/SOURCES.txt` & `gofigr-0.17.2/gofigr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gofigr-0.17.1/pyproject.toml` & `gofigr-0.17.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gofigr"
-version = "0.17.1"
+version = "0.17.2"
 description = "GoFigr client library"
 readme = "README.rst"
 authors = [{ name = "Maciej Pacula", email = "maciej@gofigr.io" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -27,21 +27,21 @@
 [project.optional-dependencies]
 dev = ["pip-tools", "bumpver", "build", "twine", "pylint", "flake8", "sphinx", "sphinx_rtd_theme",
        "sphinxcontrib-jquery", "seaborn", "matplotlib", "tqdm", "selenium", "webdriver-manager", "openpyxl",
        "py3Dmol", "html2image", "teamcity-messages"]
 
 [project.urls]
 Homepage = "https://www.gofigr.io"
-Documentation = "https://gofigr.io/docs/gofigr-python/0.17.1/"
+Documentation = "https://gofigr.io/docs/gofigr-python/0.17.2/"
 
 [project.scripts]
 gfconfig = "gofigr.gfconfig:main"
 
 [tool.bumpver]
-current_version = "0.17.1"
+current_version = "0.17.2"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "Bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `gofigr-0.17.1/tests/test_client.py` & `gofigr-0.17.2/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `gofigr-0.17.1/tests/test_invites.py` & `gofigr-0.17.2/tests/test_invites.py`

 * *Files identical despite different names*

### Comparing `gofigr-0.17.1/tests/test_logs.py` & `gofigr-0.17.2/tests/test_logs.py`

 * *Files identical despite different names*

### Comparing `gofigr-0.17.1/tests/test_metadata.py` & `gofigr-0.17.2/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `gofigr-0.17.1/tests/test_models.py` & `gofigr-0.17.2/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `gofigr-0.17.1/tests/test_watermarks.py` & `gofigr-0.17.2/tests/test_watermarks.py`

 * *Files identical despite different names*

