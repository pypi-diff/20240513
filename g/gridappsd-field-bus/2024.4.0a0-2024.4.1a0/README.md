# Comparing `tmp/gridappsd_field_bus-2024.4.0a0.tar.gz` & `tmp/gridappsd_field_bus-2024.4.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gridappsd_field_bus-2024.4.0a0.tar", max compression
+gzip compressed data, was "gridappsd_field_bus-2024.4.1a0.tar", max compression
```

## Comparing `gridappsd_field_bus-2024.4.0a0.tar` & `gridappsd_field_bus-2024.4.1a0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        0 2024-05-02 16:40:43.790433 gridappsd_field_bus-2024.4.0a0/README.md
--rw-r--r--   0        0        0        0 2024-05-02 16:40:43.790433 gridappsd_field_bus-2024.4.0a0/gridappsd/__no_init__here
--rw-r--r--   0        0        0      217 2024-05-02 16:40:43.790433 gridappsd_field_bus-2024.4.0a0/gridappsd/field_interface/__init__.py
--rw-r--r--   0        0        0      350 2024-05-02 16:40:43.790433 gridappsd_field_bus-2024.4.0a0/gridappsd/field_interface/agents/__init__.py
--rw-r--r--   0        0        0    15723 2024-05-02 16:40:43.790433 gridappsd_field_bus-2024.4.0a0/gridappsd/field_interface/agents/agents.py
--rw-r--r--   0        0        0     3361 2024-05-02 16:40:43.790433 gridappsd_field_bus-2024.4.0a0/gridappsd/field_interface/context.py
--rw-r--r--   0        0        0    12316 2024-05-02 16:40:43.790433 gridappsd_field_bus-2024.4.0a0/gridappsd/field_interface/context_manager.py
--rw-r--r--   0        0        0     1829 2024-05-02 16:40:43.790433 gridappsd_field_bus-2024.4.0a0/gridappsd/field_interface/gridappsd_field_bus.py
--rw-r--r--   0        0        0     7544 2024-05-02 16:40:43.790433 gridappsd_field_bus-2024.4.0a0/gridappsd/field_interface/interfaces.py
--rw-r--r--   0        0        0     1264 2024-05-02 16:41:40.206314 gridappsd_field_bus-2024.4.0a0/pyproject.toml
--rw-r--r--   0        0        0      854 1970-01-01 00:00:00.000000 gridappsd_field_bus-2024.4.0a0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-13 20:14:27.052062 gridappsd_field_bus-2024.4.1a0/README.md
+-rw-r--r--   0        0        0        0 2024-05-13 20:14:27.052062 gridappsd_field_bus-2024.4.1a0/gridappsd/__no_init__here
+-rw-r--r--   0        0        0      217 2024-05-13 20:14:27.052062 gridappsd_field_bus-2024.4.1a0/gridappsd/field_interface/__init__.py
+-rw-r--r--   0        0        0      350 2024-05-13 20:14:27.052062 gridappsd_field_bus-2024.4.1a0/gridappsd/field_interface/agents/__init__.py
+-rw-r--r--   0        0        0    15723 2024-05-13 20:14:27.052062 gridappsd_field_bus-2024.4.1a0/gridappsd/field_interface/agents/agents.py
+-rw-r--r--   0        0        0     3361 2024-05-13 20:14:27.052062 gridappsd_field_bus-2024.4.1a0/gridappsd/field_interface/context.py
+-rw-r--r--   0        0        0    12377 2024-05-13 20:14:27.052062 gridappsd_field_bus-2024.4.1a0/gridappsd/field_interface/context_manager.py
+-rw-r--r--   0        0        0     1829 2024-05-13 20:14:27.052062 gridappsd_field_bus-2024.4.1a0/gridappsd/field_interface/gridappsd_field_bus.py
+-rw-r--r--   0        0        0     7544 2024-05-13 20:14:27.052062 gridappsd_field_bus-2024.4.1a0/gridappsd/field_interface/interfaces.py
+-rw-r--r--   0        0        0     1264 2024-05-13 20:15:46.148598 gridappsd_field_bus-2024.4.1a0/pyproject.toml
+-rw-r--r--   0        0        0      854 1970-01-01 00:00:00.000000 gridappsd_field_bus-2024.4.1a0/PKG-INFO
```

### Comparing `gridappsd_field_bus-2024.4.0a0/gridappsd/field_interface/agents/agents.py` & `gridappsd_field_bus-2024.4.1a0/gridappsd/field_interface/agents/agents.py`

 * *Files identical despite different names*

### Comparing `gridappsd_field_bus-2024.4.0a0/gridappsd/field_interface/context.py` & `gridappsd_field_bus-2024.4.1a0/gridappsd/field_interface/context.py`

 * *Files identical despite different names*

### Comparing `gridappsd_field_bus-2024.4.0a0/gridappsd/field_interface/context_manager.py` & `gridappsd_field_bus-2024.4.1a0/gridappsd/field_interface/context_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
                     time.sleep(5)
         super().__init__(upstream_message_bus_def, downstream_message_bus_def, agent_config,
                          feeder_dict, simulation_id)
 
         #Override agent_id to a static value
         self.agent_id = downstream_message_bus_def.id + '.context_manager'
 
-        self.context = None
+        self.context = {'data':feeder_dict}
 
         self.registered_agents = {}
         self.registered_agents[self.agent_id] = self.get_registration_details()
 
         self.neighbouring_agents = {}
         self.upstream_agents = {}
         self.downstream_agents = {}
@@ -109,15 +109,15 @@
 
         super().__init__(upstream_message_bus_def, downstream_message_bus_def, agent_config,
                          switch_area_dict, simulation_id)
 
         #Override agent_id to a static value
         self.agent_id = downstream_message_bus_def.id + '.context_manager'
 
-        self.context = None
+        self.context = {'data':switch_area_dict}
 
         self.registered_agents = {}
         self.registered_agents[self.agent_id] = self.get_registration_details()
         self.ot_connection.get_logger().info("Switch Area "+self.agent_id+" Context Manager Created")
 
     def on_request(self, message_bus, headers: Dict, message):
 
@@ -168,15 +168,15 @@
 
         super().__init__(upstream_message_bus_def, downstream_message_bus_def, agent_config,
                          secondary_area_dict, simulation_id)
 
         #Override agent_id to a static value
         self.agent_id = downstream_message_bus_def.id + '.context_manager'
 
-        self.context = None
+        self.context = {'data':secondary_area_dict}
 
         self.registered_agents = {}
         self.registered_agents[self.agent_id] = self.get_registration_details()
         self.ot_connection.get_logger().info("Secondary Area "+self.agent_id+" Context Manager Created")
 
     def on_request(self, message_bus, headers: Dict, message):
```

### Comparing `gridappsd_field_bus-2024.4.0a0/gridappsd/field_interface/gridappsd_field_bus.py` & `gridappsd_field_bus-2024.4.1a0/gridappsd/field_interface/gridappsd_field_bus.py`

 * *Files identical despite different names*

### Comparing `gridappsd_field_bus-2024.4.0a0/gridappsd/field_interface/interfaces.py` & `gridappsd_field_bus-2024.4.1a0/gridappsd/field_interface/interfaces.py`

 * *Files identical despite different names*

### Comparing `gridappsd_field_bus-2024.4.0a0/pyproject.toml` & `gridappsd_field_bus-2024.4.1a0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gridappsd-field-bus"
-version = "2024.4.0a0"
+version = "2024.4.1a0"
 description = "GridAPPS-D Field Bus Implementation"
 authors = [
     "C. Allwardt <3979063+craig8@users.noreply.github.com>",
     "P. Sharma <poorva.sharma@pnnl.gov",
     "A. Fisher <andrew.fisher@pnnl.gov"
 ]
 license = "BSD-3-Clause"
@@ -24,15 +24,15 @@
 [tool.poetry.scripts]
 # Add things in the form
 # myscript = 'my_package:main'
 context_manager = 'gridappsd.field_interface.context_manager:_main'
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-gridappsd-python = "^2024.4.0a0"
+gridappsd-python = "^2024.4.1a0"
 cim-graph = ">=0.1.1a0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^6.2.2"
 pytest-html = "^3.1.1"
 mock = "^4.0.3"
 docker = "^4.4.4"
```

### Comparing `gridappsd_field_bus-2024.4.0a0/PKG-INFO` & `gridappsd_field_bus-2024.4.1a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: gridappsd-field-bus
-Version: 2024.4.0a0
+Version: 2024.4.1a0
 Summary: GridAPPS-D Field Bus Implementation
 Home-page: https://gridappsd.readthedocs.io
 License: BSD-3-Clause
 Keywords: gridappsd,grid,activmq,powergrid,simulation,library
 Author: C. Allwardt
 Author-email: 3979063+craig8@users.noreply.github.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: cim-graph (>=0.1.1a0)
-Requires-Dist: gridappsd-python (>=2024.4.0a0,<2025.0.0)
+Requires-Dist: gridappsd-python (>=2024.4.1a0,<2025.0.0)
 Project-URL: Repository, https://github.com/GRIDAPPSD/gridappsd-python
 Description-Content-Type: text/markdown
```

