# Comparing `tmp/FlowVisor-0.1.7.tar.gz` & `tmp/FlowVisor-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FlowVisor-0.1.7.tar", last modified: Mon May 13 10:00:24 2024, max compression
+gzip compressed data, was "FlowVisor-0.1.8.tar", last modified: Mon May 13 10:10:08 2024, max compression
```

## Comparing `FlowVisor-0.1.7.tar` & `FlowVisor-0.1.8.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-13 10:00:24.626227 FlowVisor-0.1.7/
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-13 10:00:24.626227 FlowVisor-0.1.7/FlowVisor.egg-info/
--rw-rw-r--   0 phil      (1000) phil      (1000)     3697 2024-05-13 10:00:24.000000 FlowVisor-0.1.7/FlowVisor.egg-info/PKG-INFO
--rw-rw-r--   0 phil      (1000) phil      (1000)      593 2024-05-13 10:00:24.000000 FlowVisor-0.1.7/FlowVisor.egg-info/SOURCES.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)        1 2024-05-13 10:00:24.000000 FlowVisor-0.1.7/FlowVisor.egg-info/dependency_links.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)      138 2024-05-13 10:00:24.000000 FlowVisor-0.1.7/FlowVisor.egg-info/entry_points.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)       59 2024-05-13 10:00:24.000000 FlowVisor-0.1.7/FlowVisor.egg-info/requires.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)       10 2024-05-13 10:00:24.000000 FlowVisor-0.1.7/FlowVisor.egg-info/top_level.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)     1067 2024-04-22 08:55:02.000000 FlowVisor-0.1.7/LICENSE
--rw-rw-r--   0 phil      (1000) phil      (1000)     3697 2024-05-13 10:00:24.626227 FlowVisor-0.1.7/PKG-INFO
--rw-rw-r--   0 phil      (1000) phil      (1000)     3016 2024-04-25 13:11:25.000000 FlowVisor-0.1.7/README.md
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-13 10:00:24.626227 FlowVisor-0.1.7/flowvisor/
--rw-rw-r--   0 phil      (1000) phil      (1000)      221 2024-05-08 20:53:18.000000 FlowVisor-0.1.7/flowvisor/__init__.py
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-13 10:00:24.626227 FlowVisor-0.1.7/flowvisor/cli/
--rw-rw-r--   0 phil      (1000) phil      (1000)        0 2024-04-25 10:31:43.000000 FlowVisor-0.1.7/flowvisor/cli/__init__.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     3199 2024-04-25 13:10:53.000000 FlowVisor-0.1.7/flowvisor/cli/add_vis.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     2270 2024-04-25 13:16:50.000000 FlowVisor-0.1.7/flowvisor/cli/remove_vis.py
--rw-rw-r--   0 phil      (1000) phil      (1000)      911 2024-04-25 13:10:38.000000 FlowVisor-0.1.7/flowvisor/cli/vis_file.py
--rw-rw-r--   0 phil      (1000) phil      (1000)    14023 2024-05-13 09:09:16.000000 FlowVisor-0.1.7/flowvisor/flowvisor.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     2214 2024-05-13 09:29:39.000000 FlowVisor-0.1.7/flowvisor/flowvisor_config.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     8113 2024-05-13 09:29:19.000000 FlowVisor-0.1.7/flowvisor/flowvisor_verifier.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     8373 2024-05-13 09:21:33.000000 FlowVisor-0.1.7/flowvisor/function_node.py
--rw-rw-r--   0 phil      (1000) phil      (1000)      887 2024-05-13 06:45:56.000000 FlowVisor-0.1.7/flowvisor/logger.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     2181 2024-05-08 16:32:50.000000 FlowVisor-0.1.7/flowvisor/sankey.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     2732 2024-04-25 11:15:11.000000 FlowVisor-0.1.7/flowvisor/time_tracker.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     2474 2024-05-13 09:18:43.000000 FlowVisor-0.1.7/flowvisor/time_value.py
--rw-rw-r--   0 phil      (1000) phil      (1000)      300 2024-05-08 13:28:52.000000 FlowVisor-0.1.7/flowvisor/timer.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     3132 2024-05-09 07:27:11.000000 FlowVisor-0.1.7/flowvisor/utils.py
--rw-rw-r--   0 phil      (1000) phil      (1000)       38 2024-05-13 10:00:24.626227 FlowVisor-0.1.7/setup.cfg
--rw-rw-r--   0 phil      (1000) phil      (1000)     1585 2024-04-25 13:18:25.000000 FlowVisor-0.1.7/setup.py
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-13 10:10:08.019278 FlowVisor-0.1.8/
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-13 10:10:08.019278 FlowVisor-0.1.8/FlowVisor.egg-info/
+-rw-rw-r--   0 phil      (1000) phil      (1000)     3697 2024-05-13 10:10:07.000000 FlowVisor-0.1.8/FlowVisor.egg-info/PKG-INFO
+-rw-rw-r--   0 phil      (1000) phil      (1000)      593 2024-05-13 10:10:07.000000 FlowVisor-0.1.8/FlowVisor.egg-info/SOURCES.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)        1 2024-05-13 10:10:07.000000 FlowVisor-0.1.8/FlowVisor.egg-info/dependency_links.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)      138 2024-05-13 10:10:07.000000 FlowVisor-0.1.8/FlowVisor.egg-info/entry_points.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)       59 2024-05-13 10:10:07.000000 FlowVisor-0.1.8/FlowVisor.egg-info/requires.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)       10 2024-05-13 10:10:07.000000 FlowVisor-0.1.8/FlowVisor.egg-info/top_level.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)     1067 2024-04-22 08:55:02.000000 FlowVisor-0.1.8/LICENSE
+-rw-rw-r--   0 phil      (1000) phil      (1000)     3697 2024-05-13 10:10:08.019278 FlowVisor-0.1.8/PKG-INFO
+-rw-rw-r--   0 phil      (1000) phil      (1000)     3016 2024-04-25 13:11:25.000000 FlowVisor-0.1.8/README.md
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-13 10:10:08.019278 FlowVisor-0.1.8/flowvisor/
+-rw-rw-r--   0 phil      (1000) phil      (1000)      221 2024-05-08 20:53:18.000000 FlowVisor-0.1.8/flowvisor/__init__.py
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-13 10:10:08.019278 FlowVisor-0.1.8/flowvisor/cli/
+-rw-rw-r--   0 phil      (1000) phil      (1000)        0 2024-04-25 10:31:43.000000 FlowVisor-0.1.8/flowvisor/cli/__init__.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     3199 2024-04-25 13:10:53.000000 FlowVisor-0.1.8/flowvisor/cli/add_vis.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     2270 2024-04-25 13:16:50.000000 FlowVisor-0.1.8/flowvisor/cli/remove_vis.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)      911 2024-04-25 13:10:38.000000 FlowVisor-0.1.8/flowvisor/cli/vis_file.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)    14119 2024-05-13 10:08:25.000000 FlowVisor-0.1.8/flowvisor/flowvisor.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     2214 2024-05-13 09:29:39.000000 FlowVisor-0.1.8/flowvisor/flowvisor_config.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     8113 2024-05-13 10:09:22.000000 FlowVisor-0.1.8/flowvisor/flowvisor_verifier.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     8373 2024-05-13 09:21:33.000000 FlowVisor-0.1.8/flowvisor/function_node.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)      887 2024-05-13 06:45:56.000000 FlowVisor-0.1.8/flowvisor/logger.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     2181 2024-05-08 16:32:50.000000 FlowVisor-0.1.8/flowvisor/sankey.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     2732 2024-04-25 11:15:11.000000 FlowVisor-0.1.8/flowvisor/time_tracker.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     2474 2024-05-13 09:18:43.000000 FlowVisor-0.1.8/flowvisor/time_value.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)      300 2024-05-08 13:28:52.000000 FlowVisor-0.1.8/flowvisor/timer.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     3132 2024-05-09 07:27:11.000000 FlowVisor-0.1.8/flowvisor/utils.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)       38 2024-05-13 10:10:08.019278 FlowVisor-0.1.8/setup.cfg
+-rw-rw-r--   0 phil      (1000) phil      (1000)     1585 2024-04-25 13:18:25.000000 FlowVisor-0.1.8/setup.py
```

### Comparing `FlowVisor-0.1.7/FlowVisor.egg-info/PKG-INFO` & `FlowVisor-0.1.8/FlowVisor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlowVisor
-Version: 0.1.7
+Version: 0.1.8
 Summary: Visualize and profile your python code with FlowVisor.
 Home-page: https://github.com/cophilot/FlowVisor
 Author: cophilot (Philipp B.)
 Author-email: <info@philipp-bonin.com>
 License: MIT
 Keywords: python,flow,visualize,code,flowvisor,profiling,profile,decorator
 Platform: UNKNOWN
```

### Comparing `FlowVisor-0.1.7/FlowVisor.egg-info/SOURCES.txt` & `FlowVisor-0.1.8/FlowVisor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.1.7/LICENSE` & `FlowVisor-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.1.7/PKG-INFO` & `FlowVisor-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlowVisor
-Version: 0.1.7
+Version: 0.1.8
 Summary: Visualize and profile your python code with FlowVisor.
 Home-page: https://github.com/cophilot/FlowVisor
 Author: cophilot (Philipp B.)
 Author-email: <info@philipp-bonin.com>
 License: MIT
 Keywords: python,flow,visualize,code,flowvisor,profiling,profile,decorator
 Platform: UNKNOWN
```

### Comparing `FlowVisor-0.1.7/README.md` & `FlowVisor-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.1.7/flowvisor/cli/add_vis.py` & `FlowVisor-0.1.8/flowvisor/cli/add_vis.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.1.7/flowvisor/cli/remove_vis.py` & `FlowVisor-0.1.8/flowvisor/cli/remove_vis.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.1.7/flowvisor/cli/vis_file.py` & `FlowVisor-0.1.8/flowvisor/cli/vis_file.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.1.7/flowvisor/flowvisor.py` & `FlowVisor-0.1.8/flowvisor/flowvisor.py`

 * *Files 1% similar despite different names*

```diff
@@ -297,15 +297,17 @@
         if export_type == "pickle":
             if not file.endswith(".pickle"):
                 file += ".pickle"
             with open(file, "wb") as f:
                 pickle.dump(nodes_dict, f)
 
     @staticmethod
-    def generate_graph(file: str = ""):
+    def generate_graph(
+        file: str = "", verify=False, verify_file_name="flowvisor_verifier.json"
+    ):
         """
         Generates the graph from a file.
         """
         mode = "pickle"
         if file.endswith(".json"):
             mode = "json"
         if mode == "json":
@@ -317,15 +319,15 @@
 
         for n in raw_nodes:
             node = FunctionNode.from_dict(n)
             FlowVisor.NODES.append(node)
         for node in FlowVisor.NODES:
             node.resolve_children_ids(FlowVisor.NODES)
 
-        FlowVisor.graph()
+        FlowVisor.graph(verify, verify_file_name)
 
     @staticmethod
     def draw_function_node(func_node: FunctionNode):
         """
         Draws the function node.
         """
         time_value = TimeValue(FlowVisor.NODES, FlowVisor.CONFIG, FlowVisor.ROOTS)
```

### Comparing `FlowVisor-0.1.7/flowvisor/flowvisor_config.py` & `FlowVisor-0.1.8/flowvisor/flowvisor_config.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.1.7/flowvisor/flowvisor_verifier.py` & `FlowVisor-0.1.8/flowvisor/flowvisor_verifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,19 +185,19 @@
             print_warning = False
 
             if not FlowVisorVerifier.is_function_verified(entry, node_time, threshold):
                 is_verified = False
                 print_warning = True
 
             time_delta_direction = "more"
-            time_delta_direction_arrow = "🔼"
+            time_delta_direction_arrow = "📈"
             if time_delta < 0:
                 time_delta *= -1
                 time_delta_direction = "less"
-                time_delta_direction_arrow = "🔽"
+                time_delta_direction_arrow = "📉"
 
             Logger.log(
                 f"  Function '{node.file_function_name()}' took {utils.get_time_as_string(time_delta)} {time_delta_direction} than expected ({time_delta_percentage * 100}%) {time_delta_direction_arrow}{'🚨' if print_warning else ''}"
             )
 
         if is_verified:
             Logger.log("All functions are verified! ✅")
```

### Comparing `FlowVisor-0.1.7/flowvisor/function_node.py` & `FlowVisor-0.1.8/flowvisor/function_node.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.1.7/flowvisor/logger.py` & `FlowVisor-0.1.8/flowvisor/logger.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.1.7/flowvisor/sankey.py` & `FlowVisor-0.1.8/flowvisor/sankey.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.1.7/flowvisor/time_tracker.py` & `FlowVisor-0.1.8/flowvisor/time_tracker.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.1.7/flowvisor/time_value.py` & `FlowVisor-0.1.8/flowvisor/time_value.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.1.7/flowvisor/utils.py` & `FlowVisor-0.1.8/flowvisor/utils.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.1.7/setup.py` & `FlowVisor-0.1.8/setup.py`

 * *Files identical despite different names*

