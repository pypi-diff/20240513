# Comparing `tmp/PyStratum-Backend-1.0.2.tar.gz` & `tmp/pystratum_backend-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PyStratum-Backend-1.0.2.tar", last modified: Mon Oct 26 10:20:29 2020, max compression
+gzip compressed data, was "pystratum_backend-2.0.0.tar", last modified: Mon May 13 05:30:10 2024, max compression
```

## Comparing `PyStratum-Backend-1.0.2.tar` & `pystratum_backend-2.0.0.tar`

### file list

```diff
@@ -1,18 +1,12 @@
-drwxrwxr-x   0 water     (1000) water     (1000)        0 2020-10-26 10:20:29.275184 PyStratum-Backend-1.0.2/
--rw-rw-r--   0 water     (1000) water     (1000)     4106 2020-10-26 10:20:29.275184 PyStratum-Backend-1.0.2/PKG-INFO
-drwxrwxr-x   0 water     (1000) water     (1000)        0 2020-10-26 10:20:29.274183 PyStratum-Backend-1.0.2/PyStratum_Backend.egg-info/
--rw-rw-r--   0 water     (1000) water     (1000)     4106 2020-10-26 10:20:29.000000 PyStratum-Backend-1.0.2/PyStratum_Backend.egg-info/PKG-INFO
--rw-rw-r--   0 water     (1000) water     (1000)      444 2020-10-26 10:20:29.000000 PyStratum-Backend-1.0.2/PyStratum_Backend.egg-info/SOURCES.txt
--rw-rw-r--   0 water     (1000) water     (1000)        1 2020-10-26 10:20:29.000000 PyStratum-Backend-1.0.2/PyStratum_Backend.egg-info/dependency_links.txt
--rw-rw-r--   0 water     (1000) water     (1000)       12 2020-10-26 10:20:29.000000 PyStratum-Backend-1.0.2/PyStratum_Backend.egg-info/requires.txt
--rw-rw-r--   0 water     (1000) water     (1000)       18 2020-10-26 10:20:29.000000 PyStratum-Backend-1.0.2/PyStratum_Backend.egg-info/top_level.txt
--rw-rw-r--   0 water     (1000) water     (1000)     3114 2020-10-15 09:33:05.000000 PyStratum-Backend-1.0.2/README.rst
-drwxrwxr-x   0 water     (1000) water     (1000)        0 2020-10-26 10:20:29.275184 PyStratum-Backend-1.0.2/pystratum_backend/
--rw-rw-r--   0 water     (1000) water     (1000)     2299 2020-08-23 04:21:36.000000 PyStratum-Backend-1.0.2/pystratum_backend/Backend.py
--rw-rw-r--   0 water     (1000) water     (1000)      616 2020-08-23 04:21:36.000000 PyStratum-Backend-1.0.2/pystratum_backend/ConstantWorker.py
--rw-rw-r--   0 water     (1000) water     (1000)      872 2020-08-23 04:23:06.000000 PyStratum-Backend-1.0.2/pystratum_backend/RoutineLoaderWorker.py
--rw-rw-r--   0 water     (1000) water     (1000)      665 2020-08-23 05:39:26.000000 PyStratum-Backend-1.0.2/pystratum_backend/RoutineWrapperGeneratorWorker.py
--rw-rw-r--   0 water     (1000) water     (1000)     2965 2020-09-10 05:33:30.000000 PyStratum-Backend-1.0.2/pystratum_backend/StratumStyle.py
--rw-rw-r--   0 water     (1000) water     (1000)        0 2016-09-27 15:36:45.000000 PyStratum-Backend-1.0.2/pystratum_backend/__init__.py
--rw-rw-r--   0 water     (1000) water     (1000)       38 2020-10-26 10:20:29.275184 PyStratum-Backend-1.0.2/setup.cfg
--rw-rw-r--   0 water     (1000) water     (1000)     1203 2020-10-26 10:20:19.000000 PyStratum-Backend-1.0.2/setup.py
+-rw-r--r--   0        0        0     1091 2020-08-23 05:34:30.000000 pystratum_backend-2.0.0/LICENSE.md
+-rw-r--r--   0        0        0     3114 2020-10-15 09:33:05.000000 pystratum_backend-2.0.0/README.rst
+-rw-r--r--   0        0        0     1094 2024-05-13 05:30:10.224010 pystratum_backend-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2070 2024-05-12 08:46:46.824319 pystratum_backend-2.0.0/pystratum_backend/Backend.py
+-rw-r--r--   0        0        0      596 2024-05-12 16:02:37.455296 pystratum_backend-2.0.0/pystratum_backend/ConstantWorker.py
+-rw-r--r--   0        0        0     4930 2024-05-12 15:15:31.152588 pystratum_backend-2.0.0/pystratum_backend/Helper/Terminal.py
+-rw-r--r--   0        0        0        0 2024-05-12 15:09:47.603196 pystratum_backend-2.0.0/pystratum_backend/Helper/__init__.py
+-rw-r--r--   0        0        0      798 2024-05-12 16:02:37.459296 pystratum_backend-2.0.0/pystratum_backend/RoutineLoaderWorker.py
+-rw-r--r--   0        0        0      645 2024-05-12 08:40:14.422898 pystratum_backend-2.0.0/pystratum_backend/RoutineWrapperGeneratorWorker.py
+-rw-r--r--   0        0        0     6114 2024-05-12 16:02:37.269292 pystratum_backend-2.0.0/pystratum_backend/StratumIO.py
+-rw-r--r--   0        0        0        0 2016-09-27 15:36:45.000000 pystratum_backend-2.0.0/pystratum_backend/__init__.py
+-rw-r--r--   0        0        0     4064 1970-01-01 00:00:00.000000 pystratum_backend-2.0.0/PKG-INFO
```

### Comparing `PyStratum-Backend-1.0.2/PKG-INFO` & `pystratum_backend-2.0.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,43 +1,46 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: PyStratum-Backend
-Version: 1.0.2
+Version: 2.0.0
 Summary: PyStratum Backend: The glue between PyStratum and backends for RDBMS
-Home-page: https://github.com/DatabaseStratum/py-stratum-backend
-Author: Set Based IT Consultancy
-Author-email: info@setbased.nl
-License: MIT
-Description: PyStratum Backend
-        =================
-        The glue between PyStratum and backends for database systems.
-        
-        +-----------------------------------------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------+--------------------------------------------------------------------------------------------------------------+
-        | Social                                                                                                                      | Release                                                                                            | Code                                                                                                         |
-        +=============================================================================================================================+====================================================================================================+==============================================================================================================+
-        | .. image:: https://badges.gitter.im/SetBased/py-stratum.svg                                                                 | .. image:: https://badge.fury.io/py/PyStratum-Backend.svg                                          | .. image:: https://scrutinizer-ci.com/g/DatabaseStratum/py-stratum-backend/badges/quality-score.png?b=master |
-        |   :target: https://gitter.im/SetBased/py-stratum?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge  |   :target: https://badge.fury.io/py/PyStratum-Backend                                              |   :target: https://scrutinizer-ci.com/g/DatabaseStratum/py-stratum-backend/?branch=master                    |
-        |                                                                                                                             |                                                                                                    |                                                                                                              |
-        |                                                                                                                             |                                                                                                    |                                                                                                              |
-        +-----------------------------------------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------+--------------------------------------------------------------------------------------------------------------+
-        
-        Overview
-        ========
-        PyStratum is a tool and library for loading and invoking stored procedures from Python code.
-        
-        The documentation of PyStratum is available at https://stratum.readthedocs.io/.
-        
-        License
-        =======
-        
-        This project is licensed under the terms of the MIT license.
-        
 Keywords: PyStratum,Backend
-Platform: UNKNOWN
+Author-Email: Set Based IT Consultancy <info@setbased.nl>
+License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: Topic :: Software Development :: Code Generators
-Classifier: Topic :: System :: Installation/Setup
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: Topic :: Software Development :: Code Generators
+Classifier: Topic :: System :: Installation/Setup
+Project-URL: Homepage, https://github.com/DatabaseStratum/py-stratum-backend
+Requires-Python: >=3.9
+Requires-Dist: cleo~=2.0.1
+Description-Content-Type: text/x-rst
+
+PyStratum Backend
+=================
+The glue between PyStratum and backends for database systems.
+
++-----------------------------------------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------+--------------------------------------------------------------------------------------------------------------+
+| Social                                                                                                                      | Release                                                                                            | Code                                                                                                         |
++=============================================================================================================================+====================================================================================================+==============================================================================================================+
+| .. image:: https://badges.gitter.im/SetBased/py-stratum.svg                                                                 | .. image:: https://badge.fury.io/py/PyStratum-Backend.svg                                          | .. image:: https://scrutinizer-ci.com/g/DatabaseStratum/py-stratum-backend/badges/quality-score.png?b=master |
+|   :target: https://gitter.im/SetBased/py-stratum?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge  |   :target: https://badge.fury.io/py/PyStratum-Backend                                              |   :target: https://scrutinizer-ci.com/g/DatabaseStratum/py-stratum-backend/?branch=master                    |
+|                                                                                                                             |                                                                                                    |                                                                                                              |
+|                                                                                                                             |                                                                                                    |                                                                                                              |
++-----------------------------------------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------+--------------------------------------------------------------------------------------------------------------+
+
+Overview
+========
+PyStratum is a tool and library for loading and invoking stored procedures from Python code.
+
+The documentation of PyStratum is available at https://stratum.readthedocs.io/.
+
+License
+=======
+
+This project is licensed under the terms of the MIT license.
```

### Comparing `PyStratum-Backend-1.0.2/README.rst` & `pystratum_backend-2.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `PyStratum-Backend-1.0.2/pystratum_backend/Backend.py` & `pystratum_backend-2.0.0/pystratum_backend/Backend.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,52 +1,46 @@
 from configparser import ConfigParser
 from typing import Optional
 
 from pystratum_backend.ConstantWorker import ConstantWorker
 from pystratum_backend.RoutineLoaderWorker import RoutineLoaderWorker
 from pystratum_backend.RoutineWrapperGeneratorWorker import RoutineWrapperGeneratorWorker
-from pystratum_backend.StratumStyle import StratumStyle
+from pystratum_backend.StratumIO import StratumIO
 
 
 class Backend:
     """
     Semi interface for PyStratum's backends.
     """
 
     # ------------------------------------------------------------------------------------------------------------------
-    def create_constant_worker(self, settings: ConfigParser, io: StratumStyle) -> Optional[ConstantWorker]:
+    def create_constant_worker(self, settings: ConfigParser, io: StratumIO) -> Optional[ConstantWorker]:
         """
         Creates the object that does the actual execution of the constant command for the backend.
 
-        :param ConfigParser settings: The settings from the PyStratum configuration file.
-        :param StratumStyle io: The output object.
-
-        :rtype: ConstantWorker|None
+        :param settings: The settings from the PyStratum configuration file.
+        :param io: The output object.
         """
         return None
 
     # ------------------------------------------------------------------------------------------------------------------
-    def create_routine_loader_worker(self, settings: ConfigParser, io: StratumStyle) -> Optional[RoutineLoaderWorker]:
+    def create_routine_loader_worker(self, settings: ConfigParser, io: StratumIO) -> Optional[RoutineLoaderWorker]:
         """
         Creates the object that does the actual execution of the routine loader command for the backend.
 
-        :param ConfigParser settings: The settings from the PyStratum configuration file.
-        :param StratumStyle io: The output object.
-
-        :rtype: RoutineLoaderWorker|None
+        :param settings: The settings from the PyStratum configuration file.
+        :param io: The output object.
         """
         return None
 
     # ------------------------------------------------------------------------------------------------------------------
-    def create_routine_wrapper_generator_worker(self, settings: ConfigParser, io: StratumStyle) \
-            -> Optional[RoutineWrapperGeneratorWorker]:
+    def create_routine_wrapper_generator_worker(self, settings: ConfigParser, io: StratumIO) -> Optional[
+        RoutineWrapperGeneratorWorker]:
         """
         Creates the object that does the actual execution of the routine wrapper generator command for the backend.
 
-        :param ConfigParser settings: The settings from the PyStratum configuration file.
-        :param StratumStyle io: The output object.
-
-        :rtype: RoutineWrapperGeneratorWorker|None
+        :param settings: The settings from the PyStratum configuration file.
+        :param io: The output object.
         """
         return None
 
 # ----------------------------------------------------------------------------------------------------------------------
```

### Comparing `PyStratum-Backend-1.0.2/pystratum_backend/ConstantWorker.py` & `pystratum_backend-2.0.0/pystratum_backend/ConstantWorker.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,13 @@
     """
     Interface for classes that implement the actual execution of the constant command.
     """
 
     # ------------------------------------------------------------------------------------------------------------------
     def execute(self) -> int:
         """
-        Does the actual execution of the constant command for the backend. Returns 0 on success. Otherwise returns
+        Does the actual execution of the constant command for the backend. Returns 0 on success. Otherwise, returns
         nonzero.
-
-        :rtype: int
         """
         pass
 
 # ----------------------------------------------------------------------------------------------------------------------
```

### Comparing `PyStratum-Backend-1.0.2/pystratum_backend/RoutineLoaderWorker.py` & `pystratum_backend-2.0.0/pystratum_backend/RoutineLoaderWorker.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,18 +6,15 @@
     """
     Interface for classes that implement the actual execution of the routine loader command.
     """
 
     # ------------------------------------------------------------------------------------------------------------------
     def execute(self, file_names: Optional[List[str]] = None) -> int:
         """
-        Does the actual execution of the routine loader command for the backend. Returns 0 on success. Otherwise
+        Does the actual execution of the routine loader command for the backend. Returns 0 on success. Otherwise,
         returns nonzero.
 
-        :param list[str]|None file_names: The sources that must be loaded. If none all sources (if required) will
-                                          loaded.
-
-        :rtype: int
+        :param file_names: The sources that must be loaded. If None all sources (if required) will be loaded.
         """
         pass
 
 # ----------------------------------------------------------------------------------------------------------------------
```

