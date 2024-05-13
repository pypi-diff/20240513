# Comparing `tmp/RDG-Networks-0.2.3.tar.gz` & `tmp/RDG-Networks-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RDG-Networks-0.2.3.tar", last modified: Tue May  7 14:08:46 2024, max compression
+gzip compressed data, was "RDG-Networks-0.2.4.tar", last modified: Mon May 13 19:35:11 2024, max compression
```

## Comparing `RDG-Networks-0.2.3.tar` & `RDG-Networks-0.2.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 5746604    (501) staff       (20)        0 2024-05-07 14:08:46.754495 RDG-Networks-0.2.3/
--rw-r--r--   0 5746604    (501) staff       (20)      598 2024-05-07 14:05:23.000000 RDG-Networks-0.2.3/LICENSE.txt
--rw-r--r--   0 5746604    (501) staff       (20)     2422 2024-05-07 14:08:46.754295 RDG-Networks-0.2.3/PKG-INFO
-drwxr-xr-x   0 5746604    (501) staff       (20)        0 2024-05-07 14:08:46.752820 RDG-Networks-0.2.3/RDG_Networks.egg-info/
--rw-r--r--   0 5746604    (501) staff       (20)     2422 2024-05-07 14:08:46.000000 RDG-Networks-0.2.3/RDG_Networks.egg-info/PKG-INFO
--rw-r--r--   0 5746604    (501) staff       (20)      527 2024-05-07 14:08:46.000000 RDG-Networks-0.2.3/RDG_Networks.egg-info/SOURCES.txt
--rw-r--r--   0 5746604    (501) staff       (20)        1 2024-05-07 14:08:46.000000 RDG-Networks-0.2.3/RDG_Networks.egg-info/dependency_links.txt
--rw-r--r--   0 5746604    (501) staff       (20)      350 2024-05-07 14:08:46.000000 RDG-Networks-0.2.3/RDG_Networks.egg-info/entry_points.txt
--rw-r--r--   0 5746604    (501) staff       (20)       36 2024-05-07 14:08:46.000000 RDG-Networks-0.2.3/RDG_Networks.egg-info/requires.txt
--rw-r--r--   0 5746604    (501) staff       (20)       13 2024-05-07 14:08:46.000000 RDG-Networks-0.2.3/RDG_Networks.egg-info/top_level.txt
-drwxr-xr-x   0 5746604    (501) staff       (20)        0 2024-05-07 14:08:46.754063 RDG-Networks-0.2.3/RDG_networks/
--rw-r--r--   0 5746604    (501) staff       (20)     7977 2024-03-04 14:31:37.000000 RDG-Networks-0.2.3/RDG_networks/Classes.py
--rw-r--r--   0 5746604    (501) staff       (20)      661 2024-05-06 18:35:06.000000 RDG-Networks-0.2.3/RDG_networks/__init__.py
--rw-r--r--   0 5746604    (501) staff       (20)      984 2024-03-04 14:31:54.000000 RDG-Networks-0.2.3/RDG_networks/draw_segments.py
--rw-r--r--   0 5746604    (501) staff       (20)     1127 2024-03-04 14:31:51.000000 RDG-Networks-0.2.3/RDG_networks/generate_line_network.py
--rw-r--r--   0 5746604    (501) staff       (20)     9004 2024-05-06 18:31:39.000000 RDG-Networks-0.2.3/RDG_networks/generate_line_segments.py
--rw-r--r--   0 5746604    (501) staff       (20)     7438 2024-05-06 19:46:48.000000 RDG-Networks-0.2.3/RDG_networks/generate_line_segments_dynamic.py
--rw-r--r--   0 5746604    (501) staff       (20)     2797 2024-03-04 14:52:33.000000 RDG-Networks-0.2.3/RDG_networks/get_intersection_segments.py
--rw-r--r--   0 5746604    (501) staff       (20)     1605 2024-03-01 14:53:20.000000 RDG-Networks-0.2.3/RDG_networks/sample_in_polygon.py
--rw-r--r--   0 5746604    (501) staff       (20)     1940 2024-05-07 14:03:34.000000 RDG-Networks-0.2.3/README.md
--rw-r--r--   0 5746604    (501) staff       (20)       38 2024-05-07 14:08:46.754543 RDG-Networks-0.2.3/setup.cfg
--rw-r--r--   0 5746604    (501) staff       (20)     1162 2024-05-07 14:08:35.000000 RDG-Networks-0.2.3/setup.py
+drwxr-xr-x   0 5746604    (501) staff       (20)        0 2024-05-13 19:35:11.938723 RDG-Networks-0.2.4/
+-rw-r--r--   0 5746604    (501) staff       (20)      598 2024-05-07 14:05:23.000000 RDG-Networks-0.2.4/LICENSE.txt
+-rw-r--r--   0 5746604    (501) staff       (20)     2422 2024-05-13 19:35:11.938527 RDG-Networks-0.2.4/PKG-INFO
+drwxr-xr-x   0 5746604    (501) staff       (20)        0 2024-05-13 19:35:11.937037 RDG-Networks-0.2.4/RDG_Networks.egg-info/
+-rw-r--r--   0 5746604    (501) staff       (20)     2422 2024-05-13 19:35:11.000000 RDG-Networks-0.2.4/RDG_Networks.egg-info/PKG-INFO
+-rw-r--r--   0 5746604    (501) staff       (20)      527 2024-05-13 19:35:11.000000 RDG-Networks-0.2.4/RDG_Networks.egg-info/SOURCES.txt
+-rw-r--r--   0 5746604    (501) staff       (20)        1 2024-05-13 19:35:11.000000 RDG-Networks-0.2.4/RDG_Networks.egg-info/dependency_links.txt
+-rw-r--r--   0 5746604    (501) staff       (20)      350 2024-05-13 19:35:11.000000 RDG-Networks-0.2.4/RDG_Networks.egg-info/entry_points.txt
+-rw-r--r--   0 5746604    (501) staff       (20)       36 2024-05-13 19:35:11.000000 RDG-Networks-0.2.4/RDG_Networks.egg-info/requires.txt
+-rw-r--r--   0 5746604    (501) staff       (20)       13 2024-05-13 19:35:11.000000 RDG-Networks-0.2.4/RDG_Networks.egg-info/top_level.txt
+drwxr-xr-x   0 5746604    (501) staff       (20)        0 2024-05-13 19:35:11.938292 RDG-Networks-0.2.4/RDG_networks/
+-rw-r--r--   0 5746604    (501) staff       (20)     7977 2024-03-04 14:31:37.000000 RDG-Networks-0.2.4/RDG_networks/Classes.py
+-rw-r--r--   0 5746604    (501) staff       (20)      661 2024-05-06 18:35:06.000000 RDG-Networks-0.2.4/RDG_networks/__init__.py
+-rw-r--r--   0 5746604    (501) staff       (20)      984 2024-03-04 14:31:54.000000 RDG-Networks-0.2.4/RDG_networks/draw_segments.py
+-rw-r--r--   0 5746604    (501) staff       (20)     1127 2024-03-04 14:31:51.000000 RDG-Networks-0.2.4/RDG_networks/generate_line_network.py
+-rw-r--r--   0 5746604    (501) staff       (20)     9004 2024-05-06 18:31:39.000000 RDG-Networks-0.2.4/RDG_networks/generate_line_segments.py
+-rw-r--r--   0 5746604    (501) staff       (20)     7531 2024-05-13 19:33:11.000000 RDG-Networks-0.2.4/RDG_networks/generate_line_segments_dynamic.py
+-rw-r--r--   0 5746604    (501) staff       (20)     2797 2024-03-04 14:52:33.000000 RDG-Networks-0.2.4/RDG_networks/get_intersection_segments.py
+-rw-r--r--   0 5746604    (501) staff       (20)     1605 2024-03-01 14:53:20.000000 RDG-Networks-0.2.4/RDG_networks/sample_in_polygon.py
+-rw-r--r--   0 5746604    (501) staff       (20)     1940 2024-05-07 14:03:34.000000 RDG-Networks-0.2.4/README.md
+-rw-r--r--   0 5746604    (501) staff       (20)       38 2024-05-13 19:35:11.938772 RDG-Networks-0.2.4/setup.cfg
+-rw-r--r--   0 5746604    (501) staff       (20)     1162 2024-05-13 19:35:05.000000 RDG-Networks-0.2.4/setup.py
```

### Comparing `RDG-Networks-0.2.3/LICENSE.txt` & `RDG-Networks-0.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `RDG-Networks-0.2.3/PKG-INFO` & `RDG-Networks-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RDG-Networks
-Version: 0.2.3
+Version: 0.2.4
 Summary: Most of the code from the RDG Networks project
 Home-page: https://github.com/NiekMooij/RDG_networks
 Author: Niek Mooij
 Author-email: mooij.niek@gmail.com
 License: All Rights Reserved
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `RDG-Networks-0.2.3/RDG_Networks.egg-info/PKG-INFO` & `RDG-Networks-0.2.4/RDG_Networks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RDG-Networks
-Version: 0.2.3
+Version: 0.2.4
 Summary: Most of the code from the RDG Networks project
 Home-page: https://github.com/NiekMooij/RDG_networks
 Author: Niek Mooij
 Author-email: mooij.niek@gmail.com
 License: All Rights Reserved
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `RDG-Networks-0.2.3/RDG_Networks.egg-info/SOURCES.txt` & `RDG-Networks-0.2.4/RDG_Networks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RDG-Networks-0.2.3/RDG_networks/Classes.py` & `RDG-Networks-0.2.4/RDG_networks/Classes.py`

 * *Files identical despite different names*

### Comparing `RDG-Networks-0.2.3/RDG_networks/__init__.py` & `RDG-Networks-0.2.4/RDG_networks/__init__.py`

 * *Files identical despite different names*

### Comparing `RDG-Networks-0.2.3/RDG_networks/draw_segments.py` & `RDG-Networks-0.2.4/RDG_networks/draw_segments.py`

 * *Files identical despite different names*

### Comparing `RDG-Networks-0.2.3/RDG_networks/generate_line_network.py` & `RDG-Networks-0.2.4/RDG_networks/generate_line_network.py`

 * *Files identical despite different names*

### Comparing `RDG-Networks-0.2.3/RDG_networks/generate_line_segments.py` & `RDG-Networks-0.2.4/RDG_networks/generate_line_segments.py`

 * *Files identical despite different names*

### Comparing `RDG-Networks-0.2.3/RDG_networks/generate_line_segments_dynamic.py` & `RDG-Networks-0.2.4/RDG_networks/generate_line_segments_dynamic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import numpy as np
 import random
 from shapely.geometry import LineString
 from typing import List, Dict, Any, Tuple
+import matplotlib.pyplot as plt
 
 from .Classes import LineSegment
 
 def grow_lines(lines: List[Dict[str, Any]], epsilon: float) -> List[Dict[str, Any]]:
     """
     Grows lines based on their current status.
 
@@ -84,55 +85,56 @@
         if lines[index]['growth_status'] == True and (line['end'][0] < 0 or line['end'][0] > 1 or line['end'][1] < 0 or line['end'][1] > 1):
             # If line has intersected with the border, update its properties
             lines[index]['neighbors_initial'] = lines[index]['neighbors_initial'] + ['border']
             lines[index]['growth_status'] = False
             
     return lines
 
-def check_and_update_when_intersect(lines: List[Dict[str, Any]], epsilon: float) -> List[Dict[str, Any]]:
+def check_and_update_when_intersect(lines: List[Dict[str, Any]], epsilon: float, dt: float) -> List[Dict[str, Any]]:
     """
     Check for intersections between lines and update their properties accordingly.
 
     Args:
         lines (List[Dict[str, Any]]): A list of dictionaries representing lines.
         epsilon (float): The growth rate of the lines.
 
     Returns:
         List[Dict[str, Any]]: The updated list of lines after handling intersections.
     """
+        
     for index1, j1 in enumerate(lines):
         for index2, j2 in enumerate(lines):
             if j1['id'][:-2] == j2['id'][:-2] or index2 < index1:
                 continue
-                
+            
             if j1['growth_status'] == False and j2['growth_status'] == False:
                 continue
-                
+            
             line1 = LineString([j1['start'], j1['end']])
             line2 = LineString([j2['start'], j2['end']])
-
+            
             intersection_pt = line1.intersection(line2)
 
             if not intersection_pt.is_empty:
                 d1 = np.linalg.norm(np.array(j1['start']) - np.array([intersection_pt.x, intersection_pt.y]))
                 d2 = np.linalg.norm(np.array(j2['start']) - np.array([intersection_pt.x, intersection_pt.y]))
                 
-                arrival_1 = j1['introduction_time'] + d1 / epsilon
-                arrival_2 = j2['introduction_time'] + d2 / epsilon
+                arrival_1 = j1['introduction_time'] + d1 / epsilon * dt
+                arrival_2 = j2['introduction_time'] + d2 / epsilon * dt
 
                 if arrival_1 > arrival_2:
                     lines[index1]['end'] = (intersection_pt.x, intersection_pt.y)
                     lines[index1]['neighbors_initial'] = lines[index1]['neighbors_initial'] + [j2['id'][:-2]]
-                    lines[index1]['growth_status'] = False
+                    lines[index1]['growth_status'] = False                    
 
                 else:                        
                     lines[index2]['end'] = (intersection_pt.x, intersection_pt.y)
                     lines[index2]['neighbors_initial'] = lines[index2]['neighbors_initial'] + [j1['id'][:-2]]
                     lines[index2]['growth_status'] = False
-                    
+
     return lines
 
 def transform_to_standard_lines(lines: List[Dict[str, Any]]) -> List[LineSegment]:
     """
     Transform a list of lines into a list of standard line segments.
 
     Args:
@@ -169,33 +171,34 @@
         angles (str or List): The allowed angles in the system (default is 'uniform' for random angles).
 
     Returns:
         List[LineSegment]: A list of LineSegment objects representing standard line segments.
     """
     lines = []
     line_id, t, t_total = 1, 0, 0
-
+    
     # Stop loop whenever we have enough lines and all lines have stopped growing
     while len(lines) / 2 < size or np.any([item['growth_status'] for item in lines]):
 
         t += dt
         t_total += dt
         
         if t > time and len(lines) / 2 < size:
             
             if time == 0:
                 number_of_lines_to_add = size
             else:
-                number_of_lines_to_add = int(t - (t % time))
+                number_of_lines_to_add = int(t / time)
+                
             for _ in range(number_of_lines_to_add):
                 lines = add_new_line(lines, line_id, t_total, angles=angles)
                 line_id += 1
-            
-                t = 0
+                
+            t = 0
 
         lines = grow_lines(lines, epsilon)
         lines = update_for_border_intersections(lines)
-        lines = check_and_update_when_intersect(lines, epsilon)
-
+        lines = check_and_update_when_intersect(lines, epsilon, dt)
+        
     lines = transform_to_standard_lines(lines)
         
     return lines
```

### Comparing `RDG-Networks-0.2.3/RDG_networks/get_intersection_segments.py` & `RDG-Networks-0.2.4/RDG_networks/get_intersection_segments.py`

 * *Files identical despite different names*

### Comparing `RDG-Networks-0.2.3/RDG_networks/sample_in_polygon.py` & `RDG-Networks-0.2.4/RDG_networks/sample_in_polygon.py`

 * *Files identical despite different names*

### Comparing `RDG-Networks-0.2.3/README.md` & `RDG-Networks-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `RDG-Networks-0.2.3/setup.py` & `RDG-Networks-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='RDG-Networks',
-    version='0.2.3',
+    version='0.2.4',
     author='Niek Mooij',
     author_email='mooij.niek@gmail.com',
     description='Most of the code from the RDG Networks project',
     long_description=open('README.md').read(),
     url='https://github.com/NiekMooij/RDG_networks',
     classifiers=[
             'Programming Language :: Python :: 3',
```

