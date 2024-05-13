# Comparing `tmp/contact_user_external_local-0.0.3.tar.gz` & `tmp/contact_user_external_local-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contact_user_external_local-0.0.3.tar", last modified: Fri May 10 04:05:55 2024, max compression
+gzip compressed data, was "contact_user_external_local-0.0.4.tar", last modified: Mon May 13 11:35:09 2024, max compression
```

## Comparing `contact_user_external_local-0.0.3.tar` & `contact_user_external_local-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:05:55.796910 contact_user_external_local-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-10 04:05:55.796910 contact_user_external_local-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-10 04:05:35.000000 contact_user_external_local-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:05:55.796910 contact_user_external_local-0.0.3/contact_user_external_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:05:55.796910 contact_user_external_local-0.0.3/contact_user_external_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 04:05:35.000000 contact_user_external_local-0.0.3/contact_user_external_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6469 2024-05-10 04:05:35.000000 contact_user_external_local-0.0.3/contact_user_external_local/src/contact_user_external_local.py
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-10 04:05:35.000000 contact_user_external_local-0.0.3/contact_user_external_local/src/contact_user_external_local_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:05:55.796910 contact_user_external_local-0.0.3/contact_user_external_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-10 04:05:55.000000 contact_user_external_local-0.0.3/contact_user_external_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-10 04:05:55.000000 contact_user_external_local-0.0.3/contact_user_external_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 04:05:55.000000 contact_user_external_local-0.0.3/contact_user_external_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-10 04:05:55.000000 contact_user_external_local-0.0.3/contact_user_external_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-10 04:05:55.000000 contact_user_external_local-0.0.3/contact_user_external_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-10 04:05:35.000000 contact_user_external_local-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 04:05:55.796910 contact_user_external_local-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-10 04:05:35.000000 contact_user_external_local-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:35:09.082780 contact_user_external_local-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-13 11:35:09.082780 contact_user_external_local-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-13 11:34:53.000000 contact_user_external_local-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:35:09.082780 contact_user_external_local-0.0.4/contact_user_external_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:35:09.082780 contact_user_external_local-0.0.4/contact_user_external_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 11:34:53.000000 contact_user_external_local-0.0.4/contact_user_external_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6551 2024-05-13 11:34:53.000000 contact_user_external_local-0.0.4/contact_user_external_local/src/contact_user_external_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-13 11:34:53.000000 contact_user_external_local-0.0.4/contact_user_external_local/src/contact_user_external_local_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:35:09.082780 contact_user_external_local-0.0.4/contact_user_external_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-13 11:35:09.000000 contact_user_external_local-0.0.4/contact_user_external_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-13 11:35:09.000000 contact_user_external_local-0.0.4/contact_user_external_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 11:35:09.000000 contact_user_external_local-0.0.4/contact_user_external_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-13 11:35:09.000000 contact_user_external_local-0.0.4/contact_user_external_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-13 11:35:09.000000 contact_user_external_local-0.0.4/contact_user_external_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-13 11:34:53.000000 contact_user_external_local-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 11:35:09.082780 contact_user_external_local-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-13 11:34:53.000000 contact_user_external_local-0.0.4/setup.py
```

### Comparing `contact_user_external_local-0.0.3/PKG-INFO` & `contact_user_external_local-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contact-user-external-local
-Version: 0.0.3
+Version: 0.0.4
 Summary: PyPI Package for Circles contact-user-external-local Python
 Home-page: https://github.com/circles-zone/contact-user-external-local-python-package
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `contact_user_external_local-0.0.3/contact_user_external_local/src/contact_user_external_local.py` & `contact_user_external_local-0.0.4/contact_user_external_local/src/contact_user_external_local.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,25 +87,27 @@
                 order_by="start_timestamp DESC")
             if not user_external_id:
                 exception_message = "user_external_id not found"
                 logger.exception(exception_message)
                 raise Exception(exception_message)
             contact_user_external_id = self.insert_mapping(
                 entity_name1=self.default_entity_name1, entity_name2=self.default_entity_name2,
-                entity_id1=contact_id, entity_id2=user_external_id)
+                entity_id1=contact_id, entity_id2=user_external_id,
+                ignore_duplicate=True)
         else:
             # link to existing user_external
             logger.info(log_message="user_external_id is not None, linking to existing user_external")
             mapping_tuple = self.select_multi_mapping_tuple_by_id(
                 entity_name1=self.default_entity_name1, entity_name2=self.default_entity_name2,
                 entity_id1=contact_id, entity_id2=user_external_id)
             if not mapping_tuple:
                 logger.info(log_message="mapping_tuple is None, creating new mapping")
                 contact_user_external_id = self.insert_mapping(
                     entity_name1=self.default_entity_name1, entity_name2=self.default_entity_name2,
-                    entity_id1=contact_id, entity_id2=user_external_id)
+                    entity_id1=contact_id, entity_id2=user_external_id,
+                    ignore_duplicate=True)
             else:
                 logger.info(log_message="mapping_tuple is not None")
                 contact_user_external_id = mapping_tuple[0]
 
         logger.end(object={"contact_user_external_id": contact_user_external_id})
         return contact_user_external_id
```

### Comparing `contact_user_external_local-0.0.3/contact_user_external_local/src/contact_user_external_local_constants.py` & `contact_user_external_local-0.0.4/contact_user_external_local/src/contact_user_external_local_constants.py`

 * *Files identical despite different names*

### Comparing `contact_user_external_local-0.0.3/contact_user_external_local.egg-info/PKG-INFO` & `contact_user_external_local-0.0.4/contact_user_external_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contact-user-external-local
-Version: 0.0.3
+Version: 0.0.4
 Summary: PyPI Package for Circles contact-user-external-local Python
 Home-page: https://github.com/circles-zone/contact-user-external-local-python-package
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `contact_user_external_local-0.0.3/setup.py` & `contact_user_external_local-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "contact-user-external-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.3',  # https://pypi.org/project/contact-user-external-local/
+    version='0.0.4',  # https://pypi.org/project/contact-user-external-local/
     author="Circles",
     author_email="info@circlez.ai",
     description="PyPI Package for Circles contact-user-external-local Python",
     long_description="PyPI Package for Circles contact-user-external-local Python",
     long_description_content_type='text/markdown',
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     package_dir={package_dir: f'{package_dir}/src'},
```

