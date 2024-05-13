# Comparing `tmp/pyterrgen-0.0.1.38.tar.gz` & `tmp/pyterrgen-0.0.1.39.tar.gz`

## Comparing `pyterrgen-0.0.1.38.tar` & `pyterrgen-0.0.1.39.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.38/.pylintrc
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.38/automata.dot
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.38/requirements.txt
--rw-r--r--   0        0        0     3253 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.38/src/PyTerrGen/.gitignore
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.38/src/PyTerrGen/__init__.py
--rw-r--r--   0        0        0     9021 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.38/src/PyTerrGen/cells.py
--rw-r--r--   0        0        0     7552 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.38/src/PyTerrGen/grid.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.38/src/PyTerrGen/main.py
--rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.38/src/PyTerrGen/style.qss
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.38/src/PyTerrGen/ui/__init__.py
--rw-r--r--   0        0        0     3902 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.38/src/PyTerrGen/ui/grid_ui.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.38/src/PyTerrGen/ui/main.py
--rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.38/src/PyTerrGen/ui/main_window.py
--rw-r--r--   0        0        0    11005 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.38/src/PyTerrGen/ui/widgets.py
--rw-r--r--   0        0        0   121979 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.38/src/PyTerrGen/ui/assets/.readme/automata.png
--rw-r--r--   0        0        0   332949 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.38/src/PyTerrGen/ui/assets/.readme/generation.gif
--rw-r--r--   0        0        0    18712 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.38/src/PyTerrGen/ui/assets/.readme/generation_stage12.png
--rw-r--r--   0        0        0    53212 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.38/src/PyTerrGen/ui/assets/.readme/logo.png
--rw-r--r--   0        0        0    30349 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.38/src/PyTerrGen/ui/assets/.readme/sidepanel.png
--rw-r--r--   0        0        0    61087 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.38/src/PyTerrGen/ui/assets/.readme/ui.png
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.38/src/PyTerrGen/ui/assets/desert/cacti.png
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.38/src/PyTerrGen/ui/assets/desert/pyramid1.png
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.38/src/PyTerrGen/ui/assets/desert/pyramid2.png
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.38/src/PyTerrGen/ui/assets/desert/pyramid3.png
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.38/src/PyTerrGen/ui/assets/desert/pyramid4.png
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.38/src/PyTerrGen/ui/assets/desert/wasteland.png
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.38/src/PyTerrGen/ui/assets/forest/birch.png
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.38/src/PyTerrGen/ui/assets/forest/oak.png
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.38/src/PyTerrGen/ui/assets/forest/pine.png
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.38/src/PyTerrGen/ui/assets/mountain/peaky.png
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.38/src/PyTerrGen/ui/assets/mountain/steep.png
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.38/src/PyTerrGen/ui/assets/plains/grassy.png
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.38/src/PyTerrGen/ui/assets/plains/house1.png
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.38/src/PyTerrGen/ui/assets/plains/house2.png
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.38/src/PyTerrGen/ui/assets/plains/house3.png
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.38/src/PyTerrGen/ui/assets/plains/house4.png
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.38/src/PyTerrGen/ui/assets/snowy/mountain.png
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.38/src/PyTerrGen/ui/assets/snowy/snowy.png
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.38/src/PyTerrGen/ui/assets/swamp/swamp.png
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.38/src/PyTerrGen/ui/assets/water/ship1.png
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.38/src/PyTerrGen/ui/assets/water/ship2.png
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.38/src/PyTerrGen/ui/assets/water/ship3.png
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.38/src/PyTerrGen/ui/assets/water/ship4.png
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.38/src/PyTerrGen/ui/assets/water/wavy1.png
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.38/src/PyTerrGen/ui/assets/water/wavy2.png
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.38/src/PyTerrGen/ui/assets/water/wavy3.png
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.38/src/PyTerrGen/ui/assets/water/wavy4.png
--rw-r--r--   0        0        0     3253 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.38/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.38/LICENSE
--rw-r--r--   0        0        0    10239 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.38/README.md
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.38/pyproject.toml
--rw-r--r--   0        0        0    11154 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.38/PKG-INFO
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.39/.pylintrc
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.39/automata.dot
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.39/requirements.txt
+-rw-r--r--   0        0        0     3253 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.39/src/PyTerrGen/.gitignore
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.39/src/PyTerrGen/__init__.py
+-rw-r--r--   0        0        0     8998 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.39/src/PyTerrGen/cells.py
+-rw-r--r--   0        0        0     7582 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.39/src/PyTerrGen/grid.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.39/src/PyTerrGen/main.py
+-rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.39/src/PyTerrGen/style.qss
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.39/src/PyTerrGen/ui/__init__.py
+-rw-r--r--   0        0        0     3982 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.39/src/PyTerrGen/ui/grid_ui.py
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.39/src/PyTerrGen/ui/main.py
+-rw-r--r--   0        0        0     2711 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.39/src/PyTerrGen/ui/main_window.py
+-rw-r--r--   0        0        0    11005 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.39/src/PyTerrGen/ui/widgets.py
+-rw-r--r--   0        0        0   121979 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.39/src/PyTerrGen/ui/assets/.readme/automata.png
+-rw-r--r--   0        0        0   332949 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.39/src/PyTerrGen/ui/assets/.readme/generation.gif
+-rw-r--r--   0        0        0    18712 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.39/src/PyTerrGen/ui/assets/.readme/generation_stage12.png
+-rw-r--r--   0        0        0    53212 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.39/src/PyTerrGen/ui/assets/.readme/logo.png
+-rw-r--r--   0        0        0    30349 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.39/src/PyTerrGen/ui/assets/.readme/sidepanel.png
+-rw-r--r--   0        0        0    61087 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.39/src/PyTerrGen/ui/assets/.readme/ui.png
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.39/src/PyTerrGen/ui/assets/desert/cacti.png
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.39/src/PyTerrGen/ui/assets/desert/pyramid1.png
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.39/src/PyTerrGen/ui/assets/desert/pyramid2.png
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.39/src/PyTerrGen/ui/assets/desert/pyramid3.png
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.39/src/PyTerrGen/ui/assets/desert/pyramid4.png
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.39/src/PyTerrGen/ui/assets/desert/wasteland.png
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.39/src/PyTerrGen/ui/assets/forest/birch.png
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.39/src/PyTerrGen/ui/assets/forest/oak.png
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.39/src/PyTerrGen/ui/assets/forest/pine.png
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.39/src/PyTerrGen/ui/assets/mountain/peaky.png
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.39/src/PyTerrGen/ui/assets/mountain/steep.png
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.39/src/PyTerrGen/ui/assets/plains/grassy.png
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.39/src/PyTerrGen/ui/assets/plains/house1.png
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.39/src/PyTerrGen/ui/assets/plains/house2.png
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.39/src/PyTerrGen/ui/assets/plains/house3.png
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.39/src/PyTerrGen/ui/assets/plains/house4.png
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.39/src/PyTerrGen/ui/assets/snowy/mountain.png
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.39/src/PyTerrGen/ui/assets/snowy/snowy.png
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.39/src/PyTerrGen/ui/assets/swamp/swamp.png
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.39/src/PyTerrGen/ui/assets/water/ship1.png
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.39/src/PyTerrGen/ui/assets/water/ship2.png
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.39/src/PyTerrGen/ui/assets/water/ship3.png
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.39/src/PyTerrGen/ui/assets/water/ship4.png
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.39/src/PyTerrGen/ui/assets/water/wavy1.png
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.39/src/PyTerrGen/ui/assets/water/wavy2.png
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.39/src/PyTerrGen/ui/assets/water/wavy3.png
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.39/src/PyTerrGen/ui/assets/water/wavy4.png
+-rw-r--r--   0        0        0     3253 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.39/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.39/LICENSE
+-rw-r--r--   0        0        0    10330 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.39/README.md
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.39/pyproject.toml
+-rw-r--r--   0        0        0    11241 2020-02-02 00:00:00.000000 pyterrgen-0.0.1.39/PKG-INFO
```

### Comparing `pyterrgen-0.0.1.38/src/PyTerrGen/.gitignore` & `pyterrgen-0.0.1.39/src/PyTerrGen/.gitignore`

 * *Files identical despite different names*

### Comparing `pyterrgen-0.0.1.38/src/PyTerrGen/cells.py` & `pyterrgen-0.0.1.39/src/PyTerrGen/cells.py`

 * *Files 1% similar despite different names*

```diff
@@ -255,15 +255,21 @@
     A cell that represents a snowy area
     """
 
     SUBTYPES = {"snowy": 0.5, "mountain": 0.5}
 
     def __init__(self, coordinates: tuple[int, int], age: int = 0) -> None:
         super().__init__(
-            coordinates, age, 7, "snowy", "#ecfffd", ["forest", "mountain", "plains"], 0.11
+            coordinates,
+            age,
+            7,
+            "snowy",
+            "#ecfffd",
+            ["forest", "mountain", "plains"],
+            0.11,
         )
 
     def infect(self, other: Cell, coeff: int = 0) -> None:
         """
         Snowy cell's infect method
         Infects forest, mountain and plains cells with either a certain chance or if there are from
         1 to 3 swamp cells around it
@@ -281,23 +287,15 @@
     Mountain cell class
     A cell class that represents an area of mountain type
     """
 
     SUBTYPES = {"peaky": 0.05, "steep": 0.95}
 
     def __init__(self, coordinates: tuple[int, int], age: int = 0) -> None:
-        super().__init__(
-            coordinates,
-            age,
-            7,
-            "mountain",
-            "#808080",
-            ["plains"],
-            0.17
-        )
+        super().__init__(coordinates, age, 7, "mountain", "#808080", ["plains"], 0.17)
 
     def infect(self, other: Cell, coeff: int = 0) -> None:
         """
         Mountain cell's infect method
         """
         if (
             other.type in self.submissive
```

### Comparing `pyterrgen-0.0.1.38/src/PyTerrGen/grid.py` & `pyterrgen-0.0.1.39/src/PyTerrGen/grid.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Map/grid class
 """
 
 import random
 import numpy as np
 
-from py_terrain.cells import Cell, Void, Water, Plains, Desert, Forest, Mountain, Swamp, Snowy
+from PyTerrGen.cells import Cell, Void, Water, Plains, Desert, Forest, Mountain, Swamp, Snowy
 
 
 class Grid:
     """
     Grid class
     """
 
@@ -20,15 +20,17 @@
         self._m = m
         self.seed = seed if seed else self.generate_seed()
         self.destinations = [0, 0]
         self.scaling_coeff = (n * m) / (43 * 28)
         if self.scaling_coeff < 0.8:
             self.scaling_coeff += (1 - self.scaling_coeff) / ((self._n + self._m) / 10)
         elif self.scaling_coeff > 1.2:
-            self.scaling_coeff -=  (self.scaling_coeff) / ((self._n + self._m) / 10) ** 0.2
+            self.scaling_coeff -= (self.scaling_coeff) / (
+                (self._n + self._m) / 10
+            ) ** 0.2
         self.set_up()
 
     def __getitem__(self, i):
         return self._map[i]
 
     def generate_seed(self):
         """
```

### Comparing `pyterrgen-0.0.1.38/src/PyTerrGen/style.qss` & `pyterrgen-0.0.1.39/src/PyTerrGen/style.qss`

 * *Files identical despite different names*

### Comparing `pyterrgen-0.0.1.38/src/PyTerrGen/ui/grid_ui.py` & `pyterrgen-0.0.1.39/src/PyTerrGen/ui/grid_ui.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,30 +3,32 @@
 """
 
 from PySide6.QtWidgets import QWidget, QVBoxLayout, QHBoxLayout, QLabel, QFileDialog
 
 from PySide6.QtCore import Qt
 from PySide6.QtGui import QColor, QPixmap
 
-from py_terrain.grid import Grid
+from PyTerrGen.grid import Grid
 
 
 class GridWidget(QWidget):
     """
     Map grid widget
     """
 
     DELAY = 300
 
     def __init__(
         self, n_rows: int, n_cols: int, seed: str | None = None, parent=None
     ) -> None:
         super().__init__(parent)
         self.grid = Grid(n_rows, n_cols, seed)
-        self.setFixedSize((int(1400*parent.width()/1920)),(int(900*parent.height()/1080)))
+        self.setFixedSize(
+            (int(1400 * parent.width() / 1920)), (int(900 * parent.height() / 1080))
+        )
         self.n_rows = n_rows
         self.n_cols = n_cols
         self.cells = []
         self.grid_layout = QVBoxLayout()
         self.grid_layout.setSpacing(0)
         self.setContentsMargins(0, 0, 0, 0)
         self.parent_ = parent
@@ -95,15 +97,17 @@
     Cell widget
     """
 
     def __init__(self, parent=None, grid_width=None, grid_height=None):
         super().__init__()
         self.size = grid_width, grid_height
         self.parent_ = parent
-        min_side = min(self.parent_.width() / grid_width, self.parent_.height() / grid_height)
+        min_side = min(
+            self.parent_.width() / grid_width, self.parent_.height() / grid_height
+        )
         self.setFixedSize(min_side, min_side)
         self.setAutoFillBackground(True)
         self.setAlignment(Qt.AlignmentFlag.AlignCenter)
 
     def set_color(self, color):
         """
         Set color of the cell
@@ -117,10 +121,14 @@
         Set texture to cell
         """
         pixmap = QPixmap(filepath)
         self.setPixmap(pixmap)
         self.setScaledContents(True)
 
     def resize_(self):
-        min_side = min(self.parent_.width() / self.size[0], self.parent_.height() / self.size[1])
-        print(min_side, self.parent_.width())
+        """
+        Resize cell
+        """
+        min_side = min(
+            self.parent_.width() / self.size[0], self.parent_.height() / self.size[1]
+        )
         self.setFixedSize(min_side, min_side)
```

### Comparing `pyterrgen-0.0.1.38/src/PyTerrGen/ui/main_window.py` & `pyterrgen-0.0.1.39/src/PyTerrGen/ui/main_window.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,30 +5,30 @@
 from PySide6.QtWidgets import (
     QMainWindow,
     QHBoxLayout,
     QWidget,
 )
 
 from PySide6.QtCore import QTimer, Qt
-from py_terrain.ui.grid_ui import GridWidget
-from py_terrain.ui.widgets import SidePanelWidget
+from PyTerrGen.ui.grid_ui import GridWidget
+from PyTerrGen.ui.widgets import SidePanelWidget
 
 
 class MainWindow(QMainWindow):
     """
     Main window
     """
 
     DELAY = 300
 
     def __init__(self) -> None:
         super().__init__()
         self.setMaximumSize(1920, 1080)
         self.setMinimumSize(1280, 720)
-        self.resize(1280, 720)
+        self.resize(1400, 720)
         self.setWindowTitle("Terrain Generation")
         self.central_widget = QWidget()
         self.setCentralWidget(self.central_widget)
 
         self.window_layout = QHBoxLayout()
         self.central_widget.setLayout(self.window_layout)
 
@@ -79,12 +79,13 @@
         """
         cls.DELAY = new
 
     def resizeEvent(self, event):
         """
         Resize
         """
-        # print("AAA")
-        self.grid.setFixedSize((int(1400*self.width()/1920)),(int(900*self.height()/1080)))
+        self.grid.setFixedSize(
+            (int(1400 * self.width() / 1920)), (int(900 * self.height() / 1080))
+        )
         for cell in self.grid.cells:
             cell.resize_()
         QMainWindow.resizeEvent(self, event)
```

### Comparing `pyterrgen-0.0.1.38/src/PyTerrGen/ui/widgets.py` & `pyterrgen-0.0.1.39/src/PyTerrGen/ui/widgets.py`

 * *Files identical despite different names*

### Comparing `pyterrgen-0.0.1.38/src/PyTerrGen/ui/assets/.readme/automata.png` & `pyterrgen-0.0.1.39/src/PyTerrGen/ui/assets/.readme/automata.png`

 * *Files identical despite different names*

### Comparing `pyterrgen-0.0.1.38/src/PyTerrGen/ui/assets/.readme/generation.gif` & `pyterrgen-0.0.1.39/src/PyTerrGen/ui/assets/.readme/generation.gif`

 * *Files identical despite different names*

### Comparing `pyterrgen-0.0.1.38/src/PyTerrGen/ui/assets/.readme/generation_stage12.png` & `pyterrgen-0.0.1.39/src/PyTerrGen/ui/assets/.readme/generation_stage12.png`

 * *Files identical despite different names*

### Comparing `pyterrgen-0.0.1.38/src/PyTerrGen/ui/assets/.readme/logo.png` & `pyterrgen-0.0.1.39/src/PyTerrGen/ui/assets/.readme/logo.png`

 * *Files identical despite different names*

### Comparing `pyterrgen-0.0.1.38/src/PyTerrGen/ui/assets/.readme/sidepanel.png` & `pyterrgen-0.0.1.39/src/PyTerrGen/ui/assets/.readme/sidepanel.png`

 * *Files identical despite different names*

### Comparing `pyterrgen-0.0.1.38/src/PyTerrGen/ui/assets/.readme/ui.png` & `pyterrgen-0.0.1.39/src/PyTerrGen/ui/assets/.readme/ui.png`

 * *Files identical despite different names*

### Comparing `pyterrgen-0.0.1.38/.gitignore` & `pyterrgen-0.0.1.39/.gitignore`

 * *Files identical despite different names*

### Comparing `pyterrgen-0.0.1.38/LICENSE` & `pyterrgen-0.0.1.39/LICENSE`

 * *Files identical despite different names*

### Comparing `pyterrgen-0.0.1.38/README.md` & `pyterrgen-0.0.1.39/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,19 @@
     - [Cells types](#cells-types-and-certain-behaviours)
 - [Showcase](#showcase)
 - [Credits](#developers-and-responsibilities)
 - [License](#license)
 
 ## Installation
 ### Install via PyPi
-...
+**Prerequisites:** Python 3.11, latest pip version
+```
+pip install PyTerrGen
+PyTerrGen
+```
 ### Manual install
 **Prerequisites:** Python 3.11  
 Clone the repo, cd into the folder, install dependencies and run main file
 ```
 git clone https://github.com/n1n1n1q/Terrain-Generation
 cd Terrain-Generation
 pip install -r requirements.txt
```

### Comparing `pyterrgen-0.0.1.38/pyproject.toml` & `pyterrgen-0.0.1.39/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "PyTerrGen"
-version = "0.0.1.38"
+version = "0.0.1.39"
 authors = [
   {author = "Oleh Basystyi", name = "Oleh"},
   {author = "Anna Stasyshyn", name = "Anna"},
   {author = "Viktor Pakholok", name = "Viktor"},
 ]
 description = "Procedural map generation with cellular automata in Python"
 readme = "README.md"
```

### Comparing `pyterrgen-0.0.1.38/PKG-INFO` & `pyterrgen-0.0.1.39/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: PyTerrGen
-Version: 0.0.1.38
+Version: 0.0.1.39
 Summary: Procedural map generation with cellular automata in Python
 Project-URL: Homepage, https://github.com/n1n1n1q/Terrain-Generation
 Project-URL: Issues, https://github.com/n1n1n1q/Terrain-Generation/issues
 Author: Oleh, Anna, Viktor
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -43,15 +43,19 @@
     - [Cells types](#cells-types-and-certain-behaviours)
 - [Showcase](#showcase)
 - [Credits](#developers-and-responsibilities)
 - [License](#license)
 
 ## Installation
 ### Install via PyPi
-...
+**Prerequisites:** Python 3.11, latest pip version
+```
+pip install PyTerrGen
+PyTerrGen
+```
 ### Manual install
 **Prerequisites:** Python 3.11  
 Clone the repo, cd into the folder, install dependencies and run main file
 ```
 git clone https://github.com/n1n1n1q/Terrain-Generation
 cd Terrain-Generation
 pip install -r requirements.txt
```

