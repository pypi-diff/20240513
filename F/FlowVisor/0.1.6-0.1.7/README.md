# Comparing `tmp/FlowVisor-0.1.6.tar.gz` & `tmp/FlowVisor-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FlowVisor-0.1.6.tar", last modified: Mon May 13 06:48:36 2024, max compression
+gzip compressed data, was "FlowVisor-0.1.7.tar", last modified: Mon May 13 10:00:24 2024, max compression
```

## Comparing `FlowVisor-0.1.6.tar` & `FlowVisor-0.1.7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-13 06:48:36.533249 FlowVisor-0.1.6/
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-13 06:48:36.529249 FlowVisor-0.1.6/FlowVisor.egg-info/
--rw-rw-r--   0 phil      (1000) phil      (1000)     3697 2024-05-13 06:48:36.000000 FlowVisor-0.1.6/FlowVisor.egg-info/PKG-INFO
--rw-rw-r--   0 phil      (1000) phil      (1000)      593 2024-05-13 06:48:36.000000 FlowVisor-0.1.6/FlowVisor.egg-info/SOURCES.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)        1 2024-05-13 06:48:36.000000 FlowVisor-0.1.6/FlowVisor.egg-info/dependency_links.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)      138 2024-05-13 06:48:36.000000 FlowVisor-0.1.6/FlowVisor.egg-info/entry_points.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)       59 2024-05-13 06:48:36.000000 FlowVisor-0.1.6/FlowVisor.egg-info/requires.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)       10 2024-05-13 06:48:36.000000 FlowVisor-0.1.6/FlowVisor.egg-info/top_level.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)     1067 2024-04-22 08:55:02.000000 FlowVisor-0.1.6/LICENSE
--rw-rw-r--   0 phil      (1000) phil      (1000)     3697 2024-05-13 06:48:36.533249 FlowVisor-0.1.6/PKG-INFO
--rw-rw-r--   0 phil      (1000) phil      (1000)     3016 2024-04-25 13:11:25.000000 FlowVisor-0.1.6/README.md
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-13 06:48:36.533249 FlowVisor-0.1.6/flowvisor/
--rw-rw-r--   0 phil      (1000) phil      (1000)      221 2024-05-08 20:53:18.000000 FlowVisor-0.1.6/flowvisor/__init__.py
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-13 06:48:36.533249 FlowVisor-0.1.6/flowvisor/cli/
--rw-rw-r--   0 phil      (1000) phil      (1000)        0 2024-04-25 10:31:43.000000 FlowVisor-0.1.6/flowvisor/cli/__init__.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     3199 2024-04-25 13:10:53.000000 FlowVisor-0.1.6/flowvisor/cli/add_vis.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     2270 2024-04-25 13:16:50.000000 FlowVisor-0.1.6/flowvisor/cli/remove_vis.py
--rw-rw-r--   0 phil      (1000) phil      (1000)      911 2024-04-25 13:10:38.000000 FlowVisor-0.1.6/flowvisor/cli/vis_file.py
--rw-rw-r--   0 phil      (1000) phil      (1000)    16758 2024-05-13 06:45:04.000000 FlowVisor-0.1.6/flowvisor/flowvisor.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     2030 2024-05-11 05:24:19.000000 FlowVisor-0.1.6/flowvisor/flowvisor_config.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     7969 2024-05-13 06:42:22.000000 FlowVisor-0.1.6/flowvisor/flowvisor_verifier.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     8004 2024-05-09 07:05:50.000000 FlowVisor-0.1.6/flowvisor/function_node.py
--rw-rw-r--   0 phil      (1000) phil      (1000)      887 2024-05-13 06:45:56.000000 FlowVisor-0.1.6/flowvisor/logger.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     2181 2024-05-08 16:32:50.000000 FlowVisor-0.1.6/flowvisor/sankey.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     2732 2024-04-25 11:15:11.000000 FlowVisor-0.1.6/flowvisor/time_tracker.py
--rw-rw-r--   0 phil      (1000) phil      (1000)      292 2024-05-08 15:25:05.000000 FlowVisor-0.1.6/flowvisor/time_value.py
--rw-rw-r--   0 phil      (1000) phil      (1000)      300 2024-05-08 13:28:52.000000 FlowVisor-0.1.6/flowvisor/timer.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     3132 2024-05-09 07:27:11.000000 FlowVisor-0.1.6/flowvisor/utils.py
--rw-rw-r--   0 phil      (1000) phil      (1000)       38 2024-05-13 06:48:36.533249 FlowVisor-0.1.6/setup.cfg
--rw-rw-r--   0 phil      (1000) phil      (1000)     1585 2024-04-25 13:18:25.000000 FlowVisor-0.1.6/setup.py
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-13 10:00:24.626227 FlowVisor-0.1.7/
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-13 10:00:24.626227 FlowVisor-0.1.7/FlowVisor.egg-info/
+-rw-rw-r--   0 phil      (1000) phil      (1000)     3697 2024-05-13 10:00:24.000000 FlowVisor-0.1.7/FlowVisor.egg-info/PKG-INFO
+-rw-rw-r--   0 phil      (1000) phil      (1000)      593 2024-05-13 10:00:24.000000 FlowVisor-0.1.7/FlowVisor.egg-info/SOURCES.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)        1 2024-05-13 10:00:24.000000 FlowVisor-0.1.7/FlowVisor.egg-info/dependency_links.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)      138 2024-05-13 10:00:24.000000 FlowVisor-0.1.7/FlowVisor.egg-info/entry_points.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)       59 2024-05-13 10:00:24.000000 FlowVisor-0.1.7/FlowVisor.egg-info/requires.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)       10 2024-05-13 10:00:24.000000 FlowVisor-0.1.7/FlowVisor.egg-info/top_level.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)     1067 2024-04-22 08:55:02.000000 FlowVisor-0.1.7/LICENSE
+-rw-rw-r--   0 phil      (1000) phil      (1000)     3697 2024-05-13 10:00:24.626227 FlowVisor-0.1.7/PKG-INFO
+-rw-rw-r--   0 phil      (1000) phil      (1000)     3016 2024-04-25 13:11:25.000000 FlowVisor-0.1.7/README.md
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-13 10:00:24.626227 FlowVisor-0.1.7/flowvisor/
+-rw-rw-r--   0 phil      (1000) phil      (1000)      221 2024-05-08 20:53:18.000000 FlowVisor-0.1.7/flowvisor/__init__.py
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-13 10:00:24.626227 FlowVisor-0.1.7/flowvisor/cli/
+-rw-rw-r--   0 phil      (1000) phil      (1000)        0 2024-04-25 10:31:43.000000 FlowVisor-0.1.7/flowvisor/cli/__init__.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     3199 2024-04-25 13:10:53.000000 FlowVisor-0.1.7/flowvisor/cli/add_vis.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     2270 2024-04-25 13:16:50.000000 FlowVisor-0.1.7/flowvisor/cli/remove_vis.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)      911 2024-04-25 13:10:38.000000 FlowVisor-0.1.7/flowvisor/cli/vis_file.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)    14023 2024-05-13 09:09:16.000000 FlowVisor-0.1.7/flowvisor/flowvisor.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     2214 2024-05-13 09:29:39.000000 FlowVisor-0.1.7/flowvisor/flowvisor_config.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     8113 2024-05-13 09:29:19.000000 FlowVisor-0.1.7/flowvisor/flowvisor_verifier.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     8373 2024-05-13 09:21:33.000000 FlowVisor-0.1.7/flowvisor/function_node.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)      887 2024-05-13 06:45:56.000000 FlowVisor-0.1.7/flowvisor/logger.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     2181 2024-05-08 16:32:50.000000 FlowVisor-0.1.7/flowvisor/sankey.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     2732 2024-04-25 11:15:11.000000 FlowVisor-0.1.7/flowvisor/time_tracker.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     2474 2024-05-13 09:18:43.000000 FlowVisor-0.1.7/flowvisor/time_value.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)      300 2024-05-08 13:28:52.000000 FlowVisor-0.1.7/flowvisor/timer.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     3132 2024-05-09 07:27:11.000000 FlowVisor-0.1.7/flowvisor/utils.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)       38 2024-05-13 10:00:24.626227 FlowVisor-0.1.7/setup.cfg
+-rw-rw-r--   0 phil      (1000) phil      (1000)     1585 2024-04-25 13:18:25.000000 FlowVisor-0.1.7/setup.py
```

### Comparing `FlowVisor-0.1.6/FlowVisor.egg-info/PKG-INFO` & `FlowVisor-0.1.7/FlowVisor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlowVisor
-Version: 0.1.6
+Version: 0.1.7
 Summary: Visualize and profile your python code with FlowVisor.
 Home-page: https://github.com/cophilot/FlowVisor
 Author: cophilot (Philipp B.)
 Author-email: <info@philipp-bonin.com>
 License: MIT
 Keywords: python,flow,visualize,code,flowvisor,profiling,profile,decorator
 Platform: UNKNOWN
```

### Comparing `FlowVisor-0.1.6/FlowVisor.egg-info/SOURCES.txt` & `FlowVisor-0.1.7/FlowVisor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.1.6/LICENSE` & `FlowVisor-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.1.6/PKG-INFO` & `FlowVisor-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlowVisor
-Version: 0.1.6
+Version: 0.1.7
 Summary: Visualize and profile your python code with FlowVisor.
 Home-page: https://github.com/cophilot/FlowVisor
 Author: cophilot (Philipp B.)
 Author-email: <info@philipp-bonin.com>
 License: MIT
 Keywords: python,flow,visualize,code,flowvisor,profiling,profile,decorator
 Platform: UNKNOWN
```

### Comparing `FlowVisor-0.1.6/README.md` & `FlowVisor-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.1.6/flowvisor/cli/add_vis.py` & `FlowVisor-0.1.7/flowvisor/cli/add_vis.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.1.6/flowvisor/cli/remove_vis.py` & `FlowVisor-0.1.7/flowvisor/cli/remove_vis.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.1.6/flowvisor/cli/vis_file.py` & `FlowVisor-0.1.7/flowvisor/cli/vis_file.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.1.6/flowvisor/flowvisor.py` & `FlowVisor-0.1.7/flowvisor/flowvisor.py`

 * *Files 14% similar despite different names*

```diff
@@ -199,52 +199,14 @@
     def sankey_diagram():
         """
         Generates the sankey diagram.
         """
         make_sankey_diagram(FlowVisor.ROOTS, FlowVisor.NODES)
 
     @staticmethod
-    def get_highest_time():
-        """
-        Returns the highest time.
-        """
-        highest_time = -1
-        for node in FlowVisor.NODES:
-            node_time = node.get_time(FlowVisor.CONFIG.exclusive_time_mode)
-            if node_time > highest_time:
-                highest_time = node_time
-        return highest_time
-
-    @staticmethod
-    def get_total_time():
-        """
-        Returns the total time.
-        """
-        total_time = 0
-        nodes = FlowVisor.NODES
-        if not FlowVisor.CONFIG.exclusive_time_mode:
-            nodes = FlowVisor.ROOTS
-
-        for node in nodes:
-            total_time += node.get_time(FlowVisor.CONFIG.exclusive_time_mode)
-
-        return total_time
-
-    @staticmethod
-    def get_mean_time():
-        """
-        Returns the mean time.
-        """
-        sum_time = 0
-        for node in FlowVisor.NODES:
-            sum_time += node.get_time(FlowVisor.CONFIG.exclusive_time_mode)
-
-        return sum_time / len(FlowVisor.NODES)
-
-    @staticmethod
     def draw_meta_data(blank_image, verify_text):
         """
         Draws some metadata on the graph.
         """
         with Cluster("Metadata", graph_attr={"bgcolor": "#FFFFFF"}):
             if verify_text is not None:
                 Custom(verify_text, blank_image, width="2", height="0.1")
@@ -263,17 +225,15 @@
 
     @staticmethod
     def draw_nodes_with_cluster(nodes: List[FunctionNode]):
         """
         Draws the nodes with cluster.
         """
         sorted_nodes = FlowVisor.get_node_sorted_by_filename(nodes)
-        total_times = [
-            sum([n.get_time_without_children() for n in row]) for row in sorted_nodes
-        ]
+        total_times = [sum([n.get_time() for n in row]) for row in sorted_nodes]
         highest_time_file_time = max(total_times)
         for index, row in enumerate(sorted_nodes):
             cluster_title = (
                 f"{row[0].file_name} ({utils.get_time_as_string(total_times[index])})"
             )
             bg_color = utils.value_to_hex_color(
                 total_times[index],
@@ -364,18 +324,15 @@
         FlowVisor.graph()
 
     @staticmethod
     def draw_function_node(func_node: FunctionNode):
         """
         Draws the function node.
         """
-        time_value = TimeValue()
-        time_value.max_time = FlowVisor.get_highest_time()
-        time_value.total_time = FlowVisor.get_total_time()
-        time_value.mean_time = FlowVisor.get_mean_time()
+        time_value = TimeValue(FlowVisor.NODES, FlowVisor.CONFIG, FlowVisor.ROOTS)
 
         node = func_node.get_as_diagram_node(time_value, FlowVisor.CONFIG)
         for child in func_node.children:
             _ = node >> child.get_as_diagram_node(time_value, FlowVisor.CONFIG)
 
     @staticmethod
     def is_function_excluded(func):
@@ -503,53 +460,7 @@
 
     @staticmethod
     def disable_console_logging():
         """
         Disables console logging.
         """
         Logger.LOG_TO_CONSOLE = False
-
-    '''
-    @staticmethod
-    def visualize_all():
-        """
-        Visualizes all the functions in this project.
-        """
-        FlowVisor.visualize_module_by_name("__main__")
-
-    @staticmethod
-    def visualize_module_by_name(module_name: str):
-        """
-        Visualizes all the functions in a module.
-        """
-        module = __import__(module_name)
-
-        FlowVisor.visualize_module(module)
-
-    @staticmethod
-    def visualize_module(module: object):
-        FlowVisor.visualize_module_helper(module, [])
-
-    @staticmethod
-    def visualize_module_helper(module: object, added_modules):
-        """
-        Visualizes all the functions in a module.
-        """
-        print("This function is still buggy and will not work as expected. Workin on it!")
-        for name, obj in getmembers(module, isfunction):
-            setattr(module, name, vis(obj))
-
-        # TODO
-        # # add for all submodules
-        #for name, sub_module in getmembers(module, ismodule):
-        #    if sub_module.__name__ in added_modules:
-        #        with open(f"log.txt", "a") as f:
-        #            f.write(f"NOT Visualizing module: {sub_module.__name__}\n")
-#
-        #        continue
-        #    added_modules.append(sub_module.__name__)
-        #    print(f"Visualizing module: {sub_module.__name__}")
-        #    # write to a file
-        #    with open(f"log.txt", "a") as f:
-        #        f.write(f"Visualizing module: {sub_module.__name__}\n")
-        #    FlowVisor.visualize_module_helper(sub_module, added_modules)
-    '''
```

### Comparing `FlowVisor-0.1.6/flowvisor/flowvisor_config.py` & `FlowVisor-0.1.7/flowvisor/flowvisor_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,36 +30,41 @@
         # File settings
         self.output_file: str = "function_flow"
 
         # Functional settings
         self.reduce_overhead: bool = True
         self.exclusive_time_mode: bool = True
         self.advanced_overhead_reduction = None
+        self.use_avg_time: bool = False
 
         # Verifier settings
         self.verify_threshold: float = 0.2
 
         # Other
         self.dev_mode: bool = False
 
     def get_node_scale(self):
         """
         Get the node scale as a string
         """
         return str(self.node_scale)
 
     def get_functional_settings_string(self):
+        """
+        Returns a string with the functional settings
+        """
         s = "Reduce Overhead: " + str(self.reduce_overhead) + "\n"
         if self.reduce_overhead and self.advanced_overhead_reduction is not None:
             s += (
                 "Advanced Overhead reduction: "
                 + utils.get_time_as_string(self.advanced_overhead_reduction)
                 + "\n"
             )
         s += "Exclusive Time Mode: " + str(self.exclusive_time_mode) + "\n"
+        s += "Use Average Time: " + str(self.use_avg_time) + "\n"
         return s
 
     @staticmethod
     def from_dict(config_dict: dict):
         """
         Create a FlowVisorConfig object from a dictionary
         """
```

### Comparing `FlowVisor-0.1.6/flowvisor/flowvisor_verifier.py` & `FlowVisor-0.1.7/flowvisor/flowvisor_verifier.py`

 * *Files 5% similar despite different names*

```diff
@@ -185,20 +185,22 @@
             print_warning = False
 
             if not FlowVisorVerifier.is_function_verified(entry, node_time, threshold):
                 is_verified = False
                 print_warning = True
 
             time_delta_direction = "more"
+            time_delta_direction_arrow = "🔼"
             if time_delta < 0:
                 time_delta *= -1
                 time_delta_direction = "less"
+                time_delta_direction_arrow = "🔽"
 
             Logger.log(
-                f"  Function '{node.name}' took {utils.get_time_as_string(time_delta)} {time_delta_direction} than expected ({time_delta_percentage * 100}%) {'🚨' if print_warning else ''}"
+                f"  Function '{node.file_function_name()}' took {utils.get_time_as_string(time_delta)} {time_delta_direction} than expected ({time_delta_percentage * 100}%) {time_delta_direction_arrow}{'🚨' if print_warning else ''}"
             )
 
         if is_verified:
             Logger.log("All functions are verified! ✅")
         else:
             Logger.log("Some functions are not verified! ❌")
         return is_verified
```

### Comparing `FlowVisor-0.1.6/flowvisor/function_node.py` & `FlowVisor-0.1.7/flowvisor/function_node.py`

 * *Files 7% similar despite different names*

```diff
@@ -40,18 +40,24 @@
         Generates the node image background.
         """
         dim = FunctionNode.NODE_IMAGE_SCALE
         image = Image.new("RGB", (dim, dim), "white")
         draw = ImageDraw.Draw(image)
 
         t = self.get_time(config.exclusive_time_mode)
+        mean = time_value.mean_time
+        max = time_value.max_time
+        if config.use_avg_time:
+            t = self.get_avg_time(config.exclusive_time_mode)
+            mean = time_value.mean_avg_time
+            max = time_value.max_avg_time
 
-        color = utils.value_to_hex_color_using_mean(t, time_value.mean_time)
+        color = utils.value_to_hex_color_using_mean(t, mean)
 
-        if t >= time_value.max_time * (1 - config.outline_threshold):
+        if t >= max * (1 - config.outline_threshold):
             # draw outline
             draw.rectangle((0, 0, dim, dim), fill="#ff0000")
             ## draw inner
             draw.rectangle((10, 10, dim - 10, dim - 10), fill=color)
         else:
             draw.rectangle((0, 0, dim, dim), fill=color)
 
@@ -77,17 +83,22 @@
 
         size = config.node_scale
 
         title = self.get_node_title(time_value, config)
 
         font_color = config.static_font_color
         if font_color == "":
+            t = self.get_time(config.exclusive_time_mode)
+            m = time_value.mean_time
+            if config.use_avg_time:
+                t = self.get_avg_time(config.exclusive_time_mode)
+                m = time_value.mean_avg_time
             font_color = utils.value_to_hex_color_using_mean(
-                self.get_time(config.exclusive_time_mode),
-                time_value.mean_time,
+                t,
+                m,
                 dark_color=[0xFF, 0xC0, 0x82],
                 light_color=[0x00, 0x00, 0x00],
             )
 
         self.diagram_node = Custom(
             title, node_image, width=str(size), height=str(size), fontcolor=font_color
         )
@@ -105,15 +116,15 @@
 
         if config.show_node_call_count:
             title += f" ({self.called})"
 
         title += "\n"
 
         if config.show_node_avg_time:
-            title += f"avg {utils.get_time_as_string(t / self.called)}"
+            title += f"avg {utils.get_time_as_string(self.get_avg_time(config.exclusive_time_mode))}"
 
         title += "\n"
 
         if config.show_function_time_percantage:
             percentage = (t / time_value.total_time) * 100
             title += f"{round(percentage, 2)}%"
 
@@ -202,34 +213,31 @@
         """
         self.children = []
         for child_id in self.children_ids:
             for node in all_nodes:
                 if node.uuid == child_id:
                     self.add_child(node)
 
-    def get_time_without_children(self):
-        """
-        Gets the time without the children.
-        """
-        time = self.get_time()
-        for child in self.children:
-            time -= child.time
-        return time
-
     def get_time(self, exclusive=True):
         """
         Gets the time of the node.
 
         Args:
             exclusive: If the time should be exclusive.
         """
         if exclusive:
             return self.__time - self.child_time
         return self.__time
 
+    def get_avg_time(self, exclusive=True):
+        """
+        Gets the average time of the node.
+        """
+        return self.get_time(exclusive) / self.called
+
     @staticmethod
     def make_node_image_cache():
         """
         Makes the node image cache.
 
         Returns:
             The file name of the blank image.
```

### Comparing `FlowVisor-0.1.6/flowvisor/logger.py` & `FlowVisor-0.1.7/flowvisor/logger.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.1.6/flowvisor/sankey.py` & `FlowVisor-0.1.7/flowvisor/sankey.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.1.6/flowvisor/time_tracker.py` & `FlowVisor-0.1.7/flowvisor/time_tracker.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.1.6/flowvisor/utils.py` & `FlowVisor-0.1.7/flowvisor/utils.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.1.6/setup.py` & `FlowVisor-0.1.7/setup.py`

 * *Files identical despite different names*

