# Comparing `tmp/hdsr_wis_config_reader-1.8.tar.gz` & `tmp/hdsr_wis_config_reader-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\hdsr_wis_config_reader-1.8.tar", last modified: Mon Dec 20 12:47:13 2021, max compression
+gzip compressed data, was "dist\hdsr_wis_config_reader-1.9.tar", last modified: Fri Jan  7 16:29:34 2022, max compression
```

## Comparing `hdsr_wis_config_reader-1.8.tar` & `hdsr_wis_config_reader-1.9.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxrwx   0        0        0        0 2021-12-20 12:47:14.000000 hdsr_wis_config_reader-1.8/
--rw-rw-rw-   0        0        0     1086 2021-11-16 15:31:24.000000 hdsr_wis_config_reader-1.8/LICENSE
--rw-rw-rw-   0        0        0    11656 2021-12-20 12:47:16.000000 hdsr_wis_config_reader-1.8/PKG-INFO
--rw-rw-rw-   0        0        0    10842 2021-12-07 13:36:13.000000 hdsr_wis_config_reader-1.8/README.md
-drwxrwxrwx   0        0        0        0 2021-12-20 12:47:14.000000 hdsr_wis_config_reader-1.8/hdsr_wis_config_reader/
--rw-rw-rw-   0        0        0      570 2021-11-22 10:52:30.000000 hdsr_wis_config_reader-1.8/hdsr_wis_config_reader/__init__.py
--rw-rw-rw-   0        0        0      350 2021-11-22 19:00:44.000000 hdsr_wis_config_reader-1.8/hdsr_wis_config_reader/constants.py
-drwxrwxrwx   0        0        0        0 2021-12-20 12:47:14.000000 hdsr_wis_config_reader-1.8/hdsr_wis_config_reader/idmappings/
--rw-rw-rw-   0        0        0        0 2021-11-22 09:27:01.000000 hdsr_wis_config_reader-1.8/hdsr_wis_config_reader/idmappings/__init__.py
--rw-rw-rw-   0        0        0     4486 2021-12-07 13:33:27.000000 hdsr_wis_config_reader-1.8/hdsr_wis_config_reader/idmappings/collection.py
--rw-rw-rw-   0        0        0     4468 2021-11-16 15:31:25.000000 hdsr_wis_config_reader-1.8/hdsr_wis_config_reader/idmappings/columns.py
--rw-rw-rw-   0        0        0     2401 2021-11-22 11:26:09.000000 hdsr_wis_config_reader-1.8/hdsr_wis_config_reader/idmappings/custom_dataframe.py
--rw-rw-rw-   0        0        0      267 2021-11-16 15:31:25.000000 hdsr_wis_config_reader-1.8/hdsr_wis_config_reader/idmappings/files.py
--rw-rw-rw-   0        0        0     1657 2021-11-22 09:21:19.000000 hdsr_wis_config_reader-1.8/hdsr_wis_config_reader/idmappings/sections.py
-drwxrwxrwx   0        0        0        0 2021-12-20 12:47:14.000000 hdsr_wis_config_reader-1.8/hdsr_wis_config_reader/location_sets/
--rw-rw-rw-   0        0        0        0 2021-11-22 10:52:54.000000 hdsr_wis_config_reader-1.8/hdsr_wis_config_reader/location_sets/__init__.py
--rw-rw-rw-   0        0        0     5762 2021-11-22 10:46:42.000000 hdsr_wis_config_reader-1.8/hdsr_wis_config_reader/location_sets/base.py
--rw-rw-rw-   0        0        0     2590 2021-11-22 10:46:51.000000 hdsr_wis_config_reader-1.8/hdsr_wis_config_reader/location_sets/collection.py
--rw-rw-rw-   0        0        0     1060 2021-11-22 09:21:19.000000 hdsr_wis_config_reader-1.8/hdsr_wis_config_reader/location_sets/hoofd.py
--rw-rw-rw-   0        0        0      479 2021-11-22 09:21:19.000000 hdsr_wis_config_reader-1.8/hdsr_wis_config_reader/location_sets/msw.py
--rw-rw-rw-   0        0        0     1106 2021-11-22 09:21:19.000000 hdsr_wis_config_reader-1.8/hdsr_wis_config_reader/location_sets/ow.py
--rw-rw-rw-   0        0        0      495 2021-11-22 09:21:20.000000 hdsr_wis_config_reader-1.8/hdsr_wis_config_reader/location_sets/ps.py
--rw-rw-rw-   0        0        0     3541 2021-11-22 09:21:19.000000 hdsr_wis_config_reader-1.8/hdsr_wis_config_reader/location_sets/sub.py
-drwxrwxrwx   0        0        0        0 2021-12-20 12:47:14.000000 hdsr_wis_config_reader-1.8/hdsr_wis_config_reader/readers/
--rw-rw-rw-   0        0        0        0 2021-11-22 10:40:51.000000 hdsr_wis_config_reader-1.8/hdsr_wis_config_reader/readers/__init__.py
--rw-rw-rw-   0        0        0     9609 2021-11-22 17:25:06.000000 hdsr_wis_config_reader-1.8/hdsr_wis_config_reader/readers/config_reader.py
--rw-rw-rw-   0        0        0     3231 2021-11-22 10:44:28.000000 hdsr_wis_config_reader-1.8/hdsr_wis_config_reader/readers/xml_reader.py
-drwxrwxrwx   0        0        0        0 2021-12-20 12:47:14.000000 hdsr_wis_config_reader-1.8/hdsr_wis_config_reader/tests/
--rw-rw-rw-   0        0        0        0 2021-11-16 15:31:25.000000 hdsr_wis_config_reader-1.8/hdsr_wis_config_reader/tests/__init__.py
--rw-rw-rw-   0        0        0      923 2021-11-22 18:02:33.000000 hdsr_wis_config_reader-1.8/hdsr_wis_config_reader/tests/fixtures.py
--rw-rw-rw-   0        0        0     2313 2021-11-21 13:00:25.000000 hdsr_wis_config_reader-1.8/hdsr_wis_config_reader/tests/helpers.py
-drwxrwxrwx   0        0        0        0 2021-12-20 12:47:14.000000 hdsr_wis_config_reader-1.8/hdsr_wis_config_reader/tests/locationsets/
--rw-rw-rw-   0        0        0        0 2021-11-19 11:41:54.000000 hdsr_wis_config_reader-1.8/hdsr_wis_config_reader/tests/locationsets/__init__.py
--rw-rw-rw-   0        0        0     7381 2021-11-22 17:25:06.000000 hdsr_wis_config_reader-1.8/hdsr_wis_config_reader/tests/locationsets/test_hoofdlocationset.py
--rw-rw-rw-   0        0        0     1853 2021-11-22 10:43:11.000000 hdsr_wis_config_reader-1.8/hdsr_wis_config_reader/tests/locationsets/test_mswlocationset.py
--rw-rw-rw-   0        0        0     2834 2021-11-22 10:43:11.000000 hdsr_wis_config_reader-1.8/hdsr_wis_config_reader/tests/locationsets/test_pslocationset.py
--rw-rw-rw-   0        0        0    24285 2021-11-22 10:43:12.000000 hdsr_wis_config_reader-1.8/hdsr_wis_config_reader/tests/locationsets/test_sublocationset.py
--rw-rw-rw-   0        0        0    88814 2021-11-22 09:21:19.000000 hdsr_wis_config_reader-1.8/hdsr_wis_config_reader/tests/locationsets/test_uniqueness.py
--rw-rw-rw-   0        0        0    18073 2021-11-22 10:43:11.000000 hdsr_wis_config_reader-1.8/hdsr_wis_config_reader/tests/locationsets/test_waterstandlocationset.py
--rw-rw-rw-   0        0        0     2895 2021-11-22 18:03:07.000000 hdsr_wis_config_reader-1.8/hdsr_wis_config_reader/tests/test_config_reader.py
--rw-rw-rw-   0        0        0     3679 2021-12-07 13:33:27.000000 hdsr_wis_config_reader-1.8/hdsr_wis_config_reader/tests/test_id_mappings.py
--rw-rw-rw-   0        0        0     2134 2021-11-22 10:43:11.000000 hdsr_wis_config_reader-1.8/hdsr_wis_config_reader/tests/test_idmapping_choices.py
--rw-rw-rw-   0        0        0     1633 2021-11-22 09:27:01.000000 hdsr_wis_config_reader-1.8/hdsr_wis_config_reader/tests/test_validation_logic.py
-drwxrwxrwx   0        0        0        0 2021-12-20 12:47:14.000000 hdsr_wis_config_reader-1.8/hdsr_wis_config_reader/validation_rules/
--rw-rw-rw-   0        0        0      177 2021-11-22 09:27:01.000000 hdsr_wis_config_reader-1.8/hdsr_wis_config_reader/validation_rules/__init__.py
--rw-rw-rw-   0        0        0     3570 2021-12-20 12:46:38.000000 hdsr_wis_config_reader-1.8/hdsr_wis_config_reader/validation_rules/files.py
--rw-rw-rw-   0        0        0     2521 2021-11-16 15:31:25.000000 hdsr_wis_config_reader-1.8/hdsr_wis_config_reader/validation_rules/logic.py
-drwxrwxrwx   0        0        0        0 2021-12-20 12:47:14.000000 hdsr_wis_config_reader-1.8/hdsr_wis_config_reader.egg-info/
--rw-rw-rw-   0        0        0    11656 2021-12-20 12:47:14.000000 hdsr_wis_config_reader-1.8/hdsr_wis_config_reader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2063 2021-12-20 12:47:14.000000 hdsr_wis_config_reader-1.8/hdsr_wis_config_reader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-12-20 12:47:14.000000 hdsr_wis_config_reader-1.8/hdsr_wis_config_reader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2021-12-20 12:47:14.000000 hdsr_wis_config_reader-1.8/hdsr_wis_config_reader.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2021-12-20 12:47:14.000000 hdsr_wis_config_reader-1.8/hdsr_wis_config_reader.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1065 2021-11-21 13:00:25.000000 hdsr_wis_config_reader-1.8/pyproject.toml
--rw-rw-rw-   0        0        0      515 2021-12-20 12:47:16.000000 hdsr_wis_config_reader-1.8/setup.cfg
--rw-rw-rw-   0        0        0     1538 2021-12-20 12:46:38.000000 hdsr_wis_config_reader-1.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-01-07 16:29:33.000000 hdsr_wis_config_reader-1.9/
+-rw-rw-rw-   0        0        0     1086 2021-11-16 15:31:24.000000 hdsr_wis_config_reader-1.9/LICENSE
+-rw-rw-rw-   0        0        0    11615 2022-01-07 16:29:34.000000 hdsr_wis_config_reader-1.9/PKG-INFO
+-rw-rw-rw-   0        0        0    10801 2022-01-07 16:29:12.000000 hdsr_wis_config_reader-1.9/README.md
+drwxrwxrwx   0        0        0        0 2022-01-07 16:29:33.000000 hdsr_wis_config_reader-1.9/hdsr_wis_config_reader/
+-rw-rw-rw-   0        0        0      570 2021-11-22 10:52:30.000000 hdsr_wis_config_reader-1.9/hdsr_wis_config_reader/__init__.py
+-rw-rw-rw-   0        0        0      954 2022-01-07 16:29:12.000000 hdsr_wis_config_reader-1.9/hdsr_wis_config_reader/constants.py
+drwxrwxrwx   0        0        0        0 2022-01-07 16:29:33.000000 hdsr_wis_config_reader-1.9/hdsr_wis_config_reader/idmappings/
+-rw-rw-rw-   0        0        0        0 2021-11-22 09:27:01.000000 hdsr_wis_config_reader-1.9/hdsr_wis_config_reader/idmappings/__init__.py
+-rw-rw-rw-   0        0        0     4486 2021-12-07 13:33:27.000000 hdsr_wis_config_reader-1.9/hdsr_wis_config_reader/idmappings/collection.py
+-rw-rw-rw-   0        0        0     4468 2021-11-16 15:31:25.000000 hdsr_wis_config_reader-1.9/hdsr_wis_config_reader/idmappings/columns.py
+-rw-rw-rw-   0        0        0     2401 2021-11-22 11:26:09.000000 hdsr_wis_config_reader-1.9/hdsr_wis_config_reader/idmappings/custom_dataframe.py
+-rw-rw-rw-   0        0        0      267 2021-11-16 15:31:25.000000 hdsr_wis_config_reader-1.9/hdsr_wis_config_reader/idmappings/files.py
+-rw-rw-rw-   0        0        0     1657 2021-11-22 09:21:19.000000 hdsr_wis_config_reader-1.9/hdsr_wis_config_reader/idmappings/sections.py
+drwxrwxrwx   0        0        0        0 2022-01-07 16:29:33.000000 hdsr_wis_config_reader-1.9/hdsr_wis_config_reader/location_sets/
+-rw-rw-rw-   0        0        0        0 2021-11-22 10:52:54.000000 hdsr_wis_config_reader-1.9/hdsr_wis_config_reader/location_sets/__init__.py
+-rw-rw-rw-   0        0        0     5734 2022-01-07 16:29:12.000000 hdsr_wis_config_reader-1.9/hdsr_wis_config_reader/location_sets/base.py
+-rw-rw-rw-   0        0        0     2590 2021-11-22 10:46:51.000000 hdsr_wis_config_reader-1.9/hdsr_wis_config_reader/location_sets/collection.py
+-rw-rw-rw-   0        0        0     1060 2021-11-22 09:21:19.000000 hdsr_wis_config_reader-1.9/hdsr_wis_config_reader/location_sets/hoofd.py
+-rw-rw-rw-   0        0        0      479 2021-11-22 09:21:19.000000 hdsr_wis_config_reader-1.9/hdsr_wis_config_reader/location_sets/msw.py
+-rw-rw-rw-   0        0        0     1106 2021-11-22 09:21:19.000000 hdsr_wis_config_reader-1.9/hdsr_wis_config_reader/location_sets/ow.py
+-rw-rw-rw-   0        0        0      495 2021-11-22 09:21:20.000000 hdsr_wis_config_reader-1.9/hdsr_wis_config_reader/location_sets/ps.py
+-rw-rw-rw-   0        0        0     3541 2021-11-22 09:21:19.000000 hdsr_wis_config_reader-1.9/hdsr_wis_config_reader/location_sets/sub.py
+drwxrwxrwx   0        0        0        0 2022-01-07 16:29:33.000000 hdsr_wis_config_reader-1.9/hdsr_wis_config_reader/readers/
+-rw-rw-rw-   0        0        0        0 2021-11-22 10:40:51.000000 hdsr_wis_config_reader-1.9/hdsr_wis_config_reader/readers/__init__.py
+-rw-rw-rw-   0        0        0    12016 2022-01-07 16:29:12.000000 hdsr_wis_config_reader-1.9/hdsr_wis_config_reader/readers/config_reader.py
+-rw-rw-rw-   0        0        0     3231 2021-11-22 10:44:28.000000 hdsr_wis_config_reader-1.9/hdsr_wis_config_reader/readers/xml_reader.py
+drwxrwxrwx   0        0        0        0 2022-01-07 16:29:33.000000 hdsr_wis_config_reader-1.9/hdsr_wis_config_reader/tests/
+-rw-rw-rw-   0        0        0        0 2021-11-16 15:31:25.000000 hdsr_wis_config_reader-1.9/hdsr_wis_config_reader/tests/__init__.py
+-rw-rw-rw-   0        0        0     1903 2022-01-07 16:29:12.000000 hdsr_wis_config_reader-1.9/hdsr_wis_config_reader/tests/fixtures.py
+-rw-rw-rw-   0        0        0     2313 2021-11-21 13:00:25.000000 hdsr_wis_config_reader-1.9/hdsr_wis_config_reader/tests/helpers.py
+drwxrwxrwx   0        0        0        0 2022-01-07 16:29:33.000000 hdsr_wis_config_reader-1.9/hdsr_wis_config_reader/tests/locationsets/
+-rw-rw-rw-   0        0        0        0 2021-11-19 11:41:54.000000 hdsr_wis_config_reader-1.9/hdsr_wis_config_reader/tests/locationsets/__init__.py
+-rw-rw-rw-   0        0        0     7381 2021-11-22 17:25:06.000000 hdsr_wis_config_reader-1.9/hdsr_wis_config_reader/tests/locationsets/test_hoofdlocationset.py
+-rw-rw-rw-   0        0        0     1853 2021-11-22 10:43:11.000000 hdsr_wis_config_reader-1.9/hdsr_wis_config_reader/tests/locationsets/test_mswlocationset.py
+-rw-rw-rw-   0        0        0     2834 2021-11-22 10:43:11.000000 hdsr_wis_config_reader-1.9/hdsr_wis_config_reader/tests/locationsets/test_pslocationset.py
+-rw-rw-rw-   0        0        0    24285 2021-11-22 10:43:12.000000 hdsr_wis_config_reader-1.9/hdsr_wis_config_reader/tests/locationsets/test_sublocationset.py
+-rw-rw-rw-   0        0        0    88814 2021-11-22 09:21:19.000000 hdsr_wis_config_reader-1.9/hdsr_wis_config_reader/tests/locationsets/test_uniqueness.py
+-rw-rw-rw-   0        0        0    18073 2021-11-22 10:43:11.000000 hdsr_wis_config_reader-1.9/hdsr_wis_config_reader/tests/locationsets/test_waterstandlocationset.py
+-rw-rw-rw-   0        0        0     3553 2022-01-07 16:29:12.000000 hdsr_wis_config_reader-1.9/hdsr_wis_config_reader/tests/test_config_reader.py
+-rw-rw-rw-   0        0        0     3733 2022-01-07 16:29:12.000000 hdsr_wis_config_reader-1.9/hdsr_wis_config_reader/tests/test_id_mappings.py
+-rw-rw-rw-   0        0        0     2134 2021-11-22 10:43:11.000000 hdsr_wis_config_reader-1.9/hdsr_wis_config_reader/tests/test_idmapping_choices.py
+-rw-rw-rw-   0        0        0     1633 2021-11-22 09:27:01.000000 hdsr_wis_config_reader-1.9/hdsr_wis_config_reader/tests/test_validation_logic.py
+drwxrwxrwx   0        0        0        0 2022-01-07 16:29:33.000000 hdsr_wis_config_reader-1.9/hdsr_wis_config_reader/validation_rules/
+-rw-rw-rw-   0        0        0      177 2021-11-22 09:27:01.000000 hdsr_wis_config_reader-1.9/hdsr_wis_config_reader/validation_rules/__init__.py
+-rw-rw-rw-   0        0        0     3570 2021-12-20 12:46:38.000000 hdsr_wis_config_reader-1.9/hdsr_wis_config_reader/validation_rules/files.py
+-rw-rw-rw-   0        0        0     2521 2021-11-16 15:31:25.000000 hdsr_wis_config_reader-1.9/hdsr_wis_config_reader/validation_rules/logic.py
+drwxrwxrwx   0        0        0        0 2022-01-07 16:29:33.000000 hdsr_wis_config_reader-1.9/hdsr_wis_config_reader.egg-info/
+-rw-rw-rw-   0        0        0    11615 2022-01-07 16:29:33.000000 hdsr_wis_config_reader-1.9/hdsr_wis_config_reader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2063 2022-01-07 16:29:33.000000 hdsr_wis_config_reader-1.9/hdsr_wis_config_reader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-01-07 16:29:33.000000 hdsr_wis_config_reader-1.9/hdsr_wis_config_reader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2022-01-07 16:29:33.000000 hdsr_wis_config_reader-1.9/hdsr_wis_config_reader.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2022-01-07 16:29:33.000000 hdsr_wis_config_reader-1.9/hdsr_wis_config_reader.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1065 2021-11-21 13:00:25.000000 hdsr_wis_config_reader-1.9/pyproject.toml
+-rw-rw-rw-   0        0        0      515 2022-01-07 16:29:34.000000 hdsr_wis_config_reader-1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1538 2022-01-07 16:29:12.000000 hdsr_wis_config_reader-1.9/setup.py
```

### Comparing `hdsr_wis_config_reader-1.8/LICENSE` & `hdsr_wis_config_reader-1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hdsr_wis_config_reader-1.8/PKG-INFO` & `hdsr_wis_config_reader-1.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdsr_wis_config_reader
-Version: 1.8
+Version: 1.9
 Summary: Read HDSR FEWS WIS config into python objects
 Home-page: https://github.com/hdsr-mid/hdsr_wis_config_reader
 Author: Renier Kramer
 Author-email: renier.kramer@hdsr.nl
 License: MIT
 Keywords: HDSR,FEWS,WIS,config,hdsr_wis_config_reader
 Platform: UNKNOWN
@@ -50,32 +50,20 @@
 >>> location_sets.hoofdloc.name
 # 'hoofdlocaties'
 >>> location_sets.hoofdloc.csv_filename
 'oppvlwater_hoofdloc'
 >>> location_sets.hoofdloc.fews_name
 'OPVLWATER_HOOFDLOC'
 --------------------------------------------------------------------------------
-# 3. Extract a dictionary of parameter(groups)
->>> fews_config.get_parameters(dict_keys="groups")["Neerslag"]
-# {
-#   "parameterType": "accumulative",
-#   "unit": "mm", 
-#   "valueResolution": "0.001",
-#   "parameter": [{"shortName: ...
-#   etc..
-# }
->>> fews_config.get_parameters(dict_keys="parameters")["RHdef.d"]
-# {
-#    "shortName": "Neerslagtekort [mm] - dag",
-#    "name": "Neerslagtekort [mm] - dag",
-#    "parameterType": "accumulative",
-#    "unit": "mm",
-#    "valueResolution": "0.001",
-#    "groupId": "Neerslag",
-# }
+# 3. Get a dataframe of parameters
+>>> fews_config.get_parameters()
+# GROUP     DESCRIPTION PARAMETERTYPE   UNIT    VALUERESOLUTION USESDATUM   ID  NAME                                SHORTNAME
+# Biomassa              instantaneous   kg/ha   0.1                         B.d Biomassa productie [kg/ha] - dag    Biomassa productie [kg/ha] - dag
+# Biomassa              instantaneous   kg/ha   0.1                         B.m Biomassa productie [kg/ha] - maand  Biomassa productie [kg/ha] - maand
+# etc...
 --------------------------------------------------------------------------------       
 # 4. Get a geodataframe with hoofd locations (note that geomeometry height (z) gets -9999 when if Z is nan)
 >>> location_sets.hoofdloc.geo_df
 # LOC_ID      LOC_NAME                            X       Y       Z       ALLE_TYPES          START       ...     geometry
 # KW100110    WIJKERSLOOT_1001-K_WIJKERSLOOT      150501  442988  2.87    krooshek/pompvijzel 19970101    ...     POINT Z (150501 442988 2.87)
 # KW100120    WIJKERSLOOT_1001-K_WIJKERSLOOT STUW 150439  442885  nan     stuw                20120321    ...     POINT Z (150439 442885 -9999)
 # etc...
@@ -136,34 +124,34 @@
 
 ### Test Coverage
 ```
 ---------- coverage: platform win32, python 3.7.11-final-0 -----------
 Name                                                    Stmts   Miss  Cover
 ---------------------------------------------------------------------------
 hdsr_wis_config_reader\__init__.py                         10      0   100%
-hdsr_wis_config_reader\constants.py                         5      1    80%
+hdsr_wis_config_reader\constants.py                        13      1    92%
 hdsr_wis_config_reader\idmappings\collection.py            79      4    95%
 hdsr_wis_config_reader\idmappings\columns.py               80     16    80%
 hdsr_wis_config_reader\idmappings\custom_dataframe.py      28      1    96%
 hdsr_wis_config_reader\idmappings\files.py                  7      0   100%
 hdsr_wis_config_reader\idmappings\sections.py               8      0   100%
 hdsr_wis_config_reader\location_sets\base.py               98     10    90%
 hdsr_wis_config_reader\location_sets\collection.py         54      4    93%
 hdsr_wis_config_reader\location_sets\hoofd.py              18      1    94%
 hdsr_wis_config_reader\location_sets\msw.py                12      1    92%
 hdsr_wis_config_reader\location_sets\ow.py                 13      1    92%
 hdsr_wis_config_reader\location_sets\ps.py                 12      1    92%
 hdsr_wis_config_reader\location_sets\sub.py                27      2    93%
-hdsr_wis_config_reader\readers\config_reader.py           134     14    90%
+hdsr_wis_config_reader\readers\config_reader.py           154     11    93%
 hdsr_wis_config_reader\readers\xml_reader.py               48     10    79%
 hdsr_wis_config_reader\validation_rules\__init__.py         4      0   100%
 hdsr_wis_config_reader\validation_rules\files.py           35     10    71%
 hdsr_wis_config_reader\validation_rules\logic.py           28      0   100%
 ---------------------------------------------------------------------------
-TOTAL                                                     700     76    89%
+TOTAL                                                     728     73    90%
 ```
 
 ### Conda general tips
 #### Build conda environment (on Windows) from any directory using environment.yml:
 ```
 > conda env create --name <conda_env_name> --file <path_to_project>/environment.yml python=<python_version>
 > conda info --envs  # verify that <conda_env_name> is in this list
```

### Comparing `hdsr_wis_config_reader-1.8/README.md` & `hdsr_wis_config_reader-1.9/hdsr_wis_config_reader.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: hdsr-wis-config-reader
+Version: 1.9
+Summary: Read HDSR FEWS WIS config into python objects
+Home-page: https://github.com/hdsr-mid/hdsr_wis_config_reader
+Author: Renier Kramer
+Author-email: renier.kramer@hdsr.nl
+License: MIT
+Keywords: HDSR,FEWS,WIS,config,hdsr_wis_config_reader
+Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >3.6
+Description-Content-Type: text/markdown
+Provides-Extra: test
+License-File: LICENSE
+
 ### Context
 * Created: November 2021
 * Author: Renier Kramer, renier.kramer@hdsr.nl
 * Python version: >3.5
 
 ### Description
 A python project that you can use to read the HDSR FEWS-WIS configuration. 
@@ -28,32 +50,20 @@
 >>> location_sets.hoofdloc.name
 # 'hoofdlocaties'
 >>> location_sets.hoofdloc.csv_filename
 'oppvlwater_hoofdloc'
 >>> location_sets.hoofdloc.fews_name
 'OPVLWATER_HOOFDLOC'
 --------------------------------------------------------------------------------
-# 3. Extract a dictionary of parameter(groups)
->>> fews_config.get_parameters(dict_keys="groups")["Neerslag"]
-# {
-#   "parameterType": "accumulative",
-#   "unit": "mm", 
-#   "valueResolution": "0.001",
-#   "parameter": [{"shortName: ...
-#   etc..
-# }
->>> fews_config.get_parameters(dict_keys="parameters")["RHdef.d"]
-# {
-#    "shortName": "Neerslagtekort [mm] - dag",
-#    "name": "Neerslagtekort [mm] - dag",
-#    "parameterType": "accumulative",
-#    "unit": "mm",
-#    "valueResolution": "0.001",
-#    "groupId": "Neerslag",
-# }
+# 3. Get a dataframe of parameters
+>>> fews_config.get_parameters()
+# GROUP     DESCRIPTION PARAMETERTYPE   UNIT    VALUERESOLUTION USESDATUM   ID  NAME                                SHORTNAME
+# Biomassa              instantaneous   kg/ha   0.1                         B.d Biomassa productie [kg/ha] - dag    Biomassa productie [kg/ha] - dag
+# Biomassa              instantaneous   kg/ha   0.1                         B.m Biomassa productie [kg/ha] - maand  Biomassa productie [kg/ha] - maand
+# etc...
 --------------------------------------------------------------------------------       
 # 4. Get a geodataframe with hoofd locations (note that geomeometry height (z) gets -9999 when if Z is nan)
 >>> location_sets.hoofdloc.geo_df
 # LOC_ID      LOC_NAME                            X       Y       Z       ALLE_TYPES          START       ...     geometry
 # KW100110    WIJKERSLOOT_1001-K_WIJKERSLOOT      150501  442988  2.87    krooshek/pompvijzel 19970101    ...     POINT Z (150501 442988 2.87)
 # KW100120    WIJKERSLOOT_1001-K_WIJKERSLOOT STUW 150439  442885  nan     stuw                20120321    ...     POINT Z (150439 442885 -9999)
 # etc...
@@ -114,34 +124,34 @@
 
 ### Test Coverage
 ```
 ---------- coverage: platform win32, python 3.7.11-final-0 -----------
 Name                                                    Stmts   Miss  Cover
 ---------------------------------------------------------------------------
 hdsr_wis_config_reader\__init__.py                         10      0   100%
-hdsr_wis_config_reader\constants.py                         5      1    80%
+hdsr_wis_config_reader\constants.py                        13      1    92%
 hdsr_wis_config_reader\idmappings\collection.py            79      4    95%
 hdsr_wis_config_reader\idmappings\columns.py               80     16    80%
 hdsr_wis_config_reader\idmappings\custom_dataframe.py      28      1    96%
 hdsr_wis_config_reader\idmappings\files.py                  7      0   100%
 hdsr_wis_config_reader\idmappings\sections.py               8      0   100%
 hdsr_wis_config_reader\location_sets\base.py               98     10    90%
 hdsr_wis_config_reader\location_sets\collection.py         54      4    93%
 hdsr_wis_config_reader\location_sets\hoofd.py              18      1    94%
 hdsr_wis_config_reader\location_sets\msw.py                12      1    92%
 hdsr_wis_config_reader\location_sets\ow.py                 13      1    92%
 hdsr_wis_config_reader\location_sets\ps.py                 12      1    92%
 hdsr_wis_config_reader\location_sets\sub.py                27      2    93%
-hdsr_wis_config_reader\readers\config_reader.py           134     14    90%
+hdsr_wis_config_reader\readers\config_reader.py           154     11    93%
 hdsr_wis_config_reader\readers\xml_reader.py               48     10    79%
 hdsr_wis_config_reader\validation_rules\__init__.py         4      0   100%
 hdsr_wis_config_reader\validation_rules\files.py           35     10    71%
 hdsr_wis_config_reader\validation_rules\logic.py           28      0   100%
 ---------------------------------------------------------------------------
-TOTAL                                                     700     76    89%
+TOTAL                                                     728     73    90%
 ```
 
 ### Conda general tips
 #### Build conda environment (on Windows) from any directory using environment.yml:
 ```
 > conda env create --name <conda_env_name> --file <path_to_project>/environment.yml python=<python_version>
 > conda info --envs  # verify that <conda_env_name> is in this list 
@@ -212,7 +222,9 @@
   - pip:
     - <a pip package>==<version>
 ```
 You can also write a requirements.txt file:
 ```
 > pip list --format=freeze > <path_to_project>/requirements.txt
 ```
+
+
```

### Comparing `hdsr_wis_config_reader-1.8/hdsr_wis_config_reader/__init__.py` & `hdsr_wis_config_reader-1.9/hdsr_wis_config_reader/__init__.py`

 * *Files identical despite different names*

### Comparing `hdsr_wis_config_reader-1.8/hdsr_wis_config_reader/idmappings/collection.py` & `hdsr_wis_config_reader-1.9/hdsr_wis_config_reader/idmappings/collection.py`

 * *Files identical despite different names*

### Comparing `hdsr_wis_config_reader-1.8/hdsr_wis_config_reader/idmappings/columns.py` & `hdsr_wis_config_reader-1.9/hdsr_wis_config_reader/idmappings/columns.py`

 * *Files identical despite different names*

### Comparing `hdsr_wis_config_reader-1.8/hdsr_wis_config_reader/idmappings/custom_dataframe.py` & `hdsr_wis_config_reader-1.9/hdsr_wis_config_reader/idmappings/custom_dataframe.py`

 * *Files identical despite different names*

### Comparing `hdsr_wis_config_reader-1.8/hdsr_wis_config_reader/idmappings/sections.py` & `hdsr_wis_config_reader-1.9/hdsr_wis_config_reader/idmappings/sections.py`

 * *Files identical despite different names*

### Comparing `hdsr_wis_config_reader-1.8/hdsr_wis_config_reader/location_sets/base.py` & `hdsr_wis_config_reader-1.9/hdsr_wis_config_reader/location_sets/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         assert len(set(ids)) == len(ids), "we expected unique id's in RegionConfigFiles LocationSets"
         return self._general_location_sets_dict
 
     @property
     def csv_file_meta(self) -> Dict:
         """
         e.g. {
-                'file': 'oppvlwater_hoofdloc',
+                'file': 'ow_hl',
                 'geoDatum': 'Rijks Driehoekstelsel',
                 'id': '%LOC_ID%',
                 'name': '%LOC_NAME%',
                 'description': 'Hoofdlocaties oppervlaktewater',
                 etc..
             }
         """
@@ -97,15 +97,15 @@
         csvfile_meta = [loc_set for loc_set in self.general_location_sets_dict if loc_set["id"] == self.fews_name]
         assert len(csvfile_meta) == 1
         self._csvfile_meta = csvfile_meta[0]["csvFile"]
         return self._csvfile_meta
 
     @property
     def csv_filename(self) -> str:
-        """e.g. 'oppvlwater_hoofdloc'"""
+        """e.g. 'ow_hl'"""
         return self.csv_file_meta["file"]
 
     @property
     def attrib_files(self) -> List:
         if self._attrib_files is not None:
             return self._attrib_files
         attribute_files = self.csv_file_meta.get("attributeFile", None)
```

### Comparing `hdsr_wis_config_reader-1.8/hdsr_wis_config_reader/location_sets/collection.py` & `hdsr_wis_config_reader-1.9/hdsr_wis_config_reader/location_sets/collection.py`

 * *Files identical despite different names*

### Comparing `hdsr_wis_config_reader-1.8/hdsr_wis_config_reader/location_sets/hoofd.py` & `hdsr_wis_config_reader-1.9/hdsr_wis_config_reader/location_sets/hoofd.py`

 * *Files identical despite different names*

### Comparing `hdsr_wis_config_reader-1.8/hdsr_wis_config_reader/location_sets/ow.py` & `hdsr_wis_config_reader-1.9/hdsr_wis_config_reader/location_sets/ow.py`

 * *Files identical despite different names*

### Comparing `hdsr_wis_config_reader-1.8/hdsr_wis_config_reader/location_sets/sub.py` & `hdsr_wis_config_reader-1.9/hdsr_wis_config_reader/location_sets/sub.py`

 * *Files identical despite different names*

### Comparing `hdsr_wis_config_reader-1.8/hdsr_wis_config_reader/readers/xml_reader.py` & `hdsr_wis_config_reader-1.9/hdsr_wis_config_reader/readers/xml_reader.py`

 * *Files identical despite different names*

### Comparing `hdsr_wis_config_reader-1.8/hdsr_wis_config_reader/tests/helpers.py` & `hdsr_wis_config_reader-1.9/hdsr_wis_config_reader/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `hdsr_wis_config_reader-1.8/hdsr_wis_config_reader/tests/locationsets/test_hoofdlocationset.py` & `hdsr_wis_config_reader-1.9/hdsr_wis_config_reader/tests/locationsets/test_hoofdlocationset.py`

 * *Files identical despite different names*

### Comparing `hdsr_wis_config_reader-1.8/hdsr_wis_config_reader/tests/locationsets/test_mswlocationset.py` & `hdsr_wis_config_reader-1.9/hdsr_wis_config_reader/tests/locationsets/test_mswlocationset.py`

 * *Files identical despite different names*

### Comparing `hdsr_wis_config_reader-1.8/hdsr_wis_config_reader/tests/locationsets/test_pslocationset.py` & `hdsr_wis_config_reader-1.9/hdsr_wis_config_reader/tests/locationsets/test_pslocationset.py`

 * *Files identical despite different names*

### Comparing `hdsr_wis_config_reader-1.8/hdsr_wis_config_reader/tests/locationsets/test_sublocationset.py` & `hdsr_wis_config_reader-1.9/hdsr_wis_config_reader/tests/locationsets/test_sublocationset.py`

 * *Files identical despite different names*

### Comparing `hdsr_wis_config_reader-1.8/hdsr_wis_config_reader/tests/locationsets/test_uniqueness.py` & `hdsr_wis_config_reader-1.9/hdsr_wis_config_reader/tests/locationsets/test_uniqueness.py`

 * *Files identical despite different names*

### Comparing `hdsr_wis_config_reader-1.8/hdsr_wis_config_reader/tests/locationsets/test_waterstandlocationset.py` & `hdsr_wis_config_reader-1.9/hdsr_wis_config_reader/tests/locationsets/test_waterstandlocationset.py`

 * *Files identical despite different names*

### Comparing `hdsr_wis_config_reader-1.8/hdsr_wis_config_reader/tests/test_id_mappings.py` & `hdsr_wis_config_reader-1.9/hdsr_wis_config_reader/tests/test_id_mappings.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from hdsr_wis_config_reader import IdMappingCollection
 from hdsr_wis_config_reader.constants import WIS_CONFIG_TEST_DIR
 from hdsr_wis_config_reader.idmappings.columns import IdMapColumnChoices
 from hdsr_wis_config_reader.idmappings.files import IdMapChoices
-from hdsr_wis_config_reader.tests.fixtures import fews_config
+from hdsr_wis_config_reader.tests.fixtures import fews_config_local
 from hdsr_wis_config_reader.tests.helpers import is_equal_dataframes
 
 import pandas as pd  # noqa pandas comes with geopandas
 
 
 # silence flake8
-fews_config = fews_config
+fews_config_local = fews_config_local
 
 
 expected_df_a = pd.DataFrame(
     data={
         "externalLocation": {2880: "610", 5929: "7610"},
         "externalParameter": {2880: "Q1", 5929: "Q1"},
         "internalLocation": {2880: "KW761001", 5929: "KW761001"},
@@ -33,16 +33,16 @@
         "histtag": {2880: "610_Q1", 5929: "7610_Q1", 2252: "610_Q1"},
     }
 )
 
 expected_ex_par_values = ["1GW", "GW1", "GW2", "GW3", "HB1", "HB2", "HB3", "HB4", "HB5", "HB6", "HB7", "HB8"]
 
 
-def test_idmapping_opvl_water(fews_config):
-    id_mappings = IdMappingCollection(fews_config=fews_config)
+def test_idmapping_opvl_water(fews_config_local):
+    id_mappings = IdMappingCollection(fews_config=fews_config_local)
     assert id_mappings.idmap_opvl_water.shape == (6050, 6)
 
     df_idmap_opvl_water = id_mappings.idmap_opvl_water.get_filtered_df(int_loc="KW761001")
     assert isinstance(df_idmap_opvl_water, pd.DataFrame)
     assert len(df_idmap_opvl_water) == 2
     assert is_equal_dataframes(expected_df=expected_df_a, test_df=df_idmap_opvl_water)
 
@@ -53,30 +53,30 @@
 
     df_all = id_mappings.idmap_all.get_filtered_df(int_loc="KW761001")
     assert isinstance(df_all, pd.DataFrame)
     assert len(df_all) == 3
     assert is_equal_dataframes(expected_df=expected_df_b, test_df=df_all)
 
 
-def test_read_idmap_oppvl(fews_config):
+def test_read_idmap_oppvl(fews_config_local):
 
     # read without fews config
     oppvl_path1 = WIS_CONFIG_TEST_DIR / "IdMapFiles" / "IdOPVLWATER.xml"
     df_oppvl_without_fews = IdMappingCollection.get_idmap_df_via_path(file_path=oppvl_path1)
     assert len(df_oppvl_without_fews) == 6050
 
     # read same idmap but now via fews config
-    collection = IdMappingCollection(fews_config=fews_config)
+    collection = IdMappingCollection(fews_config=fews_config_local)
     df_oppvl_with_fews = collection.get_idmap_df_via_choice(IdMapChoices.idmap_opvl_water)
     assert is_equal_dataframes(expected_df=df_oppvl_without_fews, test_df=df_oppvl_with_fews)
 
 
-def test_read_idmap_oppvl_hymos(fews_config):
+def test_read_idmap_oppvl_hymos(fews_config_local):
     # read without fews config
     oppvl_path1 = WIS_CONFIG_TEST_DIR / "IdMapFiles" / "IdOPVLWATER_HYMOS.xml"
     df_oppvl_hymos_without_fews = IdMappingCollection.get_idmap_df_via_path(file_path=oppvl_path1)
     assert len(df_oppvl_hymos_without_fews) == 2360
 
     # read same idmap but now via fews config
-    collection = IdMappingCollection(fews_config=fews_config)
+    collection = IdMappingCollection(fews_config=fews_config_local)
     df_oppvl_hymos_with_fews = collection.get_idmap_df_via_choice(IdMapChoices.idmap_opvl_water_hymos)
     assert is_equal_dataframes(expected_df=df_oppvl_hymos_without_fews, test_df=df_oppvl_hymos_with_fews)
```

### Comparing `hdsr_wis_config_reader-1.8/hdsr_wis_config_reader/tests/test_idmapping_choices.py` & `hdsr_wis_config_reader-1.9/hdsr_wis_config_reader/tests/test_idmapping_choices.py`

 * *Files identical despite different names*

### Comparing `hdsr_wis_config_reader-1.8/hdsr_wis_config_reader/tests/test_validation_logic.py` & `hdsr_wis_config_reader-1.9/hdsr_wis_config_reader/tests/test_validation_logic.py`

 * *Files identical despite different names*

### Comparing `hdsr_wis_config_reader-1.8/hdsr_wis_config_reader/validation_rules/files.py` & `hdsr_wis_config_reader-1.9/hdsr_wis_config_reader/validation_rules/files.py`

 * *Files identical despite different names*

### Comparing `hdsr_wis_config_reader-1.8/hdsr_wis_config_reader/validation_rules/logic.py` & `hdsr_wis_config_reader-1.9/hdsr_wis_config_reader/validation_rules/logic.py`

 * *Files identical despite different names*

### Comparing `hdsr_wis_config_reader-1.8/hdsr_wis_config_reader.egg-info/PKG-INFO` & `hdsr_wis_config_reader-1.9/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: hdsr-wis-config-reader
-Version: 1.8
-Summary: Read HDSR FEWS WIS config into python objects
-Home-page: https://github.com/hdsr-mid/hdsr_wis_config_reader
-Author: Renier Kramer
-Author-email: renier.kramer@hdsr.nl
-License: MIT
-Keywords: HDSR,FEWS,WIS,config,hdsr_wis_config_reader
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >3.6
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE
-
 ### Context
 * Created: November 2021
 * Author: Renier Kramer, renier.kramer@hdsr.nl
 * Python version: >3.5
 
 ### Description
 A python project that you can use to read the HDSR FEWS-WIS configuration. 
@@ -50,32 +28,20 @@
 >>> location_sets.hoofdloc.name
 # 'hoofdlocaties'
 >>> location_sets.hoofdloc.csv_filename
 'oppvlwater_hoofdloc'
 >>> location_sets.hoofdloc.fews_name
 'OPVLWATER_HOOFDLOC'
 --------------------------------------------------------------------------------
-# 3. Extract a dictionary of parameter(groups)
->>> fews_config.get_parameters(dict_keys="groups")["Neerslag"]
-# {
-#   "parameterType": "accumulative",
-#   "unit": "mm", 
-#   "valueResolution": "0.001",
-#   "parameter": [{"shortName: ...
-#   etc..
-# }
->>> fews_config.get_parameters(dict_keys="parameters")["RHdef.d"]
-# {
-#    "shortName": "Neerslagtekort [mm] - dag",
-#    "name": "Neerslagtekort [mm] - dag",
-#    "parameterType": "accumulative",
-#    "unit": "mm",
-#    "valueResolution": "0.001",
-#    "groupId": "Neerslag",
-# }
+# 3. Get a dataframe of parameters
+>>> fews_config.get_parameters()
+# GROUP     DESCRIPTION PARAMETERTYPE   UNIT    VALUERESOLUTION USESDATUM   ID  NAME                                SHORTNAME
+# Biomassa              instantaneous   kg/ha   0.1                         B.d Biomassa productie [kg/ha] - dag    Biomassa productie [kg/ha] - dag
+# Biomassa              instantaneous   kg/ha   0.1                         B.m Biomassa productie [kg/ha] - maand  Biomassa productie [kg/ha] - maand
+# etc...
 --------------------------------------------------------------------------------       
 # 4. Get a geodataframe with hoofd locations (note that geomeometry height (z) gets -9999 when if Z is nan)
 >>> location_sets.hoofdloc.geo_df
 # LOC_ID      LOC_NAME                            X       Y       Z       ALLE_TYPES          START       ...     geometry
 # KW100110    WIJKERSLOOT_1001-K_WIJKERSLOOT      150501  442988  2.87    krooshek/pompvijzel 19970101    ...     POINT Z (150501 442988 2.87)
 # KW100120    WIJKERSLOOT_1001-K_WIJKERSLOOT STUW 150439  442885  nan     stuw                20120321    ...     POINT Z (150439 442885 -9999)
 # etc...
@@ -136,34 +102,34 @@
 
 ### Test Coverage
 ```
 ---------- coverage: platform win32, python 3.7.11-final-0 -----------
 Name                                                    Stmts   Miss  Cover
 ---------------------------------------------------------------------------
 hdsr_wis_config_reader\__init__.py                         10      0   100%
-hdsr_wis_config_reader\constants.py                         5      1    80%
+hdsr_wis_config_reader\constants.py                        13      1    92%
 hdsr_wis_config_reader\idmappings\collection.py            79      4    95%
 hdsr_wis_config_reader\idmappings\columns.py               80     16    80%
 hdsr_wis_config_reader\idmappings\custom_dataframe.py      28      1    96%
 hdsr_wis_config_reader\idmappings\files.py                  7      0   100%
 hdsr_wis_config_reader\idmappings\sections.py               8      0   100%
 hdsr_wis_config_reader\location_sets\base.py               98     10    90%
 hdsr_wis_config_reader\location_sets\collection.py         54      4    93%
 hdsr_wis_config_reader\location_sets\hoofd.py              18      1    94%
 hdsr_wis_config_reader\location_sets\msw.py                12      1    92%
 hdsr_wis_config_reader\location_sets\ow.py                 13      1    92%
 hdsr_wis_config_reader\location_sets\ps.py                 12      1    92%
 hdsr_wis_config_reader\location_sets\sub.py                27      2    93%
-hdsr_wis_config_reader\readers\config_reader.py           134     14    90%
+hdsr_wis_config_reader\readers\config_reader.py           154     11    93%
 hdsr_wis_config_reader\readers\xml_reader.py               48     10    79%
 hdsr_wis_config_reader\validation_rules\__init__.py         4      0   100%
 hdsr_wis_config_reader\validation_rules\files.py           35     10    71%
 hdsr_wis_config_reader\validation_rules\logic.py           28      0   100%
 ---------------------------------------------------------------------------
-TOTAL                                                     700     76    89%
+TOTAL                                                     728     73    90%
 ```
 
 ### Conda general tips
 #### Build conda environment (on Windows) from any directory using environment.yml:
 ```
 > conda env create --name <conda_env_name> --file <path_to_project>/environment.yml python=<python_version>
 > conda info --envs  # verify that <conda_env_name> is in this list 
@@ -234,9 +200,7 @@
   - pip:
     - <a pip package>==<version>
 ```
 You can also write a requirements.txt file:
 ```
 > pip list --format=freeze > <path_to_project>/requirements.txt
 ```
-
-
```

### Comparing `hdsr_wis_config_reader-1.8/hdsr_wis_config_reader.egg-info/SOURCES.txt` & `hdsr_wis_config_reader-1.9/hdsr_wis_config_reader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hdsr_wis_config_reader-1.8/pyproject.toml` & `hdsr_wis_config_reader-1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hdsr_wis_config_reader-1.8/setup.cfg` & `hdsr_wis_config_reader-1.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `hdsr_wis_config_reader-1.8/setup.py` & `hdsr_wis_config_reader-1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 # read the contents of your README file
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
-version = "1.8"
+version = "1.9"
 
 install_requires = [
     "geopandas",
     "lxml",
     "pathlib",
     "typing",
 ]
```

