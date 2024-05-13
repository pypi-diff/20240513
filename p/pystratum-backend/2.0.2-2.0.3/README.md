# Comparing `tmp/pystratum_backend-2.0.2.tar.gz` & `tmp/pystratum_backend-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pystratum_backend-2.0.2.tar", last modified: Mon May 13 10:43:27 2024, max compression
+gzip compressed data, was "pystratum_backend-2.0.3.tar", last modified: Mon May 13 12:37:42 2024, max compression
```

## Comparing `pystratum_backend-2.0.2.tar` & `pystratum_backend-2.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1091 2020-08-23 05:34:30.000000 pystratum_backend-2.0.2/LICENSE.md
--rw-r--r--   0        0        0     3114 2020-10-15 09:33:05.000000 pystratum_backend-2.0.2/README.rst
--rw-r--r--   0        0        0     1094 2024-05-13 10:43:27.133279 pystratum_backend-2.0.2/pyproject.toml
--rw-r--r--   0        0        0     2070 2024-05-12 08:46:46.824319 pystratum_backend-2.0.2/pystratum_backend/Backend.py
--rw-r--r--   0        0        0      596 2024-05-12 16:02:37.455296 pystratum_backend-2.0.2/pystratum_backend/ConstantWorker.py
--rw-r--r--   0        0        0     4930 2024-05-12 15:15:31.152588 pystratum_backend-2.0.2/pystratum_backend/Helper/Terminal.py
--rw-r--r--   0        0        0        0 2024-05-12 15:09:47.603196 pystratum_backend-2.0.2/pystratum_backend/Helper/__init__.py
--rw-r--r--   0        0        0      798 2024-05-12 16:02:37.459296 pystratum_backend-2.0.2/pystratum_backend/RoutineLoaderWorker.py
--rw-r--r--   0        0        0      645 2024-05-12 08:40:14.422898 pystratum_backend-2.0.2/pystratum_backend/RoutineWrapperGeneratorWorker.py
--rw-r--r--   0        0        0     6139 2024-05-13 10:41:46.699079 pystratum_backend-2.0.2/pystratum_backend/StratumIO.py
--rw-r--r--   0        0        0        0 2016-09-27 15:36:45.000000 pystratum_backend-2.0.2/pystratum_backend/__init__.py
--rw-r--r--   0        0        0     4064 1970-01-01 00:00:00.000000 pystratum_backend-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1091 2020-08-23 05:34:30.000000 pystratum_backend-2.0.3/LICENSE.md
+-rw-r--r--   0        0        0     3114 2020-10-15 09:33:05.000000 pystratum_backend-2.0.3/README.rst
+-rw-r--r--   0        0        0     1198 2024-05-13 12:37:42.560685 pystratum_backend-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2070 2024-05-12 08:46:46.824319 pystratum_backend-2.0.3/pystratum_backend/Backend.py
+-rw-r--r--   0        0        0      596 2024-05-12 16:02:37.455296 pystratum_backend-2.0.3/pystratum_backend/ConstantWorker.py
+-rw-r--r--   0        0        0     4930 2024-05-12 15:15:31.152588 pystratum_backend-2.0.3/pystratum_backend/Helper/Terminal.py
+-rw-r--r--   0        0        0        0 2024-05-12 15:09:47.603196 pystratum_backend-2.0.3/pystratum_backend/Helper/__init__.py
+-rw-r--r--   0        0        0      798 2024-05-12 16:02:37.459296 pystratum_backend-2.0.3/pystratum_backend/RoutineLoaderWorker.py
+-rw-r--r--   0        0        0      645 2024-05-12 08:40:14.422898 pystratum_backend-2.0.3/pystratum_backend/RoutineWrapperGeneratorWorker.py
+-rw-r--r--   0        0        0     6139 2024-05-13 10:41:46.699079 pystratum_backend-2.0.3/pystratum_backend/StratumIO.py
+-rw-r--r--   0        0        0        0 2016-09-27 15:36:45.000000 pystratum_backend-2.0.3/pystratum_backend/__init__.py
+-rw-r--r--   0        0        0     4190 1970-01-01 00:00:00.000000 pystratum_backend-2.0.3/PKG-INFO
```

### Comparing `pystratum_backend-2.0.2/LICENSE.md` & `pystratum_backend-2.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pystratum_backend-2.0.2/README.rst` & `pystratum_backend-2.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `pystratum_backend-2.0.2/pyproject.toml` & `pystratum_backend-2.0.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "PyStratum-Backend"
-version = "2.0.2"
+version = "2.0.3"
 description = "PyStratum Backend: The glue between PyStratum and backends for RDBMS"
 keywords = [
     "PyStratum",
     "Backend",
 ]
 readme = "README.rst"
 authors = [
@@ -20,24 +20,30 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Topic :: Software Development :: Build Tools",
     "Topic :: Software Development :: Code Generators",
     "Topic :: System :: Installation/Setup",
 ]
 dependencies = [
-    "cleo~=2.0.1",
+    "cleo>=2.0.1, ==2.*",
 ]
 requires-python = ">=3.9"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://github.com/DatabaseStratum/py-stratum-backend"
 
+[project.optional-dependencies]
+dev = [
+    "build>=1.2.1, ==1.*",
+    "twine>=5.0.0, ==5.*",
+]
+
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [tool]
```

### Comparing `pystratum_backend-2.0.2/pystratum_backend/Backend.py` & `pystratum_backend-2.0.3/pystratum_backend/Backend.py`

 * *Files identical despite different names*

### Comparing `pystratum_backend-2.0.2/pystratum_backend/ConstantWorker.py` & `pystratum_backend-2.0.3/pystratum_backend/ConstantWorker.py`

 * *Files identical despite different names*

### Comparing `pystratum_backend-2.0.2/pystratum_backend/Helper/Terminal.py` & `pystratum_backend-2.0.3/pystratum_backend/Helper/Terminal.py`

 * *Files identical despite different names*

### Comparing `pystratum_backend-2.0.2/pystratum_backend/RoutineLoaderWorker.py` & `pystratum_backend-2.0.3/pystratum_backend/RoutineLoaderWorker.py`

 * *Files identical despite different names*

### Comparing `pystratum_backend-2.0.2/pystratum_backend/RoutineWrapperGeneratorWorker.py` & `pystratum_backend-2.0.3/pystratum_backend/RoutineWrapperGeneratorWorker.py`

 * *Files identical despite different names*

### Comparing `pystratum_backend-2.0.2/pystratum_backend/StratumIO.py` & `pystratum_backend-2.0.3/pystratum_backend/StratumIO.py`

 * *Files identical despite different names*

### Comparing `pystratum_backend-2.0.2/PKG-INFO` & `pystratum_backend-2.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyStratum-Backend
-Version: 2.0.2
+Version: 2.0.3
 Summary: PyStratum Backend: The glue between PyStratum and backends for RDBMS
 Keywords: PyStratum,Backend
 Author-Email: Set Based IT Consultancy <info@setbased.nl>
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -14,15 +14,18 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: System :: Installation/Setup
 Project-URL: Homepage, https://github.com/DatabaseStratum/py-stratum-backend
 Requires-Python: >=3.9
-Requires-Dist: cleo~=2.0.1
+Requires-Dist: cleo==2.*,>=2.0.1
+Requires-Dist: build==1.*,>=1.2.1; extra == "dev"
+Requires-Dist: twine==5.*,>=5.0.0; extra == "dev"
+Provides-Extra: dev
 Description-Content-Type: text/x-rst
 
 PyStratum Backend
 =================
 The glue between PyStratum and backends for database systems.
 
 +-----------------------------------------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------+--------------------------------------------------------------------------------------------------------------+
```

