# Comparing `tmp/pystratum_backend-2.0.1.tar.gz` & `tmp/pystratum_backend-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pystratum_backend-2.0.1.tar", last modified: Mon May 13 05:59:17 2024, max compression
+gzip compressed data, was "pystratum_backend-2.0.2.tar", last modified: Mon May 13 10:43:27 2024, max compression
```

## Comparing `pystratum_backend-2.0.1.tar` & `pystratum_backend-2.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1091 2020-08-23 05:34:30.000000 pystratum_backend-2.0.1/LICENSE.md
--rw-r--r--   0        0        0     3114 2020-10-15 09:33:05.000000 pystratum_backend-2.0.1/README.rst
--rw-r--r--   0        0        0     1094 2024-05-13 05:59:17.148007 pystratum_backend-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     2070 2024-05-12 08:46:46.824319 pystratum_backend-2.0.1/pystratum_backend/Backend.py
--rw-r--r--   0        0        0      596 2024-05-12 16:02:37.455296 pystratum_backend-2.0.1/pystratum_backend/ConstantWorker.py
--rw-r--r--   0        0        0     4930 2024-05-12 15:15:31.152588 pystratum_backend-2.0.1/pystratum_backend/Helper/Terminal.py
--rw-r--r--   0        0        0        0 2024-05-12 15:09:47.603196 pystratum_backend-2.0.1/pystratum_backend/Helper/__init__.py
--rw-r--r--   0        0        0      798 2024-05-12 16:02:37.459296 pystratum_backend-2.0.1/pystratum_backend/RoutineLoaderWorker.py
--rw-r--r--   0        0        0      645 2024-05-12 08:40:14.422898 pystratum_backend-2.0.1/pystratum_backend/RoutineWrapperGeneratorWorker.py
--rw-r--r--   0        0        0     6115 2024-05-13 05:55:40.866324 pystratum_backend-2.0.1/pystratum_backend/StratumIO.py
--rw-r--r--   0        0        0        0 2016-09-27 15:36:45.000000 pystratum_backend-2.0.1/pystratum_backend/__init__.py
--rw-r--r--   0        0        0     4064 1970-01-01 00:00:00.000000 pystratum_backend-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1091 2020-08-23 05:34:30.000000 pystratum_backend-2.0.2/LICENSE.md
+-rw-r--r--   0        0        0     3114 2020-10-15 09:33:05.000000 pystratum_backend-2.0.2/README.rst
+-rw-r--r--   0        0        0     1094 2024-05-13 10:43:27.133279 pystratum_backend-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2070 2024-05-12 08:46:46.824319 pystratum_backend-2.0.2/pystratum_backend/Backend.py
+-rw-r--r--   0        0        0      596 2024-05-12 16:02:37.455296 pystratum_backend-2.0.2/pystratum_backend/ConstantWorker.py
+-rw-r--r--   0        0        0     4930 2024-05-12 15:15:31.152588 pystratum_backend-2.0.2/pystratum_backend/Helper/Terminal.py
+-rw-r--r--   0        0        0        0 2024-05-12 15:09:47.603196 pystratum_backend-2.0.2/pystratum_backend/Helper/__init__.py
+-rw-r--r--   0        0        0      798 2024-05-12 16:02:37.459296 pystratum_backend-2.0.2/pystratum_backend/RoutineLoaderWorker.py
+-rw-r--r--   0        0        0      645 2024-05-12 08:40:14.422898 pystratum_backend-2.0.2/pystratum_backend/RoutineWrapperGeneratorWorker.py
+-rw-r--r--   0        0        0     6139 2024-05-13 10:41:46.699079 pystratum_backend-2.0.2/pystratum_backend/StratumIO.py
+-rw-r--r--   0        0        0        0 2016-09-27 15:36:45.000000 pystratum_backend-2.0.2/pystratum_backend/__init__.py
+-rw-r--r--   0        0        0     4064 1970-01-01 00:00:00.000000 pystratum_backend-2.0.2/PKG-INFO
```

### Comparing `pystratum_backend-2.0.1/LICENSE.md` & `pystratum_backend-2.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pystratum_backend-2.0.1/README.rst` & `pystratum_backend-2.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `pystratum_backend-2.0.1/pyproject.toml` & `pystratum_backend-2.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "PyStratum-Backend"
-version = "2.0.1"
+version = "2.0.2"
 description = "PyStratum Backend: The glue between PyStratum and backends for RDBMS"
 keywords = [
     "PyStratum",
     "Backend",
 ]
 readme = "README.rst"
 authors = [
```

### Comparing `pystratum_backend-2.0.1/pystratum_backend/Backend.py` & `pystratum_backend-2.0.2/pystratum_backend/Backend.py`

 * *Files identical despite different names*

### Comparing `pystratum_backend-2.0.1/pystratum_backend/ConstantWorker.py` & `pystratum_backend-2.0.2/pystratum_backend/ConstantWorker.py`

 * *Files identical despite different names*

### Comparing `pystratum_backend-2.0.1/pystratum_backend/Helper/Terminal.py` & `pystratum_backend-2.0.2/pystratum_backend/Helper/Terminal.py`

 * *Files identical despite different names*

### Comparing `pystratum_backend-2.0.1/pystratum_backend/RoutineLoaderWorker.py` & `pystratum_backend-2.0.2/pystratum_backend/RoutineLoaderWorker.py`

 * *Files identical despite different names*

### Comparing `pystratum_backend-2.0.1/pystratum_backend/RoutineWrapperGeneratorWorker.py` & `pystratum_backend-2.0.2/pystratum_backend/RoutineWrapperGeneratorWorker.py`

 * *Files identical despite different names*

### Comparing `pystratum_backend-2.0.1/pystratum_backend/StratumIO.py` & `pystratum_backend-2.0.2/pystratum_backend/StratumIO.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,25 +88,25 @@
     # ------------------------------------------------------------------------------------------------------------------
     def log_verbose(self, message: Union[str, Iterable[str]]) -> None:
         """
         Logs a message only when logging level is verbose.
 
         :param message: The message or messages.
         """
-        if self._output.verbosity >= Verbosity.VERBOSE:
+        if self._output.verbosity.value >= Verbosity.VERBOSE.value:
             self.text(message)
 
     # ------------------------------------------------------------------------------------------------------------------
     def log_very_verbose(self, messages: Union[str, Iterable[str]]) -> None:
         """
         Logs a message only when logging level is very verbose.
 
         :param messages: The message or messages.
         """
-        if self._output.verbosity >= Verbosity.VERY_VERBOSE:
+        if self._output.verbosity.value >= Verbosity.VERY_VERBOSE.value:
             self.text(messages)
 
     # ------------------------------------------------------------------------------------------------------------------
     def __block(self, block_type: str, messages: Union[str, Iterable[str]]) -> None:
         """
         Writes a block message to the output.
```

### Comparing `pystratum_backend-2.0.1/PKG-INFO` & `pystratum_backend-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyStratum-Backend
-Version: 2.0.1
+Version: 2.0.2
 Summary: PyStratum Backend: The glue between PyStratum and backends for RDBMS
 Keywords: PyStratum,Backend
 Author-Email: Set Based IT Consultancy <info@setbased.nl>
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

