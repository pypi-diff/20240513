# Comparing `tmp/pih-plb_db-0.18.tar.gz` & `tmp/pih-plb_db-0.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-plb_db-0.18.tar", last modified: Mon Apr 22 04:03:54 2024, max compression
+gzip compressed data, was "pih-plb_db-0.19.tar", last modified: Mon May 13 02:49:17 2024, max compression
```

## Comparing `pih-plb_db-0.18.tar` & `pih-plb_db-0.19.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 04:03:54.723813 pih-plb_db-0.18/
--rw-rw-rw-   0        0        0      280 2024-04-22 04:03:54.692557 pih-plb_db-0.18/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-22 04:03:54.367854 pih-plb_db-0.18/PolibaseDatabaseService/
--rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-plb_db-0.18/PolibaseDatabaseService/__init__.py
--rw-rw-rw-   0        0        0      158 2024-02-15 00:09:03.000000 pih-plb_db-0.18/PolibaseDatabaseService/__main__.py
--rw-rw-rw-   0        0        0     9811 2024-04-22 03:57:57.000000 pih-plb_db-0.18/PolibaseDatabaseService/api.py
--rw-rw-rw-   0        0        0     1074 2024-04-22 04:02:19.000000 pih-plb_db-0.18/PolibaseDatabaseService/const.py
--rw-rw-rw-   0        0        0     1135 2024-04-22 03:09:08.000000 pih-plb_db-0.18/PolibaseDatabaseService/service.py
-drwxrwxrwx   0        0        0        0 2024-04-22 04:03:54.661314 pih-plb_db-0.18/pih_plb_db.egg-info/
--rw-rw-rw-   0        0        0      280 2024-04-22 04:03:53.000000 pih-plb_db-0.18/pih_plb_db.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      376 2024-04-22 04:03:54.000000 pih-plb_db-0.18/pih_plb_db.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 04:03:53.000000 pih-plb_db-0.18/pih_plb_db.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2024-04-22 04:03:53.000000 pih-plb_db-0.18/pih_plb_db.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        5 2024-04-22 04:03:53.000000 pih-plb_db-0.18/pih_plb_db.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2024-04-22 04:03:53.000000 pih-plb_db-0.18/pih_plb_db.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-22 04:03:54.739437 pih-plb_db-0.18/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-13 02:49:17.877786 pih-plb_db-0.19/
+-rw-rw-rw-   0        0        0      280 2024-05-13 02:49:17.846535 pih-plb_db-0.19/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-13 02:49:15.804259 pih-plb_db-0.19/PolibaseDatabaseService/
+-rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-plb_db-0.19/PolibaseDatabaseService/__init__.py
+-rw-rw-rw-   0        0        0      158 2024-02-15 00:09:03.000000 pih-plb_db-0.19/PolibaseDatabaseService/__main__.py
+-rw-rw-rw-   0        0        0    10548 2024-04-23 00:05:41.000000 pih-plb_db-0.19/PolibaseDatabaseService/api.py
+-rw-rw-rw-   0        0        0     1046 2024-04-22 22:35:45.000000 pih-plb_db-0.19/PolibaseDatabaseService/const.py
+-rw-rw-rw-   0        0        0     1135 2024-04-22 03:09:08.000000 pih-plb_db-0.19/PolibaseDatabaseService/service.py
+drwxrwxrwx   0        0        0        0 2024-05-13 02:49:17.815289 pih-plb_db-0.19/pih_plb_db.egg-info/
+-rw-rw-rw-   0        0        0      280 2024-05-13 02:49:15.000000 pih-plb_db-0.19/pih_plb_db.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      376 2024-05-13 02:49:15.000000 pih-plb_db-0.19/pih_plb_db.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 02:49:15.000000 pih-plb_db-0.19/pih_plb_db.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2024-05-13 02:49:15.000000 pih-plb_db-0.19/pih_plb_db.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        5 2024-05-13 02:49:15.000000 pih-plb_db-0.19/pih_plb_db.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2024-05-13 02:49:15.000000 pih-plb_db-0.19/pih_plb_db.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 02:49:17.893409 pih-plb_db-0.19/setup.cfg
```

### Comparing `pih-plb_db-0.18/PolibaseDatabaseService/api.py` & `pih-plb_db-0.19/PolibaseDatabaseService/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import ipih
 
 import os
 from pih import A
-from pih.tools import j, n, js, esc
+from pih.tools import j, n, js, nn, esc
 from PolibaseDatabaseService.const import *
 
 TEST: bool = False
 #
 
 
 class PolibaseDBApi:
@@ -147,32 +147,49 @@
                 )
             )
             os.system(nas_create_connection_command)
             os.system(polibase2_create_connection_command)
 
         # step 3
         A.E.backup_notify_about_polibase_creation_archived_db_dumb_start()
-        print(
-            os.system(
-                js(
+        archive_creation_parameters: str = A.S.get(
+            A.CT_S.POLIBASE_DB_DUMP_ARCHIVE_CREATION_PARAMETERS
+        )
+        password_parameter: str = j(
+            (
+                "-p",
+                esc(A.D_V_E.value("POLIBASE_DATABASE_ARCHIVE_PASSWORD")),
+            )
+        )
+        os.system(
+            js(
+                (
+                    archiver_program_path,
                     (
-                        archiver_program_path,
-                        j(("a -t", ARCHIVE_TYPE)),
-                        j(("-mx", COMPRESSION_RATIO)),
-                        j(
-                            (
-                                "-p",
-                                esc(
-                                    A.D_V_E.value("POLIBASE_DATABASE_ARCHIVE_PASSWORD")
-                                ),
+                        (
+                            js(
+                                (
+                                    j(("a -t", ARCHIVE_TYPE)),
+                                    j(
+                                        (
+                                            "-mx",
+                                            A.S.get(
+                                                A.CT_S.POLIBASE_DB_DUMP_ARCHIVE_COMPRESSION_LEVEL
+                                            ),
+                                        )
+                                    ),
+                                    password_parameter,
+                                )
                             )
-                        ),
-                        file_out_name,
-                        file_database_dump_name_out,
-                    )
+                        )
+                        if n(archive_creation_parameters)
+                        else js((archive_creation_parameters, password_parameter))
+                    ),
+                    file_out_name,
+                    file_database_dump_name_out,
                 )
             )
         )
 
         A.E.backup_notify_about_polibase_creation_archived_db_dumb_complete(
             os.path.getsize(A.PTH.join(polibase_folder_path, file_out_name)), not test
         )
```

### Comparing `pih-plb_db-0.18/PolibaseDatabaseService/const.py` & `pih-plb_db-0.19/PolibaseDatabaseService/const.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pih.consts import CONST
 from pih.collections.service import ServiceDescription
 
 NAME: str = "PolibaseDatabase"
 
 HOST = A.CT_H.POLIBASE
 
-VERSION: str = "0.18"
+VERSION: str = "0.19"
 
 
 SD: ServiceDescription = ServiceDescription(
     name=NAME,
     host=HOST.NAME,
     description="Polibase database service",
     commands=("create_polibase_database_backup",),
@@ -24,15 +24,14 @@
 )
 
 TEST_NAME: str = "test"
 STUB_DIRECTORY_NAME: str = "stub"
 #
 POLIBASE_NAME: str = "Polibase"
 ARCHIVE_TYPE: str = A.CT_F_E.ARCHIVE
-COMPRESSION_RATIO: int = 9
 
 
 USE_PRECONNECTED_DISKS: bool = True
 
 class MOUNT_POINT:
     POLIBASE: str = "C"
     NAS: str = "K"
```

### Comparing `pih-plb_db-0.18/PolibaseDatabaseService/service.py` & `pih-plb_db-0.19/PolibaseDatabaseService/service.py`

 * *Files identical despite different names*

