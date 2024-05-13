# Comparing `tmp/qpiai_opt_api-1.0.2.tar.gz` & `tmp/qpiai_opt_api-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qpiai_opt_api-1.0.2.tar", last modified: Sat Apr 27 12:15:57 2024, max compression
+gzip compressed data, was "qpiai_opt_api-1.0.3.tar", last modified: Mon May 13 16:11:33 2024, max compression
```

## Comparing `qpiai_opt_api-1.0.2.tar` & `qpiai_opt_api-1.0.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 akshat    (1005) akshat    (1005)        0 2024-04-27 12:15:57.965112 qpiai_opt_api-1.0.2/
--rw-rw-r--   0 akshat    (1005) akshat    (1005)     1099 2024-04-27 12:14:36.000000 qpiai_opt_api-1.0.2/LICENSE.txt
--rw-r--r--   0 akshat    (1005) akshat    (1005)     3484 2024-04-27 12:15:57.965112 qpiai_opt_api-1.0.2/PKG-INFO
--rw-rw-r--   0 akshat    (1005) akshat    (1005)     1709 2024-04-27 12:14:36.000000 qpiai_opt_api-1.0.2/README.md
--rw-rw-r--   0 akshat    (1005) akshat    (1005)       84 2024-04-27 12:14:36.000000 qpiai_opt_api-1.0.2/pyproject.toml
--rw-rw-r--   0 akshat    (1005) akshat    (1005)      796 2024-04-27 12:15:57.965112 qpiai_opt_api-1.0.2/setup.cfg
-drwxrwxr-x   0 akshat    (1005) akshat    (1005)        0 2024-04-27 12:15:57.961112 qpiai_opt_api-1.0.2/src/
-drwxrwxr-x   0 akshat    (1005) akshat    (1005)        0 2024-04-27 12:15:57.965112 qpiai_opt_api-1.0.2/src/qpiai_opt/
--rw-rw-r--   0 akshat    (1005) akshat    (1005)        0 2024-04-27 12:14:36.000000 qpiai_opt_api-1.0.2/src/qpiai_opt/__init__.py
-drwxrwxr-x   0 akshat    (1005) akshat    (1005)        0 2024-04-27 12:15:57.965112 qpiai_opt_api-1.0.2/src/qpiai_opt/problem/
--rw-rw-r--   0 akshat    (1005) akshat    (1005)      319 2024-04-27 12:14:36.000000 qpiai_opt_api-1.0.2/src/qpiai_opt/problem/__init__.py
--rw-rw-r--   0 akshat    (1005) akshat    (1005)     1187 2024-04-27 12:14:36.000000 qpiai_opt_api-1.0.2/src/qpiai_opt/problem/max_cut.py
--rw-rw-r--   0 akshat    (1005) akshat    (1005)     1006 2024-04-27 12:14:36.000000 qpiai_opt_api-1.0.2/src/qpiai_opt/problem/max_independet_set.py
--rw-rw-r--   0 akshat    (1005) akshat    (1005)      895 2024-04-27 12:14:36.000000 qpiai_opt_api-1.0.2/src/qpiai_opt/problem/number_partition.py
--rw-rw-r--   0 akshat    (1005) akshat    (1005)      807 2024-04-27 12:14:36.000000 qpiai_opt_api-1.0.2/src/qpiai_opt/problem/qubo.py
--rw-rw-r--   0 akshat    (1005) akshat    (1005)      964 2024-04-27 12:14:36.000000 qpiai_opt_api-1.0.2/src/qpiai_opt/problem/vertex_cover.py
-drwxrwxr-x   0 akshat    (1005) akshat    (1005)        0 2024-04-27 12:15:57.965112 qpiai_opt_api-1.0.2/src/qpiai_opt/solver/
--rw-rw-r--   0 akshat    (1005) akshat    (1005)       43 2024-04-27 12:14:36.000000 qpiai_opt_api-1.0.2/src/qpiai_opt/solver/__init__.py
--rw-rw-r--   0 akshat    (1005) akshat    (1005)     2698 2024-04-27 12:14:36.000000 qpiai_opt_api-1.0.2/src/qpiai_opt/solver/solver.py
-drwxrwxr-x   0 akshat    (1005) akshat    (1005)        0 2024-04-27 12:15:57.965112 qpiai_opt_api-1.0.2/src/qpiai_opt/wrappers/
--rw-rw-r--   0 akshat    (1005) akshat    (1005)       98 2024-04-27 12:14:36.000000 qpiai_opt_api-1.0.2/src/qpiai_opt/wrappers/__init__.py
--rw-rw-r--   0 akshat    (1005) akshat    (1005)     1798 2024-04-27 12:14:36.000000 qpiai_opt_api-1.0.2/src/qpiai_opt/wrappers/dwave.py
--rw-rw-r--   0 akshat    (1005) akshat    (1005)     1932 2024-04-27 12:14:36.000000 qpiai_opt_api-1.0.2/src/qpiai_opt/wrappers/qiskit.py
-drwxrwxr-x   0 akshat    (1005) akshat    (1005)        0 2024-04-27 12:15:57.965112 qpiai_opt_api-1.0.2/src/qpiai_opt_api.egg-info/
--rw-r--r--   0 akshat    (1005) akshat    (1005)     3484 2024-04-27 12:15:57.000000 qpiai_opt_api-1.0.2/src/qpiai_opt_api.egg-info/PKG-INFO
--rw-rw-r--   0 akshat    (1005) akshat    (1005)      621 2024-04-27 12:15:57.000000 qpiai_opt_api-1.0.2/src/qpiai_opt_api.egg-info/SOURCES.txt
--rw-rw-r--   0 akshat    (1005) akshat    (1005)        1 2024-04-27 12:15:57.000000 qpiai_opt_api-1.0.2/src/qpiai_opt_api.egg-info/dependency_links.txt
--rw-rw-r--   0 akshat    (1005) akshat    (1005)       10 2024-04-27 12:15:57.000000 qpiai_opt_api-1.0.2/src/qpiai_opt_api.egg-info/top_level.txt
+drwxrwxr-x   0 akshat    (1005) akshat    (1005)        0 2024-05-13 16:11:33.788771 qpiai_opt_api-1.0.3/
+-rw-rw-r--   0 akshat    (1005) akshat    (1005)     1099 2024-04-27 12:14:36.000000 qpiai_opt_api-1.0.3/LICENSE.txt
+-rw-r--r--   0 akshat    (1005) akshat    (1005)     3484 2024-05-13 16:11:33.788771 qpiai_opt_api-1.0.3/PKG-INFO
+-rw-rw-r--   0 akshat    (1005) akshat    (1005)     1709 2024-04-27 12:14:36.000000 qpiai_opt_api-1.0.3/README.md
+-rw-rw-r--   0 akshat    (1005) akshat    (1005)       84 2024-04-27 12:14:36.000000 qpiai_opt_api-1.0.3/pyproject.toml
+-rw-rw-r--   0 akshat    (1005) akshat    (1005)      796 2024-05-13 16:11:33.788771 qpiai_opt_api-1.0.3/setup.cfg
+drwxrwxr-x   0 akshat    (1005) akshat    (1005)        0 2024-05-13 16:11:33.784771 qpiai_opt_api-1.0.3/src/
+drwxrwxr-x   0 akshat    (1005) akshat    (1005)        0 2024-05-13 16:11:33.784771 qpiai_opt_api-1.0.3/src/qpiai_opt/
+-rw-rw-r--   0 akshat    (1005) akshat    (1005)        0 2024-04-27 12:14:36.000000 qpiai_opt_api-1.0.3/src/qpiai_opt/__init__.py
+drwxrwxr-x   0 akshat    (1005) akshat    (1005)        0 2024-05-13 16:11:33.784771 qpiai_opt_api-1.0.3/src/qpiai_opt/problem/
+-rw-rw-r--   0 akshat    (1005) akshat    (1005)      319 2024-04-27 12:14:36.000000 qpiai_opt_api-1.0.3/src/qpiai_opt/problem/__init__.py
+-rw-rw-r--   0 akshat    (1005) akshat    (1005)     1187 2024-04-27 12:14:36.000000 qpiai_opt_api-1.0.3/src/qpiai_opt/problem/max_cut.py
+-rw-rw-r--   0 akshat    (1005) akshat    (1005)     1006 2024-04-27 12:14:36.000000 qpiai_opt_api-1.0.3/src/qpiai_opt/problem/max_independet_set.py
+-rw-rw-r--   0 akshat    (1005) akshat    (1005)      895 2024-04-27 12:14:36.000000 qpiai_opt_api-1.0.3/src/qpiai_opt/problem/number_partition.py
+-rw-rw-r--   0 akshat    (1005) akshat    (1005)      807 2024-04-27 12:14:36.000000 qpiai_opt_api-1.0.3/src/qpiai_opt/problem/qubo.py
+-rw-rw-r--   0 akshat    (1005) akshat    (1005)      964 2024-04-27 12:14:36.000000 qpiai_opt_api-1.0.3/src/qpiai_opt/problem/vertex_cover.py
+drwxrwxr-x   0 akshat    (1005) akshat    (1005)        0 2024-05-13 16:11:33.784771 qpiai_opt_api-1.0.3/src/qpiai_opt/solver/
+-rw-rw-r--   0 akshat    (1005) akshat    (1005)       43 2024-04-27 12:14:36.000000 qpiai_opt_api-1.0.3/src/qpiai_opt/solver/__init__.py
+-rw-rw-r--   0 akshat    (1005) akshat    (1005)     4171 2024-05-13 15:22:57.000000 qpiai_opt_api-1.0.3/src/qpiai_opt/solver/solver.py
+drwxrwxr-x   0 akshat    (1005) akshat    (1005)        0 2024-05-13 16:11:33.788771 qpiai_opt_api-1.0.3/src/qpiai_opt/wrappers/
+-rw-rw-r--   0 akshat    (1005) akshat    (1005)       98 2024-04-27 12:14:36.000000 qpiai_opt_api-1.0.3/src/qpiai_opt/wrappers/__init__.py
+-rw-rw-r--   0 akshat    (1005) akshat    (1005)     1798 2024-04-27 12:14:36.000000 qpiai_opt_api-1.0.3/src/qpiai_opt/wrappers/dwave.py
+-rw-rw-r--   0 akshat    (1005) akshat    (1005)     1932 2024-04-27 12:14:36.000000 qpiai_opt_api-1.0.3/src/qpiai_opt/wrappers/qiskit.py
+drwxrwxr-x   0 akshat    (1005) akshat    (1005)        0 2024-05-13 16:11:33.788771 qpiai_opt_api-1.0.3/src/qpiai_opt_api.egg-info/
+-rw-r--r--   0 akshat    (1005) akshat    (1005)     3484 2024-05-13 16:11:33.000000 qpiai_opt_api-1.0.3/src/qpiai_opt_api.egg-info/PKG-INFO
+-rw-rw-r--   0 akshat    (1005) akshat    (1005)      621 2024-05-13 16:11:33.000000 qpiai_opt_api-1.0.3/src/qpiai_opt_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 akshat    (1005) akshat    (1005)        1 2024-05-13 16:11:33.000000 qpiai_opt_api-1.0.3/src/qpiai_opt_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 akshat    (1005) akshat    (1005)       10 2024-05-13 16:11:33.000000 qpiai_opt_api-1.0.3/src/qpiai_opt_api.egg-info/top_level.txt
```

### Comparing `qpiai_opt_api-1.0.2/LICENSE.txt` & `qpiai_opt_api-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qpiai_opt_api-1.0.2/PKG-INFO` & `qpiai_opt_api-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qpiai-opt-api
-Version: 1.0.2
+Version: 1.0.3
 Summary: QpiAI-Opt-API is a an interface python package to access QpiAI-Opt solvers on cloud
 Home-page: https://gitlab.qpiai.tech/qpiquantum/optimisation/qpiai-opt-api/
 Author: Sagar B Dollin
 Project-URL: Bug Tracker, https://gitlab.qpiai.tech/qpiquantum/optimisation/qpiai-opt-api/-/issues
 Project-URL: repository, https://gitlab.qpiai.tech/qpiquantum/optimisation/qpiai-opt-api/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `qpiai_opt_api-1.0.2/README.md` & `qpiai_opt_api-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `qpiai_opt_api-1.0.2/setup.cfg` & `qpiai_opt_api-1.0.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = qpiai-opt-api
-version = 1.0.2
+version = 1.0.3
 author = Sagar B Dollin
 description = QpiAI-Opt-API is a an interface python package to access QpiAI-Opt solvers on cloud
 long_description = file: README.md, LICENSE.txt
 long_description_content_type = text/markdown
 url = https://gitlab.qpiai.tech/qpiquantum/optimisation/qpiai-opt-api/
 project_urls = 
 	Bug Tracker = https://gitlab.qpiai.tech/qpiquantum/optimisation/qpiai-opt-api/-/issues
```

### Comparing `qpiai_opt_api-1.0.2/src/qpiai_opt/problem/max_cut.py` & `qpiai_opt_api-1.0.3/src/qpiai_opt/problem/max_cut.py`

 * *Files identical despite different names*

### Comparing `qpiai_opt_api-1.0.2/src/qpiai_opt/problem/max_independet_set.py` & `qpiai_opt_api-1.0.3/src/qpiai_opt/problem/max_independet_set.py`

 * *Files identical despite different names*

### Comparing `qpiai_opt_api-1.0.2/src/qpiai_opt/problem/number_partition.py` & `qpiai_opt_api-1.0.3/src/qpiai_opt/problem/number_partition.py`

 * *Files identical despite different names*

### Comparing `qpiai_opt_api-1.0.2/src/qpiai_opt/problem/qubo.py` & `qpiai_opt_api-1.0.3/src/qpiai_opt/problem/qubo.py`

 * *Files identical despite different names*

### Comparing `qpiai_opt_api-1.0.2/src/qpiai_opt/problem/vertex_cover.py` & `qpiai_opt_api-1.0.3/src/qpiai_opt/problem/vertex_cover.py`

 * *Files identical despite different names*

### Comparing `qpiai_opt_api-1.0.2/src/qpiai_opt/wrappers/dwave.py` & `qpiai_opt_api-1.0.3/src/qpiai_opt/wrappers/dwave.py`

 * *Files identical despite different names*

### Comparing `qpiai_opt_api-1.0.2/src/qpiai_opt/wrappers/qiskit.py` & `qpiai_opt_api-1.0.3/src/qpiai_opt/wrappers/qiskit.py`

 * *Files identical despite different names*

### Comparing `qpiai_opt_api-1.0.2/src/qpiai_opt_api.egg-info/PKG-INFO` & `qpiai_opt_api-1.0.3/src/qpiai_opt_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qpiai-opt-api
-Version: 1.0.2
+Version: 1.0.3
 Summary: QpiAI-Opt-API is a an interface python package to access QpiAI-Opt solvers on cloud
 Home-page: https://gitlab.qpiai.tech/qpiquantum/optimisation/qpiai-opt-api/
 Author: Sagar B Dollin
 Project-URL: Bug Tracker, https://gitlab.qpiai.tech/qpiquantum/optimisation/qpiai-opt-api/-/issues
 Project-URL: repository, https://gitlab.qpiai.tech/qpiquantum/optimisation/qpiai-opt-api/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `qpiai_opt_api-1.0.2/src/qpiai_opt_api.egg-info/SOURCES.txt` & `qpiai_opt_api-1.0.3/src/qpiai_opt_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

