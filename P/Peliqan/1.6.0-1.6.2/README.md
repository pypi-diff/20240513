# Comparing `tmp/Peliqan-1.6.0.tar.gz` & `tmp/Peliqan-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Peliqan-1.6.0.tar", last modified: Wed May  8 06:43:12 2024, max compression
+gzip compressed data, was "Peliqan-1.6.2.tar", last modified: Mon May 13 15:08:53 2024, max compression
```

## Comparing `Peliqan-1.6.0.tar` & `Peliqan-1.6.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 sudarshanv.s.   (501) staff       (20)        0 2024-05-08 06:43:12.826866 Peliqan-1.6.0/
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      665 2024-05-08 06:43:12.826574 Peliqan-1.6.0/PKG-INFO
-drwxr-xr-x   0 sudarshanv.s.   (501) staff       (20)        0 2024-05-08 06:43:12.818428 Peliqan-1.6.0/Peliqan.egg-info/
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      665 2024-05-08 06:43:12.000000 Peliqan-1.6.0/Peliqan.egg-info/PKG-INFO
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      437 2024-05-08 06:43:12.000000 Peliqan-1.6.0/Peliqan.egg-info/SOURCES.txt
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)        1 2024-05-08 06:43:12.000000 Peliqan-1.6.0/Peliqan.egg-info/dependency_links.txt
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)       16 2024-05-08 06:43:12.000000 Peliqan-1.6.0/Peliqan.egg-info/requires.txt
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)        8 2024-05-08 06:43:12.000000 Peliqan-1.6.0/Peliqan.egg-info/top_level.txt
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)     1411 2023-08-02 11:35:09.000000 Peliqan-1.6.0/README.md
-drwxr-xr-x   0 sudarshanv.s.   (501) staff       (20)        0 2024-05-08 06:43:12.822224 Peliqan-1.6.0/peliqan/
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      872 2024-05-07 13:16:48.000000 Peliqan-1.6.0/peliqan/__init__.py
-drwxr-xr-x   0 sudarshanv.s.   (501) staff       (20)        0 2024-05-08 06:43:12.826061 Peliqan-1.6.0/peliqan/client/
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      421 2023-11-07 06:42:14.000000 Peliqan-1.6.0/peliqan/client/__init__.py
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)    17466 2024-05-07 13:12:03.000000 Peliqan-1.6.0/peliqan/client/backend_service.py
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)     2657 2024-04-22 06:47:06.000000 Peliqan-1.6.0/peliqan/client/base.py
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)    10609 2024-04-23 09:30:50.000000 Peliqan-1.6.0/peliqan/client/dbclient.py
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      928 2023-09-12 06:13:12.000000 Peliqan-1.6.0/peliqan/client/sftpclient.py
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)     4549 2024-04-23 09:30:50.000000 Peliqan-1.6.0/peliqan/client/writeback.py
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)    28999 2024-05-07 13:10:02.000000 Peliqan-1.6.0/peliqan/core.py
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      393 2024-04-22 06:47:06.000000 Peliqan-1.6.0/peliqan/exceptions.py
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)    20342 2024-03-21 07:17:47.000000 Peliqan-1.6.0/peliqan/local_test.py
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)       40 2024-05-07 09:05:00.000000 Peliqan-1.6.0/peliqan/utils.py
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)       38 2024-05-08 06:43:12.826951 Peliqan-1.6.0/setup.cfg
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)     1371 2024-04-22 06:47:06.000000 Peliqan-1.6.0/setup.py
+drwxr-xr-x   0 sudarshanv.s.   (501) staff       (20)        0 2024-05-13 15:08:53.686333 Peliqan-1.6.2/
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      665 2024-05-13 15:08:53.686174 Peliqan-1.6.2/PKG-INFO
+drwxr-xr-x   0 sudarshanv.s.   (501) staff       (20)        0 2024-05-13 15:08:53.682064 Peliqan-1.6.2/Peliqan.egg-info/
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      665 2024-05-13 15:08:53.000000 Peliqan-1.6.2/Peliqan.egg-info/PKG-INFO
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      437 2024-05-13 15:08:53.000000 Peliqan-1.6.2/Peliqan.egg-info/SOURCES.txt
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)        1 2024-05-13 15:08:53.000000 Peliqan-1.6.2/Peliqan.egg-info/dependency_links.txt
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)       16 2024-05-13 15:08:53.000000 Peliqan-1.6.2/Peliqan.egg-info/requires.txt
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)        8 2024-05-13 15:08:53.000000 Peliqan-1.6.2/Peliqan.egg-info/top_level.txt
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)     1411 2023-08-02 11:35:09.000000 Peliqan-1.6.2/README.md
+drwxr-xr-x   0 sudarshanv.s.   (501) staff       (20)        0 2024-05-13 15:08:53.683782 Peliqan-1.6.2/peliqan/
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      872 2024-05-13 13:52:39.000000 Peliqan-1.6.2/peliqan/__init__.py
+drwxr-xr-x   0 sudarshanv.s.   (501) staff       (20)        0 2024-05-13 15:08:53.685734 Peliqan-1.6.2/peliqan/client/
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      421 2024-05-13 13:01:35.000000 Peliqan-1.6.2/peliqan/client/__init__.py
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)    17466 2024-05-13 13:01:35.000000 Peliqan-1.6.2/peliqan/client/backend_service.py
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)     2747 2024-05-13 14:34:03.000000 Peliqan-1.6.2/peliqan/client/base.py
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)    10609 2024-05-13 13:01:35.000000 Peliqan-1.6.2/peliqan/client/dbclient.py
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      928 2024-05-13 13:01:35.000000 Peliqan-1.6.2/peliqan/client/sftpclient.py
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)     4549 2024-05-13 13:01:35.000000 Peliqan-1.6.2/peliqan/client/writeback.py
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)    28778 2024-05-13 13:50:10.000000 Peliqan-1.6.2/peliqan/core.py
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      393 2024-05-10 06:48:15.000000 Peliqan-1.6.2/peliqan/exceptions.py
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)    20342 2024-03-21 07:17:47.000000 Peliqan-1.6.2/peliqan/local_test.py
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)       40 2024-05-10 13:32:52.000000 Peliqan-1.6.2/peliqan/utils.py
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)       38 2024-05-13 15:08:53.686392 Peliqan-1.6.2/setup.cfg
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)     1371 2024-05-10 06:48:22.000000 Peliqan-1.6.2/setup.py
```

### Comparing `Peliqan-1.6.0/PKG-INFO` & `Peliqan-1.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Peliqan
-Version: 1.6.0
+Version: 1.6.2
 Summary: This package is an sdk that allows any python client to connect with a Peliqan environment.
 Home-page: https://peliqan.io/
 Author: Peliqan.io
 Author-email: dev@peliqan.io
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `Peliqan-1.6.0/Peliqan.egg-info/PKG-INFO` & `Peliqan-1.6.2/Peliqan.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Peliqan
-Version: 1.6.0
+Version: 1.6.2
 Summary: This package is an sdk that allows any python client to connect with a Peliqan environment.
 Home-page: https://peliqan.io/
 Author: Peliqan.io
 Author-email: dev@peliqan.io
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `Peliqan-1.6.0/README.md` & `Peliqan-1.6.2/README.md`

 * *Files identical despite different names*

### Comparing `Peliqan-1.6.0/peliqan/__init__.py` & `Peliqan-1.6.2/peliqan/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.6.0"
+__version__ = "1.6.2"
 __author__ = 'Peliqan.io'
 __credits__ = 'Peliqan.io'
 
 __all__ = [
     "Peliqan",
     "BasePeliqanClient"
 ]
```

### Comparing `Peliqan-1.6.0/peliqan/client/backend_service.py` & `Peliqan-1.6.2/peliqan/client/backend_service.py`

 * *Files identical despite different names*

### Comparing `Peliqan-1.6.0/peliqan/client/base.py` & `Peliqan-1.6.2/peliqan/client/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,31 +2,33 @@
 
 import requests
 
 from peliqan.exceptions import PeliqanClientException, PeliqanJsonSerializerException
 
 
 def _serialize_data(obj):
-    if type(obj) == dict:
+    if isinstance(obj, dict):
         for k in obj:
             obj[k] = _serialize_data(obj[k])
 
         formatted_obj = obj
     elif type(obj) in (list, tuple):
-        if type(obj) == tuple:
-            obj = list(obj)
-
         obj_len = len(obj)
         for i in range(obj_len):
             obj[i] = _serialize_data(obj[i])
 
         formatted_obj = obj
 
-    elif isinstance(obj, (int, float, type(None), str)):
+    elif isinstance(obj, (int, float, str)):
         formatted_obj = obj
+        if isinstance(obj, float) and str(obj) == 'nan':
+            formatted_obj = None
+
+    elif isinstance(obj, type(None)):
+        formatted_obj = None
 
     else:
         try:
             formatted_obj = JSONEncoder().encode(obj)
         except Exception as e:
             try:
                 formatted_obj = str(obj)
```

### Comparing `Peliqan-1.6.0/peliqan/client/dbclient.py` & `Peliqan-1.6.2/peliqan/client/dbclient.py`

 * *Files identical despite different names*

### Comparing `Peliqan-1.6.0/peliqan/client/sftpclient.py` & `Peliqan-1.6.2/peliqan/client/sftpclient.py`

 * *Files identical despite different names*

### Comparing `Peliqan-1.6.0/peliqan/client/writeback.py` & `Peliqan-1.6.2/peliqan/client/writeback.py`

 * *Files identical despite different names*

### Comparing `Peliqan-1.6.0/peliqan/core.py` & `Peliqan-1.6.2/peliqan/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -175,15 +175,15 @@
                 interval = 10
 
             response = refresh_func()
             running = response.get('running', True)
             if not running:
                 return {
                     'task_id': response['task_id'],
-                    'run_id': response['run_id'],
+                    'run_id': response.get('run_id'),
                     'detail': 'The sync task has completed.',
                     'syncing': False
                 }
 
             time.sleep(interval)
             count += 1
 
@@ -553,37 +553,36 @@
         If a column does not exist in one of the tables, it will be added with a null value.
         Optionally, a "source" column can be added to indicate from which table each row originated.
 
         :param table_ids: required, list of integers, list of table ids to include in UNION query
         :param sources: optional, dict, if set an extra 'source' column will be added to indicate to which table the record belongs. Keys are table ids. Values are source value to include in UNION result. Example: { 1: "Paris", 2: "London" }. This will add a column "source" to the UNION where all records from table id 1 will have value "Paris" for the source.
         :return: result of update
         """
-        databases = self.__service_client__.list_databases()
+
         tables = []
         fields = []
         field_types = {}
         fields_to_cast = []
-        for database in databases:
-            for table in database["tables"]:
-                if table["id"] in table_ids:
-                    tables.append(table)
-                    for field in table["all_fields"]:
-                        if field["name"] not in fields:
-                            fields.append(field["name"])
-                            if field["sql_data_type"]:
-                                # Actual field type in source, e.g. timestamp, timestamptz...
-                                # (might not be available for all sources)
-                                field_types[field["name"]] = field["sql_data_type"]
-                            else:
-                                # Peliqan field type, e.g. "date"
-                                field_types[field["name"]] = field["type"]
-                        elif (
-                            field["sql_data_type"] and field["sql_data_type"] != field_types[field["name"]]
-                        ) or field["type"] != field_types[field["name"]]:
-                            fields_to_cast.append(field["name"])
+        for table_id in table_ids:
+            table = self.get_table(table_id)
+            tables.append(table)
+            for field in table["all_fields"]:
+                if field["name"] not in fields:
+                    fields.append(field["name"])
+                    if field["sql_data_type"]:
+                        # Actual field type in source, e.g. timestamp, timestamptz...
+                        # (might not be available for all sources)
+                        field_types[field["name"]] = field["sql_data_type"]
+                    else:
+                        # Peliqan field type, e.g. "date"
+                        field_types[field["name"]] = field["type"]
+                elif (
+                    field["sql_data_type"] and field["sql_data_type"] != field_types[field["name"]]
+                ) or field["type"] != field_types[field["name"]]:
+                    fields_to_cast.append(field["name"])
 
         table_selects = []
         for table in tables:
             table_select_fields = []
             if sources:
                 source_name = ""
                 for source_table_id, source_table_name in sources.items():
```

### Comparing `Peliqan-1.6.0/peliqan/local_test.py` & `Peliqan-1.6.2/peliqan/local_test.py`

 * *Files identical despite different names*

### Comparing `Peliqan-1.6.0/setup.py` & `Peliqan-1.6.2/setup.py`

 * *Files identical despite different names*

