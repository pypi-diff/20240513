# Comparing `tmp/echordpost-0.1.1.tar.gz` & `tmp/echordpost-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echordpost-0.1.1.tar", max compression
+gzip compressed data, was "echordpost-0.1.2.tar", max compression
```

## Comparing `echordpost-0.1.1.tar` & `echordpost-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    10223 2024-01-27 11:57:10.555640 echordpost-0.1.1/eCHORDpost/IPF_V1.py
--rw-r--r--   0        0        0     6608 2024-01-04 08:16:59.256806 echordpost-0.1.1/eCHORDpost/Symetry.py
--rw-r--r--   0        0        0     4541 2024-01-05 09:41:12.000000 echordpost-0.1.1/eCHORDpost/Xallo.py
--rw-r--r--   0        0        0    35823 2024-05-12 20:06:13.943321 echordpost-0.1.1/LICENSE
--rw-r--r--   0        0        0      577 2024-05-12 20:49:04.289054 echordpost-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       12 2024-05-12 20:06:13.944270 echordpost-0.1.1/README.md
--rw-r--r--   0        0        0      904 1970-01-01 00:00:00.000000 echordpost-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    10187 2024-05-12 21:11:27.484859 echordpost-0.1.2/eCHORDpost/IPF_V1.py
+-rw-r--r--   0        0        0     6587 2024-05-12 21:09:35.750260 echordpost-0.1.2/eCHORDpost/Symetry.py
+-rw-r--r--   0        0        0     4541 2024-01-05 09:41:12.000000 echordpost-0.1.2/eCHORDpost/Xallo.py
+-rw-r--r--   0        0        0    35823 2024-05-12 20:06:13.943321 echordpost-0.1.2/LICENSE
+-rw-r--r--   0        0        0      577 2024-05-12 21:12:10.682111 echordpost-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       12 2024-05-12 20:06:13.944270 echordpost-0.1.2/README.md
+-rw-r--r--   0        0        0      904 1970-01-01 00:00:00.000000 echordpost-0.1.2/PKG-INFO
```

### Comparing `echordpost-0.1.1/eCHORDpost/IPF_V1.py` & `echordpost-0.1.2/eCHORDpost/IPF_V1.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,26 +7,26 @@
 
 import numpy as np
 
 import matplotlib.pyplot as plt
 import diffpy.structure as dfs
 
 import Dans_Diffraction as da
-import LibrairiesCyril.Xallo as xa
-from LibrairiesCyril import Symetry as sy
+import Xallo as xa
+import Symetry as sy
 
 from orix.crystal_map import CrystalMap, PhaseList
 from orix.quaternion import Rotation, symmetry
 from orix import plot as orixPlot
 from orix.vector import Vector3d
 
 import tkinter as tk
 from tkinter import filedialog
 
-from LibrairiesCyril import general_functions as gf
+#from LibrairiesCyril import general_functions as gf
 
 root = tk.Tk()       # initialisation du dialogue
 root.withdraw()
 
 #%% réarrangement du tableau d'indexation
 # pour le meilleur score déjà
```

### Comparing `echordpost-0.1.1/eCHORDpost/Symetry.py` & `echordpost-0.1.2/eCHORDpost/Symetry.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 """
 
 
 import os
 
 sep = os.sep
 
-from LibrairiesCyril import Xallo as xa
+import Xallo as xa
 import numpy as np
 import Dans_Diffraction as dif
 
 
 # instruction pour afficher les atbleaux de façon lisible
 np.set_printoptions(suppress=True, precision=2)
```

### Comparing `echordpost-0.1.1/eCHORDpost/Xallo.py` & `echordpost-0.1.2/eCHORDpost/Xallo.py`

 * *Files identical despite different names*

### Comparing `echordpost-0.1.1/LICENSE` & `echordpost-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `echordpost-0.1.1/pyproject.toml` & `echordpost-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "echordpost"
-version = "0.1.1"
+version = "0.1.2"
 description = "Library to run eCHORD post-treatment program"
 authors = ["Langlois Cyril <cyril.langlois@insa-lyon.fr> L'Hôte Gabriel <gabriel.l-hote@insa-lyon.fr>"]
 license = "CECILL"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `echordpost-0.1.1/PKG-INFO` & `echordpost-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echordpost
-Version: 0.1.1
+Version: 0.1.2
 Summary: Library to run eCHORD post-treatment program
 License: CECILL
 Author: Langlois Cyril
 Author-email: cyril.langlois@insa-lyon.fr> L'Hôte Gabriel <gabriel.l-hote@insa-lyon.fr
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

