# Comparing `tmp/group_local-0.0.22.tar.gz` & `tmp/group_local-0.0.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "group_local-0.0.22.tar", last modified: Thu May  9 12:09:24 2024, max compression
+gzip compressed data, was "group_local-0.0.23.tar", last modified: Mon May 13 17:38:42 2024, max compression
```

## Comparing `group_local-0.0.22.tar` & `group_local-0.0.23.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:09:24.557467 group_local-0.0.22/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-09 12:09:24.557467 group_local-0.0.22/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:09:24.557467 group_local-0.0.22/group_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:09:24.557467 group_local-0.0.22/group_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 12:09:10.000000 group_local-0.0.22/group_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13304 2024-05-09 12:09:10.000000 group_local-0.0.22/group_local/src/group_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-09 12:09:10.000000 group_local-0.0.22/group_local/src/group_local_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:09:24.557467 group_local-0.0.22/group_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-09 12:09:24.000000 group_local-0.0.22/group_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-09 12:09:24.000000 group_local-0.0.22/group_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 12:09:24.000000 group_local-0.0.22/group_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-09 12:09:24.000000 group_local-0.0.22/group_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-09 12:09:24.000000 group_local-0.0.22/group_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-09 12:09:10.000000 group_local-0.0.22/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 12:09:24.557467 group_local-0.0.22/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-09 12:09:10.000000 group_local-0.0.22/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:38:42.275359 group_local-0.0.23/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-13 17:38:42.275359 group_local-0.0.23/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:38:42.271359 group_local-0.0.23/group_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:38:42.275359 group_local-0.0.23/group_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 17:38:26.000000 group_local-0.0.23/group_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13304 2024-05-13 17:38:26.000000 group_local-0.0.23/group_local/src/group_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-13 17:38:26.000000 group_local-0.0.23/group_local/src/group_local_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:38:42.275359 group_local-0.0.23/group_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-13 17:38:42.000000 group_local-0.0.23/group_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-13 17:38:42.000000 group_local-0.0.23/group_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 17:38:42.000000 group_local-0.0.23/group_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-13 17:38:42.000000 group_local-0.0.23/group_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-13 17:38:42.000000 group_local-0.0.23/group_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-13 17:38:26.000000 group_local-0.0.23/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 17:38:42.275359 group_local-0.0.23/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-13 17:38:26.000000 group_local-0.0.23/setup.py
```

### Comparing `group_local-0.0.22/PKG-INFO` & `group_local-0.0.23/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: group-local
-Version: 0.0.22
+Version: 0.0.23
 Summary: PyPI Package for Circles group-local Python
 Home-page: https://github.com/circles-zone/group-main-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: PyMySQL>=1.0.2
 Requires-Dist: pytest>=7.4.0
 Requires-Dist: mysql-connector>=2.2.9
 Requires-Dist: logzio-python-handler>=4.1.0
 Requires-Dist: database-infrastructure-local>=0.0.23
-Requires-Dist: user-context-remote>=0.0.58
+Requires-Dist: user-context-remote>=0.0.77
 
 PyPI Package for Circles group-local Python
```

### Comparing `group_local-0.0.22/group_local/src/group_local.py` & `group_local-0.0.23/group_local/src/group_local.py`

 * *Files 13% similar despite different names*

```diff
@@ -57,31 +57,31 @@
                 "description": "description",
                 "is_title_approved": True,
                 "is_description_approved": True,
                 "created_user_id": 1
             }
         """
         logger.start(object={'data': str(group_dict)})
-        group_data_json = {
+        group_data_dict = {
             "name": group_dict.get('name'),
             "hashtag": group_dict.get('hashtag'),
             "is_approved": group_dict.get('is_approved', None),
             "parent_group_id": group_dict.get('parent_group_id'),
             "is_interest": group_dict.get('is_interest'),
             "non_members_visibility_id": group_dict.get('non_members_visibility_id', 1),
             "members_visibility_id": group_dict.get('members_visibility_id', 1),
         }
 
-        group_id = GenericCRUDML.insert(self, data_json=group_data_json, ignore_duplicate=ignore_duplicate)
+        group_id = GenericCRUDML.insert(self, data_dict=group_data_dict, ignore_duplicate=ignore_duplicate)
 
         if not lang_code:
             lang_code = group_dict.get('lang_code') or LangCode.detect_lang_code(group_dict.get('title'))
             if lang_code != LangCode.ENGLISH and lang_code != LangCode.HEBREW:
                 lang_code = LangCode.ENGLISH
-        group_ml_data_json = {
+        group_ml_data_dict = {
             "lang_code": lang_code.value,
             "group_id": group_id,
             "title": group_dict.get('title'),
             "is_main_title": group_dict.get('is_main_title', False),
             "description": group_dict.get('description'),
             "created_user_id": user_context.get_effective_user_id(),
             "created_real_user_id": user_context.get_real_user_id(),
@@ -90,21 +90,21 @@
             "updated_user_id": user_context.get_effective_user_id(),
             "updated_real_user_id": user_context.get_real_user_id(),
             "updated_effective_user_id": user_context.get_effective_user_id(),
             "updated_effective_profile_id": user_context.get_effective_profile_id(),
             "is_title_approved": group_dict.get('is_title_approved', None),
             "is_description_approved": group_dict.get('is_description_approved', None)
         }
-        group_ml_id = GenericCRUDML.insert(self, table_name="group_ml_table", data_json=group_ml_data_json,
+        group_ml_id = GenericCRUDML.insert(self, table_name="group_ml_table", data_dict=group_ml_data_dict,
                                            ignore_duplicate=ignore_duplicate)
 
         logger.end(object={'group_id': group_id, 'group_ml_id': group_ml_id})
         return group_id, group_ml_id
 
-    def upsert_group(self, group_dict: Dict[str, any], data_json_compare: dict = None,
+    def upsert_group(self, group_dict: Dict[str, any], data_dict_compare: dict = None,
                      lang_code: LangCode = None,
                      order_by: str = "") -> dict:
         """
             Returns the new group_id
             group_dict has to include the following
             for group_ml_table:
             title: str, lang_code: str = None,
@@ -138,53 +138,53 @@
             }
         """
         logger.start(object={'data': str(group_dict)})
         if not lang_code:
             lang_code = group_dict.get('lang_code') or LangCode.detect_lang_code(group_dict.get('title'))
             if lang_code != LangCode.ENGLISH and lang_code != LangCode.HEBREW:
                 lang_code = LangCode.ENGLISH
-        if not data_json_compare:
-            data_json_compare = {
+        if not data_dict_compare:
+            data_dict_compare = {
                 "name": group_dict.get('name'),
             }
-        group_data_json = {
+        group_data_dict = {
             "name": group_dict.get('name'),
             "hashtag": group_dict.get('hashtag'),
             "is_approved": group_dict.get('is_approved', None),
             "parent_group_id": group_dict.get('parent_group_id'),
             "is_interest": group_dict.get('is_interest'),
             "non_members_visibility_id": group_dict.get('non_members_visibility_id', 1),
             "members_visibility_id": group_dict.get('members_visibility_id', 1),
         }
 
-        group_ml_data_json = {
+        group_ml_data_dict = {
             "title": group_dict.get('title'),
             "is_main_title": group_dict.get('is_main_title', False),
             "description": group_dict.get('description'),
             "updated_user_id": user_context.get_effective_user_id(),
             "updated_real_user_id": user_context.get_real_user_id(),
             "updated_effective_user_id": user_context.get_effective_user_id(),
             "updated_effective_profile_id": user_context.get_effective_profile_id(),
             "is_title_approved": group_dict.get('is_title_approved', None),
             "is_description_approved": group_dict.get('is_description_approved', None)
         }
         if "(" and ")" in group_dict.get('title'):
             group_id, group_ml_ids_list = GenericCRUDML.upsert_value_with_abbreviations(
-                self, table_name="group_table", data_json=group_ml_data_json,
-                data_ml_json=group_ml_data_json,
+                self, table_name="group_table", data_dict=group_ml_data_dict,
+                data_ml_json=group_ml_data_dict,
                 ml_table_name="group_ml_table",
                 lang_code=lang_code,
-                data_json_compare=data_json_compare,
+                data_dict_compare=data_dict_compare,
                 compare_view_name="group_ml_also_not_approved_view",
                 order_by=order_by
             )
         else:
             group_id, group_ml_id = GenericCRUDML.upsert_value(
-                self, data_json=group_data_json, data_ml_json=group_ml_data_json,
-                ml_table_name="group_ml_table", data_json_compare=data_json_compare,
+                self, data_dict=group_data_dict, data_ml_json=group_ml_data_dict,
+                ml_table_name="group_ml_table", data_dict_compare=data_dict_compare,
                 lang_code=lang_code, compare_view_name="group_ml_also_not_approved_view",
                 order_by=order_by
             )
             group_ml_ids_list = [group_ml_id]
         upsert_information = {
             "group_id": group_id,
             "group_ml_ids_list": group_ml_ids_list
@@ -192,29 +192,29 @@
 
         # TODO Shall we add upsert_informaiton to the logger.end()?
         logger.end(object={'group_id': group_id, 'group_ml_ids_list': group_ml_ids_list})
         return upsert_information
 
     def update_group(self, group_id: int, group_dict: Dict[str, any], lang_code: LangCode = None) -> None:
         logger.start(object={'group_id': group_id, 'data': str(group_dict)})
-        group_data_json = {
+        group_data_dict = {
             "name": group_dict.get('name'),
             "hashtag": group_dict.get('hashtag'),
             "is_approved": group_dict.get('is_approved', None),
             "parent_group_id": group_dict.get('parent_group_id'),
             "is_interest": group_dict.get('is_interest'),
             "non_members_visibility_id": group_dict.get('non_members_visibility_id', 1),
             "members_visibility_id": group_dict.get('members_visibility_id', 1),
         }
-        GenericCRUDML.update_by_id(self, id_column_value=group_id, data_json=group_data_json)
+        GenericCRUDML.update_by_id(self, id_column_value=group_id, data_dict=group_data_dict)
         if not lang_code:
             lang_code = group_dict.get('lang_code') or LangCode.detect_lang_code(group_dict.get('title'))
             if lang_code != LangCode.ENGLISH and lang_code != LangCode.HEBREW:
                 lang_code = LangCode.ENGLISH
-        group_ml_data_json = {
+        group_ml_data_dict = {
             "group_id": group_id,
             "lang_code": lang_code.value,
             "title": group_dict.get('title'),
             "is_main_title": group_dict.get('is_main_title', True),
             "description": group_dict.get('description'),
             "updated_user_id": user_context.get_effective_user_id(),
             "updated_real_user_id": user_context.get_real_user_id(),
@@ -224,15 +224,15 @@
             "is_description_approved": group_dict.get('is_description_approved', None)
         }
         where_clause = "group_id = %s AND lang_code = %s"
         GenericCRUDML.update_by_where(
             self, table_name="group_ml_table",
             where=where_clause,
             params=(group_id, lang_code.value),
-            data_json=group_ml_data_json
+            data_dict=group_ml_data_dict
         )
         logger.end()
 
     def get_group_dict_by_group_id(self, group_id: int, group_ml_id: int = None,
                                    view_name: str = "group_view",
                                    ml_view_name: str = "group_ml_also_not_approved_view") -> Dict[str, any]:
         logger.start(object={'group_id': group_id})
```

### Comparing `group_local-0.0.22/group_local/src/group_local_constants.py` & `group_local-0.0.23/group_local/src/group_local_constants.py`

 * *Files identical despite different names*

### Comparing `group_local-0.0.22/group_local.egg-info/PKG-INFO` & `group_local-0.0.23/group_local.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: group-local
-Version: 0.0.22
+Version: 0.0.23
 Summary: PyPI Package for Circles group-local Python
 Home-page: https://github.com/circles-zone/group-main-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: PyMySQL>=1.0.2
 Requires-Dist: pytest>=7.4.0
 Requires-Dist: mysql-connector>=2.2.9
 Requires-Dist: logzio-python-handler>=4.1.0
 Requires-Dist: database-infrastructure-local>=0.0.23
-Requires-Dist: user-context-remote>=0.0.58
+Requires-Dist: user-context-remote>=0.0.77
 
 PyPI Package for Circles group-local Python
```

### Comparing `group_local-0.0.22/setup.py` & `group_local-0.0.23/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "group-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,  # https://pypi.org/project/group-local
-    version='0.0.22',
+    version='0.0.23',
     author="Circles",
     author_email="info@circles.life",
     description="PyPI Package for Circles group-local Python",
     long_description="PyPI Package for Circles group-local Python",
     long_description_content_type='text/markdown',
     url="https://github.com/circles-zone/group-main-local-python-package",
     packages=[package_dir],
@@ -22,10 +22,10 @@
     ],
     install_requires=[
         'PyMySQL>=1.0.2',
         'pytest>=7.4.0',
         'mysql-connector>=2.2.9',
         'logzio-python-handler>= 4.1.0',
         'database-infrastructure-local>=0.0.23',
-        'user-context-remote>=0.0.58'
+        'user-context-remote>=0.0.77'
     ],
 )
```

