# Comparing `tmp/test_core_package-0.0.4.tar.gz` & `tmp/test_core_package-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_core_package-0.0.4.tar", last modified: Mon May 13 07:24:29 2024, max compression
+gzip compressed data, was "test_core_package-0.0.5.tar", last modified: Mon May 13 07:31:45 2024, max compression
```

## Comparing `test_core_package-0.0.4.tar` & `test_core_package-0.0.5.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 07:24:29.653765 test_core_package-0.0.4/
--rw-rw-rw-   0        0        0        0 2024-04-29 09:27:23.000000 test_core_package-0.0.4/LICENCE.txt
--rw-rw-rw-   0        0        0      241 2024-05-13 07:24:29.652762 test_core_package-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-29 09:27:23.000000 test_core_package-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-13 07:24:29.579855 test_core_package-0.0.4/qa_qc_check/
--rw-rw-rw-   0        0        0        0 2024-05-07 12:52:35.000000 test_core_package-0.0.4/qa_qc_check/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 07:24:29.603599 test_core_package-0.0.4/qa_qc_check/controller/
--rw-rw-rw-   0        0        0        0 2024-05-02 09:51:13.000000 test_core_package-0.0.4/qa_qc_check/controller/__init__.py
--rw-rw-rw-   0        0        0     4161 2024-05-06 12:22:37.000000 test_core_package-0.0.4/qa_qc_check/controller/checks.json
--rw-rw-rw-   0        0        0     4310 2024-05-13 06:11:44.000000 test_core_package-0.0.4/qa_qc_check/controller/meta_data.py
--rw-rw-rw-   0        0        0     3732 2024-05-13 07:21:49.000000 test_core_package-0.0.4/qa_qc_check/controller/meta_data_extractor.py
--rw-rw-rw-   0        0        0     1951 2024-05-07 07:45:01.000000 test_core_package-0.0.4/qa_qc_check/controller/meta_data_validator.py
--rw-rw-rw-   0        0        0      932 2024-05-07 07:38:44.000000 test_core_package-0.0.4/qa_qc_check/controller/metadata_model.py
--rw-rw-rw-   0        0        0     1587 2024-05-13 07:08:30.000000 test_core_package-0.0.4/qa_qc_check/controller/qa_qc.py
-drwxrwxrwx   0        0        0        0 2024-05-13 07:24:29.606593 test_core_package-0.0.4/qa_qc_check/tests/
--rw-rw-rw-   0        0        0        0 2024-05-07 11:46:23.000000 test_core_package-0.0.4/qa_qc_check/tests/__init__.py
--rw-rw-rw-   0        0        0     1296 2024-05-07 12:24:28.000000 test_core_package-0.0.4/qa_qc_check/tests/test_meta_data_extractor.py
-drwxrwxrwx   0        0        0        0 2024-05-13 07:24:29.612197 test_core_package-0.0.4/satelite/
--rw-rw-rw-   0        0        0        0 2024-05-07 11:29:36.000000 test_core_package-0.0.4/satelite/__init__.py
--rw-rw-rw-   0        0        0      651 2024-05-07 11:29:36.000000 test_core_package-0.0.4/satelite/config.py
-drwxrwxrwx   0        0        0        0 2024-05-13 07:24:29.617677 test_core_package-0.0.4/satelite/sentinel2/
--rw-rw-rw-   0        0        0      160 2024-05-07 11:29:36.000000 test_core_package-0.0.4/satelite/sentinel2/__init__.py
--rw-rw-rw-   0        0        0     2486 2024-05-07 11:29:36.000000 test_core_package-0.0.4/satelite/sentinel2/fetch_unique_tile_date.py
--rw-rw-rw-   0        0        0     1679 2024-05-07 11:29:36.000000 test_core_package-0.0.4/satelite/sentinel2/fetch_unique_tile_date_pystac.py
--rw-rw-rw-   0        0        0     3086 2024-05-07 11:29:36.000000 test_core_package-0.0.4/satelite/sentinel2/get_tiles.py
-drwxrwxrwx   0        0        0        0 2024-05-13 07:24:29.619970 test_core_package-0.0.4/satelite/tests/
--rw-rw-rw-   0        0        0        0 2024-05-07 11:29:36.000000 test_core_package-0.0.4/satelite/tests/__init__.py
--rw-rw-rw-   0        0        0      772 2024-05-07 11:29:36.000000 test_core_package-0.0.4/satelite/tests/conftest.py
-drwxrwxrwx   0        0        0        0 2024-05-13 07:24:29.630805 test_core_package-0.0.4/satelite/tests/sentinel2/
--rw-rw-rw-   0        0        0        0 2024-05-07 11:29:36.000000 test_core_package-0.0.4/satelite/tests/sentinel2/__init__.py
--rw-rw-rw-   0        0        0      396 2024-05-07 11:29:36.000000 test_core_package-0.0.4/satelite/tests/sentinel2/test_fetch_unique_tile_date.py
--rw-rw-rw-   0        0        0      443 2024-05-07 11:29:36.000000 test_core_package-0.0.4/satelite/tests/sentinel2/test_fetch_unique_tile_date_pystac.py
--rw-rw-rw-   0        0        0     1362 2024-05-07 11:29:36.000000 test_core_package-0.0.4/satelite/tests/sentinel2/test_get_tile.py
--rw-rw-rw-   0        0        0       42 2024-05-13 07:24:29.654969 test_core_package-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      898 2024-05-13 07:24:27.000000 test_core_package-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-13 07:24:29.650762 test_core_package-0.0.4/test_core_package.egg-info/
--rw-rw-rw-   0        0        0      241 2024-05-13 07:24:29.000000 test_core_package-0.0.4/test_core_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1057 2024-05-13 07:24:29.000000 test_core_package-0.0.4/test_core_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 07:24:29.000000 test_core_package-0.0.4/test_core_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      289 2024-05-13 07:24:29.000000 test_core_package-0.0.4/test_core_package.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2024-05-13 07:24:29.000000 test_core_package-0.0.4/test_core_package.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-13 07:31:45.159911 test_core_package-0.0.5/
+-rw-rw-rw-   0        0        0        0 2024-04-29 09:27:23.000000 test_core_package-0.0.5/LICENCE.txt
+-rw-rw-rw-   0        0        0      241 2024-05-13 07:31:45.158673 test_core_package-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-29 09:27:23.000000 test_core_package-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 07:31:45.099569 test_core_package-0.0.5/qa_qc_check/
+-rw-rw-rw-   0        0        0        0 2024-05-07 12:52:35.000000 test_core_package-0.0.5/qa_qc_check/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 07:31:45.110131 test_core_package-0.0.5/qa_qc_check/controller/
+-rw-rw-rw-   0        0        0        0 2024-05-02 09:51:13.000000 test_core_package-0.0.5/qa_qc_check/controller/__init__.py
+-rw-rw-rw-   0        0        0     4161 2024-05-06 12:22:37.000000 test_core_package-0.0.5/qa_qc_check/controller/checks.json
+-rw-rw-rw-   0        0        0     4310 2024-05-13 06:11:44.000000 test_core_package-0.0.5/qa_qc_check/controller/meta_data.py
+-rw-rw-rw-   0        0        0     9348 2024-05-13 07:31:05.000000 test_core_package-0.0.5/qa_qc_check/controller/meta_data_extractor.py
+-rw-rw-rw-   0        0        0     1951 2024-05-07 07:45:01.000000 test_core_package-0.0.5/qa_qc_check/controller/meta_data_validator.py
+-rw-rw-rw-   0        0        0      932 2024-05-07 07:38:44.000000 test_core_package-0.0.5/qa_qc_check/controller/metadata_model.py
+-rw-rw-rw-   0        0        0     1587 2024-05-13 07:08:30.000000 test_core_package-0.0.5/qa_qc_check/controller/qa_qc.py
+drwxrwxrwx   0        0        0        0 2024-05-13 07:31:45.113129 test_core_package-0.0.5/qa_qc_check/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-07 11:46:23.000000 test_core_package-0.0.5/qa_qc_check/tests/__init__.py
+-rw-rw-rw-   0        0        0     1296 2024-05-07 12:24:28.000000 test_core_package-0.0.5/qa_qc_check/tests/test_meta_data_extractor.py
+drwxrwxrwx   0        0        0        0 2024-05-13 07:31:45.116546 test_core_package-0.0.5/satelite/
+-rw-rw-rw-   0        0        0        0 2024-05-07 11:29:36.000000 test_core_package-0.0.5/satelite/__init__.py
+-rw-rw-rw-   0        0        0      651 2024-05-07 11:29:36.000000 test_core_package-0.0.5/satelite/config.py
+drwxrwxrwx   0        0        0        0 2024-05-13 07:31:45.122547 test_core_package-0.0.5/satelite/sentinel2/
+-rw-rw-rw-   0        0        0      160 2024-05-07 11:29:36.000000 test_core_package-0.0.5/satelite/sentinel2/__init__.py
+-rw-rw-rw-   0        0        0     2486 2024-05-07 11:29:36.000000 test_core_package-0.0.5/satelite/sentinel2/fetch_unique_tile_date.py
+-rw-rw-rw-   0        0        0     1679 2024-05-07 11:29:36.000000 test_core_package-0.0.5/satelite/sentinel2/fetch_unique_tile_date_pystac.py
+-rw-rw-rw-   0        0        0     3086 2024-05-07 11:29:36.000000 test_core_package-0.0.5/satelite/sentinel2/get_tiles.py
+drwxrwxrwx   0        0        0        0 2024-05-13 07:31:45.124578 test_core_package-0.0.5/satelite/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-07 11:29:36.000000 test_core_package-0.0.5/satelite/tests/__init__.py
+-rw-rw-rw-   0        0        0      772 2024-05-07 11:29:36.000000 test_core_package-0.0.5/satelite/tests/conftest.py
+drwxrwxrwx   0        0        0        0 2024-05-13 07:31:45.130598 test_core_package-0.0.5/satelite/tests/sentinel2/
+-rw-rw-rw-   0        0        0        0 2024-05-07 11:29:36.000000 test_core_package-0.0.5/satelite/tests/sentinel2/__init__.py
+-rw-rw-rw-   0        0        0      396 2024-05-07 11:29:36.000000 test_core_package-0.0.5/satelite/tests/sentinel2/test_fetch_unique_tile_date.py
+-rw-rw-rw-   0        0        0      443 2024-05-07 11:29:36.000000 test_core_package-0.0.5/satelite/tests/sentinel2/test_fetch_unique_tile_date_pystac.py
+-rw-rw-rw-   0        0        0     1362 2024-05-07 11:29:36.000000 test_core_package-0.0.5/satelite/tests/sentinel2/test_get_tile.py
+-rw-rw-rw-   0        0        0       42 2024-05-13 07:31:45.160918 test_core_package-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      898 2024-05-13 07:31:35.000000 test_core_package-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 07:31:45.157670 test_core_package-0.0.5/test_core_package.egg-info/
+-rw-rw-rw-   0        0        0      241 2024-05-13 07:31:45.000000 test_core_package-0.0.5/test_core_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1057 2024-05-13 07:31:45.000000 test_core_package-0.0.5/test_core_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 07:31:45.000000 test_core_package-0.0.5/test_core_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      289 2024-05-13 07:31:45.000000 test_core_package-0.0.5/test_core_package.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2024-05-13 07:31:45.000000 test_core_package-0.0.5/test_core_package.egg-info/top_level.txt
```

### Comparing `test_core_package-0.0.4/qa_qc_check/controller/checks.json` & `test_core_package-0.0.5/qa_qc_check/controller/checks.json`

 * *Files identical despite different names*

### Comparing `test_core_package-0.0.4/qa_qc_check/controller/meta_data.py` & `test_core_package-0.0.5/qa_qc_check/controller/meta_data.py`

 * *Files identical despite different names*

### Comparing `test_core_package-0.0.4/qa_qc_check/controller/meta_data_validator.py` & `test_core_package-0.0.5/qa_qc_check/controller/meta_data_validator.py`

 * *Files identical despite different names*

### Comparing `test_core_package-0.0.4/qa_qc_check/controller/metadata_model.py` & `test_core_package-0.0.5/qa_qc_check/controller/metadata_model.py`

 * *Files identical despite different names*

### Comparing `test_core_package-0.0.4/qa_qc_check/controller/qa_qc.py` & `test_core_package-0.0.5/qa_qc_check/controller/qa_qc.py`

 * *Files identical despite different names*

### Comparing `test_core_package-0.0.4/qa_qc_check/tests/test_meta_data_extractor.py` & `test_core_package-0.0.5/qa_qc_check/tests/test_meta_data_extractor.py`

 * *Files identical despite different names*

### Comparing `test_core_package-0.0.4/satelite/config.py` & `test_core_package-0.0.5/satelite/config.py`

 * *Files identical despite different names*

### Comparing `test_core_package-0.0.4/satelite/sentinel2/fetch_unique_tile_date.py` & `test_core_package-0.0.5/satelite/sentinel2/fetch_unique_tile_date.py`

 * *Files identical despite different names*

### Comparing `test_core_package-0.0.4/satelite/sentinel2/fetch_unique_tile_date_pystac.py` & `test_core_package-0.0.5/satelite/sentinel2/fetch_unique_tile_date_pystac.py`

 * *Files identical despite different names*

### Comparing `test_core_package-0.0.4/satelite/sentinel2/get_tiles.py` & `test_core_package-0.0.5/satelite/sentinel2/get_tiles.py`

 * *Files identical despite different names*

### Comparing `test_core_package-0.0.4/satelite/tests/conftest.py` & `test_core_package-0.0.5/satelite/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `test_core_package-0.0.4/satelite/tests/sentinel2/test_get_tile.py` & `test_core_package-0.0.5/satelite/tests/sentinel2/test_get_tile.py`

 * *Files identical despite different names*

### Comparing `test_core_package-0.0.4/setup.py` & `test_core_package-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="test_core_package",
-    version="0.0.4",
+    version="0.0.5",
     description="satsure core package",
     author="Satsure",
     author_email="kmstpm@email.com",
     packages=find_packages(),
     install_requires=[
         "requests",
         "fiona",
```

### Comparing `test_core_package-0.0.4/test_core_package.egg-info/SOURCES.txt` & `test_core_package-0.0.5/test_core_package.egg-info/SOURCES.txt`

 * *Files identical despite different names*

