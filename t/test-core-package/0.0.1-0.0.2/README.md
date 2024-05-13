# Comparing `tmp/test_core_package-0.0.1.tar.gz` & `tmp/test_core_package-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_core_package-0.0.1.tar", last modified: Mon May 13 06:56:39 2024, max compression
+gzip compressed data, was "test_core_package-0.0.2.tar", last modified: Mon May 13 07:09:10 2024, max compression
```

## Comparing `test_core_package-0.0.1.tar` & `test_core_package-0.0.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 06:56:39.694380 test_core_package-0.0.1/
--rw-rw-rw-   0        0        0        0 2024-04-29 09:27:23.000000 test_core_package-0.0.1/LICENCE.txt
--rw-rw-rw-   0        0        0      241 2024-05-13 06:56:39.693345 test_core_package-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-29 09:27:23.000000 test_core_package-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-13 06:56:39.549832 test_core_package-0.0.1/qa_qc_check/
--rw-rw-rw-   0        0        0        0 2024-05-07 12:52:35.000000 test_core_package-0.0.1/qa_qc_check/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 06:56:39.569711 test_core_package-0.0.1/qa_qc_check/controller/
--rw-rw-rw-   0        0        0        0 2024-05-02 09:51:13.000000 test_core_package-0.0.1/qa_qc_check/controller/__init__.py
--rw-rw-rw-   0        0        0     4161 2024-05-06 12:22:37.000000 test_core_package-0.0.1/qa_qc_check/controller/checks.json
--rw-rw-rw-   0        0        0     4310 2024-05-13 06:11:44.000000 test_core_package-0.0.1/qa_qc_check/controller/meta_data.py
--rw-rw-rw-   0        0        0     3756 2024-05-13 06:11:23.000000 test_core_package-0.0.1/qa_qc_check/controller/meta_data_extractor.py
--rw-rw-rw-   0        0        0     1951 2024-05-07 07:45:01.000000 test_core_package-0.0.1/qa_qc_check/controller/meta_data_validator.py
--rw-rw-rw-   0        0        0      932 2024-05-07 07:38:44.000000 test_core_package-0.0.1/qa_qc_check/controller/metadata_model.py
--rw-rw-rw-   0        0        0     1541 2024-05-07 07:46:19.000000 test_core_package-0.0.1/qa_qc_check/controller/qa_qc.py
-drwxrwxrwx   0        0        0        0 2024-05-13 06:56:39.573266 test_core_package-0.0.1/qa_qc_check/tests/
--rw-rw-rw-   0        0        0        0 2024-05-07 11:46:23.000000 test_core_package-0.0.1/qa_qc_check/tests/__init__.py
--rw-rw-rw-   0        0        0     1296 2024-05-07 12:24:28.000000 test_core_package-0.0.1/qa_qc_check/tests/test_meta_data_extractor.py
-drwxrwxrwx   0        0        0        0 2024-05-13 06:56:39.579136 test_core_package-0.0.1/satelite/
--rw-rw-rw-   0        0        0        0 2024-05-07 11:29:36.000000 test_core_package-0.0.1/satelite/__init__.py
--rw-rw-rw-   0        0        0      651 2024-05-07 11:29:36.000000 test_core_package-0.0.1/satelite/config.py
-drwxrwxrwx   0        0        0        0 2024-05-13 06:56:39.595262 test_core_package-0.0.1/satelite/sentinel2/
--rw-rw-rw-   0        0        0      160 2024-05-07 11:29:36.000000 test_core_package-0.0.1/satelite/sentinel2/__init__.py
--rw-rw-rw-   0        0        0     2486 2024-05-07 11:29:36.000000 test_core_package-0.0.1/satelite/sentinel2/fetch_unique_tile_date.py
--rw-rw-rw-   0        0        0     1679 2024-05-07 11:29:36.000000 test_core_package-0.0.1/satelite/sentinel2/fetch_unique_tile_date_pystac.py
--rw-rw-rw-   0        0        0     3086 2024-05-07 11:29:36.000000 test_core_package-0.0.1/satelite/sentinel2/get_tiles.py
-drwxrwxrwx   0        0        0        0 2024-05-13 06:56:39.600182 test_core_package-0.0.1/satelite/tests/
--rw-rw-rw-   0        0        0        0 2024-05-07 11:29:36.000000 test_core_package-0.0.1/satelite/tests/__init__.py
--rw-rw-rw-   0        0        0      772 2024-05-07 11:29:36.000000 test_core_package-0.0.1/satelite/tests/conftest.py
-drwxrwxrwx   0        0        0        0 2024-05-13 06:56:39.611811 test_core_package-0.0.1/satelite/tests/sentinel2/
--rw-rw-rw-   0        0        0        0 2024-05-07 11:29:36.000000 test_core_package-0.0.1/satelite/tests/sentinel2/__init__.py
--rw-rw-rw-   0        0        0      396 2024-05-07 11:29:36.000000 test_core_package-0.0.1/satelite/tests/sentinel2/test_fetch_unique_tile_date.py
--rw-rw-rw-   0        0        0      443 2024-05-07 11:29:36.000000 test_core_package-0.0.1/satelite/tests/sentinel2/test_fetch_unique_tile_date_pystac.py
--rw-rw-rw-   0        0        0     1362 2024-05-07 11:29:36.000000 test_core_package-0.0.1/satelite/tests/sentinel2/test_get_tile.py
--rw-rw-rw-   0        0        0       42 2024-05-13 06:56:39.695102 test_core_package-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      880 2024-05-13 06:56:31.000000 test_core_package-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-13 06:56:39.686312 test_core_package-0.0.1/test_core_package.egg-info/
--rw-rw-rw-   0        0        0      241 2024-05-13 06:56:39.000000 test_core_package-0.0.1/test_core_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1057 2024-05-13 06:56:39.000000 test_core_package-0.0.1/test_core_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 06:56:39.000000 test_core_package-0.0.1/test_core_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      289 2024-05-13 06:56:39.000000 test_core_package-0.0.1/test_core_package.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2024-05-13 06:56:39.000000 test_core_package-0.0.1/test_core_package.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-13 07:09:10.018471 test_core_package-0.0.2/
+-rw-rw-rw-   0        0        0        0 2024-04-29 09:27:23.000000 test_core_package-0.0.2/LICENCE.txt
+-rw-rw-rw-   0        0        0      241 2024-05-13 07:09:10.017189 test_core_package-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-29 09:27:23.000000 test_core_package-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 07:09:09.696488 test_core_package-0.0.2/qa_qc_check/
+-rw-rw-rw-   0        0        0        0 2024-05-07 12:52:35.000000 test_core_package-0.0.2/qa_qc_check/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 07:09:09.764019 test_core_package-0.0.2/qa_qc_check/controller/
+-rw-rw-rw-   0        0        0        0 2024-05-02 09:51:13.000000 test_core_package-0.0.2/qa_qc_check/controller/__init__.py
+-rw-rw-rw-   0        0        0     4161 2024-05-06 12:22:37.000000 test_core_package-0.0.2/qa_qc_check/controller/checks.json
+-rw-rw-rw-   0        0        0     4310 2024-05-13 06:11:44.000000 test_core_package-0.0.2/qa_qc_check/controller/meta_data.py
+-rw-rw-rw-   0        0        0     3756 2024-05-13 06:11:23.000000 test_core_package-0.0.2/qa_qc_check/controller/meta_data_extractor.py
+-rw-rw-rw-   0        0        0     1951 2024-05-07 07:45:01.000000 test_core_package-0.0.2/qa_qc_check/controller/meta_data_validator.py
+-rw-rw-rw-   0        0        0      932 2024-05-07 07:38:44.000000 test_core_package-0.0.2/qa_qc_check/controller/metadata_model.py
+-rw-rw-rw-   0        0        0     1587 2024-05-13 07:08:30.000000 test_core_package-0.0.2/qa_qc_check/controller/qa_qc.py
+drwxrwxrwx   0        0        0        0 2024-05-13 07:09:09.770978 test_core_package-0.0.2/qa_qc_check/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-07 11:46:23.000000 test_core_package-0.0.2/qa_qc_check/tests/__init__.py
+-rw-rw-rw-   0        0        0     1296 2024-05-07 12:24:28.000000 test_core_package-0.0.2/qa_qc_check/tests/test_meta_data_extractor.py
+drwxrwxrwx   0        0        0        0 2024-05-13 07:09:09.780521 test_core_package-0.0.2/satelite/
+-rw-rw-rw-   0        0        0        0 2024-05-07 11:29:36.000000 test_core_package-0.0.2/satelite/__init__.py
+-rw-rw-rw-   0        0        0      651 2024-05-07 11:29:36.000000 test_core_package-0.0.2/satelite/config.py
+drwxrwxrwx   0        0        0        0 2024-05-13 07:09:09.797462 test_core_package-0.0.2/satelite/sentinel2/
+-rw-rw-rw-   0        0        0      160 2024-05-07 11:29:36.000000 test_core_package-0.0.2/satelite/sentinel2/__init__.py
+-rw-rw-rw-   0        0        0     2486 2024-05-07 11:29:36.000000 test_core_package-0.0.2/satelite/sentinel2/fetch_unique_tile_date.py
+-rw-rw-rw-   0        0        0     1679 2024-05-07 11:29:36.000000 test_core_package-0.0.2/satelite/sentinel2/fetch_unique_tile_date_pystac.py
+-rw-rw-rw-   0        0        0     3086 2024-05-07 11:29:36.000000 test_core_package-0.0.2/satelite/sentinel2/get_tiles.py
+drwxrwxrwx   0        0        0        0 2024-05-13 07:09:09.803157 test_core_package-0.0.2/satelite/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-07 11:29:36.000000 test_core_package-0.0.2/satelite/tests/__init__.py
+-rw-rw-rw-   0        0        0      772 2024-05-07 11:29:36.000000 test_core_package-0.0.2/satelite/tests/conftest.py
+drwxrwxrwx   0        0        0        0 2024-05-13 07:09:09.824702 test_core_package-0.0.2/satelite/tests/sentinel2/
+-rw-rw-rw-   0        0        0        0 2024-05-07 11:29:36.000000 test_core_package-0.0.2/satelite/tests/sentinel2/__init__.py
+-rw-rw-rw-   0        0        0      396 2024-05-07 11:29:36.000000 test_core_package-0.0.2/satelite/tests/sentinel2/test_fetch_unique_tile_date.py
+-rw-rw-rw-   0        0        0      443 2024-05-07 11:29:36.000000 test_core_package-0.0.2/satelite/tests/sentinel2/test_fetch_unique_tile_date_pystac.py
+-rw-rw-rw-   0        0        0     1362 2024-05-07 11:29:36.000000 test_core_package-0.0.2/satelite/tests/sentinel2/test_get_tile.py
+-rw-rw-rw-   0        0        0       42 2024-05-13 07:09:10.018992 test_core_package-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      880 2024-05-13 07:09:01.000000 test_core_package-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 07:09:10.014059 test_core_package-0.0.2/test_core_package.egg-info/
+-rw-rw-rw-   0        0        0      241 2024-05-13 07:09:09.000000 test_core_package-0.0.2/test_core_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1057 2024-05-13 07:09:09.000000 test_core_package-0.0.2/test_core_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 07:09:09.000000 test_core_package-0.0.2/test_core_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      289 2024-05-13 07:09:09.000000 test_core_package-0.0.2/test_core_package.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2024-05-13 07:09:09.000000 test_core_package-0.0.2/test_core_package.egg-info/top_level.txt
```

### Comparing `test_core_package-0.0.1/qa_qc_check/controller/checks.json` & `test_core_package-0.0.2/qa_qc_check/controller/checks.json`

 * *Files identical despite different names*

### Comparing `test_core_package-0.0.1/qa_qc_check/controller/meta_data.py` & `test_core_package-0.0.2/qa_qc_check/controller/meta_data.py`

 * *Files identical despite different names*

### Comparing `test_core_package-0.0.1/qa_qc_check/controller/meta_data_extractor.py` & `test_core_package-0.0.2/qa_qc_check/controller/meta_data_extractor.py`

 * *Files identical despite different names*

### Comparing `test_core_package-0.0.1/qa_qc_check/controller/meta_data_validator.py` & `test_core_package-0.0.2/qa_qc_check/controller/meta_data_validator.py`

 * *Files identical despite different names*

### Comparing `test_core_package-0.0.1/qa_qc_check/controller/metadata_model.py` & `test_core_package-0.0.2/qa_qc_check/controller/metadata_model.py`

 * *Files identical despite different names*

### Comparing `test_core_package-0.0.1/qa_qc_check/controller/qa_qc.py` & `test_core_package-0.0.2/qa_qc_check/controller/qa_qc.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Dict
 
-from meta_data_validator import (
+from qa_qc_check.controller.meta_data_validator import (
     FilenameProductCodeValidator,
     FileNameSeasonCodeValidator,
     ValuesRangeValidator,
 )
-from metadata_model import QaQcModel
+from qa_qc_check.controller.metadata_model import QaQcModel
 
 
 class QaQc:
 
     VALIDATORS = {
         "filename_product_code": FilenameProductCodeValidator,
         "filename_season_code_startswith": FileNameSeasonCodeValidator,
```

### Comparing `test_core_package-0.0.1/qa_qc_check/tests/test_meta_data_extractor.py` & `test_core_package-0.0.2/qa_qc_check/tests/test_meta_data_extractor.py`

 * *Files identical despite different names*

### Comparing `test_core_package-0.0.1/satelite/config.py` & `test_core_package-0.0.2/satelite/config.py`

 * *Files identical despite different names*

### Comparing `test_core_package-0.0.1/satelite/sentinel2/fetch_unique_tile_date.py` & `test_core_package-0.0.2/satelite/sentinel2/fetch_unique_tile_date.py`

 * *Files identical despite different names*

### Comparing `test_core_package-0.0.1/satelite/sentinel2/fetch_unique_tile_date_pystac.py` & `test_core_package-0.0.2/satelite/sentinel2/fetch_unique_tile_date_pystac.py`

 * *Files identical despite different names*

### Comparing `test_core_package-0.0.1/satelite/sentinel2/get_tiles.py` & `test_core_package-0.0.2/satelite/sentinel2/get_tiles.py`

 * *Files identical despite different names*

### Comparing `test_core_package-0.0.1/satelite/tests/conftest.py` & `test_core_package-0.0.2/satelite/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `test_core_package-0.0.1/satelite/tests/sentinel2/test_get_tile.py` & `test_core_package-0.0.2/satelite/tests/sentinel2/test_get_tile.py`

 * *Files identical despite different names*

### Comparing `test_core_package-0.0.1/setup.py` & `test_core_package-0.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="test_core_package",
-    version="0.0.1",
+    version="0.0.2",
     description="satsure core package",
     author="Satsure",
     author_email="kmstpm@email.com",
     packages=find_packages(),
     install_requires=[
         "requests",
         "fiona",
```

### Comparing `test_core_package-0.0.1/test_core_package.egg-info/SOURCES.txt` & `test_core_package-0.0.2/test_core_package.egg-info/SOURCES.txt`

 * *Files identical despite different names*

