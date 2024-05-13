# Comparing `tmp/testit_python_commons-3.1.0.tar.gz` & `tmp/testit_python_commons-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testit_python_commons-3.1.0.tar", last modified: Tue Apr 23 15:10:27 2024, max compression
+gzip compressed data, was "testit_python_commons-3.1.1.tar", last modified: Mon May 13 12:53:42 2024, max compression
```

## Comparing `testit_python_commons-3.1.0.tar` & `testit_python_commons-3.1.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:10:27.793763 testit_python_commons-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-23 15:10:27.793763 testit_python_commons-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-23 15:10:23.000000 testit_python_commons-3.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 15:10:27.793763 testit_python_commons-3.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-23 15:10:23.000000 testit_python_commons-3.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:10:27.789763 testit_python_commons-3.1.0/src/
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-23 15:10:23.000000 testit_python_commons-3.1.0/src/testit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:10:27.789763 testit_python_commons-3.1.0/src/testit_python_commons/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 15:10:23.000000 testit_python_commons-3.1.0/src/testit_python_commons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9166 2024-04-23 15:10:23.000000 testit_python_commons-3.1.0/src/testit_python_commons/app_properties.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:10:27.789763 testit_python_commons-3.1.0/src/testit_python_commons/client/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-23 15:10:23.000000 testit_python_commons-3.1.0/src/testit_python_commons/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7679 2024-04-23 15:10:23.000000 testit_python_commons-3.1.0/src/testit_python_commons/client/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-04-23 15:10:23.000000 testit_python_commons-3.1.0/src/testit_python_commons/client/client_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)    12871 2024-04-23 15:10:23.000000 testit_python_commons-3.1.0/src/testit_python_commons/client/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4875 2024-04-23 15:10:23.000000 testit_python_commons-3.1.0/src/testit_python_commons/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     4693 2024-04-23 15:10:23.000000 testit_python_commons-3.1.0/src/testit_python_commons/dynamic_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:10:27.793763 testit_python_commons-3.1.0/src/testit_python_commons/models/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-23 15:10:23.000000 testit_python_commons-3.1.0/src/testit_python_commons/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-23 15:10:23.000000 testit_python_commons-3.1.0/src/testit_python_commons/models/adapter_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-23 15:10:23.000000 testit_python_commons-3.1.0/src/testit_python_commons/models/link.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-23 15:10:23.000000 testit_python_commons-3.1.0/src/testit_python_commons/models/link_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-23 15:10:23.000000 testit_python_commons-3.1.0/src/testit_python_commons/models/outcome_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-04-23 15:10:23.000000 testit_python_commons-3.1.0/src/testit_python_commons/models/step_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     6214 2024-04-23 15:10:23.000000 testit_python_commons-3.1.0/src/testit_python_commons/models/test_result.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-23 15:10:23.000000 testit_python_commons-3.1.0/src/testit_python_commons/models/test_result_with_all_fixture_step_results_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:10:27.793763 testit_python_commons-3.1.0/src/testit_python_commons/services/
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-23 15:10:23.000000 testit_python_commons-3.1.0/src/testit_python_commons/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-04-23 15:10:23.000000 testit_python_commons-3.1.0/src/testit_python_commons/services/adapter_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-04-23 15:10:23.000000 testit_python_commons-3.1.0/src/testit_python_commons/services/adapter_manager_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-23 15:10:23.000000 testit_python_commons-3.1.0/src/testit_python_commons/services/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-04-23 15:10:23.000000 testit_python_commons-3.1.0/src/testit_python_commons/services/plugin_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-23 15:10:23.000000 testit_python_commons-3.1.0/src/testit_python_commons/services/step_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-23 15:10:23.000000 testit_python_commons-3.1.0/src/testit_python_commons/services/step_result_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-04-23 15:10:23.000000 testit_python_commons-3.1.0/src/testit_python_commons/services/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-04-23 15:10:23.000000 testit_python_commons-3.1.0/src/testit_python_commons/step.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:10:27.793763 testit_python_commons-3.1.0/src/testit_python_commons.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-23 15:10:27.000000 testit_python_commons-3.1.0/src/testit_python_commons.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-23 15:10:27.000000 testit_python_commons-3.1.0/src/testit_python_commons.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 15:10:27.000000 testit_python_commons-3.1.0/src/testit_python_commons.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-23 15:10:27.000000 testit_python_commons-3.1.0/src/testit_python_commons.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-23 15:10:27.000000 testit_python_commons-3.1.0/src/testit_python_commons.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:53:42.193807 testit_python_commons-3.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-13 12:53:42.193807 testit_python_commons-3.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-13 12:53:37.000000 testit_python_commons-3.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 12:53:42.193807 testit_python_commons-3.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-13 12:53:37.000000 testit_python_commons-3.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:53:42.189807 testit_python_commons-3.1.1/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-13 12:53:37.000000 testit_python_commons-3.1.1/src/testit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:53:42.189807 testit_python_commons-3.1.1/src/testit_python_commons/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 12:53:37.000000 testit_python_commons-3.1.1/src/testit_python_commons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9615 2024-05-13 12:53:37.000000 testit_python_commons-3.1.1/src/testit_python_commons/app_properties.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:53:42.189807 testit_python_commons-3.1.1/src/testit_python_commons/client/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-13 12:53:37.000000 testit_python_commons-3.1.1/src/testit_python_commons/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7679 2024-05-13 12:53:37.000000 testit_python_commons-3.1.1/src/testit_python_commons/client/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-05-13 12:53:37.000000 testit_python_commons-3.1.1/src/testit_python_commons/client/client_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12871 2024-05-13 12:53:37.000000 testit_python_commons-3.1.1/src/testit_python_commons/client/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4875 2024-05-13 12:53:37.000000 testit_python_commons-3.1.1/src/testit_python_commons/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4693 2024-05-13 12:53:37.000000 testit_python_commons-3.1.1/src/testit_python_commons/dynamic_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:53:42.193807 testit_python_commons-3.1.1/src/testit_python_commons/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-13 12:53:37.000000 testit_python_commons-3.1.1/src/testit_python_commons/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-13 12:53:37.000000 testit_python_commons-3.1.1/src/testit_python_commons/models/adapter_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-13 12:53:37.000000 testit_python_commons-3.1.1/src/testit_python_commons/models/link.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-13 12:53:37.000000 testit_python_commons-3.1.1/src/testit_python_commons/models/link_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-13 12:53:37.000000 testit_python_commons-3.1.1/src/testit_python_commons/models/outcome_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-13 12:53:37.000000 testit_python_commons-3.1.1/src/testit_python_commons/models/step_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6214 2024-05-13 12:53:37.000000 testit_python_commons-3.1.1/src/testit_python_commons/models/test_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-13 12:53:37.000000 testit_python_commons-3.1.1/src/testit_python_commons/models/test_result_with_all_fixture_step_results_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:53:42.193807 testit_python_commons-3.1.1/src/testit_python_commons/services/
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-13 12:53:37.000000 testit_python_commons-3.1.1/src/testit_python_commons/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-05-13 12:53:37.000000 testit_python_commons-3.1.1/src/testit_python_commons/services/adapter_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-13 12:53:37.000000 testit_python_commons-3.1.1/src/testit_python_commons/services/adapter_manager_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-13 12:53:37.000000 testit_python_commons-3.1.1/src/testit_python_commons/services/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-05-13 12:53:37.000000 testit_python_commons-3.1.1/src/testit_python_commons/services/plugin_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-13 12:53:37.000000 testit_python_commons-3.1.1/src/testit_python_commons/services/step_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-13 12:53:37.000000 testit_python_commons-3.1.1/src/testit_python_commons/services/step_result_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-05-13 12:53:37.000000 testit_python_commons-3.1.1/src/testit_python_commons/services/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-05-13 12:53:37.000000 testit_python_commons-3.1.1/src/testit_python_commons/step.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:53:42.193807 testit_python_commons-3.1.1/src/testit_python_commons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-13 12:53:42.000000 testit_python_commons-3.1.1/src/testit_python_commons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-13 12:53:42.000000 testit_python_commons-3.1.1/src/testit_python_commons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 12:53:42.000000 testit_python_commons-3.1.1/src/testit_python_commons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-13 12:53:42.000000 testit_python_commons-3.1.1/src/testit_python_commons.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-13 12:53:42.000000 testit_python_commons-3.1.1/src/testit_python_commons.egg-info/top_level.txt
```

### Comparing `testit_python_commons-3.1.0/PKG-INFO` & `testit_python_commons-3.1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testit-python-commons
-Version: 3.1.0
+Version: 3.1.1
 Summary: Python commons for Test IT
 Home-page: https://github.com/testit-tms/adapters-python/
 Author: Integration team
 Author-email: integrations@testit.software
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `testit_python_commons-3.1.0/setup.py` & `testit_python_commons-3.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='testit-python-commons',
-    version='3.1.0',
+    version='3.1.1',
     description='Python commons for Test IT',
     long_description=open('README.md', "r").read(),
     long_description_content_type="text/markdown",
     url='https://github.com/testit-tms/adapters-python/',
     author='Integration team',
     author_email='integrations@testit.software',
     license='Apache-2.0',
```

### Comparing `testit_python_commons-3.1.0/src/testit.py` & `testit_python_commons-3.1.1/src/testit.py`

 * *Files identical despite different names*

### Comparing `testit_python_commons-3.1.0/src/testit_python_commons/app_properties.py` & `testit_python_commons-3.1.1/src/testit_python_commons/app_properties.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import configparser
 import logging
 import os
 import re
 import warnings
+import uuid
+from urllib.parse import urlparse
 
 from testit_python_commons.models.adapter_mode import AdapterMode
 
 
 class AppProperties:
     __properties_file = 'connection_config'
     __env_prefix = 'TMS'
@@ -152,54 +154,69 @@
         if f'{cls.__env_prefix}_AUTOMATIC_CREATION_TEST_CASES' in os.environ.keys() and cls.__check_property_value(
                 os.environ.get(f'{cls.__env_prefix}_AUTOMATIC_CREATION_TEST_CASES')):
             env_properties['automaticcreationtestcases'] = os.environ.get(
                 f'{cls.__env_prefix}_AUTOMATIC_CREATION_TEST_CASES')
 
         return env_properties
 
-    @staticmethod
-    def __check_properties(properties: dict):
+    @classmethod
+    def __check_properties(cls, properties: dict):
         adapter_mode = properties.get('adaptermode')
 
         if adapter_mode == AdapterMode.NEW_TEST_RUN:
-            if properties.get('projectid') is None:
-                logging.error('Adapter mode "2" is enabled. The project ID is needed, but it was not found!')
+            try:
+                uuid.UUID(str(properties.get('testrunid')))
+                logging.error('Adapter mode "2" is enabled. Config should not contains test run id!')
                 raise SystemExit
+            except ValueError:
+                pass
+
         elif adapter_mode in (
                 AdapterMode.RUN_ALL_TESTS,
                 AdapterMode.USE_FILTER,
                 None):
-            if properties.get('testrunid') is None:
+            try:
+                uuid.UUID(str(properties.get('testrunid')))
+            except ValueError:
                 logging.error(f'Adapter mode "{adapter_mode if adapter_mode else "0"}" is enabled. '
                               f'The test run ID is needed, but it was not found!')
                 raise SystemExit
         else:
             logging.error(f'Unknown adapter mode "{adapter_mode}"!')
             raise SystemExit
 
-        if properties.get('url') is None:
-            logging.error('URL was not found!')
+        try:
+            uuid.UUID(str(properties.get('projectid')))
+        except ValueError:
+            logging.error('Project ID was not found!')
             raise SystemExit
 
-        if properties.get('privatetoken') is None:
+        try:
+            url = urlparse(properties.get('url'))
+            if not all([url.scheme, url.netloc]):
+                raise AttributeError
+        except AttributeError:
+            logging.error('URL is invalid!')
+            raise SystemExit
+
+        if not cls.__check_property_value(properties.get('privatetoken')):
             logging.error('Private token was not found!')
             raise SystemExit
 
-        if properties.get('configurationid') is None:
+        try:
+            uuid.UUID(str(properties.get('configurationid')))
+        except ValueError:
             logging.error('Configuration ID was not found!')
             raise SystemExit
 
-        if properties.get('testrunname'):
-            properties['testrunname'] = properties['testrunname']
-
-        if properties.get('certvalidation'):
-            properties['certvalidation'] = properties['certvalidation'].lower()
+        if not cls.__check_property_value(properties.get('certvalidation')):
+            properties['certvalidation'] = 'true'
 
-        if properties.get('automaticcreationtestcases'):
-            properties['automaticcreationtestcases'] = properties['automaticcreationtestcases'].lower()
+        if not cls.__check_property_value(properties.get('automaticcreationtestcases')):
+            properties['automaticcreationtestcases'] = 'false'
 
     @staticmethod
     def __search_in_environ(var_name: str):
         if re.fullmatch(r'{[a-zA-Z_]\w*}', var_name) and var_name[1:-1] in os.environ:
             return os.environ[var_name[1:-1]]
 
         return var_name
```

### Comparing `testit_python_commons-3.1.0/src/testit_python_commons/client/api_client.py` & `testit_python_commons-3.1.1/src/testit_python_commons/client/api_client.py`

 * *Files identical despite different names*

### Comparing `testit_python_commons-3.1.0/src/testit_python_commons/client/client_configuration.py` & `testit_python_commons-3.1.1/src/testit_python_commons/client/client_configuration.py`

 * *Files identical despite different names*

### Comparing `testit_python_commons-3.1.0/src/testit_python_commons/client/converter.py` & `testit_python_commons-3.1.1/src/testit_python_commons/client/converter.py`

 * *Files identical despite different names*

### Comparing `testit_python_commons-3.1.0/src/testit_python_commons/decorators.py` & `testit_python_commons-3.1.1/src/testit_python_commons/decorators.py`

 * *Files identical despite different names*

### Comparing `testit_python_commons-3.1.0/src/testit_python_commons/dynamic_methods.py` & `testit_python_commons-3.1.1/src/testit_python_commons/dynamic_methods.py`

 * *Files identical despite different names*

### Comparing `testit_python_commons-3.1.0/src/testit_python_commons/models/link.py` & `testit_python_commons-3.1.1/src/testit_python_commons/models/link.py`

 * *Files identical despite different names*

### Comparing `testit_python_commons-3.1.0/src/testit_python_commons/models/step_result.py` & `testit_python_commons-3.1.1/src/testit_python_commons/models/step_result.py`

 * *Files identical despite different names*

### Comparing `testit_python_commons-3.1.0/src/testit_python_commons/models/test_result.py` & `testit_python_commons-3.1.1/src/testit_python_commons/models/test_result.py`

 * *Files identical despite different names*

### Comparing `testit_python_commons-3.1.0/src/testit_python_commons/models/test_result_with_all_fixture_step_results_model.py` & `testit_python_commons-3.1.1/src/testit_python_commons/models/test_result_with_all_fixture_step_results_model.py`

 * *Files identical despite different names*

### Comparing `testit_python_commons-3.1.0/src/testit_python_commons/services/adapter_manager.py` & `testit_python_commons-3.1.1/src/testit_python_commons/services/adapter_manager.py`

 * *Files identical despite different names*

### Comparing `testit_python_commons-3.1.0/src/testit_python_commons/services/adapter_manager_configuration.py` & `testit_python_commons-3.1.1/src/testit_python_commons/services/adapter_manager_configuration.py`

 * *Files identical despite different names*

### Comparing `testit_python_commons-3.1.0/src/testit_python_commons/services/logger.py` & `testit_python_commons-3.1.1/src/testit_python_commons/services/logger.py`

 * *Files identical despite different names*

### Comparing `testit_python_commons-3.1.0/src/testit_python_commons/services/plugin_manager.py` & `testit_python_commons-3.1.1/src/testit_python_commons/services/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `testit_python_commons-3.1.0/src/testit_python_commons/services/step_manager.py` & `testit_python_commons-3.1.1/src/testit_python_commons/services/step_manager.py`

 * *Files identical despite different names*

### Comparing `testit_python_commons-3.1.0/src/testit_python_commons/services/step_result_storage.py` & `testit_python_commons-3.1.1/src/testit_python_commons/services/step_result_storage.py`

 * *Files identical despite different names*

### Comparing `testit_python_commons-3.1.0/src/testit_python_commons/services/utils.py` & `testit_python_commons-3.1.1/src/testit_python_commons/services/utils.py`

 * *Files identical despite different names*

### Comparing `testit_python_commons-3.1.0/src/testit_python_commons/step.py` & `testit_python_commons-3.1.1/src/testit_python_commons/step.py`

 * *Files identical despite different names*

### Comparing `testit_python_commons-3.1.0/src/testit_python_commons.egg-info/PKG-INFO` & `testit_python_commons-3.1.1/src/testit_python_commons.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testit-python-commons
-Version: 3.1.0
+Version: 3.1.1
 Summary: Python commons for Test IT
 Home-page: https://github.com/testit-tms/adapters-python/
 Author: Integration team
 Author-email: integrations@testit.software
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `testit_python_commons-3.1.0/src/testit_python_commons.egg-info/SOURCES.txt` & `testit_python_commons-3.1.1/src/testit_python_commons.egg-info/SOURCES.txt`

 * *Files identical despite different names*

