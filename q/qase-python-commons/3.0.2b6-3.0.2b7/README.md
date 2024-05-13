# Comparing `tmp/qase_python_commons-3.0.2b6.tar.gz` & `tmp/qase_python_commons-3.0.2b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qase_python_commons-3.0.2b6.tar", last modified: Fri May 10 08:33:29 2024, max compression
+gzip compressed data, was "qase_python_commons-3.0.2b7.tar", last modified: Mon May 13 15:28:47 2024, max compression
```

## Comparing `qase_python_commons-3.0.2b6.tar` & `qase_python_commons-3.0.2b7.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:33:29.349988 qase_python_commons-3.0.2b6/
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-05-10 08:33:29.345988 qase_python_commons-3.0.2b6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-10 08:33:22.000000 qase_python_commons-3.0.2b6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-05-10 08:33:22.000000 qase_python_commons-3.0.2b6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 08:33:29.349988 qase_python_commons-3.0.2b6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:33:29.341988 qase_python_commons-3.0.2b6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:33:29.337988 qase_python_commons-3.0.2b6/src/qase/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:33:29.341988 qase_python_commons-3.0.2b6/src/qase/commons/
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-10 08:33:22.000000 qase_python_commons-3.0.2b6/src/qase/commons/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:33:29.341988 qase_python_commons-3.0.2b6/src/qase/commons/client/
--rw-r--r--   0 runner    (1001) docker     (127)    10934 2024-05-10 08:33:22.000000 qase_python_commons-3.0.2b6/src/qase/commons/client/api_v1_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7043 2024-05-10 08:33:22.000000 qase_python_commons-3.0.2b6/src/qase/commons/client/api_v2_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-05-10 08:33:22.000000 qase_python_commons-3.0.2b6/src/qase/commons/client/base_api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-05-10 08:33:22.000000 qase_python_commons-3.0.2b6/src/qase/commons/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:33:29.341988 qase_python_commons-3.0.2b6/src/qase/commons/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-10 08:33:22.000000 qase_python_commons-3.0.2b6/src/qase/commons/exceptions/reporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-10 08:33:22.000000 qase_python_commons-3.0.2b6/src/qase/commons/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)      980 2024-05-10 08:33:22.000000 qase_python_commons-3.0.2b6/src/qase/commons/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:33:29.345988 qase_python_commons-3.0.2b6/src/qase/commons/models/
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-10 08:33:22.000000 qase_python_commons-3.0.2b6/src/qase/commons/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-10 08:33:22.000000 qase_python_commons-3.0.2b6/src/qase/commons/models/attachment.py
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-10 08:33:22.000000 qase_python_commons-3.0.2b6/src/qase/commons/models/basemodel.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-10 08:33:22.000000 qase_python_commons-3.0.2b6/src/qase/commons/models/relation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-05-10 08:33:22.000000 qase_python_commons-3.0.2b6/src/qase/commons/models/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-05-10 08:33:22.000000 qase_python_commons-3.0.2b6/src/qase/commons/models/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-10 08:33:22.000000 qase_python_commons-3.0.2b6/src/qase/commons/models/runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-05-10 08:33:22.000000 qase_python_commons-3.0.2b6/src/qase/commons/models/step.py
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-10 08:33:22.000000 qase_python_commons-3.0.2b6/src/qase/commons/models/suite.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:33:29.345988 qase_python_commons-3.0.2b6/src/qase/commons/profilers/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-10 08:33:22.000000 qase_python_commons-3.0.2b6/src/qase/commons/profilers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-10 08:33:22.000000 qase_python_commons-3.0.2b6/src/qase/commons/profilers/db.py
--rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-05-10 08:33:22.000000 qase_python_commons-3.0.2b6/src/qase/commons/profilers/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-10 08:33:22.000000 qase_python_commons-3.0.2b6/src/qase/commons/profilers/sleep.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:33:29.345988 qase_python_commons-3.0.2b6/src/qase/commons/reporters/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-10 08:33:22.000000 qase_python_commons-3.0.2b6/src/qase/commons/reporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7904 2024-05-10 08:33:22.000000 qase_python_commons-3.0.2b6/src/qase/commons/reporters/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     4543 2024-05-10 08:33:22.000000 qase_python_commons-3.0.2b6/src/qase/commons/reporters/report.py
--rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-05-10 08:33:22.000000 qase_python_commons-3.0.2b6/src/qase/commons/reporters/testops.py
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-05-10 08:33:22.000000 qase_python_commons-3.0.2b6/src/qase/commons/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:33:29.345988 qase_python_commons-3.0.2b6/src/qase/commons/validators/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-10 08:33:22.000000 qase_python_commons-3.0.2b6/src/qase/commons/validators/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:33:29.345988 qase_python_commons-3.0.2b6/src/qase_python_commons.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-05-10 08:33:29.000000 qase_python_commons-3.0.2b6/src/qase_python_commons.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-10 08:33:29.000000 qase_python_commons-3.0.2b6/src/qase_python_commons.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 08:33:29.000000 qase_python_commons-3.0.2b6/src/qase_python_commons.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-10 08:33:29.000000 qase_python_commons-3.0.2b6/src/qase_python_commons.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-10 08:33:29.000000 qase_python_commons-3.0.2b6/src/qase_python_commons.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:28:47.410839 qase_python_commons-3.0.2b7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-05-13 15:28:47.410839 qase_python_commons-3.0.2b7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-13 15:28:41.000000 qase_python_commons-3.0.2b7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-05-13 15:28:41.000000 qase_python_commons-3.0.2b7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 15:28:47.410839 qase_python_commons-3.0.2b7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:28:47.402839 qase_python_commons-3.0.2b7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:28:47.402839 qase_python_commons-3.0.2b7/src/qase/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:28:47.402839 qase_python_commons-3.0.2b7/src/qase/commons/
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-13 15:28:41.000000 qase_python_commons-3.0.2b7/src/qase/commons/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:28:47.406839 qase_python_commons-3.0.2b7/src/qase/commons/client/
+-rw-r--r--   0 runner    (1001) docker     (127)    11038 2024-05-13 15:28:41.000000 qase_python_commons-3.0.2b7/src/qase/commons/client/api_v1_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7043 2024-05-13 15:28:41.000000 qase_python_commons-3.0.2b7/src/qase/commons/client/api_v2_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-05-13 15:28:41.000000 qase_python_commons-3.0.2b7/src/qase/commons/client/base_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-05-13 15:28:41.000000 qase_python_commons-3.0.2b7/src/qase/commons/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:28:47.406839 qase_python_commons-3.0.2b7/src/qase/commons/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-13 15:28:41.000000 qase_python_commons-3.0.2b7/src/qase/commons/exceptions/reporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-13 15:28:41.000000 qase_python_commons-3.0.2b7/src/qase/commons/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-13 15:28:41.000000 qase_python_commons-3.0.2b7/src/qase/commons/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:28:47.406839 qase_python_commons-3.0.2b7/src/qase/commons/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-13 15:28:41.000000 qase_python_commons-3.0.2b7/src/qase/commons/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-13 15:28:41.000000 qase_python_commons-3.0.2b7/src/qase/commons/models/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-13 15:28:41.000000 qase_python_commons-3.0.2b7/src/qase/commons/models/basemodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-13 15:28:41.000000 qase_python_commons-3.0.2b7/src/qase/commons/models/relation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-05-13 15:28:41.000000 qase_python_commons-3.0.2b7/src/qase/commons/models/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-05-13 15:28:41.000000 qase_python_commons-3.0.2b7/src/qase/commons/models/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-13 15:28:41.000000 qase_python_commons-3.0.2b7/src/qase/commons/models/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-05-13 15:28:41.000000 qase_python_commons-3.0.2b7/src/qase/commons/models/step.py
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-13 15:28:41.000000 qase_python_commons-3.0.2b7/src/qase/commons/models/suite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:28:47.406839 qase_python_commons-3.0.2b7/src/qase/commons/profilers/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-13 15:28:41.000000 qase_python_commons-3.0.2b7/src/qase/commons/profilers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-13 15:28:41.000000 qase_python_commons-3.0.2b7/src/qase/commons/profilers/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-05-13 15:28:41.000000 qase_python_commons-3.0.2b7/src/qase/commons/profilers/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-13 15:28:41.000000 qase_python_commons-3.0.2b7/src/qase/commons/profilers/sleep.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:28:47.406839 qase_python_commons-3.0.2b7/src/qase/commons/reporters/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-13 15:28:41.000000 qase_python_commons-3.0.2b7/src/qase/commons/reporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7904 2024-05-13 15:28:41.000000 qase_python_commons-3.0.2b7/src/qase/commons/reporters/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4543 2024-05-13 15:28:41.000000 qase_python_commons-3.0.2b7/src/qase/commons/reporters/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-05-13 15:28:41.000000 qase_python_commons-3.0.2b7/src/qase/commons/reporters/testops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-05-13 15:28:41.000000 qase_python_commons-3.0.2b7/src/qase/commons/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:28:47.406839 qase_python_commons-3.0.2b7/src/qase/commons/validators/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-13 15:28:41.000000 qase_python_commons-3.0.2b7/src/qase/commons/validators/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:28:47.410839 qase_python_commons-3.0.2b7/src/qase_python_commons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-05-13 15:28:47.000000 qase_python_commons-3.0.2b7/src/qase_python_commons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-13 15:28:47.000000 qase_python_commons-3.0.2b7/src/qase_python_commons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 15:28:47.000000 qase_python_commons-3.0.2b7/src/qase_python_commons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-13 15:28:47.000000 qase_python_commons-3.0.2b7/src/qase_python_commons.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-13 15:28:47.000000 qase_python_commons-3.0.2b7/src/qase_python_commons.egg-info/top_level.txt
```

### Comparing `qase_python_commons-3.0.2b6/PKG-INFO` & `qase_python_commons-3.0.2b7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qase-python-commons
-Version: 3.0.2b6
+Version: 3.0.2b7
 Summary: A library for Qase TestOps and Qase Report
 Author-email: Qase Team <support@qase.io>
 Project-URL: Homepage, https://github.com/qase-tms/qase-python/tree/master/qase-python-commons
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `qase_python_commons-3.0.2b6/pyproject.toml` & `qase_python_commons-3.0.2b7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=68", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qase-python-commons"
-version = "3.0.2b6"
+version = "3.0.2b7"
 description = "A library for Qase TestOps and Qase Report"
 readme = "README.md"
 authors = [{name = "Qase Team", email = "support@qase.io"}]
 license = {file = "LICENSE"}
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python",
```

### Comparing `qase_python_commons-3.0.2b6/src/qase/commons/client/api_v1_client.py` & `qase_python_commons-3.0.2b7/src/qase/commons/client/api_v1_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,14 +198,17 @@
 
         try:
             prepared_step = {"time": step.execution.duration, "status": step.execution.status}
 
             if step.execution.status == 'untested':
                 prepared_step["status"] = 'passed'
 
+            if step.execution.status == 'skipped':
+                prepared_step["status"] = 'blocked'
+
             if step.step_type == StepType.TEXT:
                 prepared_step['action'] = step.data.action
                 if step.data.expected_result:
                     prepared_step['expected_result'] = step.data.expected_result
 
             if step.step_type == StepType.REQUEST:
                 prepared_step['action'] = step.data.request_method + " " + step.data.request_url
```

### Comparing `qase_python_commons-3.0.2b6/src/qase/commons/client/api_v2_client.py` & `qase_python_commons-3.0.2b7/src/qase/commons/client/api_v2_client.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b6/src/qase/commons/client/base_api_client.py` & `qase_python_commons-3.0.2b7/src/qase/commons/client/base_api_client.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b6/src/qase/commons/config.py` & `qase_python_commons-3.0.2b7/src/qase/commons/config.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b6/src/qase/commons/loader.py` & `qase_python_commons-3.0.2b7/src/qase/commons/loader.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b6/src/qase/commons/logger.py` & `qase_python_commons-3.0.2b7/src/qase/commons/logger.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import datetime
 
 import os
 
 
 class Logger:
-    def __init__(self, debug: bool = False, prefix: str = '', dir: str = './logs') -> None:
+    def __init__(self, debug: bool = False, prefix: str = '', dir: str = os.path.join('.', 'logs')) -> None:
         self.debug = debug
         if self.debug:
             filename = f'{prefix}_{self._get_timestamp()}.log'
             if not os.path.exists(dir):
                 os.makedirs(dir)
             self.log_file = os.path.join(dir, f'{filename}')
             with open(self.log_file, 'w'):
```

### Comparing `qase_python_commons-3.0.2b6/src/qase/commons/models/attachment.py` & `qase_python_commons-3.0.2b7/src/qase/commons/models/attachment.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b6/src/qase/commons/models/result.py` & `qase_python_commons-3.0.2b7/src/qase/commons/models/result.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b6/src/qase/commons/models/run.py` & `qase_python_commons-3.0.2b7/src/qase/commons/models/run.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b6/src/qase/commons/models/runtime.py` & `qase_python_commons-3.0.2b7/src/qase/commons/models/runtime.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b6/src/qase/commons/models/step.py` & `qase_python_commons-3.0.2b7/src/qase/commons/models/step.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,18 +76,18 @@
     def __init__(self, status: Optional[str] = 'untested', end_time: int = 0, duration: int = 0):
         self.start_time = time.time()
         self.status = status
         self.end_time = end_time
         self.duration = duration
 
     def set_status(self, status: Optional[str]):
-        if status in ['passed', 'failed', 'skipped', 'untested']:
+        if status in ['passed', 'failed', 'skipped', 'blocked', 'untested']:
             self.status = status
         else:
-            raise ValueError('Step status must be one of: passed, failed, skipped, untested')
+            raise ValueError('Step status must be one of: passed, failed, skipped, blocked, untested')
 
     def complete(self):
         self.end_time = time.time()
         self.duration = int((self.end_time - self.start_time) * 1000)
 
 
 class Step(BaseModel):
```

### Comparing `qase_python_commons-3.0.2b6/src/qase/commons/profilers/network.py` & `qase_python_commons-3.0.2b7/src/qase/commons/profilers/network.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b6/src/qase/commons/profilers/sleep.py` & `qase_python_commons-3.0.2b7/src/qase/commons/profilers/sleep.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b6/src/qase/commons/reporters/core.py` & `qase_python_commons-3.0.2b7/src/qase/commons/reporters/core.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b6/src/qase/commons/reporters/report.py` & `qase_python_commons-3.0.2b7/src/qase/commons/reporters/report.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b6/src/qase/commons/reporters/testops.py` & `qase_python_commons-3.0.2b7/src/qase/commons/reporters/testops.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b6/src/qase/commons/utils.py` & `qase_python_commons-3.0.2b7/src/qase/commons/utils.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.2b6/src/qase_python_commons.egg-info/PKG-INFO` & `qase_python_commons-3.0.2b7/src/qase_python_commons.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qase-python-commons
-Version: 3.0.2b6
+Version: 3.0.2b7
 Summary: A library for Qase TestOps and Qase Report
 Author-email: Qase Team <support@qase.io>
 Project-URL: Homepage, https://github.com/qase-tms/qase-python/tree/master/qase-python-commons
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `qase_python_commons-3.0.2b6/src/qase_python_commons.egg-info/SOURCES.txt` & `qase_python_commons-3.0.2b7/src/qase_python_commons.egg-info/SOURCES.txt`

 * *Files identical despite different names*

