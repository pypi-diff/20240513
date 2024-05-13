# Comparing `tmp/variable_local-0.0.98.tar.gz` & `tmp/variable_local-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "variable_local-0.0.98.tar", last modified: Wed May  8 03:46:25 2024, max compression
+gzip compressed data, was "variable_local-0.0.99.tar", last modified: Mon May 13 13:55:46 2024, max compression
```

## Comparing `variable_local-0.0.98.tar` & `variable_local-0.0.99.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:46:25.080272 variable_local-0.0.98/
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-08 03:46:25.080272 variable_local-0.0.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-08 03:45:58.000000 variable_local-0.0.98/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-08 03:45:58.000000 variable_local-0.0.98/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 03:46:25.080272 variable_local-0.0.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-08 03:45:58.000000 variable_local-0.0.98/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:46:25.076272 variable_local-0.0.98/variable_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:46:25.076272 variable_local-0.0.98/variable_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 03:45:58.000000 variable_local-0.0.98/variable_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-08 03:45:58.000000 variable_local-0.0.98/variable_local/src/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     9059 2024-05-08 03:45:58.000000 variable_local-0.0.98/variable_local/src/template.py
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-08 03:45:58.000000 variable_local-0.0.98/variable_local/src/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7076 2024-05-08 03:45:58.000000 variable_local-0.0.98/variable_local/src/variables_local.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:46:25.080272 variable_local-0.0.98/variable_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-08 03:46:25.000000 variable_local-0.0.98/variable_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-08 03:46:25.000000 variable_local-0.0.98/variable_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 03:46:25.000000 variable_local-0.0.98/variable_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-08 03:46:25.000000 variable_local-0.0.98/variable_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-08 03:46:25.000000 variable_local-0.0.98/variable_local.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:55:46.481827 variable_local-0.0.99/
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-13 13:55:46.481827 variable_local-0.0.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-13 13:55:11.000000 variable_local-0.0.99/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-13 13:55:11.000000 variable_local-0.0.99/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 13:55:46.481827 variable_local-0.0.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-13 13:55:11.000000 variable_local-0.0.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:55:46.477827 variable_local-0.0.99/variable_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:55:46.481827 variable_local-0.0.99/variable_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 13:55:11.000000 variable_local-0.0.99/variable_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-13 13:55:11.000000 variable_local-0.0.99/variable_local/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9059 2024-05-13 13:55:11.000000 variable_local-0.0.99/variable_local/src/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-13 13:55:11.000000 variable_local-0.0.99/variable_local/src/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7073 2024-05-13 13:55:11.000000 variable_local-0.0.99/variable_local/src/variables_local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:55:46.481827 variable_local-0.0.99/variable_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-13 13:55:46.000000 variable_local-0.0.99/variable_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-13 13:55:46.000000 variable_local-0.0.99/variable_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 13:55:46.000000 variable_local-0.0.99/variable_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-13 13:55:46.000000 variable_local-0.0.99/variable_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-13 13:55:46.000000 variable_local-0.0.99/variable_local.egg-info/top_level.txt
```

### Comparing `variable_local-0.0.98/PKG-INFO` & `variable_local-0.0.99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: variable-local
-Version: 0.0.98
+Version: 0.0.99
 Summary: PyPI Package for Circles variable Local/Remote Python
 Home-page: https://github.com/circles-zone/variable-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `variable_local-0.0.98/README.md` & `variable_local-0.0.99/README.md`

 * *Files identical despite different names*

### Comparing `variable_local-0.0.98/pyproject.toml` & `variable_local-0.0.99/pyproject.toml`

 * *Files identical despite different names*

### Comparing `variable_local-0.0.98/setup.py` & `variable_local-0.0.99/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = 'variable-local'
 package_dir = PACKAGE_NAME.replace('-', '_')
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.98',  # https://pypi.org/project/variable-local
+    version='0.0.99',  # https://pypi.org/project/variable-local
     author="Circles",
     author_email="info@circles.life",
     description="PyPI Package for Circles variable Local/Remote Python",
     long_description="PyPI Package for Circles variable Local/Remote Python",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
```

### Comparing `variable_local-0.0.98/variable_local/src/constants.py` & `variable_local-0.0.99/variable_local/src/constants.py`

 * *Files identical despite different names*

### Comparing `variable_local-0.0.98/variable_local/src/template.py` & `variable_local-0.0.99/variable_local/src/template.py`

 * *Files identical despite different names*

### Comparing `variable_local-0.0.98/variable_local/src/variables_local.py` & `variable_local-0.0.99/variable_local/src/variables_local.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 logger = Logger.create_logger(object=variable_local_logger_init_object)
 cache_with_timeout = {}
 
 
 class VariablesLocal(GenericCRUD):
     def __init__(self):
         super().__init__(default_schema_name="field", default_table_name="field_table",
-                         default_view_table_name="field_view", default_id_column_name="variable_id")
+                         default_view_table_name="field_view", default_column_name="variable_id")
         self.name2id_dict = {}
         self.id2name_dict = {}
         self.next_variable_id = 1
         variable_names_dict = self.load_variable_names_dict_from_variable_table()
         for variable_id in variable_names_dict:
             self.add(variable_id=variable_id,
                      variable_name=variable_names_dict[variable_id])
@@ -68,18 +68,18 @@
         return variable_value
 
     def set_variable_value_by_variable_id(self, variable_id: int, variable_value: str, profile_id: int,
                                           state_id: int) -> None:
         logger.start(object={'variable_id': variable_id,
                              'variable_value': variable_value, 'profile_id': profile_id})
         # TODO I believe we should keep more fields  [like what?]
-        data_json = {'variable_id': variable_id, 'variable_value_new': variable_value, 'profile_id': profile_id,
+        data_dict = {'variable_id': variable_id, 'variable_value_new': variable_value, 'profile_id': profile_id,
                      'state_id': state_id, 'record': '{}', 'message': '', 'path': '',
                      'component_id': VARIABLE_LOCAL_PYTHON_PACKAGE_COMPONENT_ID}
-        self.insert(schema_name="logger", table_name='logger_table', data_json=data_json)
+        self.insert(schema_name="logger", table_name='logger_table', data_dict=data_dict)
         logger.end()
 
     def get_variable_value_by_variable_id(self, variable_id: int, lang_code: LangCode, profile_id: int = None) -> str:
         timeout = 60  # seconds
         cache_key = (variable_id, lang_code, profile_id)
         if cache_key in cache_with_timeout:
             if cache_with_timeout[cache_key]["time"] > time.time() - timeout:
```

### Comparing `variable_local-0.0.98/variable_local.egg-info/PKG-INFO` & `variable_local-0.0.99/variable_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: variable-local
-Version: 0.0.98
+Version: 0.0.99
 Summary: PyPI Package for Circles variable Local/Remote Python
 Home-page: https://github.com/circles-zone/variable-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

