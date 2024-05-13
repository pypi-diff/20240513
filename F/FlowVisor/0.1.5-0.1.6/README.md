# Comparing `tmp/FlowVisor-0.1.5.tar.gz` & `tmp/FlowVisor-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FlowVisor-0.1.5.tar", last modified: Sat May 11 06:00:17 2024, max compression
+gzip compressed data, was "FlowVisor-0.1.6.tar", last modified: Mon May 13 06:48:36 2024, max compression
```

## Comparing `FlowVisor-0.1.5.tar` & `FlowVisor-0.1.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-11 06:00:17.583484 FlowVisor-0.1.5/
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-11 06:00:17.583484 FlowVisor-0.1.5/FlowVisor.egg-info/
--rw-rw-r--   0 phil      (1000) phil      (1000)     3697 2024-05-11 06:00:17.000000 FlowVisor-0.1.5/FlowVisor.egg-info/PKG-INFO
--rw-rw-r--   0 phil      (1000) phil      (1000)      593 2024-05-11 06:00:17.000000 FlowVisor-0.1.5/FlowVisor.egg-info/SOURCES.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)        1 2024-05-11 06:00:17.000000 FlowVisor-0.1.5/FlowVisor.egg-info/dependency_links.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)      138 2024-05-11 06:00:17.000000 FlowVisor-0.1.5/FlowVisor.egg-info/entry_points.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)       59 2024-05-11 06:00:17.000000 FlowVisor-0.1.5/FlowVisor.egg-info/requires.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)       10 2024-05-11 06:00:17.000000 FlowVisor-0.1.5/FlowVisor.egg-info/top_level.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)     1067 2024-04-22 08:55:02.000000 FlowVisor-0.1.5/LICENSE
--rw-rw-r--   0 phil      (1000) phil      (1000)     3697 2024-05-11 06:00:17.583484 FlowVisor-0.1.5/PKG-INFO
--rw-rw-r--   0 phil      (1000) phil      (1000)     3016 2024-04-25 13:11:25.000000 FlowVisor-0.1.5/README.md
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-11 06:00:17.583484 FlowVisor-0.1.5/flowvisor/
--rw-rw-r--   0 phil      (1000) phil      (1000)      221 2024-05-08 20:53:18.000000 FlowVisor-0.1.5/flowvisor/__init__.py
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-11 06:00:17.583484 FlowVisor-0.1.5/flowvisor/cli/
--rw-rw-r--   0 phil      (1000) phil      (1000)        0 2024-04-25 10:31:43.000000 FlowVisor-0.1.5/flowvisor/cli/__init__.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     3199 2024-04-25 13:10:53.000000 FlowVisor-0.1.5/flowvisor/cli/add_vis.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     2270 2024-04-25 13:16:50.000000 FlowVisor-0.1.5/flowvisor/cli/remove_vis.py
--rw-rw-r--   0 phil      (1000) phil      (1000)      911 2024-04-25 13:10:38.000000 FlowVisor-0.1.5/flowvisor/cli/vis_file.py
--rw-rw-r--   0 phil      (1000) phil      (1000)    16418 2024-05-11 05:55:43.000000 FlowVisor-0.1.5/flowvisor/flowvisor.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     2030 2024-05-11 05:24:19.000000 FlowVisor-0.1.5/flowvisor/flowvisor_config.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     7894 2024-05-11 05:40:17.000000 FlowVisor-0.1.5/flowvisor/flowvisor_verifier.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     8004 2024-05-09 07:05:50.000000 FlowVisor-0.1.5/flowvisor/function_node.py
--rw-rw-r--   0 phil      (1000) phil      (1000)       98 2024-05-09 06:06:21.000000 FlowVisor-0.1.5/flowvisor/logger.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     2181 2024-05-08 16:32:50.000000 FlowVisor-0.1.5/flowvisor/sankey.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     2732 2024-04-25 11:15:11.000000 FlowVisor-0.1.5/flowvisor/time_tracker.py
--rw-rw-r--   0 phil      (1000) phil      (1000)      292 2024-05-08 15:25:05.000000 FlowVisor-0.1.5/flowvisor/time_value.py
--rw-rw-r--   0 phil      (1000) phil      (1000)      300 2024-05-08 13:28:52.000000 FlowVisor-0.1.5/flowvisor/timer.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     3132 2024-05-09 07:27:11.000000 FlowVisor-0.1.5/flowvisor/utils.py
--rw-rw-r--   0 phil      (1000) phil      (1000)       38 2024-05-11 06:00:17.583484 FlowVisor-0.1.5/setup.cfg
--rw-rw-r--   0 phil      (1000) phil      (1000)     1585 2024-04-25 13:18:25.000000 FlowVisor-0.1.5/setup.py
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-13 06:48:36.533249 FlowVisor-0.1.6/
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-13 06:48:36.529249 FlowVisor-0.1.6/FlowVisor.egg-info/
+-rw-rw-r--   0 phil      (1000) phil      (1000)     3697 2024-05-13 06:48:36.000000 FlowVisor-0.1.6/FlowVisor.egg-info/PKG-INFO
+-rw-rw-r--   0 phil      (1000) phil      (1000)      593 2024-05-13 06:48:36.000000 FlowVisor-0.1.6/FlowVisor.egg-info/SOURCES.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)        1 2024-05-13 06:48:36.000000 FlowVisor-0.1.6/FlowVisor.egg-info/dependency_links.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)      138 2024-05-13 06:48:36.000000 FlowVisor-0.1.6/FlowVisor.egg-info/entry_points.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)       59 2024-05-13 06:48:36.000000 FlowVisor-0.1.6/FlowVisor.egg-info/requires.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)       10 2024-05-13 06:48:36.000000 FlowVisor-0.1.6/FlowVisor.egg-info/top_level.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)     1067 2024-04-22 08:55:02.000000 FlowVisor-0.1.6/LICENSE
+-rw-rw-r--   0 phil      (1000) phil      (1000)     3697 2024-05-13 06:48:36.533249 FlowVisor-0.1.6/PKG-INFO
+-rw-rw-r--   0 phil      (1000) phil      (1000)     3016 2024-04-25 13:11:25.000000 FlowVisor-0.1.6/README.md
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-13 06:48:36.533249 FlowVisor-0.1.6/flowvisor/
+-rw-rw-r--   0 phil      (1000) phil      (1000)      221 2024-05-08 20:53:18.000000 FlowVisor-0.1.6/flowvisor/__init__.py
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-13 06:48:36.533249 FlowVisor-0.1.6/flowvisor/cli/
+-rw-rw-r--   0 phil      (1000) phil      (1000)        0 2024-04-25 10:31:43.000000 FlowVisor-0.1.6/flowvisor/cli/__init__.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     3199 2024-04-25 13:10:53.000000 FlowVisor-0.1.6/flowvisor/cli/add_vis.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     2270 2024-04-25 13:16:50.000000 FlowVisor-0.1.6/flowvisor/cli/remove_vis.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)      911 2024-04-25 13:10:38.000000 FlowVisor-0.1.6/flowvisor/cli/vis_file.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)    16758 2024-05-13 06:45:04.000000 FlowVisor-0.1.6/flowvisor/flowvisor.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     2030 2024-05-11 05:24:19.000000 FlowVisor-0.1.6/flowvisor/flowvisor_config.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     7969 2024-05-13 06:42:22.000000 FlowVisor-0.1.6/flowvisor/flowvisor_verifier.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     8004 2024-05-09 07:05:50.000000 FlowVisor-0.1.6/flowvisor/function_node.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)      887 2024-05-13 06:45:56.000000 FlowVisor-0.1.6/flowvisor/logger.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     2181 2024-05-08 16:32:50.000000 FlowVisor-0.1.6/flowvisor/sankey.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     2732 2024-04-25 11:15:11.000000 FlowVisor-0.1.6/flowvisor/time_tracker.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)      292 2024-05-08 15:25:05.000000 FlowVisor-0.1.6/flowvisor/time_value.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)      300 2024-05-08 13:28:52.000000 FlowVisor-0.1.6/flowvisor/timer.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     3132 2024-05-09 07:27:11.000000 FlowVisor-0.1.6/flowvisor/utils.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)       38 2024-05-13 06:48:36.533249 FlowVisor-0.1.6/setup.cfg
+-rw-rw-r--   0 phil      (1000) phil      (1000)     1585 2024-04-25 13:18:25.000000 FlowVisor-0.1.6/setup.py
```

### Comparing `FlowVisor-0.1.5/FlowVisor.egg-info/PKG-INFO` & `FlowVisor-0.1.6/FlowVisor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlowVisor
-Version: 0.1.5
+Version: 0.1.6
 Summary: Visualize and profile your python code with FlowVisor.
 Home-page: https://github.com/cophilot/FlowVisor
 Author: cophilot (Philipp B.)
 Author-email: <info@philipp-bonin.com>
 License: MIT
 Keywords: python,flow,visualize,code,flowvisor,profiling,profile,decorator
 Platform: UNKNOWN
```

### Comparing `FlowVisor-0.1.5/FlowVisor.egg-info/SOURCES.txt` & `FlowVisor-0.1.6/FlowVisor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.1.5/LICENSE` & `FlowVisor-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.1.5/PKG-INFO` & `FlowVisor-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlowVisor
-Version: 0.1.5
+Version: 0.1.6
 Summary: Visualize and profile your python code with FlowVisor.
 Home-page: https://github.com/cophilot/FlowVisor
 Author: cophilot (Philipp B.)
 Author-email: <info@philipp-bonin.com>
 License: MIT
 Keywords: python,flow,visualize,code,flowvisor,profiling,profile,decorator
 Platform: UNKNOWN
```

### Comparing `FlowVisor-0.1.5/README.md` & `FlowVisor-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.1.5/flowvisor/cli/add_vis.py` & `FlowVisor-0.1.6/flowvisor/cli/add_vis.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.1.5/flowvisor/cli/remove_vis.py` & `FlowVisor-0.1.6/flowvisor/cli/remove_vis.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.1.5/flowvisor/cli/vis_file.py` & `FlowVisor-0.1.6/flowvisor/cli/vis_file.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.1.5/flowvisor/flowvisor.py` & `FlowVisor-0.1.6/flowvisor/flowvisor.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 import datetime
 import json
 import timeit
 from typing import List
 import pickle
 from diagrams import Diagram, Cluster
 from diagrams.custom import Custom
-from flowvisor import logger, utils
+from flowvisor import utils
+from flowvisor.logger import Logger
 from flowvisor.flowvisor_config import FlowVisorConfig
 from flowvisor.flowvisor_verifier import FlowVisorVerifier, vis_verifier
 from flowvisor.function_node import FunctionNode
 from flowvisor.sankey import make_sankey_diagram
 from flowvisor.time_tracker import TimeTracker
 from flowvisor.time_value import TimeValue
 from flowvisor.utils import function_to_id
@@ -147,15 +148,15 @@
 
     @staticmethod
     def graph(verify=False, verify_file_name="flowvisor_verifier.json"):
         """
         Generates the graph.
         """
         if FlowVisor.VERIFIER_MODE:
-            logger.log("Can not generate graph in verifier mode!")
+            Logger.log("Can not generate graph in verifier mode!")
             return
 
         verify_text = None
         if verify:
             if FlowVisor.verify(verify_file_name):
                 verify_text = "Verified ✅"
             else:
@@ -320,15 +321,15 @@
 
     @staticmethod
     def export(file: str, export_type="pickle"):
         """
         Saves the flow to a file.
         """
         if FlowVisor.VERIFIER_MODE:
-            logger.log("Can not export in verifier mode!")
+            Logger.log("Can not export in verifier mode!")
             return
 
         nodes_dict = FlowVisor.get_nodes_as_dict()
         if export_type == "json":
             if not file.endswith(".json"):
                 file += ".json"
             with open(file, "w", encoding="utf-8") as f:
@@ -413,15 +414,15 @@
     def enable_advanced_overhead_reduction():
         """
         Enables advanced overhead reduction.
         """
         n = 50000
         t = timeit.timeit(setup="import time", stmt="time.time()", number=n)
         mean = t / n
-        logger.log(f"Mean time for time.time() is: {utils.get_time_as_string(mean)}")
+        Logger.log(f"Mean time for time.time() is: {utils.get_time_as_string(mean)}")
         FlowVisor.CONFIG.advanced_overhead_reduction = mean
 
     @staticmethod
     def disable_advanced_overhead_reduction():
         """
         Disables advanced overhead reduction.
         """
@@ -454,49 +455,63 @@
         """
         Automatically enables the verifier mode.
         """
         count = FlowVisorVerifier.get_count_of_file(file_name)
         if count < verifier_limit:
             FlowVisor.enable_verifier_mode()
             return
-        logger.log(
+        Logger.log(
             f"Verifier mode not enabled. Count of calls is {count} and the limit is {verifier_limit}"
         )
 
     @staticmethod
     def enable_verifier_mode():
         """
         Enables the verifier mode.
         """
         FlowVisor.VERIFIER_MODE = True
         FlowVisor.VIS_FUNCTION = vis_verifier
-        logger.log("*** Running FlowVisor in verify mode ***")
+        Logger.log("*** Running FlowVisor in verify mode ***")
 
     @staticmethod
     def verify_export(file_name="flowvisor_verifier.json"):
         """
         Exports the verifier.
         """
         if not FlowVisor.VERIFIER_MODE:
-            logger.log("Can not export verify in non-verifier mode!")
+            Logger.log("Can not export verify in non-verifier mode!")
             return
         FlowVisorVerifier.export(file_name)
 
     @staticmethod
     def verify(verify_file_name="flowvisor_verifier.json"):
         """
         Checks the result against the verifier.
         """
         if FlowVisor.VERIFIER_MODE:
-            logger.log("Can not verify in verifier mode!")
+            Logger.log("Can not verify in verifier mode!")
             return False
         return FlowVisorVerifier.verify(
             FlowVisor.NODES, verify_file_name, FlowVisor.CONFIG.verify_threshold
         )
 
+    @staticmethod
+    def set_log_file(file_name: str = "flowvisor.log"):
+        """
+        Sets the log file.
+        """
+        Logger.LOG_FILE = file_name
+
+    @staticmethod
+    def disable_console_logging():
+        """
+        Disables console logging.
+        """
+        Logger.LOG_TO_CONSOLE = False
+
     '''
     @staticmethod
     def visualize_all():
         """
         Visualizes all the functions in this project.
         """
         FlowVisor.visualize_module_by_name("__main__")
```

### Comparing `FlowVisor-0.1.5/flowvisor/flowvisor_config.py` & `FlowVisor-0.1.6/flowvisor/flowvisor_config.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.1.5/flowvisor/flowvisor_verifier.py` & `FlowVisor-0.1.6/flowvisor/flowvisor_verifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import cProfile
 import json
 import os
 import pstats
 import time
 from typing import List
 
-from flowvisor import logger, utils
+from flowvisor import utils
+from flowvisor.logger import Logger
 from flowvisor.function_node import FunctionNode
 
 
 def vis_verifier(func):
     def wrapper(*args, **kwargs):
         start = time.time()
         res = func(*args, **kwargs)
@@ -151,31 +152,32 @@
         return new_data
 
     @staticmethod
     def verify(nodes: List[FunctionNode], verify_file_name: str, threshold: float):
         verify_file_name = utils.apply_file_end(verify_file_name, "json")
 
         if not os.path.exists(verify_file_name):
-            logger.log(f"Verify file {verify_file_name} not found...")
+            Logger.log(f"Verify file {verify_file_name} not found...")
             return
 
         content = FlowVisorVerifier.read_existing_file(verify_file_name)
 
         is_verified = True
         device_name = content["meta"]["device_name"]
         if device_name != utils.get_device_name():
-            logger.log(
+            Logger.log(
                 f"🚨 WARNING 🚨 Verifier file is not clean: Wrong device {device_name}"
             )
             is_verified = False
 
+        Logger.log("Verifying functions...")
         for entry in content["data"]:
             node = utils.get_node_by_id(entry["id"], nodes)
             if node is None:
-                logger.log(f"Function with id {entry['id']} not found")
+                Logger.log(f"Function with id {entry['id']} not found")
                 continue
 
             node_time = node.get_time(exclusive=False)
             verify_time = entry["time"]
             time_delta = node_time - verify_time
 
             # get how many percent the node time is off
@@ -187,22 +189,22 @@
                 print_warning = True
 
             time_delta_direction = "more"
             if time_delta < 0:
                 time_delta *= -1
                 time_delta_direction = "less"
 
-            logger.log(
-                f"Function '{node.name}' took {utils.get_time_as_string(time_delta)} {time_delta_direction} than expected ({time_delta_percentage * 100}%) {'🚨' if print_warning else ''}"
+            Logger.log(
+                f"  Function '{node.name}' took {utils.get_time_as_string(time_delta)} {time_delta_direction} than expected ({time_delta_percentage * 100}%) {'🚨' if print_warning else ''}"
             )
 
         if is_verified:
-            logger.log("All functions are verified! ✅")
+            Logger.log("All functions are verified! ✅")
         else:
-            logger.log("Some functions are not verified! ❌")
+            Logger.log("Some functions are not verified! ❌")
         return is_verified
 
     @staticmethod
     def is_function_verified(entry, node_time, threshold):
         max_value = entry["max"]
         min_value = entry["min"]
         mean_time = entry["time"]
```

### Comparing `FlowVisor-0.1.5/flowvisor/function_node.py` & `FlowVisor-0.1.6/flowvisor/function_node.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.1.5/flowvisor/sankey.py` & `FlowVisor-0.1.6/flowvisor/sankey.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.1.5/flowvisor/time_tracker.py` & `FlowVisor-0.1.6/flowvisor/time_tracker.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.1.5/flowvisor/utils.py` & `FlowVisor-0.1.6/flowvisor/utils.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.1.5/setup.py` & `FlowVisor-0.1.6/setup.py`

 * *Files identical despite different names*

