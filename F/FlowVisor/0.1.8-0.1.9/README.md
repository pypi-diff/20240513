# Comparing `tmp/FlowVisor-0.1.8.tar.gz` & `tmp/FlowVisor-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FlowVisor-0.1.8.tar", last modified: Mon May 13 10:10:08 2024, max compression
+gzip compressed data, was "FlowVisor-0.1.9.tar", last modified: Mon May 13 10:33:57 2024, max compression
```

## Comparing `FlowVisor-0.1.8.tar` & `FlowVisor-0.1.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-13 10:10:08.019278 FlowVisor-0.1.8/
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-13 10:10:08.019278 FlowVisor-0.1.8/FlowVisor.egg-info/
--rw-rw-r--   0 phil      (1000) phil      (1000)     3697 2024-05-13 10:10:07.000000 FlowVisor-0.1.8/FlowVisor.egg-info/PKG-INFO
--rw-rw-r--   0 phil      (1000) phil      (1000)      593 2024-05-13 10:10:07.000000 FlowVisor-0.1.8/FlowVisor.egg-info/SOURCES.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)        1 2024-05-13 10:10:07.000000 FlowVisor-0.1.8/FlowVisor.egg-info/dependency_links.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)      138 2024-05-13 10:10:07.000000 FlowVisor-0.1.8/FlowVisor.egg-info/entry_points.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)       59 2024-05-13 10:10:07.000000 FlowVisor-0.1.8/FlowVisor.egg-info/requires.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)       10 2024-05-13 10:10:07.000000 FlowVisor-0.1.8/FlowVisor.egg-info/top_level.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)     1067 2024-04-22 08:55:02.000000 FlowVisor-0.1.8/LICENSE
--rw-rw-r--   0 phil      (1000) phil      (1000)     3697 2024-05-13 10:10:08.019278 FlowVisor-0.1.8/PKG-INFO
--rw-rw-r--   0 phil      (1000) phil      (1000)     3016 2024-04-25 13:11:25.000000 FlowVisor-0.1.8/README.md
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-13 10:10:08.019278 FlowVisor-0.1.8/flowvisor/
--rw-rw-r--   0 phil      (1000) phil      (1000)      221 2024-05-08 20:53:18.000000 FlowVisor-0.1.8/flowvisor/__init__.py
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-13 10:10:08.019278 FlowVisor-0.1.8/flowvisor/cli/
--rw-rw-r--   0 phil      (1000) phil      (1000)        0 2024-04-25 10:31:43.000000 FlowVisor-0.1.8/flowvisor/cli/__init__.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     3199 2024-04-25 13:10:53.000000 FlowVisor-0.1.8/flowvisor/cli/add_vis.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     2270 2024-04-25 13:16:50.000000 FlowVisor-0.1.8/flowvisor/cli/remove_vis.py
--rw-rw-r--   0 phil      (1000) phil      (1000)      911 2024-04-25 13:10:38.000000 FlowVisor-0.1.8/flowvisor/cli/vis_file.py
--rw-rw-r--   0 phil      (1000) phil      (1000)    14119 2024-05-13 10:08:25.000000 FlowVisor-0.1.8/flowvisor/flowvisor.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     2214 2024-05-13 09:29:39.000000 FlowVisor-0.1.8/flowvisor/flowvisor_config.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     8113 2024-05-13 10:09:22.000000 FlowVisor-0.1.8/flowvisor/flowvisor_verifier.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     8373 2024-05-13 09:21:33.000000 FlowVisor-0.1.8/flowvisor/function_node.py
--rw-rw-r--   0 phil      (1000) phil      (1000)      887 2024-05-13 06:45:56.000000 FlowVisor-0.1.8/flowvisor/logger.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     2181 2024-05-08 16:32:50.000000 FlowVisor-0.1.8/flowvisor/sankey.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     2732 2024-04-25 11:15:11.000000 FlowVisor-0.1.8/flowvisor/time_tracker.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     2474 2024-05-13 09:18:43.000000 FlowVisor-0.1.8/flowvisor/time_value.py
--rw-rw-r--   0 phil      (1000) phil      (1000)      300 2024-05-08 13:28:52.000000 FlowVisor-0.1.8/flowvisor/timer.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     3132 2024-05-09 07:27:11.000000 FlowVisor-0.1.8/flowvisor/utils.py
--rw-rw-r--   0 phil      (1000) phil      (1000)       38 2024-05-13 10:10:08.019278 FlowVisor-0.1.8/setup.cfg
--rw-rw-r--   0 phil      (1000) phil      (1000)     1585 2024-04-25 13:18:25.000000 FlowVisor-0.1.8/setup.py
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-13 10:33:57.061928 FlowVisor-0.1.9/
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-13 10:33:57.061928 FlowVisor-0.1.9/FlowVisor.egg-info/
+-rw-rw-r--   0 phil      (1000) phil      (1000)     3697 2024-05-13 10:33:57.000000 FlowVisor-0.1.9/FlowVisor.egg-info/PKG-INFO
+-rw-rw-r--   0 phil      (1000) phil      (1000)      593 2024-05-13 10:33:57.000000 FlowVisor-0.1.9/FlowVisor.egg-info/SOURCES.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)        1 2024-05-13 10:33:57.000000 FlowVisor-0.1.9/FlowVisor.egg-info/dependency_links.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)      138 2024-05-13 10:33:57.000000 FlowVisor-0.1.9/FlowVisor.egg-info/entry_points.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)       59 2024-05-13 10:33:57.000000 FlowVisor-0.1.9/FlowVisor.egg-info/requires.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)       10 2024-05-13 10:33:57.000000 FlowVisor-0.1.9/FlowVisor.egg-info/top_level.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)     1067 2024-04-22 08:55:02.000000 FlowVisor-0.1.9/LICENSE
+-rw-rw-r--   0 phil      (1000) phil      (1000)     3697 2024-05-13 10:33:57.061928 FlowVisor-0.1.9/PKG-INFO
+-rw-rw-r--   0 phil      (1000) phil      (1000)     3016 2024-04-25 13:11:25.000000 FlowVisor-0.1.9/README.md
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-13 10:33:57.061928 FlowVisor-0.1.9/flowvisor/
+-rw-rw-r--   0 phil      (1000) phil      (1000)      221 2024-05-08 20:53:18.000000 FlowVisor-0.1.9/flowvisor/__init__.py
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-13 10:33:57.061928 FlowVisor-0.1.9/flowvisor/cli/
+-rw-rw-r--   0 phil      (1000) phil      (1000)        0 2024-04-25 10:31:43.000000 FlowVisor-0.1.9/flowvisor/cli/__init__.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     3199 2024-04-25 13:10:53.000000 FlowVisor-0.1.9/flowvisor/cli/add_vis.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     2270 2024-04-25 13:16:50.000000 FlowVisor-0.1.9/flowvisor/cli/remove_vis.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)      911 2024-04-25 13:10:38.000000 FlowVisor-0.1.9/flowvisor/cli/vis_file.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)    14240 2024-05-13 10:16:16.000000 FlowVisor-0.1.9/flowvisor/flowvisor.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     2214 2024-05-13 09:29:39.000000 FlowVisor-0.1.9/flowvisor/flowvisor_config.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     8113 2024-05-13 10:09:22.000000 FlowVisor-0.1.9/flowvisor/flowvisor_verifier.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     8460 2024-05-13 10:20:06.000000 FlowVisor-0.1.9/flowvisor/function_node.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)      887 2024-05-13 06:45:56.000000 FlowVisor-0.1.9/flowvisor/logger.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     2181 2024-05-08 16:32:50.000000 FlowVisor-0.1.9/flowvisor/sankey.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     2732 2024-04-25 11:15:11.000000 FlowVisor-0.1.9/flowvisor/time_tracker.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     2474 2024-05-13 09:18:43.000000 FlowVisor-0.1.9/flowvisor/time_value.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)      300 2024-05-08 13:28:52.000000 FlowVisor-0.1.9/flowvisor/timer.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     3132 2024-05-09 07:27:11.000000 FlowVisor-0.1.9/flowvisor/utils.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)       38 2024-05-13 10:33:57.061928 FlowVisor-0.1.9/setup.cfg
+-rw-rw-r--   0 phil      (1000) phil      (1000)     1585 2024-04-25 13:18:25.000000 FlowVisor-0.1.9/setup.py
```

### Comparing `FlowVisor-0.1.8/FlowVisor.egg-info/PKG-INFO` & `FlowVisor-0.1.9/FlowVisor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlowVisor
-Version: 0.1.8
+Version: 0.1.9
 Summary: Visualize and profile your python code with FlowVisor.
 Home-page: https://github.com/cophilot/FlowVisor
 Author: cophilot (Philipp B.)
 Author-email: <info@philipp-bonin.com>
 License: MIT
 Keywords: python,flow,visualize,code,flowvisor,profiling,profile,decorator
 Platform: UNKNOWN
```

### Comparing `FlowVisor-0.1.8/FlowVisor.egg-info/SOURCES.txt` & `FlowVisor-0.1.9/FlowVisor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.1.8/LICENSE` & `FlowVisor-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.1.8/PKG-INFO` & `FlowVisor-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlowVisor
-Version: 0.1.8
+Version: 0.1.9
 Summary: Visualize and profile your python code with FlowVisor.
 Home-page: https://github.com/cophilot/FlowVisor
 Author: cophilot (Philipp B.)
 Author-email: <info@philipp-bonin.com>
 License: MIT
 Keywords: python,flow,visualize,code,flowvisor,profiling,profile,decorator
 Platform: UNKNOWN
```

### Comparing `FlowVisor-0.1.8/README.md` & `FlowVisor-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.1.8/flowvisor/cli/add_vis.py` & `FlowVisor-0.1.9/flowvisor/cli/add_vis.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.1.8/flowvisor/cli/remove_vis.py` & `FlowVisor-0.1.9/flowvisor/cli/remove_vis.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.1.8/flowvisor/cli/vis_file.py` & `FlowVisor-0.1.9/flowvisor/cli/vis_file.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.1.8/flowvisor/flowvisor.py` & `FlowVisor-0.1.9/flowvisor/flowvisor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 The FlowVisor is a package that visualizes the flow of functions in a codebase.
 """
 
 import datetime
 import json
+import os
 import timeit
 from typing import List
 import pickle
 from diagrams import Diagram, Cluster
 from diagrams.custom import Custom
 from flowvisor import utils
 from flowvisor.logger import Logger
@@ -303,14 +304,17 @@
     @staticmethod
     def generate_graph(
         file: str = "", verify=False, verify_file_name="flowvisor_verifier.json"
     ):
         """
         Generates the graph from a file.
         """
+        if not os.path.exists(file):
+            Logger.log(f"File {file} does not exist!")
+            return
         mode = "pickle"
         if file.endswith(".json"):
             mode = "json"
         if mode == "json":
             with open(file, "r", encoding="utf-8") as f:
                 raw_nodes = json.load(f)
         else:
```

### Comparing `FlowVisor-0.1.8/flowvisor/flowvisor_config.py` & `FlowVisor-0.1.9/flowvisor/flowvisor_config.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.1.8/flowvisor/flowvisor_verifier.py` & `FlowVisor-0.1.9/flowvisor/flowvisor_verifier.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.1.8/flowvisor/function_node.py` & `FlowVisor-0.1.9/flowvisor/function_node.py`

 * *Files 5% similar despite different names*

```diff
@@ -273,10 +273,12 @@
         node = FunctionNode(None)
         node.id = d["id"]
         node.uuid = d["uuid"]
         node.name = d["name"]
         node.file_path = d["file_path"]
         node.file_name = d["file_name"]
         node.children_ids = [child["uuid"] for child in d["children"]]
-        node.time = d["time"]
-        node.called = d["called"]
+        ex_time = d["exclusive_time"]
+        in_time = d["inclusive_time"]
+        node.set_time(in_time)
+        node.child_time = in_time - ex_time
         return node
```

### Comparing `FlowVisor-0.1.8/flowvisor/logger.py` & `FlowVisor-0.1.9/flowvisor/logger.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.1.8/flowvisor/sankey.py` & `FlowVisor-0.1.9/flowvisor/sankey.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.1.8/flowvisor/time_tracker.py` & `FlowVisor-0.1.9/flowvisor/time_tracker.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.1.8/flowvisor/time_value.py` & `FlowVisor-0.1.9/flowvisor/time_value.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.1.8/flowvisor/utils.py` & `FlowVisor-0.1.9/flowvisor/utils.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.1.8/setup.py` & `FlowVisor-0.1.9/setup.py`

 * *Files identical despite different names*

