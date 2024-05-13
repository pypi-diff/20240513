# Comparing `tmp/DynamicAnnotationDB-5.8.1.tar.gz` & `tmp/DynamicAnnotationDB-5.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/DynamicAnnotationDB-5.8.1.tar", last modified: Mon Oct 16 02:23:52 2023, max compression
+gzip compressed data, was "DynamicAnnotationDB-5.9.0.tar", last modified: Mon May 13 19:47:14 2024, max compression
```

## Comparing `DynamicAnnotationDB-5.8.1.tar` & `DynamicAnnotationDB-5.9.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-10-16 02:23:52.488432 DynamicAnnotationDB-5.8.1/
-drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-10-16 02:23:52.478344 DynamicAnnotationDB-5.8.1/DynamicAnnotationDB.egg-info/
--rw-r--r--   0 forrestc   (503) staff       (20)      920 2023-10-16 02:23:52.000000 DynamicAnnotationDB-5.8.1/DynamicAnnotationDB.egg-info/PKG-INFO
--rw-r--r--   0 forrestc   (503) staff       (20)     1821 2023-10-16 02:23:52.000000 DynamicAnnotationDB-5.8.1/DynamicAnnotationDB.egg-info/SOURCES.txt
--rw-r--r--   0 forrestc   (503) staff       (20)        1 2023-10-16 02:23:52.000000 DynamicAnnotationDB-5.8.1/DynamicAnnotationDB.egg-info/dependency_links.txt
--rw-r--r--   0 forrestc   (503) staff       (20)      125 2023-10-16 02:23:52.000000 DynamicAnnotationDB-5.8.1/DynamicAnnotationDB.egg-info/requires.txt
--rw-r--r--   0 forrestc   (503) staff       (20)       26 2023-10-16 02:23:52.000000 DynamicAnnotationDB-5.8.1/DynamicAnnotationDB.egg-info/top_level.txt
--rw-r--r--   0 forrestc   (503) staff       (20)       36 2020-06-11 04:40:08.000000 DynamicAnnotationDB-5.8.1/MANIFEST.in
--rw-r--r--   0 forrestc   (503) staff       (20)      920 2023-10-16 02:23:52.488563 DynamicAnnotationDB-5.8.1/PKG-INFO
--rw-r--r--   0 forrestc   (503) staff       (20)      474 2022-02-12 21:27:58.000000 DynamicAnnotationDB-5.8.1/README.md
--rw-r--r--   0 forrestc   (503) staff       (20)       67 2021-06-03 21:07:33.000000 DynamicAnnotationDB-5.8.1/doc_requirements.txt
-drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-10-16 02:23:52.480988 DynamicAnnotationDB-5.8.1/dynamicannotationdb/
--rw-r--r--   0 forrestc   (503) staff       (20)       72 2023-10-16 02:23:48.000000 DynamicAnnotationDB-5.8.1/dynamicannotationdb/__init__.py
--rw-r--r--   0 forrestc   (503) staff       (20)    18101 2023-05-04 23:03:31.000000 DynamicAnnotationDB-5.8.1/dynamicannotationdb/annotation.py
--rw-r--r--   0 forrestc   (503) staff       (20)    14211 2023-10-16 02:22:50.000000 DynamicAnnotationDB-5.8.1/dynamicannotationdb/database.py
--rw-r--r--   0 forrestc   (503) staff       (20)     2064 2023-02-17 16:48:08.000000 DynamicAnnotationDB-5.8.1/dynamicannotationdb/errors.py
--rw-r--r--   0 forrestc   (503) staff       (20)     5969 2023-04-18 17:23:16.000000 DynamicAnnotationDB-5.8.1/dynamicannotationdb/interface.py
--rw-r--r--   0 forrestc   (503) staff       (20)     1139 2022-06-23 21:40:16.000000 DynamicAnnotationDB-5.8.1/dynamicannotationdb/key_utils.py
-drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-10-16 02:23:52.481680 DynamicAnnotationDB-5.8.1/dynamicannotationdb/migration/
--rw-r--r--   0 forrestc   (503) staff       (20)      166 2023-10-16 02:23:48.000000 DynamicAnnotationDB-5.8.1/dynamicannotationdb/migration/__init__.py
-drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-10-16 02:23:52.482708 DynamicAnnotationDB-5.8.1/dynamicannotationdb/migration/alembic/
--rw-r--r--   0 forrestc   (503) staff       (20)        0 2022-10-17 01:08:23.000000 DynamicAnnotationDB-5.8.1/dynamicannotationdb/migration/alembic/__init__.py
--rw-r--r--   0 forrestc   (503) staff       (20)     2373 2023-04-06 22:59:46.000000 DynamicAnnotationDB-5.8.1/dynamicannotationdb/migration/alembic/env.py
--rw-r--r--   0 forrestc   (503) staff       (20)     1100 2022-10-17 01:08:23.000000 DynamicAnnotationDB-5.8.1/dynamicannotationdb/migration/alembic/run.py
-drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-10-16 02:23:52.485897 DynamicAnnotationDB-5.8.1/dynamicannotationdb/migration/alembic/versions/
--rw-r--r--   0 forrestc   (503) staff       (20)      747 2022-10-25 16:40:35.000000 DynamicAnnotationDB-5.8.1/dynamicannotationdb/migration/alembic/versions/309cf493a1e2_adding_warning_field.py
--rw-r--r--   0 forrestc   (503) staff       (20)      969 2022-10-17 01:08:23.000000 DynamicAnnotationDB-5.8.1/dynamicannotationdb/migration/alembic/versions/5a1d7c0ad006_add_status_column.py
--rw-r--r--   0 forrestc   (503) staff       (20)      515 2022-10-17 01:08:23.000000 DynamicAnnotationDB-5.8.1/dynamicannotationdb/migration/alembic/versions/6e7f580ff680_add_error_msg.py
--rw-r--r--   0 forrestc   (503) staff       (20)     1255 2023-04-06 22:59:46.000000 DynamicAnnotationDB-5.8.1/dynamicannotationdb/migration/alembic/versions/7c79eff751b4_add_parent_version_column.py
--rw-r--r--   0 forrestc   (503) staff       (20)     1063 2022-10-17 01:08:23.000000 DynamicAnnotationDB-5.8.1/dynamicannotationdb/migration/alembic/versions/814d72d74e3b_add_version_error_table.py
--rw-r--r--   0 forrestc   (503) staff       (20)     2066 2022-10-25 19:07:59.000000 DynamicAnnotationDB-5.8.1/dynamicannotationdb/migration/alembic/versions/8fdc843fc202_adding_permission_and_last_modified.py
--rw-r--r--   0 forrestc   (503) staff       (20)      685 2022-10-17 01:08:23.000000 DynamicAnnotationDB-5.8.1/dynamicannotationdb/migration/alembic/versions/975a79461cab_add_is_merged.py
--rw-r--r--   0 forrestc   (503) staff       (20)        0 2022-10-17 01:08:23.000000 DynamicAnnotationDB-5.8.1/dynamicannotationdb/migration/alembic/versions/__init__.py
--rw-r--r--   0 forrestc   (503) staff       (20)     4403 2023-04-06 22:59:46.000000 DynamicAnnotationDB-5.8.1/dynamicannotationdb/migration/alembic/versions/ef5c2d7f96d8_initial_live_db_models.py
--rw-r--r--   0 forrestc   (503) staff       (20)     1102 2023-03-14 16:48:52.000000 DynamicAnnotationDB-5.8.1/dynamicannotationdb/migration/alembic/versions/fac66b439033_add_view_model.py
--rw-r--r--   0 forrestc   (503) staff       (20)    22717 2023-04-19 23:49:05.000000 DynamicAnnotationDB-5.8.1/dynamicannotationdb/migration/migrate.py
--rw-r--r--   0 forrestc   (503) staff       (20)     6017 2023-04-19 14:20:52.000000 DynamicAnnotationDB-5.8.1/dynamicannotationdb/models.py
--rw-r--r--   0 forrestc   (503) staff       (20)     8351 2023-10-10 03:51:46.000000 DynamicAnnotationDB-5.8.1/dynamicannotationdb/schema.py
--rw-r--r--   0 forrestc   (503) staff       (20)    13779 2022-10-17 01:08:23.000000 DynamicAnnotationDB-5.8.1/dynamicannotationdb/segmentation.py
--rw-r--r--   0 forrestc   (503) staff       (20)      124 2022-11-21 01:05:53.000000 DynamicAnnotationDB-5.8.1/requirements.txt
--rw-r--r--   0 forrestc   (503) staff       (20)      140 2023-10-16 02:23:52.488954 DynamicAnnotationDB-5.8.1/setup.cfg
--rw-r--r--   0 forrestc   (503) staff       (20)     1303 2022-02-12 21:27:58.000000 DynamicAnnotationDB-5.8.1/setup.py
--rw-r--r--   0 forrestc   (503) staff       (20)       68 2021-06-03 21:07:33.000000 DynamicAnnotationDB-5.8.1/test_requirements.txt
-drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-10-16 02:23:52.488143 DynamicAnnotationDB-5.8.1/tests/
--rw-r--r--   0 forrestc   (503) staff       (20)        0 2021-02-19 03:45:38.000000 DynamicAnnotationDB-5.8.1/tests/__init__.py
--rw-r--r--   0 forrestc   (503) staff       (20)     3308 2022-06-23 21:40:16.000000 DynamicAnnotationDB-5.8.1/tests/conftest.py
--rw-r--r--   0 forrestc   (503) staff       (20)     7393 2023-02-17 16:48:08.000000 DynamicAnnotationDB-5.8.1/tests/test_annotation.py
--rw-r--r--   0 forrestc   (503) staff       (20)     3799 2023-02-17 16:48:08.000000 DynamicAnnotationDB-5.8.1/tests/test_database.py
--rw-r--r--   0 forrestc   (503) staff       (20)     1433 2022-06-23 21:40:16.000000 DynamicAnnotationDB-5.8.1/tests/test_errors.py
--rw-r--r--   0 forrestc   (503) staff       (20)      391 2022-06-23 21:40:16.000000 DynamicAnnotationDB-5.8.1/tests/test_interface.py
--rw-r--r--   0 forrestc   (503) staff       (20)     3982 2022-09-13 20:07:43.000000 DynamicAnnotationDB-5.8.1/tests/test_schema.py
--rw-r--r--   0 forrestc   (503) staff       (20)     5705 2023-02-17 16:48:08.000000 DynamicAnnotationDB-5.8.1/tests/test_segmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:47:14.713708 DynamicAnnotationDB-5.9.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:47:14.705708 DynamicAnnotationDB-5.9.0/DynamicAnnotationDB.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-13 19:47:14.000000 DynamicAnnotationDB-5.9.0/DynamicAnnotationDB.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-05-13 19:47:14.000000 DynamicAnnotationDB-5.9.0/DynamicAnnotationDB.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 19:47:14.000000 DynamicAnnotationDB-5.9.0/DynamicAnnotationDB.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-13 19:47:14.000000 DynamicAnnotationDB-5.9.0/DynamicAnnotationDB.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-13 19:47:14.000000 DynamicAnnotationDB-5.9.0/DynamicAnnotationDB.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-13 19:47:12.000000 DynamicAnnotationDB-5.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-13 19:47:14.713708 DynamicAnnotationDB-5.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-13 19:47:12.000000 DynamicAnnotationDB-5.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-13 19:47:12.000000 DynamicAnnotationDB-5.9.0/doc_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:47:14.709708 DynamicAnnotationDB-5.9.0/dynamicannotationdb/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-13 19:47:12.000000 DynamicAnnotationDB-5.9.0/dynamicannotationdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15813 2024-05-13 19:47:12.000000 DynamicAnnotationDB-5.9.0/dynamicannotationdb/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14211 2024-05-13 19:47:12.000000 DynamicAnnotationDB-5.9.0/dynamicannotationdb/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-05-13 19:47:12.000000 DynamicAnnotationDB-5.9.0/dynamicannotationdb/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5969 2024-05-13 19:47:12.000000 DynamicAnnotationDB-5.9.0/dynamicannotationdb/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-13 19:47:12.000000 DynamicAnnotationDB-5.9.0/dynamicannotationdb/key_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:47:14.709708 DynamicAnnotationDB-5.9.0/dynamicannotationdb/migration/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-13 19:47:12.000000 DynamicAnnotationDB-5.9.0/dynamicannotationdb/migration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:47:14.709708 DynamicAnnotationDB-5.9.0/dynamicannotationdb/migration/alembic/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 19:47:12.000000 DynamicAnnotationDB-5.9.0/dynamicannotationdb/migration/alembic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-05-13 19:47:12.000000 DynamicAnnotationDB-5.9.0/dynamicannotationdb/migration/alembic/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-13 19:47:12.000000 DynamicAnnotationDB-5.9.0/dynamicannotationdb/migration/alembic/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:47:14.709708 DynamicAnnotationDB-5.9.0/dynamicannotationdb/migration/alembic/versions/
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-13 19:47:12.000000 DynamicAnnotationDB-5.9.0/dynamicannotationdb/migration/alembic/versions/309cf493a1e2_adding_warning_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-13 19:47:12.000000 DynamicAnnotationDB-5.9.0/dynamicannotationdb/migration/alembic/versions/5a1d7c0ad006_add_status_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-13 19:47:12.000000 DynamicAnnotationDB-5.9.0/dynamicannotationdb/migration/alembic/versions/6e7f580ff680_add_error_msg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-05-13 19:47:12.000000 DynamicAnnotationDB-5.9.0/dynamicannotationdb/migration/alembic/versions/7c79eff751b4_add_parent_version_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-13 19:47:12.000000 DynamicAnnotationDB-5.9.0/dynamicannotationdb/migration/alembic/versions/814d72d74e3b_add_version_error_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-05-13 19:47:12.000000 DynamicAnnotationDB-5.9.0/dynamicannotationdb/migration/alembic/versions/8fdc843fc202_adding_permission_and_last_modified.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-13 19:47:12.000000 DynamicAnnotationDB-5.9.0/dynamicannotationdb/migration/alembic/versions/975a79461cab_add_is_merged.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 19:47:12.000000 DynamicAnnotationDB-5.9.0/dynamicannotationdb/migration/alembic/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4403 2024-05-13 19:47:12.000000 DynamicAnnotationDB-5.9.0/dynamicannotationdb/migration/alembic/versions/ef5c2d7f96d8_initial_live_db_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-13 19:47:12.000000 DynamicAnnotationDB-5.9.0/dynamicannotationdb/migration/alembic/versions/fac66b439033_add_view_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22717 2024-05-13 19:47:12.000000 DynamicAnnotationDB-5.9.0/dynamicannotationdb/migration/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6017 2024-05-13 19:47:12.000000 DynamicAnnotationDB-5.9.0/dynamicannotationdb/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8351 2024-05-13 19:47:12.000000 DynamicAnnotationDB-5.9.0/dynamicannotationdb/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13779 2024-05-13 19:47:12.000000 DynamicAnnotationDB-5.9.0/dynamicannotationdb/segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-13 19:47:12.000000 DynamicAnnotationDB-5.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-13 19:47:14.713708 DynamicAnnotationDB-5.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-13 19:47:12.000000 DynamicAnnotationDB-5.9.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-13 19:47:12.000000 DynamicAnnotationDB-5.9.0/test_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:47:14.713708 DynamicAnnotationDB-5.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 19:47:12.000000 DynamicAnnotationDB-5.9.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-05-13 19:47:12.000000 DynamicAnnotationDB-5.9.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9900 2024-05-13 19:47:12.000000 DynamicAnnotationDB-5.9.0/tests/test_annotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3799 2024-05-13 19:47:12.000000 DynamicAnnotationDB-5.9.0/tests/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-13 19:47:12.000000 DynamicAnnotationDB-5.9.0/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-13 19:47:12.000000 DynamicAnnotationDB-5.9.0/tests/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3982 2024-05-13 19:47:12.000000 DynamicAnnotationDB-5.9.0/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5705 2024-05-13 19:47:12.000000 DynamicAnnotationDB-5.9.0/tests/test_segmentation.py
```

### Comparing `DynamicAnnotationDB-5.8.1/DynamicAnnotationDB.egg-info/PKG-INFO` & `DynamicAnnotationDB-5.9.0/DynamicAnnotationDB.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DynamicAnnotationDB
-Version: 5.8.1
+Version: 5.9.0
 Summary: Annotation Database pendant to the chunkedgraph
 Home-page: https://github.com/seung-lab/DynamicAnnotationDB
 Author: Sven Dorkenwald, Derrick Brittain
 Author-email: sdorkenw@princeton.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `DynamicAnnotationDB-5.8.1/DynamicAnnotationDB.egg-info/SOURCES.txt` & `DynamicAnnotationDB-5.9.0/DynamicAnnotationDB.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DynamicAnnotationDB-5.8.1/PKG-INFO` & `DynamicAnnotationDB-5.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DynamicAnnotationDB
-Version: 5.8.1
+Version: 5.9.0
 Summary: Annotation Database pendant to the chunkedgraph
 Home-page: https://github.com/seung-lab/DynamicAnnotationDB
 Author: Sven Dorkenwald, Derrick Brittain
 Author-email: sdorkenw@princeton.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `DynamicAnnotationDB-5.8.1/dynamicannotationdb/annotation.py` & `DynamicAnnotationDB-5.9.0/dynamicannotationdb/annotation.py`

 * *Files 12% similar despite different names*

```diff
@@ -92,41 +92,26 @@
 
         with_crud_columns: bool
             add additional columns to track CRUD operations on rows
         """
         existing_tables = self.db._check_table_is_unique(table_name)
 
         if table_metadata:
-            reference_table, track_updates = self.schema._parse_schema_metadata_params(
+            reference_table, _ = self.schema._parse_schema_metadata_params(
                 schema_type, table_name, table_metadata, existing_tables
             )
         else:
             reference_table = None
-            track_updates = None
 
         AnnotationModel = self.schema.create_annotation_model(
             table_name,
             schema_type,
             table_metadata=table_metadata,
             with_crud_columns=with_crud_columns,
         )
-        if hasattr(AnnotationModel, "target_id") and reference_table:
-
-            reference_table_name = self.db.get_table_sql_metadata(reference_table)
-            logging.info(
-                f"{table_name} is targeting reference table: {reference_table_name}"
-            )
-            if track_updates:
-                self.create_reference_update_trigger(
-                    table_name, reference_table, AnnotationModel
-                )
-                description += (
-                    f" [Note: This table '{AnnotationModel.__name__}' will update the 'target_id' "
-                    f"foreign_key when updates are made to the '{reference_table}' table] "
-                )
 
         self.db.base.metadata.tables[AnnotationModel.__name__].create(
             bind=self.db.engine
         )
         creation_time = datetime.datetime.utcnow()
 
         metadata_dict = {
@@ -225,56 +210,14 @@
         for column, value in update_dict.items():
             if hasattr(metadata, str(column)):
                 setattr(metadata, column, value)
         self.db.commit_session()
         logging.info(f"Table: {table_name} metadata updated ")
         return self.db.get_table_metadata(table_name)
 
-    def create_reference_update_trigger(self, table_name, reference_table, model):
-        func_name = f"{table_name}_update_reference_id"
-        func = DDL(
-            f"""
-                    CREATE or REPLACE function {func_name}()
-                    returns TRIGGER
-                    as $func$
-                    begin
-                        if EXISTS
-                            (SELECT 1
-                            FROM information_schema.columns
-                            WHERE table_name='{reference_table}'
-                                AND column_name='superceded_id') THEN
-                            update {table_name} ref
-                            set target_id = new.superceded_id
-                            where ref.target_id = old.id;
-                            return new;
-                        else
-                            return NULL;
-                        END if;
-                    end;
-                    $func$ language plpgsql;
-                    """
-        )
-        trigger = DDL(
-            f"""CREATE TRIGGER update_{table_name}_target_id AFTER UPDATE ON {reference_table}
-                    FOR EACH ROW EXECUTE PROCEDURE {func_name}();"""
-        )
-
-        event.listen(
-            model.__table__,
-            "after_create",
-            func.execute_if(dialect="postgresql"),
-        )
-
-        event.listen(
-            model.__table__,
-            "after_create",
-            trigger.execute_if(dialect="postgresql"),
-        )
-        return True
-
     def delete_table(self, table_name: str) -> bool:
         """Marks a table for deletion, which will
         remove it from user visible calls
         and stop materialization from happening on this table
         only updates metadata to reflect deleted timestamp.
 
         Parameters
@@ -406,15 +349,16 @@
         """Update an annotation
 
         Parameters
         ----------
         table_name : str
             name of targeted table to update annotations
         annotation : dict
-            new data for that annotation
+            new data for that annotation, allows for partial updates but 
+            requires an 'id' field to target the row
 
         Returns
         -------
         dict:
             dict mapping of old id : new id values
 
         Raises
@@ -423,51 +367,52 @@
             Raises if no Ids to be updated are found in the table.
         """
         anno_id = annotation.get("id")
         if not anno_id:
             return "Annotation requires an 'id' to update targeted row"
         schema_type, AnnotationModel = self._load_model(table_name)
 
+        try:
+            old_anno = (
+                self.db.cached_session.query(AnnotationModel)
+                .filter(AnnotationModel.id == anno_id)
+                .one()
+            )
+        except NoAnnotationsFoundWithID as e:
+            raise f"No result found for {anno_id}. Error: {e}" from e
+
+        if old_anno.superceded_id:
+            raise UpdateAnnotationError(anno_id, old_anno.superceded_id)
+
+        # Merge old data with new changes
+        old_data = {
+            column.name: getattr(old_anno, column.name)
+            for column in old_anno.__table__.columns
+        }
+        updated_data = {**old_data, **annotation}
+
         new_annotation, __ = self.schema.split_flattened_schema_data(
-            schema_type, annotation
+            schema_type, updated_data
         )
 
         if hasattr(AnnotationModel, "created"):
             new_annotation["created"] = datetime.datetime.utcnow()
         if hasattr(AnnotationModel, "valid"):
             new_annotation["valid"] = True
 
         new_data = AnnotationModel(**new_annotation)
 
-        try:
-            old_anno = (
-                self.db.cached_session.query(AnnotationModel)
-                .filter(AnnotationModel.id == anno_id)
-                .one()
-            )
-        except NoAnnotationsFoundWithID as e:
-            raise f"No result found for {anno_id}. Error: {e}" from e
-        if hasattr(AnnotationModel, "target_id"):
-            new_data_map = self.db.get_automap_items(new_data)
-            for column_name, value in new_data_map.items():
-                setattr(old_anno, column_name, value)
-            old_anno.valid = True
-            update_map = {anno_id: old_anno.id}
-        else:
-            if old_anno.superceded_id:
-                raise UpdateAnnotationError(anno_id, old_anno.superceded_id)
-
-            self.db.cached_session.add(new_data)
-            self.db.cached_session.flush()
+        self.db.cached_session.add(new_data)
+        self.db.cached_session.flush()
 
-            deleted_time = datetime.datetime.utcnow()
-            old_anno.deleted = deleted_time
-            old_anno.superceded_id = new_data.id
-            old_anno.valid = False
-            update_map = {anno_id: new_data.id}
+        deleted_time = datetime.datetime.utcnow()
+        old_anno.deleted = deleted_time
+        old_anno.superceded_id = new_data.id
+        old_anno.valid = False
+        update_map = {anno_id: new_data.id}
 
         (
             self.db.cached_session.query(AnnoMetadata)
             .filter(AnnoMetadata.table_name == table_name)
             .update({AnnoMetadata.last_modified: datetime.datetime.utcnow()})
         )
         self.db.commit_session()
```

### Comparing `DynamicAnnotationDB-5.8.1/dynamicannotationdb/database.py` & `DynamicAnnotationDB-5.9.0/dynamicannotationdb/database.py`

 * *Files identical despite different names*

### Comparing `DynamicAnnotationDB-5.8.1/dynamicannotationdb/errors.py` & `DynamicAnnotationDB-5.9.0/dynamicannotationdb/errors.py`

 * *Files identical despite different names*

### Comparing `DynamicAnnotationDB-5.8.1/dynamicannotationdb/interface.py` & `DynamicAnnotationDB-5.9.0/dynamicannotationdb/interface.py`

 * *Files identical despite different names*

### Comparing `DynamicAnnotationDB-5.8.1/dynamicannotationdb/key_utils.py` & `DynamicAnnotationDB-5.9.0/dynamicannotationdb/key_utils.py`

 * *Files identical despite different names*

### Comparing `DynamicAnnotationDB-5.8.1/dynamicannotationdb/migration/alembic/env.py` & `DynamicAnnotationDB-5.9.0/dynamicannotationdb/migration/alembic/env.py`

 * *Files identical despite different names*

### Comparing `DynamicAnnotationDB-5.8.1/dynamicannotationdb/migration/alembic/run.py` & `DynamicAnnotationDB-5.9.0/dynamicannotationdb/migration/alembic/run.py`

 * *Files identical despite different names*

### Comparing `DynamicAnnotationDB-5.8.1/dynamicannotationdb/migration/alembic/versions/309cf493a1e2_adding_warning_field.py` & `DynamicAnnotationDB-5.9.0/dynamicannotationdb/migration/alembic/versions/309cf493a1e2_adding_warning_field.py`

 * *Files identical despite different names*

### Comparing `DynamicAnnotationDB-5.8.1/dynamicannotationdb/migration/alembic/versions/5a1d7c0ad006_add_status_column.py` & `DynamicAnnotationDB-5.9.0/dynamicannotationdb/migration/alembic/versions/5a1d7c0ad006_add_status_column.py`

 * *Files identical despite different names*

### Comparing `DynamicAnnotationDB-5.8.1/dynamicannotationdb/migration/alembic/versions/6e7f580ff680_add_error_msg.py` & `DynamicAnnotationDB-5.9.0/dynamicannotationdb/migration/alembic/versions/6e7f580ff680_add_error_msg.py`

 * *Files identical despite different names*

### Comparing `DynamicAnnotationDB-5.8.1/dynamicannotationdb/migration/alembic/versions/7c79eff751b4_add_parent_version_column.py` & `DynamicAnnotationDB-5.9.0/dynamicannotationdb/migration/alembic/versions/7c79eff751b4_add_parent_version_column.py`

 * *Files identical despite different names*

### Comparing `DynamicAnnotationDB-5.8.1/dynamicannotationdb/migration/alembic/versions/814d72d74e3b_add_version_error_table.py` & `DynamicAnnotationDB-5.9.0/dynamicannotationdb/migration/alembic/versions/814d72d74e3b_add_version_error_table.py`

 * *Files identical despite different names*

### Comparing `DynamicAnnotationDB-5.8.1/dynamicannotationdb/migration/alembic/versions/8fdc843fc202_adding_permission_and_last_modified.py` & `DynamicAnnotationDB-5.9.0/dynamicannotationdb/migration/alembic/versions/8fdc843fc202_adding_permission_and_last_modified.py`

 * *Files identical despite different names*

### Comparing `DynamicAnnotationDB-5.8.1/dynamicannotationdb/migration/alembic/versions/975a79461cab_add_is_merged.py` & `DynamicAnnotationDB-5.9.0/dynamicannotationdb/migration/alembic/versions/975a79461cab_add_is_merged.py`

 * *Files identical despite different names*

### Comparing `DynamicAnnotationDB-5.8.1/dynamicannotationdb/migration/alembic/versions/ef5c2d7f96d8_initial_live_db_models.py` & `DynamicAnnotationDB-5.9.0/dynamicannotationdb/migration/alembic/versions/ef5c2d7f96d8_initial_live_db_models.py`

 * *Files identical despite different names*

### Comparing `DynamicAnnotationDB-5.8.1/dynamicannotationdb/migration/alembic/versions/fac66b439033_add_view_model.py` & `DynamicAnnotationDB-5.9.0/dynamicannotationdb/migration/alembic/versions/fac66b439033_add_view_model.py`

 * *Files identical despite different names*

### Comparing `DynamicAnnotationDB-5.8.1/dynamicannotationdb/migration/migrate.py` & `DynamicAnnotationDB-5.9.0/dynamicannotationdb/migration/migrate.py`

 * *Files identical despite different names*

### Comparing `DynamicAnnotationDB-5.8.1/dynamicannotationdb/models.py` & `DynamicAnnotationDB-5.9.0/dynamicannotationdb/models.py`

 * *Files identical despite different names*

### Comparing `DynamicAnnotationDB-5.8.1/dynamicannotationdb/schema.py` & `DynamicAnnotationDB-5.9.0/dynamicannotationdb/schema.py`

 * *Files identical despite different names*

### Comparing `DynamicAnnotationDB-5.8.1/dynamicannotationdb/segmentation.py` & `DynamicAnnotationDB-5.9.0/dynamicannotationdb/segmentation.py`

 * *Files identical despite different names*

### Comparing `DynamicAnnotationDB-5.8.1/setup.py` & `DynamicAnnotationDB-5.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `DynamicAnnotationDB-5.8.1/tests/conftest.py` & `DynamicAnnotationDB-5.9.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `DynamicAnnotationDB-5.8.1/tests/test_annotation.py` & `DynamicAnnotationDB-5.9.0/tests/test_annotation.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,15 +22,14 @@
         table_metadata=None,
         flat_segmentation_source=None,
     )
     assert table_name == table
 
 
 def test_create_all_schema_types(dadb_interface, annotation_metadata):
-
     vx = annotation_metadata["voxel_resolution_x"]
     vy = annotation_metadata["voxel_resolution_y"]
     vz = annotation_metadata["voxel_resolution_z"]
 
     ref_metadata = {
         "reference_table": "anno_test",
         "track_target_id_updates": True,
@@ -71,22 +70,51 @@
         description="some description",
         user_id="foo@bar.com",
         voxel_resolution_x=vx,
         voxel_resolution_y=vy,
         voxel_resolution_z=vz,
         table_metadata=table_metadata,
         flat_segmentation_source=None,
-        with_crud_columns=False,
+        with_crud_columns=True,
     )
     assert table_name == table
 
     table_info = dadb_interface.database.get_table_metadata(table)
     assert table_info["reference_table"] == "anno_test"
 
 
+def test_create_nested_reference_table(dadb_interface, annotation_metadata):
+    table_name = "reference_tag"
+    schema_type = "reference_tag"
+    vx = annotation_metadata["voxel_resolution_x"]
+    vy = annotation_metadata["voxel_resolution_y"]
+    vz = annotation_metadata["voxel_resolution_z"]
+
+    table_metadata = {
+        "reference_table": "presynaptic_bouton_types",
+        "track_target_id_updates": True,
+    }
+    table = dadb_interface.annotation.create_table(
+        table_name,
+        schema_type,
+        description="tags on 'presynaptic_bouton_types' table",
+        user_id="foo@bar.com",
+        voxel_resolution_x=vx,
+        voxel_resolution_y=vy,
+        voxel_resolution_z=vz,
+        table_metadata=table_metadata,
+        flat_segmentation_source=None,
+        with_crud_columns=True,
+    )
+    assert table_name == table
+
+    table_info = dadb_interface.database.get_table_metadata(table)
+    assert table_info["reference_table"] == "presynaptic_bouton_types"
+
+
 def test_bad_schema_reference_table(dadb_interface, annotation_metadata):
     table_name = "bad_reference_table"
     schema_type = "synapse"
     vx = annotation_metadata["voxel_resolution_x"]
     vy = annotation_metadata["voxel_resolution_y"]
     vz = annotation_metadata["voxel_resolution_z"]
 
@@ -134,14 +162,28 @@
         }
     ]
     inserted_id = dadb_interface.annotation.insert_annotations(table_name, test_data)
 
     assert inserted_id == [1]
 
 
+def test_insert_nested_reference_tag_annotation(dadb_interface, annotation_metadata):
+    table_name = "reference_tag"
+
+    test_data = [
+        {
+            "tag": "here is a tag",
+            "target_id": 1,
+        }
+    ]
+    inserted_id = dadb_interface.annotation.insert_annotations(table_name, test_data)
+
+    assert inserted_id == [1]
+
+
 def test_insert_another_annotation(dadb_interface, annotation_metadata):
     table_name = annotation_metadata["table_name"]
 
     test_data = [
         {
             "pre_pt": {"position": [111, 222, 333]},
             "ctr_pt": {"position": [444, 555, 666]},
@@ -150,20 +192,30 @@
         }
     ]
     inserted_id = dadb_interface.annotation.insert_annotations(table_name, test_data)
 
     assert inserted_id == [2]
 
 
-def test_get_annotation(dadb_interface, annotation_metadata):
+def test_get_valid_annotation(dadb_interface, annotation_metadata):
     table_name = annotation_metadata["table_name"]
     test_data = dadb_interface.annotation.get_annotations(table_name, [1])
     logging.info(test_data)
 
     assert test_data[0]["id"] == 1
+    assert test_data[0]["valid"] is True
+
+
+def test_get_reference_annotation(dadb_interface, annotation_metadata):
+    table_name = "presynaptic_bouton_types"
+    test_data = dadb_interface.annotation.get_annotations(table_name, [1])
+    logging.info(test_data)
+
+    assert test_data[0]["id"] == 1
+    assert test_data[0]["target_id"] == 1
 
 
 def test_update_annotation(dadb_interface, annotation_metadata):
     table_name = annotation_metadata["table_name"]
 
     updated_test_data = {
         "id": 1,
@@ -176,52 +228,77 @@
     )
 
     assert update_map == {1: 3}
     test_data = dadb_interface.annotation.get_annotations(table_name, [1])
     assert test_data[0]["superceded_id"] == 3
 
 
-def test_get_reference_annotation(dadb_interface, annotation_metadata):
+def test_get_not_valid_annotation(dadb_interface, annotation_metadata):
+    table_name = annotation_metadata["table_name"]
+    test_data = dadb_interface.annotation.get_annotations(table_name, [1])
+    logging.info(test_data)
+
+    assert test_data[0]["id"] == 1
+    assert test_data[0]["valid"] is False
+
+
+def test_get_reference_annotation_again(dadb_interface, annotation_metadata):
     table_name = "presynaptic_bouton_types"
     test_data = dadb_interface.annotation.get_annotations(table_name, [1])
     logging.info(test_data)
 
     assert test_data[0]["id"] == 1
-    assert test_data[0]["target_id"] == 3
+    assert test_data[0]["target_id"] == 1
 
 
 def test_update_reference_annotation(dadb_interface, annotation_metadata):
     table_name = "presynaptic_bouton_types"
 
     test_data = {
         "id": 1,
         "bouton_type": "basmati",
-        "target_id": 3,
     }
 
     update_map = dadb_interface.annotation.update_annotation(table_name, test_data)
 
-    assert update_map == {1: 1}
-    test_data = dadb_interface.annotation.get_annotations(table_name, [1])
+    assert update_map == {1: 2}
+    # return values from newly updated row
+    test_data = dadb_interface.annotation.get_annotations(table_name, [2])
     assert test_data[0]["bouton_type"] == "basmati"
 
 
+def test_nested_update_reference_annotation(dadb_interface, annotation_metadata):
+    table_name = "reference_tag"
+
+    test_data = {
+        "tag": "here is a updated tag",
+        "id": 1,
+    }
+
+    update_map = dadb_interface.annotation.update_annotation(table_name, test_data)
+
+    assert update_map == {1: 2}
+    # return values from newly updated row
+    test_data = dadb_interface.annotation.get_annotations(table_name, [2])
+    assert test_data[0]["tag"] == "here is a updated tag"
+
+
 def test_delete_reference_annotation(dadb_interface, annotation_metadata):
     table_name = "presynaptic_bouton_types"
 
-    ids_to_delete = [1]
+    ids_to_delete = [2]
     is_deleted = dadb_interface.annotation.delete_annotation(table_name, ids_to_delete)
 
     assert is_deleted == ids_to_delete
 
 
 def test_delete_annotation(dadb_interface, annotation_metadata):
     table_name = annotation_metadata["table_name"]
 
-    ids_to_delete = [1]
+    ids_to_delete = [3]
     is_deleted = dadb_interface.annotation.delete_annotation(table_name, ids_to_delete)
 
     assert is_deleted == ids_to_delete
 
 
 def test_update_table_metadata(dadb_interface, annotation_metadata):
     table_name = annotation_metadata["table_name"]
```

### Comparing `DynamicAnnotationDB-5.8.1/tests/test_database.py` & `DynamicAnnotationDB-5.9.0/tests/test_database.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 
 
 def test_get_table_valid_row_count(dadb_interface, annotation_metadata):
     table_name = annotation_metadata["table_name"]
 
     result = dadb_interface.database.get_table_row_count(table_name, filter_valid=True)
     logging.info(f"{table_name} valid row count: {result}")
-    assert result == 2
+    assert result == 1
 
 
 def test_get_table_valid_timestamp_row_count(dadb_interface, annotation_metadata):
     table_name = annotation_metadata["table_name"]
     ts = datetime.datetime.utcnow() - datetime.timedelta(days=5)
     result = dadb_interface.database.get_table_row_count(
         table_name, filter_valid=True, filter_timestamp=str(ts)
```

### Comparing `DynamicAnnotationDB-5.8.1/tests/test_errors.py` & `DynamicAnnotationDB-5.9.0/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `DynamicAnnotationDB-5.8.1/tests/test_schema.py` & `DynamicAnnotationDB-5.9.0/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `DynamicAnnotationDB-5.8.1/tests/test_segmentation.py` & `DynamicAnnotationDB-5.9.0/tests/test_segmentation.py`

 * *Files identical despite different names*

