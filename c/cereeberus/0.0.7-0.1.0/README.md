# Comparing `tmp/cereeberus-0.0.7.tar.gz` & `tmp/cereeberus-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cereeberus-0.0.7.tar", last modified: Sun Nov 27 04:33:05 2022, max compression
+gzip compressed data, was "cereeberus-0.1.0.tar", last modified: Mon May 13 17:10:39 2024, max compression
```

## Comparing `cereeberus-0.0.7.tar` & `cereeberus-0.1.0.tar`

### file list

```diff
@@ -1,31 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 04:33:05.424401 cereeberus-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (122)    35149 2022-11-27 04:32:56.000000 cereeberus-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      588 2022-11-27 04:33:05.424401 cereeberus-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       60 2022-11-27 04:32:56.000000 cereeberus-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 04:33:05.420401 cereeberus-0.0.7/cereeberus/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 04:33:05.420401 cereeberus-0.0.7/cereeberus/cereeberus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      588 2022-11-27 04:33:05.000000 cereeberus-0.0.7/cereeberus/cereeberus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      678 2022-11-27 04:33:05.000000 cereeberus-0.0.7/cereeberus/cereeberus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-27 04:33:05.000000 cereeberus-0.0.7/cereeberus/cereeberus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       26 2022-11-27 04:33:05.000000 cereeberus-0.0.7/cereeberus/cereeberus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       24 2022-11-27 04:33:05.000000 cereeberus-0.0.7/cereeberus/cereeberus.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 04:33:05.420401 cereeberus-0.0.7/cereeberus/compute/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-27 04:32:56.000000 cereeberus-0.0.7/cereeberus/compute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2531 2022-11-27 04:32:56.000000 cereeberus-0.0.7/cereeberus/compute/degree.py
--rw-r--r--   0 runner    (1001) docker     (122)     4114 2022-11-27 04:32:56.000000 cereeberus-0.0.7/cereeberus/compute/draw.py
--rw-r--r--   0 runner    (1001) docker     (122)     3877 2022-11-27 04:32:56.000000 cereeberus-0.0.7/cereeberus/compute/merge.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 04:33:05.424401 cereeberus-0.0.7/cereeberus/data/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-27 04:32:56.000000 cereeberus-0.0.7/cereeberus/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4326 2022-11-27 04:32:56.000000 cereeberus-0.0.7/cereeberus/data/graphs.py
--rw-r--r--   0 runner    (1001) docker     (122)     1103 2022-11-27 04:32:56.000000 cereeberus-0.0.7/cereeberus/data/randomMergeTrees.py
--rw-r--r--   0 runner    (1001) docker     (122)      538 2022-11-27 04:32:56.000000 cereeberus-0.0.7/cereeberus/data/shapes.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 04:33:05.424401 cereeberus-0.0.7/cereeberus/reeb/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-27 04:32:56.000000 cereeberus-0.0.7/cereeberus/reeb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3922 2022-11-27 04:32:56.000000 cereeberus-0.0.7/cereeberus/reeb/reeb.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 04:33:05.424401 cereeberus-0.0.7/cereeberus/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-27 04:32:56.000000 cereeberus-0.0.7/cereeberus/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      895 2022-11-27 04:32:56.000000 cereeberus-0.0.7/cereeberus/tests/test_node_ops.py
--rw-r--r--   0 runner    (1001) docker     (122)      323 2022-11-27 04:32:56.000000 cereeberus-0.0.7/cereeberus/tests/test_reeb_class.py
--rw-r--r--   0 runner    (1001) docker     (122)      620 2022-11-27 04:32:56.000000 cereeberus-0.0.7/cereeberus/tests/test_up_down_degree.py
--rw-r--r--   0 runner    (1001) docker     (122)      712 2022-11-27 04:32:56.000000 cereeberus-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-27 04:33:05.424401 cereeberus-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:10:39.695194 cereeberus-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-13 17:10:24.000000 cereeberus-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-05-13 17:10:39.695194 cereeberus-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-13 17:10:24.000000 cereeberus-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:10:39.687194 cereeberus-0.1.0/cereeberus/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:10:39.691194 cereeberus-0.1.0/cereeberus/cereeberus/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-13 17:10:24.000000 cereeberus-0.1.0/cereeberus/cereeberus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:10:39.691194 cereeberus-0.1.0/cereeberus/cereeberus/compute/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-13 17:10:24.000000 cereeberus-0.1.0/cereeberus/cereeberus/compute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-05-13 17:10:24.000000 cereeberus-0.1.0/cereeberus/cereeberus/compute/degree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9025 2024-05-13 17:10:24.000000 cereeberus-0.1.0/cereeberus/cereeberus/compute/distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4294 2024-05-13 17:10:24.000000 cereeberus-0.1.0/cereeberus/cereeberus/compute/draw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7741 2024-05-13 17:10:24.000000 cereeberus-0.1.0/cereeberus/cereeberus/compute/merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29088 2024-05-13 17:10:24.000000 cereeberus-0.1.0/cereeberus/cereeberus/compute/merge_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6082 2024-05-13 17:10:24.000000 cereeberus-0.1.0/cereeberus/cereeberus/compute/uf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:10:39.691194 cereeberus-0.1.0/cereeberus/cereeberus/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 17:10:24.000000 cereeberus-0.1.0/cereeberus/cereeberus/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4628 2024-05-13 17:10:24.000000 cereeberus-0.1.0/cereeberus/cereeberus/data/ex_graphs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-05-13 17:10:24.000000 cereeberus-0.1.0/cereeberus/cereeberus/data/ex_reebgraphs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-13 17:10:24.000000 cereeberus-0.1.0/cereeberus/cereeberus/data/randomMergeTrees.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-13 17:10:24.000000 cereeberus-0.1.0/cereeberus/cereeberus/data/shapes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:10:39.695194 cereeberus-0.1.0/cereeberus/cereeberus/reeb/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-13 17:10:24.000000 cereeberus-0.1.0/cereeberus/cereeberus/reeb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3326 2024-05-13 17:10:24.000000 cereeberus-0.1.0/cereeberus/cereeberus/reeb/merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17744 2024-05-13 17:10:24.000000 cereeberus-0.1.0/cereeberus/cereeberus/reeb/reebgraph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:10:39.695194 cereeberus-0.1.0/cereeberus/cereeberus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-05-13 17:10:39.000000 cereeberus-0.1.0/cereeberus/cereeberus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-13 17:10:39.000000 cereeberus-0.1.0/cereeberus/cereeberus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 17:10:39.000000 cereeberus-0.1.0/cereeberus/cereeberus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-13 17:10:39.000000 cereeberus-0.1.0/cereeberus/cereeberus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-13 17:10:39.000000 cereeberus-0.1.0/cereeberus/cereeberus.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-13 17:10:24.000000 cereeberus-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 17:10:39.695194 cereeberus-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:10:39.695194 cereeberus-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-13 17:10:24.000000 cereeberus-0.1.0/tests/test_merge_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-13 17:10:24.000000 cereeberus-0.1.0/tests/test_node_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7000 2024-05-13 17:10:24.000000 cereeberus-0.1.0/tests/test_reeb_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-13 17:10:24.000000 cereeberus-0.1.0/tests/test_up_down_degree.py
```

### Comparing `cereeberus-0.0.7/LICENSE` & `cereeberus-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cereeberus-0.0.7/cereeberus/cereeberus.egg-info/SOURCES.txt` & `cereeberus-0.1.0/cereeberus/cereeberus.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 LICENSE
 README.md
 pyproject.toml
+cereeberus/cereeberus/__init__.py
 cereeberus/cereeberus.egg-info/PKG-INFO
 cereeberus/cereeberus.egg-info/SOURCES.txt
 cereeberus/cereeberus.egg-info/dependency_links.txt
 cereeberus/cereeberus.egg-info/requires.txt
 cereeberus/cereeberus.egg-info/top_level.txt
-cereeberus/compute/__init__.py
-cereeberus/compute/degree.py
-cereeberus/compute/draw.py
-cereeberus/compute/merge.py
-cereeberus/data/__init__.py
-cereeberus/data/graphs.py
-cereeberus/data/randomMergeTrees.py
-cereeberus/data/shapes.py
-cereeberus/reeb/__init__.py
-cereeberus/reeb/reeb.py
-cereeberus/tests/__init__.py
-cereeberus/tests/test_node_ops.py
-cereeberus/tests/test_reeb_class.py
-cereeberus/tests/test_up_down_degree.py
+cereeberus/cereeberus/compute/__init__.py
+cereeberus/cereeberus/compute/degree.py
+cereeberus/cereeberus/compute/distance.py
+cereeberus/cereeberus/compute/draw.py
+cereeberus/cereeberus/compute/merge.py
+cereeberus/cereeberus/compute/merge_class.py
+cereeberus/cereeberus/compute/uf.py
+cereeberus/cereeberus/data/__init__.py
+cereeberus/cereeberus/data/ex_graphs.py
+cereeberus/cereeberus/data/ex_reebgraphs.py
+cereeberus/cereeberus/data/randomMergeTrees.py
+cereeberus/cereeberus/data/shapes.py
+cereeberus/cereeberus/reeb/__init__.py
+cereeberus/cereeberus/reeb/merge.py
+cereeberus/cereeberus/reeb/reebgraph.py
+tests/test_merge_tree.py
+tests/test_node_ops.py
+tests/test_reeb_class.py
+tests/test_up_down_degree.py
```

### Comparing `cereeberus-0.0.7/cereeberus/compute/draw.py` & `cereeberus-0.1.0/cereeberus/cereeberus/compute/draw.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+import matplotlib.pyplot as plt
+import matplotlib as mpl
+import numpy as np
+
 def dict_to_list(d):
     l = []
     for i in d:
         l.append(d[i])
     return l
 
 def line_loop_index(R):
@@ -75,45 +79,48 @@
         x1 += (midpt[0] - pt0[0])/100
         y1 = a1*x1 + b1
         x2 += (pt1[0] - midpt[0])/100
         y2 = a2*x2 + b2
     return points    
 
 def reeb_plot(R, pos, cpx=.1, cpy=.1):
-    """Compute bezier curves for plotting two edges between a single set of nodes
+    """Main plotting function for the Reeb Graph Class
     
     Args:
         R (Reeb Graph): object of Reeb Graph class
         cp (float): parameter to control curvature of loops in the plotting function
 
     Returns:
         plot (Reeb Graph): custom visualization of Reeb Graph
     """
 
-    import matplotlib.pyplot as plt
-    import matplotlib as mpl
-    import numpy as np
     viridis = mpl.colormaps['viridis'].resampled(16)
     fig, ax = plt.subplots()
 
     n = len(R.nodes)
     fx_max = 0
     fx_min = 0
-    if type(R.fx) == dict:
-        R.fxl = dict_to_list(R.fx)
+    if type(R.f) == dict:
+        f_list = dict_to_list(R.f)
     else:
-        R.fxl = R.fx
-    Rfx = np.array(R.fxl)
+        f_list = R.f
+    Rfx = np.array(f_list)
     Rfx = Rfx[np.isfinite(Rfx)]
     fx_max = Rfx.max()
     fx_min = Rfx.min()
 
-    colormap = []
-    for i in range (0,n):
-        colormap.append((R.fx[i]-fx_min)/fx_max)
+    colormap = {}
+    for i in R.nodes:
+        if R.f[i]==np.inf:
+            fx = fx_max+1
+            x = R.pos_fx[i][0]
+            R.pos_fx[i] = (x,fx)
+        else:
+            fx = R.f[i]
+        colormap[i] = ((fx-fx_min)/fx_max)
 
 
     edge_list = list(R.edges)
     line_index, loop_index = line_loop_index(R)
     for i in line_index:
         node0 = edge_list[i][0]
         node1 = edge_list[i][1]
@@ -133,9 +140,11 @@
         curve = bezier_curve(pos[node0], (xmid0, ymid0), pos[node1])
         c = np.array(curve)
         plt.plot(c[:,0], c[:,1], color='grey', zorder = 0)
         curve = bezier_curve(pos[node0], (xmid1, ymid1), pos[node1])
         c = np.array(curve)
         plt.plot(c[:,0], c[:,1], color='grey', zorder = 0)
 
-    for i in range(0, len(R.nodes)):
-        ax.scatter(pos[i][0], pos[i][1], s = 250, color = viridis(colormap[i]))
+    for i in R.nodes:
+        ax.scatter(pos[i][0], pos[i][1], s = 250, color = viridis(colormap[i]))
+
+    ax.tick_params(left = True, bottom = False, labelleft = True, labelbottom = False)
```

### Comparing `cereeberus-0.0.7/cereeberus/data/randomMergeTrees.py` & `cereeberus-0.1.0/cereeberus/cereeberus/data/randomMergeTrees.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 
-
-"""
-Some code to generate random Merge Trees to work with. 
-"""
 import networkx as nx
 import numpy as np
-from reeb.reeb import Reeb
+from cereeberus.reeb.reebgraph import ReebGraph
 
 def randomMerge(n = 10):
     """
     Generates a random tree with n nodes + 1 root.
     Function defined is inverted distance from root node. 
     """
     # Generate a random tree
@@ -27,13 +23,13 @@
 
     # Add a root node 
     T.add_node(n)
     T.add_edge(topNodeIndex,n)
     fx.append(np.inf)
 
     # Generate the Reeb graph class for this input 
-    T_Merge = Reeb(T,fx)
+    T_Merge = ReebGraph(T,fx)
 
     # Overwrite the position drawing to make drawing not freak out
     T_Merge.pos_fx[n] = ( T_Merge.pos[n][0], max(fx[:-1]) + 3)
 
     return T_Merge
```

### Comparing `cereeberus-0.0.7/cereeberus/tests/test_node_ops.py` & `cereeberus-0.1.0/tests/test_node_ops.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 import unittest
-import data.graphs as graphs
-import compute.degree as degree
+import cereeberus.data.ex_reebgraphs as reeb
+import cereeberus.compute.degree as degree
 
 class TestNodeOps(unittest.TestCase):
     def test_minimal(self):
-        R = graphs.reeb_torus()
-        R_min = degree.minimal_reeb(R)
-        nodes = [0, 1, 2, 3]
-        edges = [(0, 1, 0), (1, 2, 0), (1, 2, 1), (2, 3, 0)]
-        self.assertEqual(list(R_min.nodes), nodes)
-        self.assertEqual(list(R_min.edges), edges)
+        # TODO Need to update
+        pass
+        # R = reeb.torus()
+        # R_min = degree.minimal_reeb(R)
+        # nodes = [0, 1, 2, 3]
+        # edges = [(0, 1, 0), (1, 2, 0), (1, 2, 1), (2, 3, 0)]
+        # self.assertEqual(list(R_min.nodes), nodes)
+        # self.assertEqual(list(R_min.edges), edges)
         
     def test_add_nodes(self):
-        R = graphs.reeb_torus()
-        R_add = degree.add_nodes(R, fx=3.5, x = 1)
-        R_add = degree.add_nodes(R_add, fx = 1.5, x = 1)
-        nodes = [0, 1, 2, 3, 4, 5, 6, 7, 8]
-        edges = [(0, 8, 0), (1, 2, 0), (1, 3, 0), (1, 8, 0), (2, 6, 0), (3, 7, 0), (4, 5, 0), (4, 6, 0), (4, 7, 0)]
-        self.assertEqual(list(R_add.nodes), nodes)
-        self.assertEqual(list(R_add.edges), edges)
+        # TODO Need to update 
+        pass
+        # R = reeb.torus()
+        # R_add = degree.add_nodes(R, fx=3.5, x = 1)
+        # R_add = degree.add_nodes(R_add, fx = 1.5, x = 1)
+        # nodes = [0, 1, 2, 3, 4, 5, 6, 7, 8]
+        # edges = [(0, 8, 0), (1, 2, 0), (1, 3, 0), (1, 8, 0), (2, 6, 0), (3, 7, 0), (4, 5, 0), (4, 6, 0), (4, 7, 0)]
+        # self.assertEqual(list(R_add.nodes), nodes)
+        # self.assertEqual(list(R_add.edges), edges)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cereeberus-0.0.7/cereeberus/tests/test_up_down_degree.py` & `cereeberus-0.1.0/tests/test_up_down_degree.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import unittest
-import data.graphs as graphs
+import cereeberus.data.reeb as reeb
 
 class TestUpDownDegree(unittest.TestCase):
     def test_up_degree(self):
         actual_up_degree = {0: 0, 1: 1, 2: 1, 3: 2, 4: 0, 5:1, 6:2, 7:1}
-        dm = graphs.reeb_dancing_man()
+        dm = reeb.dancing_man()
         test_up_degree = dm.up_deg
         self.assertEqual(actual_up_degree, test_up_degree)
 
     def test_down_degree(self):
         actual_down_degree = {0: 1, 1: 2, 2: 2, 3: 1, 4:1, 5:0, 6:1, 7:0}
-        dm = graphs.reeb_dancing_man()
+        dm = reeb.dancing_man()
         test_down_degree = dm.down_deg
         self.assertEqual(actual_down_degree, test_down_degree)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cereeberus-0.0.7/pyproject.toml` & `cereeberus-0.1.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 [build]
 
 [project]
 name = "cereeberus"
-version = "0.0.7"
+version = "0.1.0"
 authors = [
+  { name="Liz Munch", email="muncheli@msu.edu" },
   { name="Danielle Barnes", email="barnesd8@msu.edu" },
 ]
-description = "Package to do fun things with Reeb graphs"
+description = "A Python package for Reeb graphs"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
 dependencies = ["numpy",
@@ -22,9 +23,9 @@
 where = ["cereeberus"]
 
 [tool.setuptools.package-data]
 cereeberus = ["data"]
 
 [project.urls]
 repository = "https://github.com/MunchLab/ceREEBerus"
-homepage = "https://github.com/MunchLab/ceREEBerus"
-documentation = "https://github.com/MunchLab/ceREEBerus"
+homepage = "https://munchlab.github.io/ceREEBerus/"
+documentation = "https://munchlab.github.io/ceREEBerus/"
```

