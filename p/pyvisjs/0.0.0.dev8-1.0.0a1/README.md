# Comparing `tmp/pyvisjs-0.0.0.dev8.tar.gz` & `tmp/pyvisjs-1.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvisjs-0.0.0.dev8.tar", last modified: Wed May  8 18:44:57 2024, max compression
+gzip compressed data, was "pyvisjs-1.0.0a1.tar", last modified: Mon May 13 07:04:57 2024, max compression
```

## Comparing `pyvisjs-0.0.0.dev8.tar` & `pyvisjs-1.0.0a1.tar`

### file list

```diff
@@ -1,41 +1,43 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 18:44:57.489679 pyvisjs-0.0.0.dev8/
--rw-rw-rw-   0 root         (0) root         (0)     1355 2024-05-08 18:44:40.000000 pyvisjs-0.0.0.dev8/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      979 2024-05-08 18:44:40.000000 pyvisjs-0.0.0.dev8/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     4015 2024-05-08 18:44:40.000000 pyvisjs-0.0.0.dev8/CONTRIBUTING.md
--rw-rw-rw-   0 root         (0) root         (0)     1091 2024-05-08 18:44:40.000000 pyvisjs-0.0.0.dev8/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3384 2024-05-08 18:44:57.489679 pyvisjs-0.0.0.dev8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1454 2024-05-08 18:44:40.000000 pyvisjs-0.0.0.dev8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 18:44:57.484679 pyvisjs-0.0.0.dev8/examples/
--rw-rw-rw-   0 root         (0) root         (0)     8435 2024-05-08 18:44:40.000000 pyvisjs-0.0.0.dev8/examples/bluor.py
--rw-rw-rw-   0 root         (0) root         (0)      525 2024-05-08 18:44:40.000000 pyvisjs-0.0.0.dev8/examples/main.py
--rw-rw-rw-   0 root         (0) root         (0)      203 2024-05-08 18:44:40.000000 pyvisjs-0.0.0.dev8/examples/readme_usage.py
--rw-rw-rw-   0 root         (0) root         (0)      811 2024-05-08 18:44:40.000000 pyvisjs-0.0.0.dev8/folder_structure.txt
--rw-rw-rw-   0 root         (0) root         (0)      830 2024-05-08 18:44:40.000000 pyvisjs-0.0.0.dev8/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 18:44:57.485679 pyvisjs-0.0.0.dev8/pyvisjs/
--rw-rw-rw-   0 root         (0) root         (0)      103 2024-05-08 18:44:40.000000 pyvisjs-0.0.0.dev8/pyvisjs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      105 2024-05-08 18:44:40.000000 pyvisjs-0.0.0.dev8/pyvisjs/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     2018 2024-05-08 18:44:40.000000 pyvisjs-0.0.0.dev8/pyvisjs/base_dictable.py
--rw-rw-rw-   0 root         (0) root         (0)      559 2024-05-08 18:44:40.000000 pyvisjs-0.0.0.dev8/pyvisjs/edge.py
--rw-rw-rw-   0 root         (0) root         (0)     5325 2024-05-08 18:44:40.000000 pyvisjs-0.0.0.dev8/pyvisjs/network.py
--rw-rw-rw-   0 root         (0) root         (0)      577 2024-05-08 18:44:40.000000 pyvisjs-0.0.0.dev8/pyvisjs/node.py
--rw-rw-rw-   0 root         (0) root         (0)    13062 2024-05-08 18:44:40.000000 pyvisjs-0.0.0.dev8/pyvisjs/options.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 18:44:57.487679 pyvisjs-0.0.0.dev8/pyvisjs/templates/
--rw-rw-rw-   0 root         (0) root         (0)     3355 2024-05-08 18:44:40.000000 pyvisjs-0.0.0.dev8/pyvisjs/templates/basic.html
--rw-rw-rw-   0 root         (0) root         (0)     5254 2024-05-08 18:44:40.000000 pyvisjs-0.0.0.dev8/pyvisjs/templates/bs-container.html
--rw-rw-rw-   0 root         (0) root         (0)     1051 2024-05-08 18:44:40.000000 pyvisjs-0.0.0.dev8/pyvisjs/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 18:44:57.488679 pyvisjs-0.0.0.dev8/pyvisjs.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3384 2024-05-08 18:44:57.000000 pyvisjs-0.0.0.dev8/pyvisjs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      691 2024-05-08 18:44:57.000000 pyvisjs-0.0.0.dev8/pyvisjs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-08 18:44:57.000000 pyvisjs-0.0.0.dev8/pyvisjs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2024-05-08 18:44:57.000000 pyvisjs-0.0.0.dev8/pyvisjs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-05-08 18:44:57.000000 pyvisjs-0.0.0.dev8/pyvisjs.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      109 2024-05-08 18:44:40.000000 pyvisjs-0.0.0.dev8/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-08 18:44:57.489679 pyvisjs-0.0.0.dev8/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 18:44:57.488679 pyvisjs-0.0.0.dev8/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-08 18:44:40.000000 pyvisjs-0.0.0.dev8/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1921 2024-05-08 18:44:40.000000 pyvisjs-0.0.0.dev8/tests/test_base_dictable.py
--rw-rw-rw-   0 root         (0) root         (0)      994 2024-05-08 18:44:40.000000 pyvisjs-0.0.0.dev8/tests/test_edge.py
--rw-rw-rw-   0 root         (0) root         (0)     8846 2024-05-08 18:44:40.000000 pyvisjs-0.0.0.dev8/tests/test_network.py
--rw-rw-rw-   0 root         (0) root         (0)     2373 2024-05-08 18:44:40.000000 pyvisjs-0.0.0.dev8/tests/test_node.py
--rw-rw-rw-   0 root         (0) root         (0)     3863 2024-05-08 18:44:40.000000 pyvisjs-0.0.0.dev8/tests/test_options.py
--rw-rw-rw-   0 root         (0) root         (0)     2561 2024-05-08 18:44:40.000000 pyvisjs-0.0.0.dev8/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 07:04:57.204625 pyvisjs-1.0.0a1/
+-rw-rw-rw-   0 root         (0) root         (0)     1396 2024-05-13 07:04:42.000000 pyvisjs-1.0.0a1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      979 2024-05-13 07:04:42.000000 pyvisjs-1.0.0a1/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     4015 2024-05-13 07:04:42.000000 pyvisjs-1.0.0a1/CONTRIBUTING.md
+-rw-rw-rw-   0 root         (0) root         (0)     1091 2024-05-13 07:04:42.000000 pyvisjs-1.0.0a1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3381 2024-05-13 07:04:57.204625 pyvisjs-1.0.0a1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1454 2024-05-13 07:04:42.000000 pyvisjs-1.0.0a1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 07:04:57.198625 pyvisjs-1.0.0a1/examples/
+-rw-rw-rw-   0 root         (0) root         (0)     8590 2024-05-13 07:04:42.000000 pyvisjs-1.0.0a1/examples/bluor.py
+-rw-rw-rw-   0 root         (0) root         (0)      289 2024-05-13 07:04:42.000000 pyvisjs-1.0.0a1/examples/readme_usage.py
+-rw-rw-rw-   0 root         (0) root         (0)      959 2024-05-13 07:04:42.000000 pyvisjs-1.0.0a1/folder_structure.txt
+-rw-rw-rw-   0 root         (0) root         (0)      890 2024-05-13 07:04:42.000000 pyvisjs-1.0.0a1/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 07:04:57.200625 pyvisjs-1.0.0a1/pyvisjs/
+-rw-rw-rw-   0 root         (0) root         (0)      103 2024-05-13 07:04:42.000000 pyvisjs-1.0.0a1/pyvisjs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      103 2024-05-13 07:04:42.000000 pyvisjs-1.0.0a1/pyvisjs/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     2018 2024-05-13 07:04:42.000000 pyvisjs-1.0.0a1/pyvisjs/base_dictable.py
+-rw-rw-rw-   0 root         (0) root         (0)     1274 2024-05-13 07:04:42.000000 pyvisjs-1.0.0a1/pyvisjs/edge.py
+-rw-rw-rw-   0 root         (0) root         (0)     8467 2024-05-13 07:04:42.000000 pyvisjs-1.0.0a1/pyvisjs/network.py
+-rw-rw-rw-   0 root         (0) root         (0)      590 2024-05-13 07:04:42.000000 pyvisjs-1.0.0a1/pyvisjs/node.py
+-rw-rw-rw-   0 root         (0) root         (0)    13062 2024-05-13 07:04:42.000000 pyvisjs-1.0.0a1/pyvisjs/options.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 07:04:57.202625 pyvisjs-1.0.0a1/pyvisjs/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      596 2024-05-13 07:04:42.000000 pyvisjs-1.0.0a1/pyvisjs/templates/base.html
+-rw-rw-rw-   0 root         (0) root         (0)      198 2024-05-13 07:04:42.000000 pyvisjs-1.0.0a1/pyvisjs/templates/basic.html
+-rw-rw-rw-   0 root         (0) root         (0)     2064 2024-05-13 07:04:42.000000 pyvisjs-1.0.0a1/pyvisjs/templates/bs-container.html
+-rw-rw-rw-   0 root         (0) root         (0)     3812 2024-05-13 07:04:42.000000 pyvisjs-1.0.0a1/pyvisjs/templates/functions.js
+-rw-rw-rw-   0 root         (0) root         (0)      377 2024-05-13 07:04:42.000000 pyvisjs-1.0.0a1/pyvisjs/templates/select-edge-filter.html
+-rw-rw-rw-   0 root         (0) root         (0)     1051 2024-05-13 07:04:42.000000 pyvisjs-1.0.0a1/pyvisjs/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 07:04:57.204625 pyvisjs-1.0.0a1/pyvisjs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3381 2024-05-13 07:04:57.000000 pyvisjs-1.0.0a1/pyvisjs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      775 2024-05-13 07:04:57.000000 pyvisjs-1.0.0a1/pyvisjs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-13 07:04:57.000000 pyvisjs-1.0.0a1/pyvisjs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2024-05-13 07:04:57.000000 pyvisjs-1.0.0a1/pyvisjs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       28 2024-05-13 07:04:57.000000 pyvisjs-1.0.0a1/pyvisjs.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      109 2024-05-13 07:04:42.000000 pyvisjs-1.0.0a1/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-13 07:04:57.204625 pyvisjs-1.0.0a1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 07:04:57.203625 pyvisjs-1.0.0a1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-13 07:04:42.000000 pyvisjs-1.0.0a1/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1921 2024-05-13 07:04:42.000000 pyvisjs-1.0.0a1/tests/test_base_dictable.py
+-rw-rw-rw-   0 root         (0) root         (0)     1006 2024-05-13 07:04:42.000000 pyvisjs-1.0.0a1/tests/test_edge.py
+-rw-rw-rw-   0 root         (0) root         (0)    11730 2024-05-13 07:04:42.000000 pyvisjs-1.0.0a1/tests/test_network.py
+-rw-rw-rw-   0 root         (0) root         (0)     2399 2024-05-13 07:04:42.000000 pyvisjs-1.0.0a1/tests/test_node.py
+-rw-rw-rw-   0 root         (0) root         (0)     3863 2024-05-13 07:04:42.000000 pyvisjs-1.0.0a1/tests/test_options.py
+-rw-rw-rw-   0 root         (0) root         (0)     2561 2024-05-13 07:04:42.000000 pyvisjs-1.0.0a1/tests/test_utils.py
```

### Comparing `pyvisjs-0.0.0.dev8/.gitignore` & `pyvisjs-1.0.0a1/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -112,7 +112,10 @@
 # mypy
 .mypy_cache/
 .dmypy.json
 dmypy.json
 
 # Pyre type checker
 .pyre/
+
+# Node.js-specific ignores
+node_modules/
```

### Comparing `pyvisjs-0.0.0.dev8/.gitlab-ci.yml` & `pyvisjs-1.0.0a1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `pyvisjs-0.0.0.dev8/CONTRIBUTING.md` & `pyvisjs-1.0.0a1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyvisjs-0.0.0.dev8/LICENSE` & `pyvisjs-1.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvisjs-0.0.0.dev8/PKG-INFO` & `pyvisjs-1.0.0a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvisjs
-Version: 0.0.0.dev8
+Version: 1.0.0a1
 Summary: A Python wrapper for vis.js Network
 Author-email: Andrey Morozov <andrey@morozov.lv>
 License: MIT License
         
         Copyright (c) 2024 Andrey Morozov (andrey@morozov.lv)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyvisjs-0.0.0.dev8/README.md` & `pyvisjs-1.0.0a1/README.md`

 * *Files identical despite different names*

### Comparing `pyvisjs-0.0.0.dev8/examples/bluor.py` & `pyvisjs-1.0.0a1/examples/bluor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """
     git clone https://gitlab.com/22kittens/pyvisjs.git
+    cd pyvisjs
     git checkout dev
     py -m venv .venv
-    .venv\Scripts\activate
+    .venv\\Scripts\\activate
     py -m pip install -r requirements.txt
     py -m pip install pandas
     py -m pip install -e .
-    py .\examples\bluor.py
+    py .\\examples\\bluor.py
 """
 
 from pyvisjs import Network, Options
 import pandas as pd
 
 d = {
     'Partner1Node': {0: '.GB82BIYS00995636046997', 1: '~035319', 2: '~035319', 3: '~035319', 4: '~035319', 5: '$035796', 6: '$035796', 7: '+039683', 8: '+039683', 9: '$038188', 10: '$035796', 11: '$035796', 12: '$038188', 13: '$038188', 14: '$035796', 15: '$035796', 16: '$038188', 17: '.LT157044060008133181', 18: '$038188', 19: '$035796',20: '.LV02HABA0001308046643', 21: '$038188', 22: '.LV73TREL6060000300000', 23: '.LV64PARX0020150460002'}, 
@@ -129,9 +130,13 @@
         , partner1_name = row["Partner1Name"]
         , partner2_name = row["Partner2Name"]
         , country = row["Countries"]
     )
 
 
 
-net.render_template(open_in_browser=True, template_filename="bs-container.html")
+net.render_template(open_in_browser=True, 
+                    template_filename="bs-container.html", 
+                    #enable_highlighting=True, 
+                    edge_filtering=["country", "category"])
+
 #net.show("example2.html")
```

### Comparing `pyvisjs-0.0.0.dev8/folder_structure.txt` & `pyvisjs-1.0.0a1/folder_structure.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 pyvisjs-dev/
 ├── pyvisjs/
 │   ├── templates/
-│   │   └── basic.html
+│   │   ├── base.html
+│   │   ├── basic.html
+│   │   ├── bs-container.html
+│   │   ├── functions.js
+│   │   └── select-edge-filter.html
 │   ├── __init__.py
 │   ├── _version.py
 │   ├── base_dictable.py
 │   ├── edge.py
 │   ├── network.py
 │   ├── node.py
 │   ├── options.py
@@ -15,17 +19,17 @@
 │   ├── test_base_dictable.py
 │   ├── test_edge.py
 │   ├── test_network.py
 │   ├── test_node.py
 │   ├── test_options.py
 │   └── test_utils.py
 ├── examples/
-│   ├── readme_usage.py
-│   └── main.py
+│   ├── readme.py
+│   └── bluor.py
 ├── .gitignore
 ├── .gitlab-ci.yml
 ├── CONTRIBUTING.md
+├── folder_structure.txt
 ├── LICENSE
+├── pyproject.toml
 ├── README.md
-├── requirements.txt
-├── folder_structure.txt
-└── pyproject.toml
+└── requirements.txt
```

### Comparing `pyvisjs-0.0.0.dev8/pyproject.toml` & `pyvisjs-1.0.0a1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -28,8 +28,11 @@
 [project.optional-dependencies]
 test = [
     "pytest",
 ]
 all = ["pyvisjs[test]"]
 
 [tool.setuptools.dynamic]
-version = {attr = "pyvisjs._version.__version__"}
+version = {attr = "pyvisjs._version.__version__"}
+
+[tool.setuptools.packages.find]
+exclude = ["node_modules"]
```

### Comparing `pyvisjs-0.0.0.dev8/pyvisjs/base_dictable.py` & `pyvisjs-1.0.0a1/pyvisjs/base_dictable.py`

 * *Files identical despite different names*

### Comparing `pyvisjs-0.0.0.dev8/pyvisjs/node.py` & `pyvisjs-1.0.0a1/pyvisjs/node.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from .base_dictable import BaseDictable
 
 class Node(BaseDictable):
-    def __init__(self, id, label:str=None, color:str=None, shape="dot", size=None, cid=None, **kwargs):
+    def __init__(self, id:str, label:str=None, color:str=None, shape="dot", size=None, cid=None, **kwargs):
         super().__init__()
-        self.id = id
+        self.id = str(id)
         self.label = label or str(id)
         self.color = color
         self.shape = shape
         self.size = size
         self.cid = cid
 
         for key, value in kwargs.items():
             setattr(self, key, value)
 
     def __repr__(self):
-        return f"Node({self.id}, \'{self.label}\', \'{self.color}\', \'{self.shape}\', {self.size}, {self.cid})"
+        return f"Node(\'{self.id}\', \'{self.label}\', \'{self.color}\', \'{self.shape}\', {self.size}, {self.cid})"
```

### Comparing `pyvisjs-0.0.0.dev8/pyvisjs/options.py` & `pyvisjs-1.0.0a1/pyvisjs/options.py`

 * *Files identical despite different names*

### Comparing `pyvisjs-0.0.0.dev8/pyvisjs/templates/basic.html` & `pyvisjs-1.0.0a1/pyvisjs/templates/functions.js`

 * *Files 23% similar despite different names*

```diff
@@ -1,210 +1,239 @@
-00000000: 3c68 746d 6c3e 0a3c 6865 6164 3e0a 2020  <html>.<head>.  
-00000010: 2020 3c73 6372 6970 7420 7479 7065 3d22    <script type="
-00000020: 7465 7874 2f6a 6176 6173 6372 6970 7422  text/javascript"
-00000030: 2073 7263 3d22 6874 7470 733a 2f2f 756e   src="https://un
-00000040: 706b 672e 636f 6d2f 7669 732d 6e65 7477  pkg.com/vis-netw
-00000050: 6f72 6b2f 7374 616e 6461 6c6f 6e65 2f75  ork/standalone/u
-00000060: 6d64 2f76 6973 2d6e 6574 776f 726b 2e6d  md/vis-network.m
-00000070: 696e 2e6a 7322 3e3c 2f73 6372 6970 743e  in.js"></script>
-00000080: 0a0a 2020 2020 3c73 7479 6c65 2074 7970  ..    <style typ
-00000090: 653d 2274 6578 742f 6373 7322 3e0a 2020  e="text/css">.  
-000000a0: 2020 2020 2020 2376 6973 6a73 6e65 7420        #visjsnet 
-000000b0: 7b0a 2020 2020 2020 2020 2020 2020 7769  {.            wi
-000000c0: 6474 683a 207b 7b77 6964 7468 7d7d 3b0a  dth: {{width}};.
-000000d0: 2020 2020 2020 2020 2020 2020 6865 6967              heig
-000000e0: 6874 3a20 7b7b 6865 6967 6874 7d7d 3b0a  ht: {{height}};.
-000000f0: 2020 2020 2020 2020 2020 2020 626f 7264              bord
-00000100: 6572 3a20 3170 7820 736f 6c69 6420 6c69  er: 1px solid li
-00000110: 6768 7467 7261 793b 0a20 2020 2020 2020  ghtgray;.       
-00000120: 207d 0a20 2020 203c 2f73 7479 6c65 3e0a   }.    </style>.
-00000130: 3c2f 6865 6164 3e0a 0a3c 626f 6479 3e0a  </head>..<body>.
-00000140: 3c64 6976 2069 643d 2276 6973 6a73 6e65  <div id="visjsne
-00000150: 7422 3e3c 2f64 6976 3e0a 0a3c 7363 7269  t"></div>..<scri
-00000160: 7074 2074 7970 653d 2274 6578 742f 6a61  pt type="text/ja
-00000170: 7661 7363 7269 7074 223e 0a20 2020 2063  vascript">.    c
-00000180: 6f6e 7374 2064 6174 6120 3d20 6372 6561  onst data = crea
-00000190: 7465 5f6e 6574 776f 726b 2829 3b0a 2020  te_network();.  
-000001a0: 2020 6461 7461 2e6e 6574 776f 726b 2e68    data.network.h
-000001b0: 6173 5f68 6964 6465 6e5f 6e6f 6465 7320  as_hidden_nodes 
-000001c0: 3d20 6661 6c73 653b 0a20 2020 2069 6620  = false;.    if 
-000001d0: 2864 6174 612e 7079 7669 736a 732e 656e  (data.pyvisjs.en
-000001e0: 6162 6c65 5f68 6967 686c 6967 6874 696e  able_highlightin
-000001f0: 6720 3d3d 3d20 7472 7565 2920 6461 7461  g === true) data
-00000200: 2e6e 6574 776f 726b 2e6f 6e28 2263 6c69  .network.on("cli
-00000210: 636b 222c 2068 6964 655f 6e6f 745f 7365  ck", hide_not_se
-00000220: 6c65 6374 6564 5f6e 6f64 6573 293b 0a0a  lected_nodes);..
-00000230: 2020 2020 6675 6e63 7469 6f6e 2068 6964      function hid
-00000240: 655f 6e6f 745f 7365 6c65 6374 6564 5f6e  e_not_selected_n
-00000250: 6f64 6573 2865 7665 6e74 2920 7b0a 2020  odes(event) {.  
-00000260: 2020 2020 2020 2f2f 2068 6173 2073 656c        // has sel
-00000270: 6563 7465 6420 6e6f 6465 7320 6f72 2061  ected nodes or a
-00000280: 6c72 6561 6479 2068 6173 2068 6964 6465  lready has hidde
-00000290: 6e20 6e6f 6465 7320 2d20 696e 2062 6f74  n nodes - in bot
-000002a0: 6820 6361 7365 7320 7765 2068 6176 6520  h cases we have 
-000002b0: 776f 726b 2074 6f20 646f 0a20 2020 2020  work to do.     
-000002c0: 2020 2069 6620 2865 7665 6e74 2e6e 6f64     if (event.nod
-000002d0: 6573 2e6c 656e 6774 6820 3e20 3020 7c7c  es.length > 0 ||
-000002e0: 2064 6174 612e 6e65 7477 6f72 6b2e 6861   data.network.ha
-000002f0: 735f 6869 6464 656e 5f6e 6f64 6573 203d  s_hidden_nodes =
-00000300: 3d3d 2074 7275 6529 207b 0a20 2020 2020  == true) {.     
-00000310: 2020 2020 2020 206c 6574 2073 656c 6563         let selec
-00000320: 7465 644e 6f64 6573 3b0a 2020 2020 2020  tedNodes;.      
-00000330: 2020 2020 2020 2f2f 2075 7365 7220 636c        // user cl
-00000340: 6963 6b65 6420 6f75 7473 6964 6520 7468  icked outside th
-00000350: 6520 6e6f 6465 7320 6e65 7477 6f72 6b20  e nodes network 
-00000360: 2d20 7765 2077 616e 7420 746f 2075 6e68  - we want to unh
-00000370: 6964 6520 616c 6c20 7468 6520 6e6f 6465  ide all the node
-00000380: 730a 2020 2020 2020 2020 2020 2020 6966  s.            if
-00000390: 2028 6576 656e 742e 6e6f 6465 732e 6c65   (event.nodes.le
-000003a0: 6e67 7468 203d 3d20 3020 2626 2064 6174  ngth == 0 && dat
-000003b0: 612e 6e65 7477 6f72 6b2e 6861 735f 6869  a.network.has_hi
-000003c0: 6464 656e 5f6e 6f64 6573 203d 3d3d 2074  dden_nodes === t
-000003d0: 7275 6529 207b 0a20 2020 2020 2020 2020  rue) {.         
-000003e0: 2020 2020 2020 2073 656c 6563 7465 644e         selectedN
-000003f0: 6f64 6573 203d 204f 626a 6563 742e 6b65  odes = Object.ke
-00000400: 7973 2864 6174 612e 6e6f 6465 7329 3b0a  ys(data.nodes);.
-00000410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000420: 6461 7461 2e6e 6574 776f 726b 2e68 6173  data.network.has
-00000430: 5f68 6964 6465 6e5f 6e6f 6465 7320 3d20  _hidden_nodes = 
-00000440: 6661 6c73 653b 0a20 2020 2020 2020 2020  false;.         
-00000450: 2020 207d 0a20 2020 2020 2020 2020 2020     }.           
-00000460: 2065 6c73 6520 7b0a 2020 2020 2020 2020   else {.        
-00000470: 2020 2020 2020 2020 636f 6e73 7420 7365          const se
-00000480: 6c65 6374 6564 4e6f 6465 203d 2065 7665  lectedNode = eve
-00000490: 6e74 2e6e 6f64 6573 5b30 5d3b 0a20 2020  nt.nodes[0];.   
-000004a0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000004b0: 6563 7465 644e 6f64 6573 203d 2064 6174  ectedNodes = dat
-000004c0: 612e 6e65 7477 6f72 6b2e 6765 7443 6f6e  a.network.getCon
-000004d0: 6e65 6374 6564 4e6f 6465 7328 7365 6c65  nectedNodes(sele
-000004e0: 6374 6564 4e6f 6465 293b 0a20 2020 2020  ctedNode);.     
-000004f0: 2020 2020 2020 2020 2020 2073 656c 6563             selec
-00000500: 7465 644e 6f64 6573 2e70 7573 6828 7365  tedNodes.push(se
-00000510: 6c65 6374 6564 4e6f 6465 293b 0a20 2020  lectedNode);.   
-00000520: 2020 2020 2020 2020 2020 2020 2064 6174               dat
-00000530: 612e 6e65 7477 6f72 6b2e 6861 735f 6869  a.network.has_hi
-00000540: 6464 656e 5f6e 6f64 6573 203d 2074 7275  dden_nodes = tru
-00000550: 653b 0a20 2020 2020 2020 2020 2020 207d  e;.            }
-00000560: 0a20 2020 2020 2020 2020 2020 2063 6f6e  .            con
-00000570: 7374 2063 6861 6e67 6564 5f6e 6f64 6573  st changed_nodes
-00000580: 203d 205b 5d0a 2020 2020 2020 2020 2020   = [].          
-00000590: 2020 0a20 2020 2020 2020 2020 2020 2066    .            f
-000005a0: 6f72 2028 7661 7220 6b65 7920 696e 2064  or (var key in d
-000005b0: 6174 612e 6e6f 6465 7329 207b 0a20 2020  ata.nodes) {.   
-000005c0: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
-000005d0: 7374 206e 6f64 6520 3d20 6461 7461 2e6e  st node = data.n
-000005e0: 6f64 6573 5b6b 6579 5d0a 2020 2020 2020  odes[key].      
-000005f0: 2020 2020 2020 2020 2020 636f 6e73 7420            const 
-00000600: 6964 203d 206e 6f64 655b 2269 6422 5d0a  id = node["id"].
-00000610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000620: 2f2f 206e 6f64 6520 6973 206e 6f74 2068  // node is not h
-00000630: 6964 6465 6e20 6279 2064 6566 6175 6c74  idden by default
-00000640: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000650: 2069 6620 286e 6f64 652e 6861 734f 776e   if (node.hasOwn
-00000660: 5072 6f70 6572 7479 2822 5f68 6964 6465  Property("_hidde
-00000670: 6e22 2920 3d3d 3d20 6661 6c73 6529 206e  n") === false) n
-00000680: 6f64 652e 5f68 6964 6465 6e20 3d20 6661  ode._hidden = fa
-00000690: 6c73 653b 0a0a 2020 2020 2020 2020 2020  lse;..          
-000006a0: 2020 2020 2020 2f2f 206e 6f64 6573 2074        // nodes t
-000006b0: 6f20 6869 6465 0a20 2020 2020 2020 2020  o hide.         
-000006c0: 2020 2020 2020 2069 6620 2873 656c 6563         if (selec
-000006d0: 7465 644e 6f64 6573 2e69 6e63 6c75 6465  tedNodes.include
-000006e0: 7328 6964 2920 3d3d 3d20 6661 6c73 6529  s(id) === false)
-000006f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000700: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-00000710: 2020 2020 2020 202f 2f20 6e6f 7420 616c         // not al
-00000720: 7265 6164 7920 6869 6464 656e 0a20 2020  ready hidden.   
-00000730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000740: 2069 6620 286e 6f64 652e 5f68 6964 6465   if (node._hidde
-00000750: 6e20 3d3d 3d20 6661 6c73 6529 0a20 2020  n === false).   
-00000760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000770: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-00000780: 2020 2020 2020 2020 2020 206e 6f64 652e             node.
-00000790: 5f68 6964 6465 6e20 3d20 7472 7565 3b0a  _hidden = true;.
-000007a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000007b0: 2020 2020 2020 2020 6e6f 6465 2e5f 636f          node._co
-000007c0: 6c6f 7220 3d20 6e6f 6465 2e63 6f6c 6f72  lor = node.color
-000007d0: 3b0a 2020 2020 2020 2020 2020 2020 2020  ;.              
-000007e0: 2020 2020 2020 2020 2020 6e6f 6465 2e63            node.c
-000007f0: 6f6c 6f72 203d 2022 7267 6261 2832 3030  olor = "rgba(200
-00000800: 2c32 3030 2c32 3030 2c30 2e35 2922 3b0a  ,200,200,0.5)";.
-00000810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000820: 2020 2020 2020 2020 6368 616e 6765 645f          changed_
-00000830: 6e6f 6465 732e 7075 7368 286e 6f64 6529  nodes.push(node)
-00000840: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000850: 2020 2020 207d 0a20 2020 2020 2020 2020       }.         
-00000860: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
-00000870: 2020 2020 2020 2020 202f 2f20 6e6f 6465           // node
-00000880: 7320 746f 2075 6e68 6964 6520 286f 6e6c  s to unhide (onl
-00000890: 7920 6966 2061 6c72 6561 6479 2068 6964  y if already hid
-000008a0: 6465 6e29 0a20 2020 2020 2020 2020 2020  den).           
-000008b0: 2020 2020 2065 6c73 6520 6966 2028 6e6f       else if (no
-000008c0: 6465 2e5f 6869 6464 656e 203d 3d3d 2074  de._hidden === t
-000008d0: 7275 6529 207b 0a20 2020 2020 2020 2020  rue) {.         
-000008e0: 2020 2020 2020 2020 2020 206e 6f64 652e             node.
-000008f0: 5f68 6964 6465 6e20 3d20 6661 6c73 653b  _hidden = false;
-00000900: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000910: 2020 2020 206e 6f64 652e 636f 6c6f 7220       node.color 
-00000920: 3d20 6e6f 6465 2e5f 636f 6c6f 723b 0a20  = node._color;. 
-00000930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000940: 2020 206e 6f64 652e 5f63 6f6c 6f72 203d     node._color =
-00000950: 2075 6e64 6566 696e 6564 3b0a 2020 2020   undefined;.    
-00000960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000970: 6368 616e 6765 645f 6e6f 6465 732e 7075  changed_nodes.pu
-00000980: 7368 286e 6f64 6529 0a20 2020 2020 2020  sh(node).       
-00000990: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
-000009a0: 2020 2020 2020 207d 0a0a 2020 2020 2020         }..      
-000009b0: 2020 2020 2020 6461 7461 2e64 735f 6e6f        data.ds_no
-000009c0: 6465 732e 7570 6461 7465 2863 6861 6e67  des.update(chang
-000009d0: 6564 5f6e 6f64 6573 290a 2020 2020 2020  ed_nodes).      
-000009e0: 2020 7d0a 2020 2020 7d0a 0a20 2020 2066    }.    }..    f
-000009f0: 756e 6374 696f 6e20 6372 6561 7465 5f6e  unction create_n
-00000a00: 6574 776f 726b 2829 207b 0a0a 2020 2020  etwork() {..    
-00000a10: 2020 2020 2f2f 2063 7265 6174 6520 616e      // create an
-00000a20: 2061 7272 6179 2077 6974 6820 6e6f 6465   array with node
-00000a30: 730a 2020 2020 2020 2020 636f 6e73 7420  s.        const 
-00000a40: 6473 5f6e 6f64 6573 203d 206e 6577 2076  ds_nodes = new v
-00000a50: 6973 2e44 6174 6153 6574 287b 7b64 6174  is.DataSet({{dat
-00000a60: 615b 226e 6f64 6573 225d 7c74 6f6a 736f  a["nodes"]|tojso
-00000a70: 6e7d 7d29 3b0a 0a20 2020 2020 2020 202f  n}});..        /
-00000a80: 2f20 6372 6561 7465 2061 6e20 6172 7261  / create an arra
-00000a90: 7920 7769 7468 2065 6467 6573 0a20 2020  y with edges.   
-00000aa0: 2020 2020 2063 6f6e 7374 2064 735f 6564       const ds_ed
-00000ab0: 6765 7320 3d20 6e65 7720 7669 732e 4461  ges = new vis.Da
-00000ac0: 7461 5365 7428 7b7b 6461 7461 5b22 6564  taSet({{data["ed
-00000ad0: 6765 7322 5d7c 746f 6a73 6f6e 7d7d 293b  ges"]|tojson}});
-00000ae0: 0a0a 2020 2020 2020 2020 2f2f 2063 7265  ..        // cre
-00000af0: 6174 6520 6120 6e65 7477 6f72 6b0a 2020  ate a network.  
-00000b00: 2020 2020 2020 636f 6e73 7420 636f 6e74        const cont
-00000b10: 6169 6e65 7220 3d20 646f 6375 6d65 6e74  ainer = document
-00000b20: 2e67 6574 456c 656d 656e 7442 7949 6428  .getElementById(
-00000b30: 2776 6973 6a73 6e65 7427 293b 0a0a 2020  'visjsnet');..  
-00000b40: 2020 2020 2020 2f2f 2070 726f 7669 6465        // provide
-00000b50: 2074 6865 2064 6174 6120 696e 2074 6865   the data in the
-00000b60: 2076 6973 2066 6f72 6d61 740a 2020 2020   vis format.    
-00000b70: 2020 2020 636f 6e73 7420 6461 7461 203d      const data =
-00000b80: 207b 0a20 2020 2020 2020 2020 2020 206e   {.            n
-00000b90: 6f64 6573 3a20 6473 5f6e 6f64 6573 2c0a  odes: ds_nodes,.
-00000ba0: 2020 2020 2020 2020 2020 2020 6564 6765              edge
-00000bb0: 733a 2064 735f 6564 6765 730a 2020 2020  s: ds_edges.    
-00000bc0: 2020 2020 7d3b 0a20 2020 2020 2020 2063      };.        c
-00000bd0: 6f6e 7374 206f 7074 696f 6e73 203d 207b  onst options = {
-00000be0: 7b64 6174 615b 226f 7074 696f 6e73 225d  {data["options"]
-00000bf0: 7c74 6f6a 736f 6e7d 7d3b 0a20 2020 2020  |tojson}};.     
-00000c00: 2020 2063 6f6e 7374 2070 7976 6973 6a73     const pyvisjs
-00000c10: 203d 207b 7b70 7976 6973 6a73 7c74 6f6a   = {{pyvisjs|toj
-00000c20: 736f 6e7d 7d3b 0a0a 2020 2020 2020 2020  son}};..        
-00000c30: 7265 7475 726e 207b 0a20 2020 2020 2020  return {.       
-00000c40: 2020 2020 206e 6574 776f 726b 3a20 6e65       network: ne
-00000c50: 7720 7669 732e 4e65 7477 6f72 6b28 636f  w vis.Network(co
-00000c60: 6e74 6169 6e65 722c 2064 6174 612c 206f  ntainer, data, o
-00000c70: 7074 696f 6e73 292c 0a20 2020 2020 2020  ptions),.       
-00000c80: 2020 2020 206e 6f64 6573 3a20 6473 5f6e       nodes: ds_n
-00000c90: 6f64 6573 2e67 6574 287b 2072 6574 7572  odes.get({ retur
-00000ca0: 6e54 7970 653a 2022 4f62 6a65 6374 2220  nType: "Object" 
-00000cb0: 7d29 2c0a 2020 2020 2020 2020 2020 2020  }),.            
-00000cc0: 6473 5f6e 6f64 6573 3a20 6473 5f6e 6f64  ds_nodes: ds_nod
-00000cd0: 6573 2c0a 2020 2020 2020 2020 2020 2020  es,.            
-00000ce0: 7079 7669 736a 733a 2070 7976 6973 6a73  pyvisjs: pyvisjs
-00000cf0: 2c0a 2020 2020 2020 2020 7d0a 2020 2020  ,.        }.    
-00000d00: 7d0a 3c2f 7363 7269 7074 3e0a 3c2f 626f  }.</script>.</bo
-00000d10: 6479 3e0a 3c2f 6874 6d6c 3e              dy>.</html>
+00000000: 636f 6e73 7420 6461 7461 203d 2063 7265  const data = cre
+00000010: 6174 655f 6e65 7477 6f72 6b28 293b 0a64  ate_network();.d
+00000020: 6174 612e 6e65 7477 6f72 6b2e 6861 735f  ata.network.has_
+00000030: 6869 6464 656e 5f6e 6f64 6573 203d 2066  hidden_nodes = f
+00000040: 616c 7365 3b0a 6966 2028 6461 7461 2e70  alse;.if (data.p
+00000050: 7976 6973 6a73 2e65 6e61 626c 655f 6869  yvisjs.enable_hi
+00000060: 6768 6c69 6768 7469 6e67 203d 3d3d 2074  ghlighting === t
+00000070: 7275 6529 2064 6174 612e 6e65 7477 6f72  rue) data.networ
+00000080: 6b2e 6f6e 2822 636c 6963 6b22 2c20 6869  k.on("click", hi
+00000090: 6465 5f6e 6f74 5f73 656c 6563 7465 645f  de_not_selected_
+000000a0: 6e6f 6465 7329 3b0a 0a0a 2f2f 2061 6c6c  nodes);...// all
+000000b0: 206a 696e 6a61 2069 6e6a 6563 7469 6f6e   jinja injection
+000000c0: 7320 7368 6f75 6c64 2068 6170 7065 6e20  s should happen 
+000000d0: 6865 7265 2062 6563 6175 7365 2069 7420  here because it 
+000000e0: 616c 6c6f 7773 2074 6f20 6d6f 636b 2074  allows to mock t
+000000f0: 6869 7320 6675 6e63 7469 6f6e 2061 6e64  his function and
+00000100: 2074 6573 7420 616c 6c20 7468 6520 7265   test all the re
+00000110: 7374 0a66 756e 6374 696f 6e20 6372 6561  st.function crea
+00000120: 7465 5f6e 6574 776f 726b 2829 207b 0a0a  te_network() {..
+00000130: 2020 2020 2f2f 2063 7265 6174 6520 616e      // create an
+00000140: 2061 7272 6179 2077 6974 6820 6e6f 6465   array with node
+00000150: 730a 2020 2020 636f 6e73 7420 6473 5f6e  s.    const ds_n
+00000160: 6f64 6573 203d 206e 6577 2076 6973 2e44  odes = new vis.D
+00000170: 6174 6153 6574 287b 7b20 6461 7461 5b22  ataSet({{ data["
+00000180: 6e6f 6465 7322 5d7c 746f 6a73 6f6e 207d  nodes"]|tojson }
+00000190: 7d29 3b0a 0a20 2020 202f 2f20 6372 6561  });..    // crea
+000001a0: 7465 2061 6e20 6172 7261 7920 7769 7468  te an array with
+000001b0: 2065 6467 6573 0a20 2020 2063 6f6e 7374   edges.    const
+000001c0: 2064 735f 6564 6765 7320 3d20 6e65 7720   ds_edges = new 
+000001d0: 7669 732e 4461 7461 5365 7428 7b7b 2064  vis.DataSet({{ d
+000001e0: 6174 615b 2265 6467 6573 225d 7c74 6f6a  ata["edges"]|toj
+000001f0: 736f 6e20 7d7d 293b 0a0a 2020 2020 2f2f  son }});..    //
+00000200: 2063 7265 6174 6520 6120 6e65 7477 6f72   create a networ
+00000210: 6b0a 2020 2020 636f 6e73 7420 636f 6e74  k.    const cont
+00000220: 6169 6e65 7220 3d20 646f 6375 6d65 6e74  ainer = document
+00000230: 2e67 6574 456c 656d 656e 7442 7949 6428  .getElementById(
+00000240: 2776 6973 6a73 6e65 7427 293b 0a0a 2020  'visjsnet');..  
+00000250: 2020 2f2f 2070 726f 7669 6465 2074 6865    // provide the
+00000260: 2064 6174 6120 696e 2074 6865 2076 6973   data in the vis
+00000270: 2066 6f72 6d61 740a 2020 2020 636f 6e73   format.    cons
+00000280: 7420 6461 7461 203d 207b 0a20 2020 2020  t data = {.     
+00000290: 2020 206e 6f64 6573 3a20 6473 5f6e 6f64     nodes: ds_nod
+000002a0: 6573 2c0a 2020 2020 2020 2020 6564 6765  es,.        edge
+000002b0: 733a 2064 735f 6564 6765 730a 2020 2020  s: ds_edges.    
+000002c0: 7d3b 0a20 2020 2063 6f6e 7374 206f 7074  };.    const opt
+000002d0: 696f 6e73 203d 207b 7b20 6461 7461 5b22  ions = {{ data["
+000002e0: 6f70 7469 6f6e 7322 5d7c 746f 6a73 6f6e  options"]|tojson
+000002f0: 207d 7d3b 0a20 2020 2063 6f6e 7374 2070   }};.    const p
+00000300: 7976 6973 6a73 203d 207b 7b20 7079 7669  yvisjs = {{ pyvi
+00000310: 736a 737c 746f 6a73 6f6e 207d 7d3b 0a0a  sjs|tojson }};..
+00000320: 2020 2020 7265 7475 726e 207b 0a20 2020      return {.   
+00000330: 2020 2020 206e 6574 776f 726b 3a20 6e65       network: ne
+00000340: 7720 7669 732e 4e65 7477 6f72 6b28 636f  w vis.Network(co
+00000350: 6e74 6169 6e65 722c 2064 6174 612c 206f  ntainer, data, o
+00000360: 7074 696f 6e73 292c 0a20 2020 2020 2020  ptions),.       
+00000370: 206e 6f64 6573 3a20 6473 5f6e 6f64 6573   nodes: ds_nodes
+00000380: 2e67 6574 287b 2072 6574 7572 6e54 7970  .get({ returnTyp
+00000390: 653a 2022 4f62 6a65 6374 2220 7d29 2c0a  e: "Object" }),.
+000003a0: 2020 2020 2020 2020 6564 6765 733a 2064          edges: d
+000003b0: 735f 6564 6765 732e 6765 7428 7b20 7265  s_edges.get({ re
+000003c0: 7475 726e 5479 7065 3a20 224f 626a 6563  turnType: "Objec
+000003d0: 7422 207d 292c 0a20 2020 2020 2020 2064  t" }),.        d
+000003e0: 735f 6e6f 6465 733a 2064 735f 6e6f 6465  s_nodes: ds_node
+000003f0: 732c 0a20 2020 2020 2020 2070 7976 6973  s,.        pyvis
+00000400: 6a73 3a20 7079 7669 736a 732c 0a20 2020  js: pyvisjs,.   
+00000410: 207d 0a7d 0a0a 6675 6e63 7469 6f6e 2067   }.}..function g
+00000420: 6574 5f6e 6f64 6573 5f62 795f 6564 6765  et_nodes_by_edge
+00000430: 5f61 7474 7269 6275 7465 5f76 616c 7565  _attribute_value
+00000440: 2866 6965 6c64 2c20 7661 6c75 6529 207b  (field, value) {
+00000450: 0a0a 2020 2020 636f 6e73 7420 7265 7375  ..    const resu
+00000460: 6c74 203d 205b 5d3b 0a0a 2020 2020 666f  lt = [];..    fo
+00000470: 7220 2863 6f6e 7374 206b 6579 2069 6e20  r (const key in 
+00000480: 6461 7461 2e65 6467 6573 2920 7b0a 2020  data.edges) {.  
+00000490: 2020 2020 2020 636f 6e73 7420 6564 6765        const edge
+000004a0: 203d 2064 6174 612e 6564 6765 735b 6b65   = data.edges[ke
+000004b0: 795d 3b0a 0a20 2020 2020 2020 2069 6620  y];..        if 
+000004c0: 2865 6467 655b 6669 656c 645d 203d 3d3d  (edge[field] ===
+000004d0: 2076 616c 7565 290a 2020 2020 2020 2020   value).        
+000004e0: 7b0a 2020 2020 2020 2020 2020 2020 6966  {.            if
+000004f0: 2028 7265 7375 6c74 2e69 6e63 6c75 6465   (result.include
+00000500: 7328 6564 6765 2e66 726f 6d29 203d 3d3d  s(edge.from) ===
+00000510: 2066 616c 7365 2920 7265 7375 6c74 2e70   false) result.p
+00000520: 7573 6828 6564 6765 2e66 726f 6d29 3b0a  ush(edge.from);.
+00000530: 2020 2020 2020 2020 2020 2020 6966 2028              if (
+00000540: 7265 7375 6c74 2e69 6e63 6c75 6465 7328  result.includes(
+00000550: 6564 6765 2e74 6f29 203d 3d3d 2066 616c  edge.to) === fal
+00000560: 7365 2920 7265 7375 6c74 2e70 7573 6828  se) result.push(
+00000570: 6564 6765 2e74 6f29 3b0a 2020 2020 2020  edge.to);.      
+00000580: 2020 7d0a 2020 2020 7d0a 0a20 2020 2072    }.    }..    r
+00000590: 6574 7572 6e20 7265 7375 6c74 3b0a 7d0a  eturn result;.}.
+000005a0: 0a66 756e 6374 696f 6e20 6869 6465 5f6e  .function hide_n
+000005b0: 6f64 6573 5f62 795f 6564 6765 5f61 7474  odes_by_edge_att
+000005c0: 7269 6275 7465 5f76 616c 7565 2866 6965  ribute_value(fie
+000005d0: 6c64 2c20 7661 6c75 6529 207b 0a0a 2020  ld, value) {..  
+000005e0: 2020 6c65 7420 7365 6c65 6374 6564 4e6f    let selectedNo
+000005f0: 6465 733b 0a0a 2020 2020 6966 2028 7661  des;..    if (va
+00000600: 6c75 6520 3d3d 3d20 2241 4c4c 2229 207b  lue === "ALL") {
+00000610: 0a20 2020 2020 2020 2073 656c 6563 7465  .        selecte
+00000620: 644e 6f64 6573 203d 204f 626a 6563 742e  dNodes = Object.
+00000630: 6b65 7973 2864 6174 612e 6e6f 6465 7329  keys(data.nodes)
+00000640: 3b0a 2020 2020 2020 2020 6461 7461 2e6e  ;.        data.n
+00000650: 6574 776f 726b 2e68 6173 5f68 6964 6465  etwork.has_hidde
+00000660: 6e5f 6e6f 6465 7320 3d20 6661 6c73 653b  n_nodes = false;
+00000670: 0a20 2020 207d 0a20 2020 2065 6c73 6520  .    }.    else 
+00000680: 7b0a 2020 2020 2020 2020 7365 6c65 6374  {.        select
+00000690: 6564 4e6f 6465 7320 3d20 6765 745f 6e6f  edNodes = get_no
+000006a0: 6465 735f 6279 5f65 6467 655f 6174 7472  des_by_edge_attr
+000006b0: 6962 7574 655f 7661 6c75 6528 6669 656c  ibute_value(fiel
+000006c0: 642c 2076 616c 7565 290a 2020 2020 2020  d, value).      
+000006d0: 2020 6461 7461 2e6e 6574 776f 726b 2e68    data.network.h
+000006e0: 6173 5f68 6964 6465 6e5f 6e6f 6465 7320  as_hidden_nodes 
+000006f0: 3d20 7472 7565 3b0a 2020 2020 7d0a 0a20  = true;.    }.. 
+00000700: 2020 2063 6861 6e67 6564 5f6e 6f64 6573     changed_nodes
+00000710: 203d 2074 6f67 676c 655f 6e6f 6465 7328   = toggle_nodes(
+00000720: 7365 6c65 6374 6564 4e6f 6465 7329 3b0a  selectedNodes);.
+00000730: 0a20 2020 2064 6174 612e 6473 5f6e 6f64  .    data.ds_nod
+00000740: 6573 2e75 7064 6174 6528 6368 616e 6765  es.update(change
+00000750: 645f 6e6f 6465 7329 0a7d 0a0a 6675 6e63  d_nodes).}..func
+00000760: 7469 6f6e 2068 6964 655f 6e6f 745f 7365  tion hide_not_se
+00000770: 6c65 6374 6564 5f6e 6f64 6573 2865 7665  lected_nodes(eve
+00000780: 6e74 2920 7b0a 2020 2020 2f2f 2068 6173  nt) {.    // has
+00000790: 2073 656c 6563 7465 6420 6e6f 6465 7320   selected nodes 
+000007a0: 6f72 2061 6c72 6561 6479 2068 6173 2068  or already has h
+000007b0: 6964 6465 6e20 6e6f 6465 7320 2d20 696e  idden nodes - in
+000007c0: 2062 6f74 6820 6361 7365 7320 7765 2068   both cases we h
+000007d0: 6176 6520 776f 726b 2074 6f20 646f 0a20  ave work to do. 
+000007e0: 2020 2069 6620 2865 7665 6e74 2e6e 6f64     if (event.nod
+000007f0: 6573 2e6c 656e 6774 6820 3e20 3020 7c7c  es.length > 0 ||
+00000800: 2064 6174 612e 6e65 7477 6f72 6b2e 6861   data.network.ha
+00000810: 735f 6869 6464 656e 5f6e 6f64 6573 203d  s_hidden_nodes =
+00000820: 3d3d 2074 7275 6529 207b 0a20 2020 2020  == true) {.     
+00000830: 2020 206c 6574 2073 656c 6563 7465 644e     let selectedN
+00000840: 6f64 6573 3b0a 2020 2020 2020 2020 0a20  odes;.        . 
+00000850: 2020 2020 2020 202f 2f20 7573 6572 2063         // user c
+00000860: 6c69 636b 6564 206f 7574 7369 6465 2074  licked outside t
+00000870: 6865 206e 6f64 6573 206e 6574 776f 726b  he nodes network
+00000880: 202d 2077 6520 7761 6e74 2074 6f20 756e   - we want to un
+00000890: 6869 6465 2061 6c6c 2074 6865 206e 6f64  hide all the nod
+000008a0: 6573 0a20 2020 2020 2020 2069 6620 2865  es.        if (e
+000008b0: 7665 6e74 2e6e 6f64 6573 2e6c 656e 6774  vent.nodes.lengt
+000008c0: 6820 3d3d 2030 2026 2620 6461 7461 2e6e  h == 0 && data.n
+000008d0: 6574 776f 726b 2e68 6173 5f68 6964 6465  etwork.has_hidde
+000008e0: 6e5f 6e6f 6465 7320 3d3d 3d20 7472 7565  n_nodes === true
+000008f0: 2920 7b0a 2020 2020 2020 2020 2020 2020  ) {.            
+00000900: 7365 6c65 6374 6564 4e6f 6465 7320 3d20  selectedNodes = 
+00000910: 4f62 6a65 6374 2e6b 6579 7328 6461 7461  Object.keys(data
+00000920: 2e6e 6f64 6573 293b 0a20 2020 2020 2020  .nodes);.       
+00000930: 2020 2020 2064 6174 612e 6e65 7477 6f72       data.networ
+00000940: 6b2e 6861 735f 6869 6464 656e 5f6e 6f64  k.has_hidden_nod
+00000950: 6573 203d 2066 616c 7365 3b0a 2020 2020  es = false;.    
+00000960: 2020 2020 7d0a 2020 2020 2020 2020 656c      }.        el
+00000970: 7365 207b 0a20 2020 2020 2020 2020 2020  se {.           
+00000980: 2063 6f6e 7374 2073 656c 6563 7465 644e   const selectedN
+00000990: 6f64 6520 3d20 6576 656e 742e 6e6f 6465  ode = event.node
+000009a0: 735b 305d 3b0a 2020 2020 2020 2020 2020  s[0];.          
+000009b0: 2020 7365 6c65 6374 6564 4e6f 6465 7320    selectedNodes 
+000009c0: 3d20 6461 7461 2e6e 6574 776f 726b 2e67  = data.network.g
+000009d0: 6574 436f 6e6e 6563 7465 644e 6f64 6573  etConnectedNodes
+000009e0: 2873 656c 6563 7465 644e 6f64 6529 3b0a  (selectedNode);.
+000009f0: 2020 2020 2020 2020 2020 2020 7365 6c65              sele
+00000a00: 6374 6564 4e6f 6465 732e 7075 7368 2873  ctedNodes.push(s
+00000a10: 656c 6563 7465 644e 6f64 6529 3b0a 2020  electedNode);.  
+00000a20: 2020 2020 2020 2020 2020 6461 7461 2e6e            data.n
+00000a30: 6574 776f 726b 2e68 6173 5f68 6964 6465  etwork.has_hidde
+00000a40: 6e5f 6e6f 6465 7320 3d20 7472 7565 3b0a  n_nodes = true;.
+00000a50: 2020 2020 2020 2020 7d0a 0a20 2020 2020          }..     
+00000a60: 2020 2063 6861 6e67 6564 5f6e 6f64 6573     changed_nodes
+00000a70: 203d 2074 6f67 676c 655f 6e6f 6465 7328   = toggle_nodes(
+00000a80: 7365 6c65 6374 6564 4e6f 6465 7329 3b0a  selectedNodes);.
+00000a90: 0a20 2020 2020 2020 2064 6174 612e 6473  .        data.ds
+00000aa0: 5f6e 6f64 6573 2e75 7064 6174 6528 6368  _nodes.update(ch
+00000ab0: 616e 6765 645f 6e6f 6465 7329 0a20 2020  anged_nodes).   
+00000ac0: 207d 0a7d 0a0a 6675 6e63 7469 6f6e 2074   }.}..function t
+00000ad0: 6f67 676c 655f 6e6f 6465 7328 7365 6c65  oggle_nodes(sele
+00000ae0: 6374 6564 4e6f 6465 7329 207b 0a20 2020  ctedNodes) {.   
+00000af0: 2063 6f6e 7374 2063 6861 6e67 6564 5f6e   const changed_n
+00000b00: 6f64 6573 203d 205b 5d3b 0a20 2020 200a  odes = [];.    .
+00000b10: 2020 2020 666f 7220 2863 6f6e 7374 206b      for (const k
+00000b20: 6579 2069 6e20 6461 7461 2e6e 6f64 6573  ey in data.nodes
+00000b30: 2920 7b0a 2020 2020 2020 2020 636f 6e73  ) {.        cons
+00000b40: 7420 6e6f 6465 203d 2064 6174 612e 6e6f  t node = data.no
+00000b50: 6465 735b 6b65 795d 3b0a 2020 2020 2020  des[key];.      
+00000b60: 2020 636f 6e73 7420 6964 203d 206e 6f64    const id = nod
+00000b70: 655b 2269 6422 5d3b 0a20 2020 2020 2020  e["id"];.       
+00000b80: 202f 2f20 6e6f 6465 2069 7320 6e6f 7420   // node is not 
+00000b90: 6869 6464 656e 2062 7920 6465 6661 756c  hidden by defaul
+00000ba0: 740a 2020 2020 2020 2020 6966 2028 6e6f  t.        if (no
+00000bb0: 6465 2e68 6173 4f77 6e50 726f 7065 7274  de.hasOwnPropert
+00000bc0: 7928 225f 6869 6464 656e 2229 203d 3d3d  y("_hidden") ===
+00000bd0: 2066 616c 7365 2920 6e6f 6465 2e5f 6869   false) node._hi
+00000be0: 6464 656e 203d 2066 616c 7365 3b0a 2020  dden = false;.  
+00000bf0: 2020 2020 2020 0a20 2020 2020 2020 202f        .        /
+00000c00: 2f20 6e6f 6465 7320 746f 2068 6964 650a  / nodes to hide.
+00000c10: 2020 2020 2020 2020 6966 2028 7365 6c65          if (sele
+00000c20: 6374 6564 4e6f 6465 732e 696e 636c 7564  ctedNodes.includ
+00000c30: 6573 2869 6429 203d 3d3d 2066 616c 7365  es(id) === false
+00000c40: 290a 2020 2020 2020 2020 7b0a 2020 2020  ).        {.    
+00000c50: 2020 2020 2020 2020 2f2f 206e 6f74 2061          // not a
+00000c60: 6c72 6561 6479 2068 6964 6465 6e0a 2020  lready hidden.  
+00000c70: 2020 2020 2020 2020 2020 6966 2028 6e6f            if (no
+00000c80: 6465 2e5f 6869 6464 656e 203d 3d3d 2066  de._hidden === f
+00000c90: 616c 7365 290a 2020 2020 2020 2020 2020  alse).          
+00000ca0: 2020 7b0a 2020 2020 2020 2020 2020 2020    {.            
+00000cb0: 2020 2020 6e6f 6465 2e5f 6869 6464 656e      node._hidden
+00000cc0: 203d 2074 7275 653b 0a20 2020 2020 2020   = true;.       
+00000cd0: 2020 2020 2020 2020 206e 6f64 652e 6869           node.hi
+00000ce0: 6464 656e 203d 2074 7275 653b 0a20 2020  dden = true;.   
+00000cf0: 2020 2020 2020 2020 2020 2020 206e 6f64               nod
+00000d00: 652e 5f63 6f6c 6f72 203d 206e 6f64 652e  e._color = node.
+00000d10: 636f 6c6f 723b 0a20 2020 2020 2020 2020  color;.         
+00000d20: 2020 2020 2020 206e 6f64 652e 636f 6c6f         node.colo
+00000d30: 7220 3d20 2272 6762 6128 3230 302c 3230  r = "rgba(200,20
+00000d40: 302c 3230 302c 302e 3529 223b 0a20 2020  0,200,0.5)";.   
+00000d50: 2020 2020 2020 2020 2020 2020 2063 6861               cha
+00000d60: 6e67 6564 5f6e 6f64 6573 2e70 7573 6828  nged_nodes.push(
+00000d70: 6e6f 6465 290a 2020 2020 2020 2020 2020  node).          
+00000d80: 2020 7d0a 2020 2020 2020 2020 7d0a 2020    }.        }.  
+00000d90: 2020 2020 2020 2f2f 206e 6f64 6573 2074        // nodes t
+00000da0: 6f20 756e 6869 6465 2028 6f6e 6c79 2069  o unhide (only i
+00000db0: 6620 616c 7265 6164 7920 6869 6464 656e  f already hidden
+00000dc0: 290a 2020 2020 2020 2020 656c 7365 2069  ).        else i
+00000dd0: 6620 286e 6f64 652e 5f68 6964 6465 6e20  f (node._hidden 
+00000de0: 3d3d 3d20 7472 7565 2920 7b0a 2020 2020  === true) {.    
+00000df0: 2020 2020 2020 2020 6e6f 6465 2e5f 6869          node._hi
+00000e00: 6464 656e 203d 2066 616c 7365 3b0a 2020  dden = false;.  
+00000e10: 2020 2020 2020 2020 2020 6e6f 6465 2e68            node.h
+00000e20: 6964 6465 6e20 3d20 6661 6c73 653b 0a20  idden = false;. 
+00000e30: 2020 2020 2020 2020 2020 206e 6f64 652e             node.
+00000e40: 636f 6c6f 7220 3d20 6e6f 6465 2e5f 636f  color = node._co
+00000e50: 6c6f 7220 3f20 6e6f 6465 2e5f 636f 6c6f  lor ? node._colo
+00000e60: 7220 3a20 2223 3937 4332 4643 223b 0a20  r : "#97C2FC";. 
+00000e70: 2020 2020 2020 2020 2020 206e 6f64 652e             node.
+00000e80: 5f63 6f6c 6f72 203d 2075 6e64 6566 696e  _color = undefin
+00000e90: 6564 3b0a 2020 2020 2020 2020 2020 2020  ed;.            
+00000ea0: 6368 616e 6765 645f 6e6f 6465 732e 7075  changed_nodes.pu
+00000eb0: 7368 286e 6f64 6529 0a20 2020 2020 2020  sh(node).       
+00000ec0: 207d 0a20 2020 207d 0a0a 2020 2020 7265   }.    }..    re
+00000ed0: 7475 726e 2063 6861 6e67 6564 5f6e 6f64  turn changed_nod
+00000ee0: 6573 0a7d                                es.}
```

### Comparing `pyvisjs-0.0.0.dev8/pyvisjs/utils.py` & `pyvisjs-1.0.0a1/pyvisjs/utils.py`

 * *Files identical despite different names*

### Comparing `pyvisjs-0.0.0.dev8/pyvisjs.egg-info/PKG-INFO` & `pyvisjs-1.0.0a1/pyvisjs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvisjs
-Version: 0.0.0.dev8
+Version: 1.0.0a1
 Summary: A Python wrapper for vis.js Network
 Author-email: Andrey Morozov <andrey@morozov.lv>
 License: MIT License
         
         Copyright (c) 2024 Andrey Morozov (andrey@morozov.lv)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyvisjs-0.0.0.dev8/pyvisjs.egg-info/SOURCES.txt` & `pyvisjs-1.0.0a1/pyvisjs.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -3,31 +3,33 @@
 CONTRIBUTING.md
 LICENSE
 README.md
 folder_structure.txt
 pyproject.toml
 requirements.txt
 examples/bluor.py
-examples/main.py
 examples/readme_usage.py
 pyvisjs/__init__.py
 pyvisjs/_version.py
 pyvisjs/base_dictable.py
 pyvisjs/edge.py
 pyvisjs/network.py
 pyvisjs/node.py
 pyvisjs/options.py
 pyvisjs/utils.py
 pyvisjs.egg-info/PKG-INFO
 pyvisjs.egg-info/SOURCES.txt
 pyvisjs.egg-info/dependency_links.txt
 pyvisjs.egg-info/requires.txt
 pyvisjs.egg-info/top_level.txt
+pyvisjs/templates/base.html
 pyvisjs/templates/basic.html
 pyvisjs/templates/bs-container.html
+pyvisjs/templates/functions.js
+pyvisjs/templates/select-edge-filter.html
 tests/__init__.py
 tests/test_base_dictable.py
 tests/test_edge.py
 tests/test_network.py
 tests/test_node.py
 tests/test_options.py
 tests/test_utils.py
```

### Comparing `pyvisjs-0.0.0.dev8/tests/test_base_dictable.py` & `pyvisjs-1.0.0a1/tests/test_base_dictable.py`

 * *Files identical despite different names*

### Comparing `pyvisjs-0.0.0.dev8/tests/test_edge.py` & `pyvisjs-1.0.0a1/tests/test_edge.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from pyvisjs import Edge
 
 def test_edge_init_default():
     # init
-    START_ID = 1
-    END_ID = 2
+    START_ID = "1"
+    END_ID = "2"
 
     # mock
 
     # call
     e = Edge(START_ID, END_ID)
     
     # assert
     assert e.start == START_ID
     assert e.end == END_ID
 
 def test_edge_init_kwargs():
     # init
-    START_ID = 1
-    END_ID = 2
+    START_ID = "1"
+    END_ID = "2"
     NODE_CATEGORY = "category1"
     NODE_AMOUNT = 1009.4
     NODE_HASVALUE = False
 
     # mock
 
     # call
@@ -31,16 +31,16 @@
     assert e.start == START_ID
     assert e.end == END_ID
     assert (e.category, e.amount, e.has_value) == (NODE_CATEGORY, NODE_AMOUNT, NODE_HASVALUE)
 
 
 def test_edge_to_dict():
     # init
-    START_ID = 1
-    END_ID = 2
+    START_ID = "A"
+    END_ID = "B"
     EDGE_DICT = {
             "from": START_ID,
             "to": END_ID,
         }
 
     # mock
```

### Comparing `pyvisjs-0.0.0.dev8/tests/test_network.py` & `pyvisjs-1.0.0a1/tests/test_network.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,22 +20,22 @@
     assert n.env is not None
     assert n.to_dict() == DEFAULT_DICT
 
 def test_network_init_with_data():
     # init
     NETWORK_DICT = {
         "nodes": [
-            { "id": 1, "label": "node 1", "shape": "dot" },
-            { "id": 2, "label": "node 2", "shape": "dot" },
-            { "id": 3, "label": "node 3", "shape": "dot" },
+            { "id": "1", "label": "node 1", "shape": "dot" },
+            { "id": "2", "label": "node 2", "shape": "dot" },
+            { "id": "3", "label": "node 3", "shape": "dot" },
         ],
         "edges": [
-            { "from": 1, "to": 2 },
-            { "from": 2, "to": 3 },
-            { "from": 3, "to": 4 }
+            { "from": "1", "to": "2" },
+            { "from": "2", "to": "3" },
+            { "from": "3", "to": "4" }
         ],
         "options": {}
     }
     # mock
 
 
     # call
@@ -94,17 +94,17 @@
     n.add_node(1)
     n.add_node(2, "name2")
     n.add_node(2) # duplicate node
     n.add_node(3, "hello", "red", "circle", None, None, category="high")
     
     # assert
     assert len(n.nodes) == 3
-    assert n.nodes[0].id == 1
+    assert n.nodes[0].id == "1"
     assert n.nodes[0].label == "1"
-    assert n.nodes[1].id == 2
+    assert n.nodes[1].id == "2"
     assert n.nodes[1].label == "name2"
     assert n.nodes[2].category == "high"
 
 def test_network_add_edges():
     # init
 
     # mock
@@ -114,36 +114,36 @@
     n.add_node(1)
     n.add_node(2, "name2")
     n.add_edge(1, 2) # both nodes exist
     n.add_edge(2, 3, country="LV") # one node missing
     n.add_edge(2, 3) # duplicate edge
     
     # assert
-    assert n.nodes[0].id == 1
-    assert n.nodes[1].id == 2
-    assert n.nodes[2].id == 3
+    assert n.nodes[0].id == "1"
+    assert n.nodes[1].id == "2"
+    assert n.nodes[2].id == "3"
 
     assert len(n.edges) == 2
-    assert n.edges[0].start == 1
-    assert n.edges[0].end == 2
-    assert n.edges[1].start == 2
-    assert n.edges[1].end == 3
+    assert n.edges[0].start == "1"
+    assert n.edges[0].end == "2"
+    assert n.edges[1].start == "2"
+    assert n.edges[1].end == "3"
     assert n.edges[1].country == "LV"
 
 def test_network_to_dict():
     # init
     NETWORK_DICT = {
         "nodes": [
-            { "id": 1, "label": "1", "shape": "dot" },
-            { "id": 2, "label": "name2", "shape": "dot" },
-            { "id": 3, "label": "3", "shape": "dot" },
+            { "id": "1", "label": "1", "shape": "dot" },
+            { "id": "2", "label": "name2", "shape": "dot" },
+            { "id": "3", "label": "3", "shape": "dot" },
         ],
         "edges": [
-            { "from": 1, "to": 2 },
-            { "from": 2, "to": 3 }
+            { "from": "1", "to": "2" },
+            { "from": "2", "to": "3" }
         ],
         "options": {}
     }
 
     # mock
 
     # call
@@ -161,14 +161,16 @@
 def test_network_render_template_passing_render_default_params(mock_Environment):
     # init
     WIDTH="100%"
     HEIGHT="100%"
     DATA={"nodes": [], "edges": [], "options": {}}
     PYVISJS={
         "enable_highlighting": False,
+        "edge_filtering_fields": None,
+        "edge_filtering_lookup": None,
     }
     
     # mock
     mock_render = mock_Environment.return_value.get_template.return_value.render
 
     # call
     network = Network("Test Network")
@@ -181,25 +183,101 @@
 def test_network_render_template_passing_render_params(mock_Environment):
     # init
     WIDTH="100%"
     HEIGHT="100%"
     DATA={"nodes": [], "edges": [], "options": {}}
     TEMPLATE_FILENAME="another_template.html"
     ENABLE_HIGHLIGHTING=True
+    EDGE_FILTERING="node_field" # str(!) not list
     PYVISJS={
         "enable_highlighting": ENABLE_HIGHLIGHTING,
+        "edge_filtering_fields": [EDGE_FILTERING],
+        "edge_filtering_lookup": {"node_field": []},
     }
     
     # mock
     mock_get_template = mock_Environment.return_value.get_template
     mock_render = mock_get_template.return_value.render
 
     # call
     network = Network("Test Network")
-    html_output = network.render_template(template_filename=TEMPLATE_FILENAME, enable_highlighting=ENABLE_HIGHLIGHTING) # <--------------------
+    html_output = network.render_template(template_filename=TEMPLATE_FILENAME, enable_highlighting=ENABLE_HIGHLIGHTING, edge_filtering=EDGE_FILTERING) # <--------------------
+
+    # assert
+    mock_get_template.assert_called_once_with(TEMPLATE_FILENAME)
+    mock_render.assert_called_once_with(width=WIDTH, height=HEIGHT, data=DATA, pyvisjs=PYVISJS)
+
+@patch('pyvisjs.network.Environment')
+def test_network_render_template_edge_filtering_list(mock_Environment):
+    # init
+    WIDTH="100%"
+    HEIGHT="100%"
+    DATA={
+        'nodes': [
+            {'id': '1', 'label': '1', 'shape': 'dot'}, 
+            {'id': '2', 'label': '2', 'shape': 'dot'}, 
+            {'id': '3', 'label': '3', 'shape': 'dot'}], 
+        'edges': [
+            {'to': '2', 'field1': 'AM', 'from': '1'}, 
+            {'to': '3', 'field1': 'AM', 'from': '1'}, 
+            {'to': '3', 'field1': 'JL', 'from': '2'}], 
+        'options': {}
+    }
+    TEMPLATE_FILENAME="another_template.html"
+    ENABLE_HIGHLIGHTING=True
+    EDGE_FILTERING=["field1", "field2"]
+    PYVISJS={
+        "enable_highlighting": ENABLE_HIGHLIGHTING,
+        "edge_filtering_fields": EDGE_FILTERING,
+        "edge_filtering_lookup": {"field1": ["AM", "JL"], "field2": []},
+    }
+    
+    # mock
+    mock_get_template = mock_Environment.return_value.get_template
+    mock_render = mock_get_template.return_value.render
+
+    # call
+    net = Network("Network1")
+    net.add_edge(1, 2, field1="AM")
+    net.add_edge(1, 3, field1="AM")
+    net.add_edge(2, 3, field1="JL")
+    html_output = net.render_template(# <--------------------
+        template_filename=TEMPLATE_FILENAME, 
+        enable_highlighting=ENABLE_HIGHLIGHTING, 
+        edge_filtering=EDGE_FILTERING) 
+
+    # assert
+    mock_get_template.assert_called_once_with(TEMPLATE_FILENAME)
+    mock_render.assert_called_once_with(width=WIDTH, height=HEIGHT, data=DATA, pyvisjs=PYVISJS)
+
+@patch('pyvisjs.network.Environment')
+def test_network_render_template_edge_filtering_int(mock_Environment):
+    # init
+    WIDTH="100%"
+    HEIGHT="100%"
+    DATA={"nodes": [], "edges": [], "options": {}}
+    TEMPLATE_FILENAME="another_template.html"
+    ENABLE_HIGHLIGHTING=True
+    EDGE_FILTERING=34
+    PYVISJS={
+        "enable_highlighting": ENABLE_HIGHLIGHTING,
+        "edge_filtering_fields": [str(EDGE_FILTERING)],
+        "edge_filtering_lookup": {"34": []},
+    }
+    
+    # mock
+    mock_get_template = mock_Environment.return_value.get_template
+    mock_render = mock_get_template.return_value.render
+
+    # call
+    net = Network("Network1")
+    html_output = net.render_template(# <--------------------
+        template_filename=TEMPLATE_FILENAME, 
+        enable_highlighting=ENABLE_HIGHLIGHTING, 
+        edge_filtering=EDGE_FILTERING) 
 
     # assert
     mock_get_template.assert_called_once_with(TEMPLATE_FILENAME)
     mock_render.assert_called_once_with(width=WIDTH, height=HEIGHT, data=DATA, pyvisjs=PYVISJS)
 
 @patch('pyvisjs.network.open_file')
 @patch('pyvisjs.network.save_file')
```

### Comparing `pyvisjs-0.0.0.dev8/tests/test_node.py` & `pyvisjs-1.0.0a1/tests/test_node.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 
     # mock
 
     # call
     n = Node(NODE_ID)
     
     # assert
-    assert n.id == NODE_ID
+    assert n.id == str(NODE_ID)
 
 def test_node_init_positional_args():
     # init
-    NODE_ID = 1
+    NODE_ID = "X"
     NODE_LABEL = "label"
     NODE_COLOR = "lime"
     NODE_SHAPE = "circle"
     NODE_SIZE = 50
 
     # mock
 
@@ -26,15 +26,15 @@
     n = Node(NODE_ID, NODE_LABEL, NODE_COLOR, NODE_SHAPE, NODE_SIZE)
     
     # assert
     assert (n.id, n.label, n.color, n.shape, n.size) == (NODE_ID, NODE_LABEL, NODE_COLOR, NODE_SHAPE, NODE_SIZE)
 
 def test_node_init_keyword_args():
     # init
-    NODE_ID = 1
+    NODE_ID = "1"
     NODE_LABEL = "label"
     NODE_COLOR = "lime"
     NODE_SHAPE = "circle"
     NODE_SIZE = 50
     NODE_CID = 1
 
     # mock
@@ -43,15 +43,15 @@
     n = Node(NODE_ID, label=NODE_LABEL, cid=NODE_CID, size=NODE_SIZE, shape=NODE_SHAPE, color=NODE_COLOR)
     
     # assert
     assert (n.id, n.label, n.color, n.shape, n.size, n.cid) == (NODE_ID, NODE_LABEL, NODE_COLOR, NODE_SHAPE, NODE_SIZE, NODE_CID)
 
 def test_node_init_kwargs():
     # init
-    NODE_ID = 1
+    NODE_ID = "hello_is_id"
     NODE_LABEL = "label"
     NODE_COLOR = "lime"
     NODE_SHAPE = "circle"
     NODE_SIZE = 50
     NODE_CID = 1
     NODE_CATEGORY = "category1"
     NODE_AMOUNT = 1009.4
@@ -72,15 +72,15 @@
     NODE_ID = 1
     NODE_LABEL = "label"
     NODE_COLOR = "lime"
     NODE_SHAPE = "circle"
     NODE_CID = None
     NODE_SIZE = 50
     NODE_DICT = {
-            "id": NODE_ID,
+            "id": str(NODE_ID),
             "label": NODE_LABEL,
             "color": NODE_COLOR,
             "shape": NODE_SHAPE,
             "size": NODE_SIZE,
             # no element for cid, because it was set to None
         }
```

### Comparing `pyvisjs-0.0.0.dev8/tests/test_options.py` & `pyvisjs-1.0.0a1/tests/test_options.py`

 * *Files identical despite different names*

### Comparing `pyvisjs-0.0.0.dev8/tests/test_utils.py` & `pyvisjs-1.0.0a1/tests/test_utils.py`

 * *Files identical despite different names*

