# Comparing `tmp/gen_wrappers-0.2.9.tar.gz` & `tmp/gen_wrappers-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gen_wrappers-0.2.9.tar", last modified: Mon May 13 17:49:11 2024, max compression
+gzip compressed data, was "gen_wrappers-0.3.0.tar", last modified: Mon May 13 18:57:50 2024, max compression
```

## Comparing `gen_wrappers-0.2.9.tar` & `gen_wrappers-0.3.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 17:49:11.220266 gen_wrappers-0.2.9/
--rw-rw-rw-   0        0        0      847 2024-05-13 17:49:11.218266 gen_wrappers-0.2.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-13 17:49:11.187699 gen_wrappers-0.2.9/creator/
--rw-rw-rw-   0        0        0        0 2024-04-09 16:36:19.000000 gen_wrappers-0.2.9/creator/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 17:49:11.192723 gen_wrappers-0.2.9/creator/auto/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:51.000000 gen_wrappers-0.2.9/creator/auto/__init__.py
--rw-rw-rw-   0        0        0     6625 2024-05-11 17:01:23.000000 gen_wrappers-0.2.9/creator/auto/creator_auto.py
--rw-rw-rw-   0        0        0     6018 2024-05-03 19:52:10.000000 gen_wrappers-0.2.9/creator/auto/request_auto.py
--rw-rw-rw-   0        0        0      644 2024-05-11 17:01:23.000000 gen_wrappers-0.2.9/creator/auto/response_auto.py
-drwxrwxrwx   0        0        0        0 2024-05-13 17:49:11.198221 gen_wrappers-0.2.9/creator/base/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:25:44.000000 gen_wrappers-0.2.9/creator/base/__init__.py
--rw-rw-rw-   0        0        0     1584 2024-05-09 21:53:52.000000 gen_wrappers-0.2.9/creator/base/base_app.py
--rw-rw-rw-   0        0        0      554 2024-05-02 19:51:12.000000 gen_wrappers-0.2.9/creator/base/base_request.py
--rw-rw-rw-   0        0        0     3374 2024-05-13 17:23:12.000000 gen_wrappers-0.2.9/creator/base/base_response.py
--rw-rw-rw-   0        0        0      228 2024-04-26 19:27:33.000000 gen_wrappers-0.2.9/creator/base/job_status.py
-drwxrwxrwx   0        0        0        0 2024-05-13 17:49:11.201220 gen_wrappers-0.2.9/creator/cmfy/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:43.000000 gen_wrappers-0.2.9/creator/cmfy/__init__.py
--rw-rw-rw-   0        0        0     9561 2024-05-11 17:02:29.000000 gen_wrappers-0.2.9/creator/cmfy/creator_cmfy.py
--rw-rw-rw-   0        0        0     9193 2024-05-11 14:41:07.000000 gen_wrappers-0.2.9/creator/cmfy/request_cmfy.py
--rw-rw-rw-   0        0        0      503 2024-05-02 15:57:38.000000 gen_wrappers-0.2.9/creator/cmfy/response_cmfy.py
-drwxrwxrwx   0        0        0        0 2024-05-13 17:49:11.206223 gen_wrappers-0.2.9/creator/fcus_api/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:36.000000 gen_wrappers-0.2.9/creator/fcus_api/__init__.py
--rw-rw-rw-   0        0        0     6345 2024-05-11 17:04:12.000000 gen_wrappers-0.2.9/creator/fcus_api/creator_fcus_api.py
--rw-rw-rw-   0        0        0     3975 2024-05-10 20:59:44.000000 gen_wrappers-0.2.9/creator/fcus_api/request_fcus_api.py
--rw-rw-rw-   0        0        0     1131 2024-05-02 15:57:38.000000 gen_wrappers-0.2.9/creator/fcus_api/response_fcus_api.py
-drwxrwxrwx   0        0        0        0 2024-05-13 17:49:11.208226 gen_wrappers-0.2.9/creator/util/
--rw-rw-rw-   0        0        0        0 2024-05-13 17:26:08.000000 gen_wrappers-0.2.9/creator/util/__init__.py
--rw-rw-rw-   0        0        0     6092 2024-05-13 17:06:45.000000 gen_wrappers-0.2.9/creator/util/helper.py
-drwxrwxrwx   0        0        0        0 2024-05-13 17:49:11.216257 gen_wrappers-0.2.9/gen_wrappers.egg-info/
--rw-rw-rw-   0        0        0      847 2024-05-13 17:49:11.000000 gen_wrappers-0.2.9/gen_wrappers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      758 2024-05-13 17:49:11.000000 gen_wrappers-0.2.9/gen_wrappers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 17:49:11.000000 gen_wrappers-0.2.9/gen_wrappers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2024-05-13 17:49:11.000000 gen_wrappers-0.2.9/gen_wrappers.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-13 17:49:11.000000 gen_wrappers-0.2.9/gen_wrappers.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-13 17:49:11.220266 gen_wrappers-0.2.9/setup.cfg
--rw-rw-rw-   0        0        0     1035 2024-05-13 17:47:33.000000 gen_wrappers-0.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 18:57:50.138563 gen_wrappers-0.3.0/
+-rw-rw-rw-   0        0        0      847 2024-05-13 18:57:50.136330 gen_wrappers-0.3.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-13 18:57:50.025400 gen_wrappers-0.3.0/creator/
+-rw-rw-rw-   0        0        0        0 2024-04-09 16:36:19.000000 gen_wrappers-0.3.0/creator/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 18:57:50.044275 gen_wrappers-0.3.0/creator/auto/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:51.000000 gen_wrappers-0.3.0/creator/auto/__init__.py
+-rw-rw-rw-   0        0        0     6625 2024-05-11 17:01:23.000000 gen_wrappers-0.3.0/creator/auto/creator_auto.py
+-rw-rw-rw-   0        0        0     6018 2024-05-03 19:52:10.000000 gen_wrappers-0.3.0/creator/auto/request_auto.py
+-rw-rw-rw-   0        0        0      644 2024-05-11 17:01:23.000000 gen_wrappers-0.3.0/creator/auto/response_auto.py
+drwxrwxrwx   0        0        0        0 2024-05-13 18:57:50.058795 gen_wrappers-0.3.0/creator/base/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:25:44.000000 gen_wrappers-0.3.0/creator/base/__init__.py
+-rw-rw-rw-   0        0        0     1584 2024-05-09 21:53:52.000000 gen_wrappers-0.3.0/creator/base/base_app.py
+-rw-rw-rw-   0        0        0      554 2024-05-02 19:51:12.000000 gen_wrappers-0.3.0/creator/base/base_request.py
+-rw-rw-rw-   0        0        0     3374 2024-05-13 17:23:12.000000 gen_wrappers-0.3.0/creator/base/base_response.py
+-rw-rw-rw-   0        0        0      228 2024-04-26 19:27:33.000000 gen_wrappers-0.3.0/creator/base/job_status.py
+drwxrwxrwx   0        0        0        0 2024-05-13 18:57:50.072588 gen_wrappers-0.3.0/creator/cmfy/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:43.000000 gen_wrappers-0.3.0/creator/cmfy/__init__.py
+-rw-rw-rw-   0        0        0     9561 2024-05-11 17:02:29.000000 gen_wrappers-0.3.0/creator/cmfy/creator_cmfy.py
+-rw-rw-rw-   0        0        0     9193 2024-05-11 14:41:07.000000 gen_wrappers-0.3.0/creator/cmfy/request_cmfy.py
+-rw-rw-rw-   0        0        0      503 2024-05-02 15:57:38.000000 gen_wrappers-0.3.0/creator/cmfy/response_cmfy.py
+drwxrwxrwx   0        0        0        0 2024-05-13 18:57:50.080691 gen_wrappers-0.3.0/creator/fcus_api/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:36.000000 gen_wrappers-0.3.0/creator/fcus_api/__init__.py
+-rw-rw-rw-   0        0        0     6345 2024-05-11 17:04:12.000000 gen_wrappers-0.3.0/creator/fcus_api/creator_fcus_api.py
+-rw-rw-rw-   0        0        0     3975 2024-05-10 20:59:44.000000 gen_wrappers-0.3.0/creator/fcus_api/request_fcus_api.py
+-rw-rw-rw-   0        0        0     1131 2024-05-02 15:57:38.000000 gen_wrappers-0.3.0/creator/fcus_api/response_fcus_api.py
+drwxrwxrwx   0        0        0        0 2024-05-13 18:57:50.085618 gen_wrappers-0.3.0/creator/util/
+-rw-rw-rw-   0        0        0        0 2024-05-13 17:26:08.000000 gen_wrappers-0.3.0/creator/util/__init__.py
+-rw-rw-rw-   0        0        0     6070 2024-05-13 18:55:27.000000 gen_wrappers-0.3.0/creator/util/helper.py
+drwxrwxrwx   0        0        0        0 2024-05-13 18:57:50.133891 gen_wrappers-0.3.0/gen_wrappers.egg-info/
+-rw-rw-rw-   0        0        0      847 2024-05-13 18:57:49.000000 gen_wrappers-0.3.0/gen_wrappers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      758 2024-05-13 18:57:49.000000 gen_wrappers-0.3.0/gen_wrappers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 18:57:49.000000 gen_wrappers-0.3.0/gen_wrappers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2024-05-13 18:57:49.000000 gen_wrappers-0.3.0/gen_wrappers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-13 18:57:49.000000 gen_wrappers-0.3.0/gen_wrappers.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 18:57:50.138563 gen_wrappers-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1035 2024-05-13 18:57:33.000000 gen_wrappers-0.3.0/setup.py
```

### Comparing `gen_wrappers-0.2.9/PKG-INFO` & `gen_wrappers-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen_wrappers
-Version: 0.2.9
+Version: 0.3.0
 Summary: A set of wrapper classes for various generative API projects
 Home-page: https://github.com/d8ahazard/gen_wrappers
 Author: d8ahazard
 Author-email: d8ahazard@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gen_wrappers-0.2.9/creator/auto/creator_auto.py` & `gen_wrappers-0.3.0/creator/auto/creator_auto.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.2.9/creator/auto/request_auto.py` & `gen_wrappers-0.3.0/creator/auto/request_auto.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.2.9/creator/auto/response_auto.py` & `gen_wrappers-0.3.0/creator/auto/response_auto.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.2.9/creator/base/base_app.py` & `gen_wrappers-0.3.0/creator/base/base_app.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.2.9/creator/base/base_request.py` & `gen_wrappers-0.3.0/creator/base/base_request.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.2.9/creator/base/base_response.py` & `gen_wrappers-0.3.0/creator/base/base_response.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.2.9/creator/cmfy/creator_cmfy.py` & `gen_wrappers-0.3.0/creator/cmfy/creator_cmfy.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.2.9/creator/cmfy/request_cmfy.py` & `gen_wrappers-0.3.0/creator/cmfy/request_cmfy.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.2.9/creator/fcus_api/creator_fcus_api.py` & `gen_wrappers-0.3.0/creator/fcus_api/creator_fcus_api.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.2.9/creator/fcus_api/request_fcus_api.py` & `gen_wrappers-0.3.0/creator/fcus_api/request_fcus_api.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.2.9/creator/fcus_api/response_fcus_api.py` & `gen_wrappers-0.3.0/creator/fcus_api/response_fcus_api.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.2.9/creator/util/helper.py` & `gen_wrappers-0.3.0/creator/util/helper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import importlib
 import pkgutil
 import sys
-from typing import Union, Type, Dict, List
+from typing import Union, Type, Dict, List, Any
 
 from creator.base.base_app import BaseApp
 from creator.base.base_request import BaseRequest
 
 
 def get_creators():
     package = sys.modules['creator']  # Make sure 'src.sb_api.creator' is the correct package path
@@ -38,15 +38,16 @@
         openapi_examples[creator] = {
             "summary": f"{creator}",
             "value": creator
         }
     return examples if not openapi_output else openapi_examples
 
 
-def get_use_cases(return_creator_names: bool = False, return_param_names: bool = False) -> Union[Dict[str, List[BaseRequest]], Dict[BaseApp, List[BaseRequest]]]:
+def get_use_cases(return_creator_names: bool = False, return_param_names: bool = False) -> Union[
+    Dict[str, List[BaseRequest]], Dict[BaseApp, List[BaseRequest]]]:
     package = sys.modules['creator']  # Make sure 'src.sb_api.creator' is the correct package path
     use_case_dict = {}
 
     for importer, modname, ispkg in pkgutil.walk_packages(package.__path__, package.__name__ + '.'):
         # Filter out unwanted modules
         if "creator_" not in modname or "base" in modname:
             continue
@@ -70,46 +71,42 @@
     return use_case_dict
 
 
 def get_use_case_examples(return_class_name=False, openapi_output=False):
     use_cases = get_use_cases(True, False)  # Always fetch class objects
     examples = []
     openapi_examples = {}
-    all_use_cases = []
-    for creator, param_classes in use_cases.items():
-        all_use_cases.extend(param_classes)
-    for param_class in all_use_cases:
-        example_param = param_class().example()  # Instantiate the class object
-        example_execution_params = {
-            "params": example_param,
-            "callback_url": "http://example.com/callback"
-        }
-        summary = f"Execute {param_class.__name__} with optional callback"
-        example_name = param_class.__name__ + ("_async" if return_class_name else "")
-        examples.append({"name": example_name, "value": example_execution_params})
-        openapi_examples[example_name] = {
-            "summary": summary,
-            "value": example_execution_params
-        }
+    for creator, use_case_list in use_cases.items():
+        for use_case in use_case_list:
+            example_param = use_case().example()
+            example_execution_params = {
+                "params": example_param,
+                "callback_url": "http://example.com/callback"
+            }
+            summary = f"Execute {creator}/{example_param.__name__}_async with optional callback"
+            example_name = example_param.__name__ + ("_async" if return_class_name else "")
+            examples.append({"name": example_name, "value": example_execution_params})
+            openapi_examples[example_name] = {
+                "summary": summary,
+                "value": example_execution_params
+            }
     return examples if not openapi_output else openapi_examples
 
 
-def get_method_examples(openapi_output=False):
+def get_method_examples(openapi_output=False) -> Union[Dict[str, Any], list[Dict[str, Any]]]:
     use_cases = get_use_cases(True, True)
     examples = []
     openapi_examples = {}
-    all_use_cases = []
-    for creator, param_classes in use_cases.items():
-        all_use_cases.extend(param_classes)
-    for method in all_use_cases:
-        examples.append({"name": method, "description": f"Example for {method} method."})
-        openapi_examples[method] = {
-            "summary": f"{method}",
-            "value": method
-        }
+    for creator, use_case_list in use_cases.items():
+        for method in use_case_list:
+            examples.append({"name": method, "description": f"Example for {method} method."})
+            openapi_examples[method] = {
+                "summary": f"{method}",
+                "value": method
+            }
     return examples if not openapi_output else openapi_examples
 
 
 def get_use_case(app_name: str, method: str, debug=False) -> Union[None, Type[BaseRequest]]:
     package = sys.modules['creator']  # Make sure 'src.sb_api.creator' is the correct package path
 
     for importer, modname, ispkg in pkgutil.walk_packages(package.__path__, package.__name__ + '.'):
```

### Comparing `gen_wrappers-0.2.9/gen_wrappers.egg-info/PKG-INFO` & `gen_wrappers-0.3.0/gen_wrappers.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen-wrappers
-Version: 0.2.9
+Version: 0.3.0
 Summary: A set of wrapper classes for various generative API projects
 Home-page: https://github.com/d8ahazard/gen_wrappers
 Author: d8ahazard
 Author-email: d8ahazard@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gen_wrappers-0.2.9/gen_wrappers.egg-info/SOURCES.txt` & `gen_wrappers-0.3.0/gen_wrappers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.2.9/setup.py` & `gen_wrappers-0.3.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gen_wrappers',
-    version='0.2.9',
+    version='0.3.0',
     author='d8ahazard',
     author_email='d8ahazard@gmail.com',
     description='A set of wrapper classes for various generative API projects',
     long_description_content_type='text/markdown',
     url='https://github.com/d8ahazard/gen_wrappers',  # Change this to your repository URL
     packages=find_packages(),
     install_requires=[
```

