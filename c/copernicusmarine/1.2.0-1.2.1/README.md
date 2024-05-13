# Comparing `tmp/copernicusmarine-1.2.0.tar.gz` & `tmp/copernicusmarine-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copernicusmarine-1.2.0.tar", max compression
+gzip compressed data, was "copernicusmarine-1.2.1.tar", max compression
```

## Comparing `copernicusmarine-1.2.0.tar` & `copernicusmarine-1.2.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0    13827 2024-04-25 14:08:43.428008 copernicusmarine-1.2.0/LICENSE.txt
--rw-r--r--   0        0        0    31604 2024-04-30 12:12:27.702358 copernicusmarine-1.2.0/README.md
--rw-r--r--   0        0        0      972 2024-04-25 14:08:43.432008 copernicusmarine-1.2.0/copernicusmarine/__init__.py
--rw-r--r--   0        0        0     1070 2024-04-25 14:08:43.432008 copernicusmarine-1.2.0/copernicusmarine/aioretry/LICENSE
--rw-r--r--   0        0        0      225 2024-04-25 14:08:43.432008 copernicusmarine-1.2.0/copernicusmarine/aioretry/__init__.py
--rw-r--r--   0        0        0     4152 2024-04-25 14:08:43.432008 copernicusmarine-1.2.0/copernicusmarine/aioretry/retry.py
--rw-r--r--   0        0        0       10 2024-04-25 14:08:43.432008 copernicusmarine-1.2.0/copernicusmarine/catalogue_parser/__init__.py
--rw-r--r--   0        0        0    32561 2024-04-26 11:29:37.955962 copernicusmarine-1.2.0/copernicusmarine/catalogue_parser/catalogue_parser.py
--rw-r--r--   0        0        0    11593 2024-04-30 12:12:27.702358 copernicusmarine-1.2.0/copernicusmarine/catalogue_parser/request_structure.py
--rw-r--r--   0        0        0       10 2024-04-25 14:08:43.432008 copernicusmarine-1.2.0/copernicusmarine/command_line_interface/__init__.py
--rw-r--r--   0        0        0      868 2024-04-25 14:08:43.432008 copernicusmarine-1.2.0/copernicusmarine/command_line_interface/copernicus_marine.py
--rw-r--r--   0        0        0     1766 2024-04-25 14:08:43.432008 copernicusmarine-1.2.0/copernicusmarine/command_line_interface/exception_handler.py
--rw-r--r--   0        0        0     4043 2024-04-26 11:29:37.955962 copernicusmarine-1.2.0/copernicusmarine/command_line_interface/group_describe.py
--rw-r--r--   0        0        0     9849 2024-04-29 15:45:50.086401 copernicusmarine-1.2.0/copernicusmarine/command_line_interface/group_get.py
--rw-r--r--   0        0        0     3033 2024-04-25 14:08:43.432008 copernicusmarine-1.2.0/copernicusmarine/command_line_interface/group_login.py
--rw-r--r--   0        0        0    12730 2024-04-30 12:12:27.702358 copernicusmarine-1.2.0/copernicusmarine/command_line_interface/group_subset.py
--rw-r--r--   0        0        0     2339 2024-04-25 14:08:43.432008 copernicusmarine-1.2.0/copernicusmarine/command_line_interface/utils.py
--rw-r--r--   0        0        0    13437 2024-04-25 14:08:43.432008 copernicusmarine-1.2.0/copernicusmarine/core_functions/credentials_utils.py
--rw-r--r--   0        0        0     4455 2024-04-25 14:08:43.432008 copernicusmarine-1.2.0/copernicusmarine/core_functions/custom_zarr_store.py
--rw-r--r--   0        0        0     2806 2024-04-25 14:08:43.432008 copernicusmarine-1.2.0/copernicusmarine/core_functions/deprecated.py
--rw-r--r--   0        0        0     2385 2024-04-25 14:08:43.432008 copernicusmarine-1.2.0/copernicusmarine/core_functions/deprecated_options.py
--rw-r--r--   0        0        0     2174 2024-04-26 11:29:37.955962 copernicusmarine-1.2.0/copernicusmarine/core_functions/describe.py
--rw-r--r--   0        0        0     1233 2024-04-25 14:08:43.432008 copernicusmarine-1.2.0/copernicusmarine/core_functions/environment_variables.py
--rw-r--r--   0        0        0      603 2024-04-25 14:08:43.432008 copernicusmarine-1.2.0/copernicusmarine/core_functions/exceptions.py
--rw-r--r--   0        0        0     8123 2024-04-26 11:40:58.688916 copernicusmarine-1.2.0/copernicusmarine/core_functions/get.py
--rw-r--r--   0        0        0     1606 2024-04-25 14:08:43.432008 copernicusmarine-1.2.0/copernicusmarine/core_functions/login.py
--rw-r--r--   0        0        0      460 2024-04-30 12:12:27.702358 copernicusmarine-1.2.0/copernicusmarine/core_functions/models.py
--rw-r--r--   0        0        0    19873 2024-04-26 11:29:37.955962 copernicusmarine-1.2.0/copernicusmarine/core_functions/services_utils.py
--rw-r--r--   0        0        0     2132 2024-04-25 14:08:43.432008 copernicusmarine-1.2.0/copernicusmarine/core_functions/sessions.py
--rw-r--r--   0        0        0     9735 2024-04-30 12:12:27.702358 copernicusmarine-1.2.0/copernicusmarine/core_functions/subset.py
--rw-r--r--   0        0        0     5941 2024-04-26 12:57:34.844935 copernicusmarine-1.2.0/copernicusmarine/core_functions/utils.py
--rw-r--r--   0        0        0     2683 2024-04-25 14:08:43.432008 copernicusmarine-1.2.0/copernicusmarine/core_functions/versions_verifier.py
--rw-r--r--   0        0        0     2484 2024-04-25 14:08:43.432008 copernicusmarine-1.2.0/copernicusmarine/download_functions/common_download.py
--rw-r--r--   0        0        0     8027 2024-04-30 12:12:27.702358 copernicusmarine-1.2.0/copernicusmarine/download_functions/download_arco_series.py
--rw-r--r--   0        0        0     1706 2024-04-25 14:08:43.432008 copernicusmarine-1.2.0/copernicusmarine/download_functions/download_get.py
--rw-r--r--   0        0        0    21043 2024-04-26 11:29:37.955962 copernicusmarine-1.2.0/copernicusmarine/download_functions/download_original_files.py
--rw-r--r--   0        0        0      918 2024-04-25 14:08:43.432008 copernicusmarine-1.2.0/copernicusmarine/download_functions/subset_parameters.py
--rw-r--r--   0        0        0    19923 2024-04-30 12:12:27.702358 copernicusmarine-1.2.0/copernicusmarine/download_functions/subset_xarray.py
--rw-r--r--   0        0        0     5634 2024-04-30 12:12:27.702358 copernicusmarine-1.2.0/copernicusmarine/download_functions/utils.py
--rw-r--r--   0        0        0      863 2024-04-25 14:08:43.432008 copernicusmarine-1.2.0/copernicusmarine/logging_conf.json
--rw-r--r--   0        0        0     2143 2024-04-26 11:29:37.955962 copernicusmarine-1.2.0/copernicusmarine/python_interface/describe.py
--rw-r--r--   0        0        0      447 2024-04-25 14:08:43.432008 copernicusmarine-1.2.0/copernicusmarine/python_interface/exception_handler.py
--rw-r--r--   0        0        0     5817 2024-04-26 11:01:14.733988 copernicusmarine-1.2.0/copernicusmarine/python_interface/get.py
--rw-r--r--   0        0        0     3545 2024-04-30 12:12:27.702358 copernicusmarine-1.2.0/copernicusmarine/python_interface/load_utils.py
--rw-r--r--   0        0        0     1464 2024-04-29 15:37:26.070685 copernicusmarine-1.2.0/copernicusmarine/python_interface/login.py
--rw-r--r--   0        0        0     6469 2024-04-30 12:12:27.702358 copernicusmarine-1.2.0/copernicusmarine/python_interface/open_dataset.py
--rw-r--r--   0        0        0     6150 2024-04-30 12:12:27.702358 copernicusmarine-1.2.0/copernicusmarine/python_interface/read_dataframe.py
--rw-r--r--   0        0        0     6620 2024-04-30 12:12:27.702358 copernicusmarine-1.2.0/copernicusmarine/python_interface/subset.py
--rw-r--r--   0        0        0      348 2024-04-25 14:08:43.432008 copernicusmarine-1.2.0/copernicusmarine/python_interface/utils.py
--rw-r--r--   0        0        0      901 2024-04-30 12:32:31.692464 copernicusmarine-1.2.0/pyproject.toml
--rw-r--r--   0        0        0    32677 1970-01-01 00:00:00.000000 copernicusmarine-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0    13827 2024-04-25 14:24:42.609554 copernicusmarine-1.2.1/LICENSE.txt
+-rw-r--r--   0        0        0    31604 2024-05-13 12:42:07.892682 copernicusmarine-1.2.1/README.md
+-rw-r--r--   0        0        0      972 2024-04-25 14:24:42.609554 copernicusmarine-1.2.1/copernicusmarine/__init__.py
+-rw-r--r--   0        0        0     1070 2024-04-25 14:24:42.609554 copernicusmarine-1.2.1/copernicusmarine/aioretry/LICENSE
+-rw-r--r--   0        0        0      225 2024-04-25 14:24:42.609554 copernicusmarine-1.2.1/copernicusmarine/aioretry/__init__.py
+-rw-r--r--   0        0        0     4152 2024-04-25 14:24:42.609554 copernicusmarine-1.2.1/copernicusmarine/aioretry/retry.py
+-rw-r--r--   0        0        0       10 2024-04-25 14:24:42.609554 copernicusmarine-1.2.1/copernicusmarine/catalogue_parser/__init__.py
+-rw-r--r--   0        0        0    32637 2024-05-09 13:59:27.452291 copernicusmarine-1.2.1/copernicusmarine/catalogue_parser/catalogue_parser.py
+-rw-r--r--   0        0        0    11593 2024-05-13 12:42:07.892682 copernicusmarine-1.2.1/copernicusmarine/catalogue_parser/request_structure.py
+-rw-r--r--   0        0        0       10 2024-04-25 14:24:42.609554 copernicusmarine-1.2.1/copernicusmarine/command_line_interface/__init__.py
+-rw-r--r--   0        0        0      868 2024-04-25 14:24:42.609554 copernicusmarine-1.2.1/copernicusmarine/command_line_interface/copernicus_marine.py
+-rw-r--r--   0        0        0     1766 2024-04-25 14:24:42.609554 copernicusmarine-1.2.1/copernicusmarine/command_line_interface/exception_handler.py
+-rw-r--r--   0        0        0     4043 2024-04-25 14:24:42.609554 copernicusmarine-1.2.1/copernicusmarine/command_line_interface/group_describe.py
+-rw-r--r--   0        0        0     9849 2024-04-30 10:50:17.146536 copernicusmarine-1.2.1/copernicusmarine/command_line_interface/group_get.py
+-rw-r--r--   0        0        0     3033 2024-04-25 14:24:42.609554 copernicusmarine-1.2.1/copernicusmarine/command_line_interface/group_login.py
+-rw-r--r--   0        0        0    12730 2024-05-13 12:42:07.892682 copernicusmarine-1.2.1/copernicusmarine/command_line_interface/group_subset.py
+-rw-r--r--   0        0        0     2339 2024-04-25 14:24:42.609554 copernicusmarine-1.2.1/copernicusmarine/command_line_interface/utils.py
+-rw-r--r--   0        0        0    13437 2024-05-09 14:13:11.836107 copernicusmarine-1.2.1/copernicusmarine/core_functions/credentials_utils.py
+-rw-r--r--   0        0        0     5312 2024-05-13 12:42:07.892682 copernicusmarine-1.2.1/copernicusmarine/core_functions/custom_zarr_store.py
+-rw-r--r--   0        0        0     2806 2024-04-25 14:24:42.609554 copernicusmarine-1.2.1/copernicusmarine/core_functions/deprecated.py
+-rw-r--r--   0        0        0     2385 2024-04-25 14:24:42.609554 copernicusmarine-1.2.1/copernicusmarine/core_functions/deprecated_options.py
+-rw-r--r--   0        0        0     2174 2024-04-25 14:24:42.609554 copernicusmarine-1.2.1/copernicusmarine/core_functions/describe.py
+-rw-r--r--   0        0        0     1233 2024-04-25 14:24:42.609554 copernicusmarine-1.2.1/copernicusmarine/core_functions/environment_variables.py
+-rw-r--r--   0        0        0      742 2024-05-08 09:43:19.127282 copernicusmarine-1.2.1/copernicusmarine/core_functions/exceptions.py
+-rw-r--r--   0        0        0     8123 2024-04-26 11:41:00.866629 copernicusmarine-1.2.1/copernicusmarine/core_functions/get.py
+-rw-r--r--   0        0        0     1606 2024-04-25 14:24:42.609554 copernicusmarine-1.2.1/copernicusmarine/core_functions/login.py
+-rw-r--r--   0        0        0      460 2024-05-13 12:42:07.892682 copernicusmarine-1.2.1/copernicusmarine/core_functions/models.py
+-rw-r--r--   0        0        0    20227 2024-05-13 12:42:07.892682 copernicusmarine-1.2.1/copernicusmarine/core_functions/services_utils.py
+-rw-r--r--   0        0        0     1984 2024-05-13 12:42:07.892682 copernicusmarine-1.2.1/copernicusmarine/core_functions/sessions.py
+-rw-r--r--   0        0        0     9735 2024-05-13 12:42:07.892682 copernicusmarine-1.2.1/copernicusmarine/core_functions/subset.py
+-rw-r--r--   0        0        0     6536 2024-05-13 12:42:07.892682 copernicusmarine-1.2.1/copernicusmarine/core_functions/utils.py
+-rw-r--r--   0        0        0     2688 2024-05-13 12:42:07.892682 copernicusmarine-1.2.1/copernicusmarine/core_functions/versions_verifier.py
+-rw-r--r--   0        0        0     2673 2024-05-07 15:20:12.688685 copernicusmarine-1.2.1/copernicusmarine/download_functions/common_download.py
+-rw-r--r--   0        0        0     8027 2024-05-13 12:42:07.892682 copernicusmarine-1.2.1/copernicusmarine/download_functions/download_arco_series.py
+-rw-r--r--   0        0        0     1706 2024-04-25 14:24:42.609554 copernicusmarine-1.2.1/copernicusmarine/download_functions/download_get.py
+-rw-r--r--   0        0        0    20555 2024-05-13 12:42:07.892682 copernicusmarine-1.2.1/copernicusmarine/download_functions/download_original_files.py
+-rw-r--r--   0        0        0      918 2024-04-25 14:24:42.609554 copernicusmarine-1.2.1/copernicusmarine/download_functions/subset_parameters.py
+-rw-r--r--   0        0        0    19923 2024-05-13 12:59:26.194277 copernicusmarine-1.2.1/copernicusmarine/download_functions/subset_xarray.py
+-rw-r--r--   0        0        0     5634 2024-04-30 10:50:17.146536 copernicusmarine-1.2.1/copernicusmarine/download_functions/utils.py
+-rw-r--r--   0        0        0      863 2024-04-25 14:24:42.609554 copernicusmarine-1.2.1/copernicusmarine/logging_conf.json
+-rw-r--r--   0        0        0     2143 2024-04-25 14:24:42.609554 copernicusmarine-1.2.1/copernicusmarine/python_interface/describe.py
+-rw-r--r--   0        0        0      447 2024-04-25 14:24:42.609554 copernicusmarine-1.2.1/copernicusmarine/python_interface/exception_handler.py
+-rw-r--r--   0        0        0     5817 2024-04-26 11:29:39.854618 copernicusmarine-1.2.1/copernicusmarine/python_interface/get.py
+-rw-r--r--   0        0        0     3545 2024-05-13 12:42:07.896682 copernicusmarine-1.2.1/copernicusmarine/python_interface/load_utils.py
+-rw-r--r--   0        0        0     1464 2024-04-30 10:50:17.146536 copernicusmarine-1.2.1/copernicusmarine/python_interface/login.py
+-rw-r--r--   0        0        0     6469 2024-05-13 12:42:07.896682 copernicusmarine-1.2.1/copernicusmarine/python_interface/open_dataset.py
+-rw-r--r--   0        0        0     6150 2024-05-13 12:42:07.896682 copernicusmarine-1.2.1/copernicusmarine/python_interface/read_dataframe.py
+-rw-r--r--   0        0        0     6620 2024-05-13 12:42:07.896682 copernicusmarine-1.2.1/copernicusmarine/python_interface/subset.py
+-rw-r--r--   0        0        0      348 2024-04-25 14:24:42.609554 copernicusmarine-1.2.1/copernicusmarine/python_interface/utils.py
+-rw-r--r--   0        0        0      901 2024-05-13 12:59:26.194277 copernicusmarine-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0    32677 1970-01-01 00:00:00.000000 copernicusmarine-1.2.1/PKG-INFO
```

### Comparing `copernicusmarine-1.2.0/LICENSE.txt` & `copernicusmarine-1.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.0/README.md` & `copernicusmarine-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.0/copernicusmarine/__init__.py` & `copernicusmarine-1.2.1/copernicusmarine/__init__.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.0/copernicusmarine/aioretry/LICENSE` & `copernicusmarine-1.2.1/copernicusmarine/aioretry/LICENSE`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.0/copernicusmarine/aioretry/retry.py` & `copernicusmarine-1.2.1/copernicusmarine/aioretry/retry.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.0/copernicusmarine/catalogue_parser/catalogue_parser.py` & `copernicusmarine-1.2.1/copernicusmarine/catalogue_parser/catalogue_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,20 +52,22 @@
     TIMESERIES = "timeseries"
     FILES = "files"
     WMTS = "wmts"
     OMI_ARCO = "omi-arco"
     STATIC_ARCO = "static-arco"
 
 
-MARINE_DATA_STORE_STAC_BASE_URL = "https://stac.marine.copernicus.eu/metadata"
+MARINE_DATA_STORE_STAC_BASE_URL = (
+    "https://s3.waw3-1.cloudferro.com/mdl-metadata/metadata"
+)
 MARINE_DATA_STORE_STAC_ROOT_CATALOG_URL = (
     MARINE_DATA_STORE_STAC_BASE_URL + "/catalog.stac.json"
 )
 MARINE_DATA_STORE_STAC_BASE_URL_STAGING = (
-    "https://stac-dta.marine.copernicus.eu/metadata"
+    "https://s3.waw3-1.cloudferro.com/mdl-metadata-dta/metadata"
 )
 MARINE_DATA_STORE_STAC_ROOT_CATALOG_URL_STAGING = (
     MARINE_DATA_STORE_STAC_BASE_URL_STAGING + "/catalog.stac.json"
 )
 
 MAX_CONCURRENT_REQUESTS = int(COPERNICUSMARINE_MAX_CONCURRENT_REQUESTS)
 
@@ -817,14 +819,15 @@
     catalog_root_url = (
         MARINE_DATA_STORE_STAC_ROOT_CATALOG_URL
         if not staging
         else MARINE_DATA_STORE_STAC_ROOT_CATALOG_URL_STAGING
     )
     json_catalog = await connection.get_json_file(catalog_root_url)
     catalog = pystac.Catalog.from_dict(json_catalog)
+    catalog.set_self_href(catalog_root_url)
     child_links = catalog.get_child_links()
     root_url = (
         MARINE_DATA_STORE_STAC_BASE_URL
         if not staging
         else (MARINE_DATA_STORE_STAC_BASE_URL_STAGING)
     )
     childs = await async_fetch_childs(root_url, connection, child_links)
```

### Comparing `copernicusmarine-1.2.0/copernicusmarine/catalogue_parser/request_structure.py` & `copernicusmarine-1.2.1/copernicusmarine/catalogue_parser/request_structure.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.0/copernicusmarine/command_line_interface/copernicus_marine.py` & `copernicusmarine-1.2.1/copernicusmarine/command_line_interface/copernicus_marine.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.0/copernicusmarine/command_line_interface/exception_handler.py` & `copernicusmarine-1.2.1/copernicusmarine/command_line_interface/exception_handler.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.0/copernicusmarine/command_line_interface/group_describe.py` & `copernicusmarine-1.2.1/copernicusmarine/command_line_interface/group_describe.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.0/copernicusmarine/command_line_interface/group_get.py` & `copernicusmarine-1.2.1/copernicusmarine/command_line_interface/group_get.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.0/copernicusmarine/command_line_interface/group_login.py` & `copernicusmarine-1.2.1/copernicusmarine/command_line_interface/group_login.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.0/copernicusmarine/command_line_interface/group_subset.py` & `copernicusmarine-1.2.1/copernicusmarine/command_line_interface/group_subset.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.0/copernicusmarine/command_line_interface/utils.py` & `copernicusmarine-1.2.1/copernicusmarine/command_line_interface/utils.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.0/copernicusmarine/core_functions/credentials_utils.py` & `copernicusmarine-1.2.1/copernicusmarine/core_functions/credentials_utils.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.0/copernicusmarine/core_functions/custom_zarr_store.py` & `copernicusmarine-1.2.1/copernicusmarine/core_functions/custom_zarr_store.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,28 +3,30 @@
 from collections.abc import MutableMapping
 from typing import Optional
 
 import botocore.config
 import botocore.exceptions
 import botocore.session
 
-log = logging.getLogger("copernicus_marine_root_logger")
+from copernicusmarine.core_functions.utils import create_custom_query_function
 
-S3_NUM_RETRIES = 9
-S3_INITIAL_RETRY_WAIT_S = 1
+logger = logging.getLogger("copernicus_marine_root_logger")
 
 
 class CustomS3Store(MutableMapping):
     def __init__(
         self,
         endpoint: str,
         bucket: str,
         root_path: str,
         secret_key: Optional[str] = None,
         access_key: Optional[str] = None,
+        copernicus_marine_username: Optional[str] = None,
+        number_of_retries: int = 9,
+        initial_retry_wait_seconds: int = 1,
     ):
         self._root_path = root_path.lstrip("/")
         self._bucket = bucket
         session = botocore.session.get_session()
         if secret_key is None and access_key is None:
             self.client = session.create_client(
                 "s3",
@@ -36,27 +38,42 @@
         else:
             self.client = session.create_client(
                 "s3",
                 endpoint_url=endpoint,
                 aws_secret_access_key=secret_key,
                 aws_access_key_id=access_key,
             )
+        self.client.meta.events.register(
+            "before-call.s3.ListObjects",
+            create_custom_query_function(copernicus_marine_username),
+        )
+        self.client.meta.events.register(
+            "before-call.s3.HeadObject",
+            create_custom_query_function(copernicus_marine_username),
+        )
+        self.client.meta.events.register(
+            "before-call.s3.GetObject",
+            create_custom_query_function(copernicus_marine_username),
+        )
+
+        self.number_of_retries = number_of_retries
+        self.initial_retry_wait_seconds = initial_retry_wait_seconds
 
     def __getitem__(self, key):
         def fn():
             full_key = f"{self._root_path}/{key}"
             try:
                 resp = self.client.get_object(
                     Bucket=self._bucket, Key=full_key
                 )
                 return resp["Body"].read()
             except botocore.exceptions.ClientError as e:
                 raise KeyError(key) from e
 
-        return with_retries(fn)
+        return self.with_retries(fn)
 
     def __contains__(self, key):
         full_key = f"{self._root_path}/{key}"
         try:
             self.client.head_object(Bucket=self._bucket, Key=full_key)
             return True
         except botocore.exceptions.ClientError as e:
@@ -68,26 +85,25 @@
         def fn():
             full_key = f"{self._root_path}/{key}"
             final_headers = headers if headers is not None else {}
             self.client.put_object(
                 Bucket=self._bucket, Key=full_key, Body=value, **final_headers
             )
 
-        return with_retries(fn)
+        return self.with_retries(fn)
 
     def __delitem__(self, key):
         def fn():
             full_key = f"{self._root_path}/{key}"
             self.client.delete_object(Bucket=self._bucket, Key=full_key)
 
-        return with_retries(fn)
+        return self.with_retries(fn)
 
     # Example of headers: {"ContentType": "application/json", "ContentEncoding": "gzip"}
     def set_item_with_headers(self, key, value, headers):
-        # pylint: disable=unnecessary-dunder-call
         return self.__setitem__(key, value, headers)
 
     def keys(self):
         keys = []
         cursor = self._root_path
         while True:
             resp = self.client.list_objects_v2(
@@ -119,25 +135,24 @@
                 map(lambda k: {"Key": f"{self._root_path}/{k}"}, some_keys)
             )
             self.client.delete_objects(
                 Bucket=self._bucket, Delete={"Objects": objects}
             )
             idx += 1000
 
-
-def with_retries(fn):
-    retry_delay = S3_INITIAL_RETRY_WAIT_S
-    for idx_try in range(S3_NUM_RETRIES):
-        try:
-            return fn()
-        # KeyError is a normal error that we want to propagate
-        # (e.g. if we try to get a chunk and it doesn't exist,
-        # we want the caller to know this has happened -- and not retry!)
-        except KeyError:
-            raise
-        except Exception as e:
-            if idx_try == S3_NUM_RETRIES - 1:
-                raise e
-            log.error(f"S3 error: {e}")
-            log.info(f"Retrying in {retry_delay} s...")
-            time.sleep(retry_delay)
-            retry_delay *= 2
+    def with_retries(self, fn):
+        retry_delay = self.initial_retry_wait_seconds
+        for index_try in range(self.number_of_retries):
+            try:
+                return fn()
+            # KeyError is a normal error that we want to propagate
+            # (e.g. if we try to get a chunk and it doesn't exist,
+            # we want the caller to know this has happened -- and not retry!)
+            except KeyError:
+                raise
+            except Exception as e:
+                if index_try == self.number_of_retries - 1:
+                    raise e
+                logger.debug(f"S3 error: {e}")
+                logger.debug(f"Retrying in {retry_delay} s...")
+                time.sleep(retry_delay)
+                retry_delay *= 2
```

### Comparing `copernicusmarine-1.2.0/copernicusmarine/core_functions/deprecated.py` & `copernicusmarine-1.2.1/copernicusmarine/core_functions/deprecated.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.0/copernicusmarine/core_functions/deprecated_options.py` & `copernicusmarine-1.2.1/copernicusmarine/core_functions/deprecated_options.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.0/copernicusmarine/core_functions/describe.py` & `copernicusmarine-1.2.1/copernicusmarine/core_functions/describe.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.0/copernicusmarine/core_functions/environment_variables.py` & `copernicusmarine-1.2.1/copernicusmarine/core_functions/environment_variables.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.0/copernicusmarine/core_functions/get.py` & `copernicusmarine-1.2.1/copernicusmarine/core_functions/get.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.0/copernicusmarine/core_functions/login.py` & `copernicusmarine-1.2.1/copernicusmarine/core_functions/login.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.0/copernicusmarine/core_functions/services_utils.py` & `copernicusmarine-1.2.1/copernicusmarine/core_functions/services_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -150,19 +150,22 @@
         _service_not_available_error(dataset_version_part, command_type),
     )
 
 
 def _get_best_arco_service_type(
     dataset_subset: DatasetTimeAndGeographicalSubset,
     dataset_url: str,
+    username: Optional[str],
 ) -> Literal[
     CopernicusMarineDatasetServiceType.TIMESERIES,
     CopernicusMarineDatasetServiceType.GEOSERIES,
 ]:
-    dataset = sessions.open_zarr(dataset_url)
+    dataset = sessions.open_zarr(
+        dataset_url, copernicus_marine_username=username
+    )
 
     latitude_size = get_size_of_coordinate_subset(
         dataset,
         "latitude",
         dataset_subset.minimum_latitude,
         dataset_subset.maximum_latitude,
     )
@@ -213,14 +216,15 @@
     )
 
 
 def _select_service_by_priority(
     dataset_version_part: CopernicusMarineVersionPart,
     command_type: CommandType,
     dataset_subset: Optional[DatasetTimeAndGeographicalSubset],
+    username: Optional[str],
 ) -> CopernicusMarineService:
     dataset_available_service_types = [
         service.service_type for service in dataset_version_part.services
     ]
     first_available_service_type = _get_first_available_service_type(
         command_type=command_type,
         dataset_available_service_types=dataset_available_service_types,
@@ -241,15 +245,15 @@
             == CopernicusMarineServiceFormat.SQLITE
         ):
             raise FormatNotSupported(
                 first_available_service.service_format.value
             )
         best_arco_service_type: CopernicusMarineDatasetServiceType = (
             _get_best_arco_service_type(
-                dataset_subset, first_available_service.uri
+                dataset_subset, first_available_service.uri, username
             )
         )
         return dataset_version_part.get_service_by_service_type(
             best_arco_service_type
         )
     return first_available_service
 
@@ -303,14 +307,15 @@
     force_dataset_version_label: Optional[str],
     force_dataset_part_label: Optional[str],
     force_service_type_string: Optional[str],
     command_type: CommandType,
     index_parts: bool = False,
     dataset_subset: Optional[DatasetTimeAndGeographicalSubset] = None,
     dataset_sync: bool = False,
+    username: Optional[str] = None,
 ) -> RetrievalService:
     force_service_type: Optional[CopernicusMarineDatasetServiceType] = (
         _service_type_from_string(force_service_type_string, command_type)
         if force_service_type_string
         else None
     )
     if dataset_id is None:
@@ -339,28 +344,30 @@
         force_dataset_version_label=force_dataset_version_label,
         force_dataset_part_label=force_dataset_part_label,
         force_service_type=force_service_type,
         command_type=command_type,
         index_parts=index_parts,
         dataset_subset=dataset_subset,
         dataset_sync=dataset_sync,
+        username=username,
     )
 
 
 def _get_retrieval_service_from_dataset_id(
     catalogue: CopernicusMarineCatalogue,
     dataset_id: str,
     suffix_path: str,
     force_dataset_version_label: Optional[str],
     force_dataset_part_label: Optional[str],
     force_service_type: Optional[CopernicusMarineDatasetServiceType],
     command_type: CommandType,
     index_parts: bool,
     dataset_subset: Optional[DatasetTimeAndGeographicalSubset],
     dataset_sync: bool,
+    username: Optional[str],
 ) -> RetrievalService:
     dataset: CopernicusMarineProductDataset = next_or_raise_exception(
         (
             dataset
             for product in catalogue.products
             for dataset in product.datasets
             if dataset_id == dataset.dataset_id
@@ -377,27 +384,29 @@
         force_dataset_version_label=force_dataset_version_label,
         force_dataset_part_label=force_dataset_part_label,
         force_service_type=force_service_type,
         command_type=command_type,
         index_parts=index_parts,
         dataset_subset=dataset_subset,
         dataset_sync=dataset_sync,
+        username=username,
     )
 
 
 def _get_retrieval_service_from_dataset(
     dataset: CopernicusMarineProductDataset,
     suffix_path: str,
     force_dataset_version_label: Optional[str],
     force_dataset_part_label: Optional[str],
     force_service_type: Optional[CopernicusMarineDatasetServiceType],
     command_type: CommandType,
     index_parts: bool,
     dataset_subset: Optional[DatasetTimeAndGeographicalSubset],
     dataset_sync: bool,
+    username: Optional[str],
 ) -> RetrievalService:
     if force_dataset_version_label:
         logger.info(
             "You forced selection of dataset version "
             + f'"{force_dataset_version_label}"'
         )
     dataset_version = dataset.get_version(force_dataset_version_label)
@@ -412,27 +421,29 @@
         force_dataset_part_label=force_dataset_part_label,
         suffix_path=suffix_path,
         force_service_type=force_service_type,
         command_type=command_type,
         index_parts=index_parts,
         dataset_subset=dataset_subset,
         dataset_sync=dataset_sync,
+        username=username,
     )
 
 
 def _get_retrieval_service_from_dataset_version(
     dataset_id: str,
     dataset_version: CopernicusMarineDatasetVersion,
     force_dataset_part_label: Optional[str],
     suffix_path: str,
     force_service_type: Optional[CopernicusMarineDatasetServiceType],
     command_type: CommandType,
     index_parts: bool,
     dataset_subset: Optional[DatasetTimeAndGeographicalSubset],
     dataset_sync: bool,
+    username: Optional[str],
 ) -> RetrievalService:
     if len(dataset_version.parts) > 1 and dataset_sync:
         raise Exception(
             "Sync is not supported for datasets with multiple parts."
         )
     if (
         force_service_type == CopernicusMarineDatasetServiceType.FILES
@@ -480,14 +491,15 @@
         if service.service_format == CopernicusMarineServiceFormat.SQLITE:
             raise FormatNotSupported(service.service_format.value)
     else:
         service = _select_service_by_priority(
             dataset_version_part=dataset_part,
             command_type=command_type,
             dataset_subset=dataset_subset,
+            username=username,
         )
         logger.info(
             "Service was not specified, the default one was "
             f'selected: "{service.service_type.service_name.value}"'
         )
     dataset_start_date = _get_dataset_start_date_from_service(service)
     return RetrievalService(
```

### Comparing `copernicusmarine-1.2.0/copernicusmarine/core_functions/sessions.py` & `copernicusmarine-1.2.1/copernicusmarine/core_functions/sessions.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,18 +10,15 @@
 from copernicusmarine.core_functions.custom_zarr_store import CustomS3Store
 from copernicusmarine.core_functions.environment_variables import (
     COPERNICUSMARINE_DISABLE_SSL_CONTEXT,
     COPERNICUSMARINE_TRUST_ENV,
     PROXY_HTTP,
     PROXY_HTTPS,
 )
-from copernicusmarine.core_functions.utils import (
-    construct_query_params_for_marine_data_store_monitoring,
-    parse_access_dataset_url,
-)
+from copernicusmarine.core_functions.utils import parse_access_dataset_url
 
 TRUST_ENV = COPERNICUSMARINE_TRUST_ENV == "True"
 PROXIES = {}
 if PROXY_HTTP:
     PROXIES["http"] = PROXY_HTTP
 if PROXY_HTTPS:
     PROXIES["https"] = PROXY_HTTPS
@@ -58,21 +55,21 @@
 ) -> xarray.Dataset:
     (
         endpoint,
         bucket,
         root_path,
     ) = parse_access_dataset_url(dataset_url)
     store = CustomS3Store(
-        endpoint=endpoint, bucket=bucket, root_path=root_path
+        endpoint=endpoint,
+        bucket=bucket,
+        root_path=root_path,
+        copernicus_marine_username=copernicus_marine_username,
     )
     kwargs.update(
         {
             "storage_options": {
-                "params": construct_query_params_for_marine_data_store_monitoring(
-                    username=copernicus_marine_username
-                ),
                 "client_kwargs": {"trust_env": TRUST_ENV, "proxies": PROXIES},
                 "ssl": _get_ssl_context(),
             }
         }
     )
     return xarray.open_zarr(store, **kwargs)
```

### Comparing `copernicusmarine-1.2.0/copernicusmarine/core_functions/subset.py` & `copernicusmarine-1.2.1/copernicusmarine/core_functions/subset.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.0/copernicusmarine/core_functions/utils.py` & `copernicusmarine-1.2.1/copernicusmarine/core_functions/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 )
 
 import cftime
 import numpy
 import xarray
 from requests import PreparedRequest
 
+from copernicusmarine import __version__ as copernicusmarine_version
 from copernicusmarine.core_functions.environment_variables import (
     COPERNICUSMARINE_CACHE_DIRECTORY,
 )
 
 logger = logging.getLogger("copernicus_marine_root_logger")
 
 OVERWRITE_SHORT_OPTION = "--overwrite"
@@ -35,22 +36,22 @@
 OVERWRITE_OPTION_HELP_TEXT = (
     "If specified and if the file already exists on destination, then it will be "
     "overwritten instead of creating new one with unique index."
 )
 
 FORCE_DOWNLOAD_CLI_PROMPT_MESSAGE = "Do you want to proceed with download?"
 
-USER_DEFINED_CACHE_DIRECTORY = COPERNICUSMARINE_CACHE_DIRECTORY
-DEFAULT_CLIENT_BASE_DIRECTORY = (
+USER_DEFINED_CACHE_DIRECTORY: str = COPERNICUSMARINE_CACHE_DIRECTORY
+DEFAULT_CLIENT_BASE_DIRECTORY: pathlib.Path = (
     pathlib.Path(USER_DEFINED_CACHE_DIRECTORY)
     if USER_DEFINED_CACHE_DIRECTORY
     else pathlib.Path.home()
 ) / ".copernicusmarine"
 
-CACHE_BASE_DIRECTORY = DEFAULT_CLIENT_BASE_DIRECTORY / "cache"
+CACHE_BASE_DIRECTORY: pathlib.Path = DEFAULT_CLIENT_BASE_DIRECTORY / "cache"
 
 DATETIME_SUPPORTED_FORMATS = [
     "%Y",
     "%Y-%m-%d",
     "%Y-%m-%dT%H:%M:%S",
     "%Y-%m-%d %H:%M:%S",
     "%Y-%m-%dT%H:%M:%S.%fZ",
@@ -115,15 +116,18 @@
     req.prepare_url(url, query_params)
     return req.url
 
 
 def construct_query_params_for_marine_data_store_monitoring(
     username: Optional[str] = None,
 ) -> dict:
-    query_params = {"x-cop-client": "copernicus-marine-client"}
+    query_params = {
+        "x-cop-client": "copernicus-marine-toolbox",
+        "x-cop-client-version": copernicusmarine_version,
+    }
     if username:
         query_params["x-cop-user"] = username
     return query_params
 
 
 class WrongDatetimeFormat(Exception):
     ...
@@ -214,7 +218,20 @@
             "/".join(segments[2:])
             if not only_dataset_root_path
             else "/".join(segments[2:5]) + "/"
         )
         return endpoint_url, bucket, path
     else:
         raise Exception(f"Invalid data path: {data_path}")
+
+
+def create_custom_query_function(username: Optional[str]) -> Callable:
+    def _add_custom_query_param(params, context, **kwargs):
+        """
+        Add custom query params for MDS's Monitoring
+        """
+        params["url"] = construct_url_with_query_params(
+            params["url"],
+            construct_query_params_for_marine_data_store_monitoring(username),
+        )
+
+    return _add_custom_query_param
```

### Comparing `copernicusmarine-1.2.0/copernicusmarine/core_functions/versions_verifier.py` & `copernicusmarine-1.2.1/copernicusmarine/core_functions/versions_verifier.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 
 import semver
 
-import copernicusmarine
+from copernicusmarine import __version__ as client_version
 from copernicusmarine.core_functions.sessions import (
     get_configured_request_session,
 )
 from copernicusmarine.core_functions.utils import (
     construct_query_params_for_marine_data_store_monitoring,
 )
 
@@ -33,15 +33,14 @@
         VersionVerifier._check_version("subset", staging)
 
     @staticmethod
     def _check_version(function_name: str, staging: bool):
         marine_data_store_versions = (
             VersionVerifier._get_client_required_versions(staging)
         )
-        client_version = copernicusmarine.__version__
         for (
             service
         ) in VersionVerifier.function_marine_data_store_service_mapping[
             function_name
         ]:
             required_version = marine_data_store_versions[service]
             if not semver.Version.parse(client_version).match(
@@ -57,17 +56,17 @@
                 )
 
     @staticmethod
     def _get_client_required_versions(
         staging: bool,
     ) -> dict[str, str]:
         url_mds_versions = (
-            "https://stac-dta.marine.copernicus.eu/mdsVersions.json"
+            "https://s3.waw3-1.cloudferro.com/mdl-metadata-dta/mdsVersions.json"
             if staging
-            else "https://stac.marine.copernicus.eu/mdsVersions.json"
+            else "https://s3.waw3-1.cloudferro.com/mdl-metadata/mdsVersions.json"
         )
         logger.debug(f"Getting required versions from {url_mds_versions}")
         session = get_configured_request_session()
         mds_versions: dict[str, str] = session.get(
             url_mds_versions,
             params=construct_query_params_for_marine_data_store_monitoring(),
             proxies=session.proxies,
```

### Comparing `copernicusmarine-1.2.0/copernicusmarine/download_functions/common_download.py` & `copernicusmarine-1.2.1/copernicusmarine/download_functions/common_download.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 import pathlib
-from typing import Optional
+from typing import Any, Optional
 
 import xarray
 import zarr
 from dask.delayed import Delayed
 from tqdm.dask import TqdmCallback
 
 from copernicusmarine.core_functions.exceptions import (
@@ -53,25 +53,31 @@
     dataset: xarray.Dataset,
     output_path: pathlib.Path,
     netcdf_compression_enabled: bool,
     netcdf_compression_level: Optional[int],
     netcdf3_compatible: bool,
 ):
     logger.debug("Writing dataset to NetCDF")
+    encoding: dict[str, Any]
+    encoding = {f"{coord}": {"_FillValue": None} for coord in dataset.coords}
     if netcdf_compression_enabled:
         complevel = (
             1 if netcdf_compression_level is None else netcdf_compression_level
         )
         logger.info(f"NetCDF compression enabled with level {complevel}")
         comp = dict(
-            zlib=True, complevel=complevel, contiguous=False, shuffle=True
+            zlib=True,
+            complevel=complevel,
+            contiguous=False,
+            shuffle=True,
+            _FillValue=None,
         )
-        encoding = {var: comp for var in dataset.data_vars}
-    else:
-        encoding = None
+        encoding_vars = {var: comp for var in dataset.data_vars}
+        encoding.update(encoding_vars)
+
     xarray_download_format = "NETCDF3_CLASSIC" if netcdf3_compatible else None
     return dataset.to_netcdf(
         output_path,
         mode="w",
         compute=False,
         encoding=encoding,
         format=xarray_download_format,
```

### Comparing `copernicusmarine-1.2.0/copernicusmarine/download_functions/download_arco_series.py` & `copernicusmarine-1.2.1/copernicusmarine/download_functions/download_arco_series.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.0/copernicusmarine/download_functions/download_get.py` & `copernicusmarine-1.2.1/copernicusmarine/download_functions/download_get.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.0/copernicusmarine/download_functions/download_original_files.py` & `copernicusmarine-1.2.1/copernicusmarine/download_functions/download_original_files.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import logging
 import os
 import pathlib
 import re
 from itertools import chain
 from multiprocessing.pool import ThreadPool
 from pathlib import Path
-from typing import Callable, List, Optional, Tuple
+from typing import List, Optional, Tuple
 
 import boto3
 import botocore
 import botocore.config
 import click
 from botocore.client import ClientError
 from numpy import append, arange
@@ -18,16 +18,15 @@
 
 from copernicusmarine.catalogue_parser.request_structure import (
     GetRequest,
     overload_regex_with_additionnal_filter,
 )
 from copernicusmarine.core_functions.utils import (
     FORCE_DOWNLOAD_CLI_PROMPT_MESSAGE,
-    construct_query_params_for_marine_data_store_monitoring,
-    construct_url_with_query_params,
+    create_custom_query_function,
     flatten,
     get_unique_filename,
     parse_access_dataset_url,
 )
 
 logger = logging.getLogger("copernicus_marine_root_logger")
 
@@ -430,27 +429,14 @@
 
 def _local_path_from_s3_url(
     s3_url: str, local_directory: pathlib.Path
 ) -> pathlib.Path:
     return local_directory / pathlib.Path("/".join(s3_url.split("/")[4:]))
 
 
-def _create_custom_query_function(username: str) -> Callable:
-    def _add_custom_query_param(params, context, **kwargs):
-        """
-        Add custom query params for MDS's Monitoring
-        """
-        params["url"] = construct_url_with_query_params(
-            params["url"],
-            construct_query_params_for_marine_data_store_monitoring(username),
-        )
-
-    return _add_custom_query_param
-
-
 def _list_files_on_marine_data_lake_s3(
     username: str,
     endpoint_url: str,
     bucket: str,
     prefix: str,
     recursive: bool,
 ) -> list[tuple[str, int, datetime.datetime, str]]:
@@ -465,15 +451,15 @@
         ),
         endpoint_url=endpoint_url,
     )
 
     # Register the botocore event handler for adding custom query params
     # to S3 LIST requests
     s3_client.meta.events.register(
-        "before-call.s3.ListObjects", _create_custom_query_function(username)
+        "before-call.s3.ListObjects", create_custom_query_function(username)
     )
 
     paginator = s3_client.get_paginator("list_objects")
     page_iterator = paginator.paginate(
         Bucket=bucket,
         Prefix=prefix,
         Delimiter="/" if not recursive else "",
@@ -506,15 +492,15 @@
             s3={"addressing_style": "virtual"},
             signature_version=botocore.UNSIGNED,
         ),
         endpoint_url=endpoint_url,
     )
 
     s3_client.meta.events.register(
-        "before-call.s3.HeadObject", _create_custom_query_function(username)
+        "before-call.s3.HeadObject", create_custom_query_function(username)
     )
 
     try:
         s3_object = s3_client.head_object(
             Bucket=bucket,
             Key=file_in.replace(f"s3://{bucket}/", ""),
         )
@@ -568,18 +554,18 @@
             endpoint_url=endpoint_url,
         )
 
         # Register the botocore event handler for adding custom query params
         # to S3 HEAD and GET requests
         s3_client.meta.events.register(
             "before-call.s3.HeadObject",
-            _create_custom_query_function(username),
+            create_custom_query_function(username),
         )
         s3_client.meta.events.register(
-            "before-call.s3.GetObject", _create_custom_query_function(username)
+            "before-call.s3.GetObject", create_custom_query_function(username)
         )
 
         last_modified_date_epoch = s3_resource.Object(
             bucket, file_in.replace(f"s3://{bucket}/", "")
         ).last_modified.timestamp()
 
         s3_client.download_file(
```

### Comparing `copernicusmarine-1.2.0/copernicusmarine/download_functions/subset_parameters.py` & `copernicusmarine-1.2.1/copernicusmarine/download_functions/subset_parameters.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.0/copernicusmarine/download_functions/subset_xarray.py` & `copernicusmarine-1.2.1/copernicusmarine/download_functions/subset_xarray.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.0/copernicusmarine/download_functions/utils.py` & `copernicusmarine-1.2.1/copernicusmarine/download_functions/utils.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.0/copernicusmarine/logging_conf.json` & `copernicusmarine-1.2.1/copernicusmarine/logging_conf.json`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.0/copernicusmarine/python_interface/describe.py` & `copernicusmarine-1.2.1/copernicusmarine/python_interface/describe.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.0/copernicusmarine/python_interface/get.py` & `copernicusmarine-1.2.1/copernicusmarine/python_interface/get.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.0/copernicusmarine/python_interface/load_utils.py` & `copernicusmarine-1.2.1/copernicusmarine/python_interface/load_utils.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.0/copernicusmarine/python_interface/login.py` & `copernicusmarine-1.2.1/copernicusmarine/python_interface/login.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.0/copernicusmarine/python_interface/open_dataset.py` & `copernicusmarine-1.2.1/copernicusmarine/python_interface/open_dataset.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.0/copernicusmarine/python_interface/read_dataframe.py` & `copernicusmarine-1.2.1/copernicusmarine/python_interface/read_dataframe.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.0/copernicusmarine/python_interface/subset.py` & `copernicusmarine-1.2.1/copernicusmarine/python_interface/subset.py`

 * *Files identical despite different names*

### Comparing `copernicusmarine-1.2.0/pyproject.toml` & `copernicusmarine-1.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "copernicusmarine"
-version = "1.2.0"
+version = "1.2.1"
 description = ""
 authors = ["Copernicus Marine User Support <servicedesk.cmems@mercator-ocean.eu>"]
 readme = "README.md"
 packages = [{include = "copernicusmarine"}]
 license = "EUPL-1.2"
 
 [tool.poetry.dependencies]
```

### Comparing `copernicusmarine-1.2.0/PKG-INFO` & `copernicusmarine-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copernicusmarine
-Version: 1.2.0
+Version: 1.2.1
 Summary: 
 License: EUPL-1.2
 Author: Copernicus Marine User Support
 Author-email: servicedesk.cmems@mercator-ocean.eu
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: copernicusmarine Version: 1.2.0 Summary: License:
+Metadata-Version: 2.1 Name: copernicusmarine Version: 1.2.1 Summary: License:
 EUPL-1.2 Author: Copernicus Marine User Support Author-email:
 servicedesk.cmems@mercator-ocean.eu Requires-Python: >=3.9,<3.13 Classifier:
 License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Requires-Dist: aiohttp (>=3.9.4) Requires-Dist:
```

