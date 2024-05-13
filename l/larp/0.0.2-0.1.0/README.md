# Comparing `tmp/larp-0.0.2.tar.gz` & `tmp/larp-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "E:\dev\Projects\LARP\dist\.tmp-i7b2vjwq\larp-0.0.2.tar", last modified: Mon Mar 11 19:25:34 2024, max compression
+gzip compressed data, was "E:\dev\Projects\LARP\dist\.tmp-55ftwsqy\larp-0.1.0.tar", last modified: Mon May 13 02:17:55 2024, max compression
```

## Comparing `larp-0.0.2.tar` & `larp-0.1.0.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-03-11 19:25:34.213404 larp-0.0.2/
--rw-rw-rw-   0        0        0    35823 2024-03-09 01:58:41.000000 larp-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      822 2024-03-11 19:25:34.211351 larp-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      319 2024-03-09 01:58:41.000000 larp-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-03-11 19:25:34.156293 larp-0.0.2/larp/
--rw-rw-rw-   0        0        0       96 2024-03-09 01:58:59.000000 larp-0.0.2/larp/__init__.py
--rw-rw-rw-   0        0        0    13029 2024-03-11 19:11:50.000000 larp-0.0.2/larp/field.py
--rw-rw-rw-   0        0        0     1570 2024-03-09 01:58:22.000000 larp-0.0.2/larp/fn.py
--rw-rw-rw-   0        0        0    11527 2024-03-10 05:24:05.000000 larp-0.0.2/larp/graph.py
--rw-rw-rw-   0        0        0     8126 2024-03-10 19:17:51.000000 larp-0.0.2/larp/quad.py
--rw-rw-rw-   0        0        0      832 2024-03-09 01:58:22.000000 larp-0.0.2/larp/types.py
-drwxrwxrwx   0        0        0        0 2024-03-11 19:25:34.210351 larp-0.0.2/larp.egg-info/
--rw-rw-rw-   0        0        0      822 2024-03-11 19:25:34.000000 larp-0.0.2/larp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      353 2024-03-11 19:25:34.000000 larp-0.0.2/larp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-11 19:25:34.000000 larp-0.0.2/larp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-03-11 19:25:34.000000 larp-0.0.2/larp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-03-11 19:25:34.000000 larp-0.0.2/larp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      586 2024-03-11 19:14:08.000000 larp-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-11 19:25:34.214013 larp-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-11 19:25:34.209351 larp-0.0.2/test/
--rw-rw-rw-   0        0        0     1633 2024-03-09 01:58:22.000000 larp-0.0.2/test/test_fn.py
--rw-rw-rw-   0        0        0     1095 2024-03-09 01:58:22.000000 larp-0.0.2/test/test_graph.py
--rw-rw-rw-   0        0        0     3822 2024-03-11 19:11:50.000000 larp-0.0.2/test/test_potential_field.py
--rw-rw-rw-   0        0        0     1228 2024-03-09 01:58:22.000000 larp-0.0.2/test/test_quad.py
--rw-rw-rw-   0        0        0     2428 2024-03-09 01:58:22.000000 larp-0.0.2/test/test_rgj.py
+drwxrwxrwx   0        0        0        0 2024-05-13 02:17:55.303143 larp-0.1.0/
+-rw-rw-rw-   0        0        0    35823 2024-03-09 01:58:41.000000 larp-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0      822 2024-05-13 02:17:55.300146 larp-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      319 2024-05-12 15:00:33.000000 larp-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 02:17:55.197152 larp-0.1.0/larp/
+-rw-rw-rw-   0        0        0       96 2024-05-09 20:16:15.000000 larp-0.1.0/larp/__init__.py
+-rw-rw-rw-   0        0        0    25700 2024-05-13 02:15:36.000000 larp-0.1.0/larp/field.py
+-rw-rw-rw-   0        0        0     1953 2024-05-13 02:15:36.000000 larp-0.1.0/larp/fn.py
+-rw-rw-rw-   0        0        0    11527 2024-03-10 05:24:05.000000 larp-0.1.0/larp/graph.py
+-rw-rw-rw-   0        0        0     4133 2024-05-11 01:24:35.000000 larp-0.1.0/larp/io.py
+-rw-rw-rw-   0        0        0     8233 2024-05-13 02:15:36.000000 larp-0.1.0/larp/quad.py
+-rw-rw-rw-   0        0        0     1115 2024-05-11 01:24:35.000000 larp-0.1.0/larp/types.py
+drwxrwxrwx   0        0        0        0 2024-05-13 02:17:55.297155 larp-0.1.0/larp.egg-info/
+-rw-rw-rw-   0        0        0      822 2024-05-13 02:17:54.000000 larp-0.1.0/larp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      380 2024-05-13 02:17:55.000000 larp-0.1.0/larp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 02:17:54.000000 larp-0.1.0/larp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-13 02:17:55.000000 larp-0.1.0/larp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-13 02:17:55.000000 larp-0.1.0/larp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      586 2024-05-13 02:15:36.000000 larp-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-13 02:17:55.303143 larp-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-13 02:17:55.293145 larp-0.1.0/test/
+-rw-rw-rw-   0        0        0     1633 2024-04-09 19:01:17.000000 larp-0.1.0/test/test_fn.py
+-rw-rw-rw-   0        0        0     1095 2024-03-09 01:58:22.000000 larp-0.1.0/test/test_graph.py
+-rw-rw-rw-   0        0        0      385 2024-05-11 01:24:35.000000 larp-0.1.0/test/test_io.py
+-rw-rw-rw-   0        0        0     3557 2024-05-11 01:24:35.000000 larp-0.1.0/test/test_potential_field.py
+-rw-rw-rw-   0        0        0     1228 2024-03-09 01:58:22.000000 larp-0.1.0/test/test_quad.py
+-rw-rw-rw-   0        0        0     9085 2024-05-11 01:24:35.000000 larp-0.1.0/test/test_rgj.py
```

### Comparing `larp-0.0.2/LICENSE` & `larp-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `larp-0.0.2/PKG-INFO` & `larp-0.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: larp
-Version: 0.0.2
+Version: 0.1.0
 Summary: Larp (/lärp/): Last-Mile Aerial Routing Path Planning
 Author-email: Josue N Rivera <josue.n.rivera@outlook.com>
 Project-URL: Homepage, https://github.com/wzjoriv/Larp
 Project-URL: Issues, https://github.com/wzjoriv/Larp/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `larp-0.0.2/larp/fn.py` & `larp-0.1.0/larp/fn.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 
 from typing import List, Tuple, Union
 import numpy as np
 from larp.types import Point
+from pyproj import CRS, Transformer
 
 """
 Author: Josue N Rivera
 """
 
 def route_distance(route:Union[np.ndarray, List[Point]], return_joints = False) -> Union[float, Tuple[float, np.ndarray]]:
     """
@@ -17,14 +18,25 @@
 
     if return_joints:
         cascade = np.cumsum(dist)
         return cascade[-1], cascade
     
     return dist.sum()
 
+def project_route(route:Union[List[Point], np.ndarray], from_crs="EPSG:3857", to_crs="EPSG:4326") -> np.ndarray:
+
+    from_crs = CRS(from_crs)
+    to_crs = CRS(to_crs)
+
+    proj = Transformer.from_crs(crs_from=from_crs, crs_to=to_crs)
+    route = np.array(route)
+
+    return np.stack(proj.transform(route[:,0], route[:, 1]), axis=1)
+
+
 def interpolate_along_route(route:Union[List[Point], np.ndarray], step=1e-3, n=0, return_step_n = False) -> Union[np.ndarray, Tuple[np.ndarray, float, int]]:
     """
     Return a set of equally spaced points along a route
     """
     route = np.array(route)
     total_dist, joints_dist = route_distance(route, return_joints=True)
     if n <= 0:
```

### Comparing `larp-0.0.2/larp/graph.py` & `larp-0.1.0/larp/graph.py`

 * *Files identical despite different names*

### Comparing `larp-0.0.2/larp/quad.py` & `larp-0.1.0/larp/quad.py`

 * *Files 7% similar despite different names*

```diff
@@ -47,57 +47,61 @@
         self.leaves.append(quad)
         quad.leaf = True
 
     def __approximated_PF_zones__(self, center_point:Point, size:float, filter_idx:Optional[List[int]] = None) -> Tuple[List[int], np.ndarray]: 
         n_rgjs = len(filter_idx)
         zones = np.ones(n_rgjs, dtype=int) * self.n_zones
 
-        dist_sqr = self.field.squared_dist_list([center_point], filted_idx=filter_idx, scaled=False).ravel()
+        rep_vectors, refs_idxs = self.field.repulsion_vectors([center_point], filted_idx=filter_idx, min_dist_select=True, reference_idx=True)
+
+        dist_sqr = (rep_vectors*rep_vectors).sum(1)
         zone0_select = dist_sqr <= (size*size)/2.0
         zones[zone0_select] = 0
 
         if sum(zone0_select) < n_rgjs:
             rgjs_idx = filter_idx[~zone0_select]
+            vectors = rep_vectors[~zone0_select]
+
+            vectors = vectors.reshape(-1, 2)
+            uni_vectors = vectors/np.linalg.norm(vectors, axis=1, keepdims=True)
 
-            dist_sqr = self.field.squared_dist_list([center_point], filted_idx=rgjs_idx, inverted=False).ravel()
-            dist_sqr_bins = (size*size)/2.0 + np.sqrt(2)*size*np.sqrt(self.__zones_rad_ln) + self.__zones_rad_ln
+            dist_sqr = self.field.squared_dist(center_point - uni_vectors*(size/np.sqrt(2)), filted_idx=rgjs_idx).ravel()
 
-            zones[~zone0_select] = np.digitize(dist_sqr, dist_sqr_bins, right=True) + 1
+            zones[~zone0_select] = np.digitize(dist_sqr, self.__zones_rad_ln, right=True) + 1
 
-        return zones
+        return zones, rep_vectors, refs_idxs
 
     def build(self) -> Optional[QuadNode]:
         self.leaves:List[QuadNode] = []
 
         def dfs(center_point:Point, size:float, filter_idx:Optional[List[int]]) -> QuadNode:
             quad = QuadNode(center_point=center_point, size=size)
             filter_n = len(filter_idx)
 
             if filter_n:
-                zones = self.__approximated_PF_zones__(center_point=center_point, size=size, filter_idx=filter_idx)
+                zones, rep_vectors, refs_idxs = self.__approximated_PF_zones__(center_point=center_point, size=size, filter_idx=filter_idx)
                 quad.boundary_zone = zone = min(zones)
             else:
                 quad.boundary_zone = zone = self.n_zones
             quad.boundary_max_range = self.ZONEToMaxRANGE[zone]
             
             if size <= self.max_sector_size:
                 if size <= self.min_sector_size or zone == self.n_zones:
                     # stop subdividing if size is too small or the active zones are too far away
                     self.mark_leaf(quad)
                     return quad
                 if zone > 0:
                     # stop subdiving if sphere does not leave zone
                     lower_range = self.ZONEToMinRANGE[zone]
-                    rgjs_idx = filter_idx[zones == zone]
 
-                    vectors, refs_idxs = self.field.repulsion_vectors([center_point], filted_idx=rgjs_idx, min_dist_select=True, reference_idx=True)
+                    vectors, refs_idxs = rep_vectors[zones == zone], refs_idxs[zones == zone]
                     vectors = vectors.reshape(-1, 2)
                     uni_vectors = vectors/np.linalg.norm(vectors, axis=1, keepdims=True)
 
-                    bounds_evals = self.field.eval_per(center_point + uni_vectors*size/np.sqrt(2), idxs=refs_idxs)
+                    bounds_evals = self.field.eval_per(center_point + uni_vectors*(size/np.sqrt(2)), idxs=refs_idxs)
                     if (bounds_evals >= lower_range).any():
                         self.mark_leaf(quad)
                         return quad
 
             size2 = size/2.0
             size4 = size2/2.0
             new_filter_idx = filter_idx[zones < self.n_zones] if filter_n else filter_idx
```

### Comparing `larp-0.0.2/larp.egg-info/PKG-INFO` & `larp-0.1.0/larp.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: larp
-Version: 0.0.2
+Version: 0.1.0
 Summary: Larp (/lärp/): Last-Mile Aerial Routing Path Planning
 Author-email: Josue N Rivera <josue.n.rivera@outlook.com>
 Project-URL: Homepage, https://github.com/wzjoriv/Larp
 Project-URL: Issues, https://github.com/wzjoriv/Larp/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `larp-0.0.2/pyproject.toml` & `larp-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "larp"
-version = "0.0.2"
+version = "0.1.0"
 authors = [
   { name="Josue N Rivera", email="josue.n.rivera@outlook.com" },
 ]
 description = "Larp (/lärp/): Last-Mile Aerial Routing Path Planning"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = ['numpy']
```

### Comparing `larp-0.0.2/test/test_fn.py` & `larp-0.1.0/test/test_fn.py`

 * *Files identical despite different names*

### Comparing `larp-0.0.2/test/test_graph.py` & `larp-0.1.0/test/test_graph.py`

 * *Files identical despite different names*

### Comparing `larp-0.0.2/test/test_potential_field.py` & `larp-0.1.0/test/test_potential_field.py`

 * *Files 8% similar despite different names*

```diff
@@ -92,19 +92,11 @@
     assert ((grad[0] - np.array([2*np.exp(-1), 0]))**2).sum() < 1e-5, "Unexpected gradient"
     assert ((grad[1] - np.array([-2*np.exp(-1), 0]))**2).sum() < 1e-5, "Unexpected gradient"
     assert ((grad[2] - np.array([-2*np.exp(-2), -2*np.exp(-2)]))**2).sum() < 1e-5, "Unexpected gradient"
 
     
     grad = field.gradient([(11, 10), (20, 11), (32, 31), (81, 82)])
 
-def test_gradient_file():
-    with open("test/data.rgj") as file:
-        rgjs:list = json.load(file)
-    
-    field = larp.PotentialField(size=(120, 120), rgjs=rgjs)
-    grad = field.gradient([(11, 10), (20, 11), (32, 31), (81, 82)])
-
 
 test_eval()
 test_area_estimation()
-test_gradient()
-test_gradient_file()
+test_gradient()
```

### Comparing `larp-0.0.2/test/test_quad.py` & `larp-0.1.0/test/test_quad.py`

 * *Files identical despite different names*

