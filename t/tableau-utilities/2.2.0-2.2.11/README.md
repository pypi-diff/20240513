# Comparing `tmp/tableau_utilities-2.2.0.tar.gz` & `tmp/tableau_utilities-2.2.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tableau_utilities-2.2.0.tar", last modified: Mon May  6 16:59:27 2024, max compression
+gzip compressed data, was "tableau_utilities-2.2.11.tar", last modified: Mon May 13 17:04:34 2024, max compression
```

## Comparing `tableau_utilities-2.2.0.tar` & `tableau_utilities-2.2.11.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 justin     (502) staff       (20)        0 2024-05-06 16:59:27.521078 tableau_utilities-2.2.0/
--rw-r--r--   0 justin     (502) staff       (20)     1062 2022-05-25 18:48:01.000000 tableau_utilities-2.2.0/LICENSE
--rw-r--r--   0 justin     (502) staff       (20)     9118 2024-05-06 16:59:27.520434 tableau_utilities-2.2.0/PKG-INFO
--rw-r--r--   0 justin     (502) staff       (20)     8544 2024-05-06 16:48:53.000000 tableau_utilities-2.2.0/README.md
--rw-r--r--   0 justin     (502) staff       (20)       38 2024-05-06 16:59:27.521216 tableau_utilities-2.2.0/setup.cfg
--rw-r--r--   0 justin     (502) staff       (20)     1257 2024-05-06 16:48:53.000000 tableau_utilities-2.2.0/setup.py
-drwxr-xr-x   0 justin     (502) staff       (20)        0 2024-05-06 16:59:27.495027 tableau_utilities-2.2.0/tableau_utilities/
--rw-r--r--   0 justin     (502) staff       (20)      306 2024-02-29 16:48:52.000000 tableau_utilities-2.2.0/tableau_utilities/__init__.py
--rw-r--r--   0 justin     (502) staff       (20)     2441 2024-02-29 16:48:52.000000 tableau_utilities-2.2.0/tableau_utilities/fetch_all_cols.py
-drwxr-xr-x   0 justin     (502) staff       (20)        0 2024-05-06 16:59:27.500756 tableau_utilities-2.2.0/tableau_utilities/general/
--rw-r--r--   0 justin     (502) staff       (20)        0 2023-06-28 16:57:49.000000 tableau_utilities-2.2.0/tableau_utilities/general/__init__.py
--rw-r--r--   0 justin     (502) staff       (20)     2235 2023-06-28 16:57:49.000000 tableau_utilities-2.2.0/tableau_utilities/general/cli_styling.py
--rw-r--r--   0 justin     (502) staff       (20)     3497 2023-06-28 16:57:49.000000 tableau_utilities-2.2.0/tableau_utilities/general/config_column_persona.py
--rw-r--r--   0 justin     (502) staff       (20)     2278 2023-06-28 16:57:49.000000 tableau_utilities-2.2.0/tableau_utilities/general/funcs.py
-drwxr-xr-x   0 justin     (502) staff       (20)        0 2024-05-06 16:59:27.501752 tableau_utilities-2.2.0/tableau_utilities/hyper/
--rw-r--r--   0 justin     (502) staff       (20)        0 2024-05-06 16:48:53.000000 tableau_utilities-2.2.0/tableau_utilities/hyper/__init__.py
--rw-r--r--   0 justin     (502) staff       (20)     5929 2024-05-06 16:48:53.000000 tableau_utilities-2.2.0/tableau_utilities/hyper/hyper.py
--rw-r--r--   0 justin     (502) staff       (20)     3030 2024-03-20 15:25:53.000000 tableau_utilities-2.2.0/tableau_utilities/scripted_testing.py
-drwxr-xr-x   0 justin     (502) staff       (20)        0 2024-05-06 16:59:27.507853 tableau_utilities-2.2.0/tableau_utilities/scripts/
--rw-r--r--   0 justin     (502) staff       (20)        0 2023-06-28 16:57:49.000000 tableau_utilities-2.2.0/tableau_utilities/scripts/__init__.py
--rw-r--r--   0 justin     (502) staff       (20)    24339 2024-05-06 16:48:53.000000 tableau_utilities-2.2.0/tableau_utilities/scripts/cli.py
--rw-r--r--   0 justin     (502) staff       (20)     1772 2023-06-28 16:57:49.000000 tableau_utilities-2.2.0/tableau_utilities/scripts/csv_config.py
--rw-r--r--   0 justin     (502) staff       (20)     9121 2024-05-06 16:58:26.000000 tableau_utilities-2.2.0/tableau_utilities/scripts/datasource.py
--rw-r--r--   0 justin     (502) staff       (20)    13151 2024-02-29 16:48:52.000000 tableau_utilities-2.2.0/tableau_utilities/scripts/gen_config.py
--rw-r--r--   0 justin     (502) staff       (20)     8539 2023-06-28 16:57:49.000000 tableau_utilities-2.2.0/tableau_utilities/scripts/merge_config.py
--rw-r--r--   0 justin     (502) staff       (20)     1867 2024-02-29 16:48:52.000000 tableau_utilities-2.2.0/tableau_utilities/scripts/server_info.py
--rw-r--r--   0 justin     (502) staff       (20)     4511 2024-05-03 15:27:55.000000 tableau_utilities-2.2.0/tableau_utilities/scripts/server_operate.py
-drwxr-xr-x   0 justin     (502) staff       (20)        0 2024-05-06 16:59:27.509921 tableau_utilities-2.2.0/tableau_utilities/tableau_file/
--rw-r--r--   0 justin     (502) staff       (20)        0 2023-06-28 16:57:49.000000 tableau_utilities-2.2.0/tableau_utilities/tableau_file/__init__.py
--rw-r--r--   0 justin     (502) staff       (20)    15040 2024-05-06 16:48:53.000000 tableau_utilities-2.2.0/tableau_utilities/tableau_file/tableau_file.py
--rw-r--r--   0 justin     (502) staff       (20)    38250 2024-05-06 16:48:53.000000 tableau_utilities-2.2.0/tableau_utilities/tableau_file/tableau_file_objects.py
-drwxr-xr-x   0 justin     (502) staff       (20)        0 2024-05-06 16:59:27.518511 tableau_utilities-2.2.0/tableau_utilities/tableau_server/
--rw-r--r--   0 justin     (502) staff       (20)        0 2023-06-28 16:57:49.000000 tableau_utilities-2.2.0/tableau_utilities/tableau_server/__init__.py
--rw-r--r--   0 justin     (502) staff       (20)     2450 2024-03-01 20:30:48.000000 tableau_utilities-2.2.0/tableau_utilities/tableau_server/base.py
--rw-r--r--   0 justin     (502) staff       (20)     1330 2024-03-01 20:30:48.000000 tableau_utilities-2.2.0/tableau_utilities/tableau_server/create.py
--rw-r--r--   0 justin     (502) staff       (20)     2193 2024-03-01 20:30:48.000000 tableau_utilities-2.2.0/tableau_utilities/tableau_server/download.py
--rw-r--r--   0 justin     (502) staff       (20)     9893 2024-03-01 20:30:48.000000 tableau_utilities-2.2.0/tableau_utilities/tableau_server/get.py
--rw-r--r--   0 justin     (502) staff       (20)    12043 2024-03-04 16:14:39.000000 tableau_utilities-2.2.0/tableau_utilities/tableau_server/publish.py
--rw-r--r--   0 justin     (502) staff       (20)      891 2024-03-01 20:30:48.000000 tableau_utilities-2.2.0/tableau_utilities/tableau_server/refresh.py
--rw-r--r--   0 justin     (502) staff       (20)     1484 2024-03-01 20:30:48.000000 tableau_utilities-2.2.0/tableau_utilities/tableau_server/static.py
--rw-r--r--   0 justin     (502) staff       (20)     5309 2024-02-29 16:48:52.000000 tableau_utilities-2.2.0/tableau_utilities/tableau_server/tableau_server.py
--rw-r--r--   0 justin     (502) staff       (20)    13195 2023-06-28 16:57:49.000000 tableau_utilities-2.2.0/tableau_utilities/tableau_server/tableau_server_objects.py
--rw-r--r--   0 justin     (502) staff       (20)     1393 2024-03-01 20:30:48.000000 tableau_utilities-2.2.0/tableau_utilities/tableau_server/update.py
--rw-r--r--   0 justin     (502) staff       (20)    11595 2023-10-24 17:53:15.000000 tableau_utilities-2.2.0/tableau_utilities/test_tableau_utilities.py
-drwxr-xr-x   0 justin     (502) staff       (20)        0 2024-05-06 16:59:27.519436 tableau_utilities-2.2.0/tableau_utilities.egg-info/
--rw-r--r--   0 justin     (502) staff       (20)     9118 2024-05-06 16:59:27.000000 tableau_utilities-2.2.0/tableau_utilities.egg-info/PKG-INFO
--rw-r--r--   0 justin     (502) staff       (20)     1617 2024-05-06 16:59:27.000000 tableau_utilities-2.2.0/tableau_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 justin     (502) staff       (20)        1 2024-05-06 16:59:27.000000 tableau_utilities-2.2.0/tableau_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 justin     (502) staff       (20)       73 2024-05-06 16:59:27.000000 tableau_utilities-2.2.0/tableau_utilities.egg-info/entry_points.txt
--rw-r--r--   0 justin     (502) staff       (20)      148 2024-05-06 16:59:27.000000 tableau_utilities-2.2.0/tableau_utilities.egg-info/requires.txt
--rw-r--r--   0 justin     (502) staff       (20)       18 2024-05-06 16:59:27.000000 tableau_utilities-2.2.0/tableau_utilities.egg-info/top_level.txt
+drwxr-xr-x   0 justin     (502) staff       (20)        0 2024-05-13 17:04:34.399607 tableau_utilities-2.2.11/
+-rw-r--r--   0 justin     (502) staff       (20)     1062 2022-05-25 18:48:01.000000 tableau_utilities-2.2.11/LICENSE
+-rw-r--r--   0 justin     (502) staff       (20)     9120 2024-05-13 17:04:34.398746 tableau_utilities-2.2.11/PKG-INFO
+-rw-r--r--   0 justin     (502) staff       (20)     8545 2024-05-13 17:03:08.000000 tableau_utilities-2.2.11/README.md
+-rw-r--r--   0 justin     (502) staff       (20)       38 2024-05-13 17:04:34.399734 tableau_utilities-2.2.11/setup.cfg
+-rw-r--r--   0 justin     (502) staff       (20)     1258 2024-05-13 17:03:08.000000 tableau_utilities-2.2.11/setup.py
+drwxr-xr-x   0 justin     (502) staff       (20)        0 2024-05-13 17:04:34.373857 tableau_utilities-2.2.11/tableau_utilities/
+-rw-r--r--   0 justin     (502) staff       (20)      306 2024-02-29 16:48:52.000000 tableau_utilities-2.2.11/tableau_utilities/__init__.py
+-rw-r--r--   0 justin     (502) staff       (20)     2441 2024-02-29 16:48:52.000000 tableau_utilities-2.2.11/tableau_utilities/fetch_all_cols.py
+drwxr-xr-x   0 justin     (502) staff       (20)        0 2024-05-13 17:04:34.379170 tableau_utilities-2.2.11/tableau_utilities/general/
+-rw-r--r--   0 justin     (502) staff       (20)        0 2023-06-28 16:57:49.000000 tableau_utilities-2.2.11/tableau_utilities/general/__init__.py
+-rw-r--r--   0 justin     (502) staff       (20)     2235 2023-06-28 16:57:49.000000 tableau_utilities-2.2.11/tableau_utilities/general/cli_styling.py
+-rw-r--r--   0 justin     (502) staff       (20)     3497 2023-06-28 16:57:49.000000 tableau_utilities-2.2.11/tableau_utilities/general/config_column_persona.py
+-rw-r--r--   0 justin     (502) staff       (20)     2278 2023-06-28 16:57:49.000000 tableau_utilities-2.2.11/tableau_utilities/general/funcs.py
+drwxr-xr-x   0 justin     (502) staff       (20)        0 2024-05-13 17:04:34.380039 tableau_utilities-2.2.11/tableau_utilities/hyper/
+-rw-r--r--   0 justin     (502) staff       (20)        0 2024-05-06 16:48:53.000000 tableau_utilities-2.2.11/tableau_utilities/hyper/__init__.py
+-rw-r--r--   0 justin     (502) staff       (20)     5929 2024-05-06 16:48:53.000000 tableau_utilities-2.2.11/tableau_utilities/hyper/hyper.py
+-rw-r--r--   0 justin     (502) staff       (20)     3030 2024-03-20 15:25:53.000000 tableau_utilities-2.2.11/tableau_utilities/scripted_testing.py
+drwxr-xr-x   0 justin     (502) staff       (20)        0 2024-05-13 17:04:34.385580 tableau_utilities-2.2.11/tableau_utilities/scripts/
+-rw-r--r--   0 justin     (502) staff       (20)        0 2023-06-28 16:57:49.000000 tableau_utilities-2.2.11/tableau_utilities/scripts/__init__.py
+-rw-r--r--   0 justin     (502) staff       (20)    24457 2024-05-13 17:03:08.000000 tableau_utilities-2.2.11/tableau_utilities/scripts/cli.py
+-rw-r--r--   0 justin     (502) staff       (20)     1772 2023-06-28 16:57:49.000000 tableau_utilities-2.2.11/tableau_utilities/scripts/csv_config.py
+-rw-r--r--   0 justin     (502) staff       (20)    10863 2024-05-13 17:03:08.000000 tableau_utilities-2.2.11/tableau_utilities/scripts/datasource.py
+-rw-r--r--   0 justin     (502) staff       (20)    13151 2024-02-29 16:48:52.000000 tableau_utilities-2.2.11/tableau_utilities/scripts/gen_config.py
+-rw-r--r--   0 justin     (502) staff       (20)     8539 2023-06-28 16:57:49.000000 tableau_utilities-2.2.11/tableau_utilities/scripts/merge_config.py
+-rw-r--r--   0 justin     (502) staff       (20)     1867 2024-02-29 16:48:52.000000 tableau_utilities-2.2.11/tableau_utilities/scripts/server_info.py
+-rw-r--r--   0 justin     (502) staff       (20)     4511 2024-05-03 15:27:55.000000 tableau_utilities-2.2.11/tableau_utilities/scripts/server_operate.py
+drwxr-xr-x   0 justin     (502) staff       (20)        0 2024-05-13 17:04:34.387814 tableau_utilities-2.2.11/tableau_utilities/tableau_file/
+-rw-r--r--   0 justin     (502) staff       (20)        0 2023-06-28 16:57:49.000000 tableau_utilities-2.2.11/tableau_utilities/tableau_file/__init__.py
+-rw-r--r--   0 justin     (502) staff       (20)    15040 2024-05-06 16:48:53.000000 tableau_utilities-2.2.11/tableau_utilities/tableau_file/tableau_file.py
+-rw-r--r--   0 justin     (502) staff       (20)    38250 2024-05-06 16:48:53.000000 tableau_utilities-2.2.11/tableau_utilities/tableau_file/tableau_file_objects.py
+drwxr-xr-x   0 justin     (502) staff       (20)        0 2024-05-13 17:04:34.396894 tableau_utilities-2.2.11/tableau_utilities/tableau_server/
+-rw-r--r--   0 justin     (502) staff       (20)        0 2023-06-28 16:57:49.000000 tableau_utilities-2.2.11/tableau_utilities/tableau_server/__init__.py
+-rw-r--r--   0 justin     (502) staff       (20)     2450 2024-03-01 20:30:48.000000 tableau_utilities-2.2.11/tableau_utilities/tableau_server/base.py
+-rw-r--r--   0 justin     (502) staff       (20)     1330 2024-03-01 20:30:48.000000 tableau_utilities-2.2.11/tableau_utilities/tableau_server/create.py
+-rw-r--r--   0 justin     (502) staff       (20)     2193 2024-03-01 20:30:48.000000 tableau_utilities-2.2.11/tableau_utilities/tableau_server/download.py
+-rw-r--r--   0 justin     (502) staff       (20)     9893 2024-03-01 20:30:48.000000 tableau_utilities-2.2.11/tableau_utilities/tableau_server/get.py
+-rw-r--r--   0 justin     (502) staff       (20)    12043 2024-03-04 16:14:39.000000 tableau_utilities-2.2.11/tableau_utilities/tableau_server/publish.py
+-rw-r--r--   0 justin     (502) staff       (20)      891 2024-03-01 20:30:48.000000 tableau_utilities-2.2.11/tableau_utilities/tableau_server/refresh.py
+-rw-r--r--   0 justin     (502) staff       (20)     1484 2024-03-01 20:30:48.000000 tableau_utilities-2.2.11/tableau_utilities/tableau_server/static.py
+-rw-r--r--   0 justin     (502) staff       (20)     5309 2024-02-29 16:48:52.000000 tableau_utilities-2.2.11/tableau_utilities/tableau_server/tableau_server.py
+-rw-r--r--   0 justin     (502) staff       (20)    13195 2023-06-28 16:57:49.000000 tableau_utilities-2.2.11/tableau_utilities/tableau_server/tableau_server_objects.py
+-rw-r--r--   0 justin     (502) staff       (20)     1393 2024-03-01 20:30:48.000000 tableau_utilities-2.2.11/tableau_utilities/tableau_server/update.py
+-rw-r--r--   0 justin     (502) staff       (20)    11595 2023-10-24 17:53:15.000000 tableau_utilities-2.2.11/tableau_utilities/test_tableau_utilities.py
+drwxr-xr-x   0 justin     (502) staff       (20)        0 2024-05-13 17:04:34.397879 tableau_utilities-2.2.11/tableau_utilities.egg-info/
+-rw-r--r--   0 justin     (502) staff       (20)     9120 2024-05-13 17:04:34.000000 tableau_utilities-2.2.11/tableau_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 justin     (502) staff       (20)     1617 2024-05-13 17:04:34.000000 tableau_utilities-2.2.11/tableau_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 justin     (502) staff       (20)        1 2024-05-13 17:04:34.000000 tableau_utilities-2.2.11/tableau_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 justin     (502) staff       (20)       73 2024-05-13 17:04:34.000000 tableau_utilities-2.2.11/tableau_utilities.egg-info/entry_points.txt
+-rw-r--r--   0 justin     (502) staff       (20)      148 2024-05-13 17:04:34.000000 tableau_utilities-2.2.11/tableau_utilities.egg-info/requires.txt
+-rw-r--r--   0 justin     (502) staff       (20)       18 2024-05-13 17:04:34.000000 tableau_utilities-2.2.11/tableau_utilities.egg-info/top_level.txt
```

### Comparing `tableau_utilities-2.2.0/LICENSE` & `tableau_utilities-2.2.11/LICENSE`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.2.0/PKG-INFO` & `tableau_utilities-2.2.11/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tableau_utilities
-Version: 2.2.0
+Version: 2.2.11
 Summary: Utility for maintaining Tableau objects
 Home-page: http://pypi.python.org/pypi/tableau-utilities/
 Author: Justin Grilli
 Author-email: justin.grilli@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -196,15 +196,15 @@
 Generate a config from a datasource in online/server and add definitions from a csv
 ```commandline
 tableau_utilities --token_name my_token_name --token_secret 1q2w3e4r5t6y7u8i9o --site mysitename --server 10az --location online --name 'My Awseome Datasource' --project_name 'My Team Project' generate_config --definitions_csv /Desktop/new_descriptions.csv
 ```
 
 Generate a config from a local file. Add a file prefix and print the debugging logs to the console
 ```commandline
-tableau_utilities --debugging_logs generate_config --location local --file_path '/code/tableau-utilities/tmp_tdsx_and_config/My Awesome Datasource.tdsx' --file_prefix
+tableau_utilities --debugging_logs  --location local --file_path '/code/tableau-utilities/tmp_tdsx_and_config/My Awesome Datasource.tdsx' generate_config --file_prefix
 ```
 
 #### csv_config
 Write the config to a csv with 1 row per field per datasource
 ```commandline
  tableau_utilities csv_config --config_list /code/airflow/dags/tableau/configs/column_config.json /code/airflow/dags/tableau/configs/tableau_calc_config.json
 ```
```

### Comparing `tableau_utilities-2.2.0/README.md` & `tableau_utilities-2.2.11/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -178,15 +178,15 @@
 Generate a config from a datasource in online/server and add definitions from a csv
 ```commandline
 tableau_utilities --token_name my_token_name --token_secret 1q2w3e4r5t6y7u8i9o --site mysitename --server 10az --location online --name 'My Awseome Datasource' --project_name 'My Team Project' generate_config --definitions_csv /Desktop/new_descriptions.csv
 ```
 
 Generate a config from a local file. Add a file prefix and print the debugging logs to the console
 ```commandline
-tableau_utilities --debugging_logs generate_config --location local --file_path '/code/tableau-utilities/tmp_tdsx_and_config/My Awesome Datasource.tdsx' --file_prefix
+tableau_utilities --debugging_logs  --location local --file_path '/code/tableau-utilities/tmp_tdsx_and_config/My Awesome Datasource.tdsx' generate_config --file_prefix
 ```
 
 #### csv_config
 Write the config to a csv with 1 row per field per datasource
 ```commandline
  tableau_utilities csv_config --config_list /code/airflow/dags/tableau/configs/column_config.json /code/airflow/dags/tableau/configs/tableau_calc_config.json
 ```
```

### Comparing `tableau_utilities-2.2.0/setup.py` & `tableau_utilities-2.2.11/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     author_email="justin.grilli@gmail.com",
     license='MIT',
     url='http://pypi.python.org/pypi/tableau-utilities/',
     description='Utility for maintaining Tableau objects',
     long_description=readme,
     long_description_content_type='text/markdown',
     name="tableau_utilities",
-    version="2.2.0",
+    version="2.2.11",
     requires_python=">=3.8",
     packages=[
         'tableau_utilities',
         'tableau_utilities.general',
         'tableau_utilities.tableau_file',
         'tableau_utilities.tableau_server',
         'tableau_utilities.hyper',
```

### Comparing `tableau_utilities-2.2.0/tableau_utilities/fetch_all_cols.py` & `tableau_utilities-2.2.11/tableau_utilities/fetch_all_cols.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.2.0/tableau_utilities/general/cli_styling.py` & `tableau_utilities-2.2.11/tableau_utilities/general/cli_styling.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.2.0/tableau_utilities/general/config_column_persona.py` & `tableau_utilities-2.2.11/tableau_utilities/general/config_column_persona.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.2.0/tableau_utilities/general/funcs.py` & `tableau_utilities-2.2.11/tableau_utilities/general/funcs.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.2.0/tableau_utilities/hyper/hyper.py` & `tableau_utilities-2.2.11/tableau_utilities/hyper/hyper.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.2.0/tableau_utilities/scripted_testing.py` & `tableau_utilities-2.2.11/tableau_utilities/scripted_testing.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.2.0/tableau_utilities/scripts/cli.py` & `tableau_utilities-2.2.11/tableau_utilities/scripts/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 import argparse
 import os
 import shutil
 from argparse import RawTextHelpFormatter
 import yaml
-import pkg_resources
-import pkgutil
 import importlib.metadata
 
 import tableau_utilities.tableau_server.tableau_server as ts
 
 from tableau_utilities.general.config_column_persona import personas
 from tableau_utilities.general.cli_styling import Color, Symbol, color_print
 from tableau_utilities.scripts.gen_config import generate_config
 from tableau_utilities.scripts.merge_config import merge_configs
 from tableau_utilities.scripts.server_info import server_info
 from tableau_utilities.scripts.server_operate import server_operate
 from tableau_utilities.scripts.datasource import datasource
 from tableau_utilities.scripts.csv_config import csv_config
 
-__version__ = pkg_resources.require("tableau_utilities")[0].version
+__version__ = importlib.metadata.version('tableau_utilities')
 
 parser = argparse.ArgumentParser(
     prog='tableau_utilities',
     description='Tableau Utilities CLI:\n'
                 '-Manage Tableau Server/Online\n'
                 '-Manage configurations to edit datasource metadata',
     formatter_class=RawTextHelpFormatter
 )
-parser.add_argument('--version', action='version', version=f'%(prog)s {__version__}',
+parser.add_argument('-v', '--version', action='version', version=f'%(prog)s {__version__}',
                     help='Print the current version of the CLI')
 parser.add_argument('-d', '--debugging_logs', action='store_true',
                     help='Print detailed logging to the console to debug CLI')
 subparsers = parser.add_subparsers(title="commands", dest="command", help='You must choose a command.', required=True)
 
 # GROUP: Tableau Server Authentication
 group_server_auth = parser.add_argument_group(
@@ -160,14 +158,15 @@
 parser_datasource.add_argument('--desc', help='A Tableau column description')
 parser_datasource.add_argument('--calculation', help='A Tableau calculation')
 parser_datasource.add_argument('-ee', '--empty_extract', action='store_true',
                                help='Adds an empty extract to the Datasource if specified.')
 parser_datasource.add_argument('-fe', '--filter_extract',
                                help='Deletes data from the extract based on the condition string provided. '
                                     """E.g. "CREATED_AT" < '1/1/2024'""")
+parser_datasource.add_argument('-ci', '--column_init', action='store_true',  help="Adds Columns from all Metadata Records, if they don't already exist.")
 parser_datasource.set_defaults(func=datasource)
 
 # GENERATE CONFIG
 parser_config_gen = subparsers.add_parser(
     'generate_config', help='Generate configs to programmatically manage metadata in Tableau '
                             'datasources via Airflow.\nRequires File arguments.\n')
 parser_config_gen.add_argument('--file_prefix', action='store_true',
```

### Comparing `tableau_utilities-2.2.0/tableau_utilities/scripts/csv_config.py` & `tableau_utilities-2.2.11/tableau_utilities/scripts/csv_config.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.2.0/tableau_utilities/scripts/datasource.py` & `tableau_utilities-2.2.11/tableau_utilities/scripts/datasource.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,17 +5,37 @@
 from time import time
 from tableau_utilities.general.config_column_persona import personas, get_persona_by_attribs, \
     get_persona_by_metadata_local_type
 from tableau_utilities.general.cli_styling import Color
 from tableau_utilities.general.cli_styling import Symbol
 from tableau_utilities.tableau_file.tableau_file import Datasource
 from tableau_utilities.tableau_server.tableau_server import TableauServer
-from tableau_utilities.hyper.hyper import create_empty_hyper_extract, filter_hyper_extract
 
 
+def create_column(name: str, persona: dict):
+    """ Creates the tfo column object with the minimum required fields to add a column
+
+    Args:
+        name: The name for the Column, and local_name of the Metadata Record.
+        persona: A dictionary showing the role, datatype, and role type
+
+    Returns:
+        A tfo column object
+
+    """
+
+    column = tfo.Column(
+        name=name,
+        role=persona['role'],
+        datatype=persona['datatype'],
+        type=persona['role_type'],
+    )
+
+    return column
+
 def datasource(args, server=None):
     """ Updates a Tableau Datasource locally
 
     Args:
         args: An argparse args object
         server (TableauServer): A TableauServer object; optional
     """
@@ -42,14 +62,15 @@
     column_name = args.column_name
     folder_name = args.folder_name
     caption = args.caption
     desc = args.desc
     calculation = args.calculation
     remote_name = args.remote_name
     list_objects = args.list.title() if args.list else None
+    column_init = args.column_init
 
     # Datasource Connection Args
     conn_type = args.conn_type
     conn_host = args.conn_host
     conn_user = args.conn_user
     conn_role = args.conn_role
     conn_db = args.conn_db
@@ -70,18 +91,20 @@
               f'Downloaded Datasource: {color.fg_yellow}{datasource_path}{color.reset}\n')
 
     datasource_file_name = os.path.basename(datasource_path)
     ds = Datasource(datasource_path)
 
     # Add an empty .hyper file to the Datasource; Useful for publishing without data
     if empty_extract:
+        from tableau_utilities.hyper.hyper import create_empty_hyper_extract
         create_empty_hyper_extract(ds)
         print(f'{color.fg_green}Added empty .hyper extract for {datasource_path}{color.reset}')
     # Otherwise, filter the extract if filter_extract string provided
     elif filter_extract:
+        from tableau_utilities.hyper.hyper import filter_hyper_extract
         start = time()
         print(f'{color.fg_cyan}...Filtering extract data...{color.reset}')
         filter_hyper_extract(ds, filter_extract)
         print(f'{color.fg_green}{symbol.success} (Done in {round(time() - start)} sec) '
               f'Filtered extract data for {datasource_path}{color.reset}')
 
     if save_tds:
@@ -102,28 +125,54 @@
     if list_objects:
         print(f'{color.fg_cyan}{list_objects}:{color.reset}')
     if list_objects == 'Columns':
         for c in ds.columns:
             print(f'  {symbol.arrow_r} '
                   f'{color.fg_yellow}caption:{color.reset} {c.caption} '
                   f'{color.fg_yellow}local-name:{color.reset} {c.name} '
+                  f'{color.fg_yellow}remote-name:{color.reset} {c.name} '
                   f'{color.fg_yellow}persona:{color.reset} {get_persona_by_attribs(c.role, c.type, c.datatype)}')
     if list_objects == 'Folders':
         for f in ds.folders_common.folder:
             print(f'  {symbol.arrow_r} {color.fg_yellow}{f.name}{color.reset}')
     if list_objects == 'Metadata':
         for m in ds.connection.metadata_records:
             print(f'  {symbol.arrow_r} '
                   f'{color.fg_yellow}local-name:{color.reset} {m.local_name} '
                   f'{color.fg_yellow}remote-name:{color.reset} {m.remote_name} '
                   f'{color.fg_yellow}persona:{color.reset} {get_persona_by_metadata_local_type(m.local_type)}')
     if list_objects == 'Connections':
         for c in ds.connection.named_connections:
             print(f'  {symbol.arrow_r} {c.connection.dict()}')
 
+    # Column Init - Add columns for any column in Metadata records but not in columns
+    if column_init:
+        columns_to_add = [
+            m for m in ds.connection.metadata_records
+            if m.local_name not in [c.name for c in ds.columns]
+        ]
+        print(f'{color.fg_yellow}Adding missing columns from Metadata Records:{color.reset} '
+              f'{[m.local_name for m in columns_to_add]}')
+
+        for m in columns_to_add:
+            if debugging_logs:
+                print(f'{color.fg_magenta}Metadata Record -> {m.local_name}:{color.reset} {m}')
+
+            persona = get_persona_by_metadata_local_type(m.local_type)
+            persona_dict = personas.get(persona, {})
+            if debugging_logs:
+                print(f'  - {color.fg_blue}Persona -> {persona}:{color.reset} {persona_dict}')
+
+            column = create_column(m.local_name, persona_dict)
+
+            if debugging_logs:
+                print(f'  - {color.fg_cyan}Creating Column -> {column.name}:{color.reset} {column.dict()}')
+            ds.enforce_column(column, remote_name=m.remote_name)
+
+
     # Add / modify a specified column
     if column_name and not delete:
         # Column name needs to be enclosed in brackets
         if debugging_logs:
             print('Going to add/update column:', column_name)
         column = ds.columns.get(column_name)
         if persona:
@@ -131,30 +180,29 @@
         else:
             persona = dict()
 
         if not column:
             if not persona:
                 raise Exception('Column does not exist, and more args are need to add a new column.\n'
                                 f'Minimum required args: {color.fg_yellow}--column_name --persona{color.reset}')
-            column = tfo.Column(
-                name=column_name,
-                role=persona['role'],
-                datatype=persona['datatype'],
-                type=persona['role_type'],
-            )
+            column = create_column(column_name, persona)
             print(f'{color.fg_cyan}Creating new column for {column_name}:{color.reset} {column.dict()}')
         else:
             print(f'{color.fg_cyan}Updating existing column:{color.reset}\n  {column.dict()}')
 
         column.caption = caption or column.caption
         column.role = persona.get('role') or column.role
         column.type = persona.get('role_type') or column.type
         column.datatype = persona.get('datatype') or column.datatype
         column.desc = desc or column.desc
         column.calculation = calculation or column.calculation
+
+        if debugging_logs:
+            print(f'{color.fg_yellow}column:{color.reset}{column}')
+
         ds.enforce_column(column, remote_name=remote_name, folder_name=folder_name)
 
     # Add a folder if it was specified and does not exist already
     if folder_name and not ds.folders_common.get(folder_name) and not delete:
         if debugging_logs:
             print(f'Going to add folder: {color.fg_cyan}{folder_name}{color.reset}')
         ds.folders_common.add(tfo.Folder(name=folder_name))
@@ -179,15 +227,15 @@
             connection.service = conn_role or connection.service
             connection.dbname = conn_db or connection.dbname
             connection.schema = conn_schema or connection.schema
             connection.warehouse = conn_warehouse or connection.warehouse
             ds.connection.update(connection)
 
     # Save the datasource if an edit may have happened
-    if column_name or folder_name or delete or enforce_connection or empty_extract:
+    if column_name or folder_name or delete or enforce_connection or empty_extract or column_init:
         start = time()
         print(f'{color.fg_cyan}...Saving datasource changes...{color.reset}')
         ds.save()
         print(f'{color.fg_green}{symbol.success} (Done in {round(time() - start)} sec) '
               f'Saved datasource changes: {color.fg_yellow}{datasource_path}{color.reset}')
 
     if save_tds:
```

### Comparing `tableau_utilities-2.2.0/tableau_utilities/scripts/gen_config.py` & `tableau_utilities-2.2.11/tableau_utilities/scripts/gen_config.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.2.0/tableau_utilities/scripts/merge_config.py` & `tableau_utilities-2.2.11/tableau_utilities/scripts/merge_config.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.2.0/tableau_utilities/scripts/server_info.py` & `tableau_utilities-2.2.11/tableau_utilities/scripts/server_info.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.2.0/tableau_utilities/scripts/server_operate.py` & `tableau_utilities-2.2.11/tableau_utilities/scripts/server_operate.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.2.0/tableau_utilities/tableau_file/tableau_file.py` & `tableau_utilities-2.2.11/tableau_utilities/tableau_file/tableau_file.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.2.0/tableau_utilities/tableau_file/tableau_file_objects.py` & `tableau_utilities-2.2.11/tableau_utilities/tableau_file/tableau_file_objects.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.2.0/tableau_utilities/tableau_server/base.py` & `tableau_utilities-2.2.11/tableau_utilities/tableau_server/base.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.2.0/tableau_utilities/tableau_server/create.py` & `tableau_utilities-2.2.11/tableau_utilities/tableau_server/create.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.2.0/tableau_utilities/tableau_server/download.py` & `tableau_utilities-2.2.11/tableau_utilities/tableau_server/download.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.2.0/tableau_utilities/tableau_server/get.py` & `tableau_utilities-2.2.11/tableau_utilities/tableau_server/get.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.2.0/tableau_utilities/tableau_server/publish.py` & `tableau_utilities-2.2.11/tableau_utilities/tableau_server/publish.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.2.0/tableau_utilities/tableau_server/refresh.py` & `tableau_utilities-2.2.11/tableau_utilities/tableau_server/refresh.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.2.0/tableau_utilities/tableau_server/static.py` & `tableau_utilities-2.2.11/tableau_utilities/tableau_server/static.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.2.0/tableau_utilities/tableau_server/tableau_server.py` & `tableau_utilities-2.2.11/tableau_utilities/tableau_server/tableau_server.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.2.0/tableau_utilities/tableau_server/tableau_server_objects.py` & `tableau_utilities-2.2.11/tableau_utilities/tableau_server/tableau_server_objects.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.2.0/tableau_utilities/tableau_server/update.py` & `tableau_utilities-2.2.11/tableau_utilities/tableau_server/update.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.2.0/tableau_utilities/test_tableau_utilities.py` & `tableau_utilities-2.2.11/tableau_utilities/test_tableau_utilities.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.2.0/tableau_utilities.egg-info/PKG-INFO` & `tableau_utilities-2.2.11/tableau_utilities.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tableau_utilities
-Version: 2.2.0
+Version: 2.2.11
 Summary: Utility for maintaining Tableau objects
 Home-page: http://pypi.python.org/pypi/tableau-utilities/
 Author: Justin Grilli
 Author-email: justin.grilli@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -196,15 +196,15 @@
 Generate a config from a datasource in online/server and add definitions from a csv
 ```commandline
 tableau_utilities --token_name my_token_name --token_secret 1q2w3e4r5t6y7u8i9o --site mysitename --server 10az --location online --name 'My Awseome Datasource' --project_name 'My Team Project' generate_config --definitions_csv /Desktop/new_descriptions.csv
 ```
 
 Generate a config from a local file. Add a file prefix and print the debugging logs to the console
 ```commandline
-tableau_utilities --debugging_logs generate_config --location local --file_path '/code/tableau-utilities/tmp_tdsx_and_config/My Awesome Datasource.tdsx' --file_prefix
+tableau_utilities --debugging_logs  --location local --file_path '/code/tableau-utilities/tmp_tdsx_and_config/My Awesome Datasource.tdsx' generate_config --file_prefix
 ```
 
 #### csv_config
 Write the config to a csv with 1 row per field per datasource
 ```commandline
  tableau_utilities csv_config --config_list /code/airflow/dags/tableau/configs/column_config.json /code/airflow/dags/tableau/configs/tableau_calc_config.json
 ```
```

### Comparing `tableau_utilities-2.2.0/tableau_utilities.egg-info/SOURCES.txt` & `tableau_utilities-2.2.11/tableau_utilities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

