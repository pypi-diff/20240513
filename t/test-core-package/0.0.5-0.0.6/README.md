# Comparing `tmp/test_core_package-0.0.5.tar.gz` & `tmp/test_core_package-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_core_package-0.0.5.tar", last modified: Mon May 13 07:31:45 2024, max compression
+gzip compressed data, was "test_core_package-0.0.6.tar", last modified: Mon May 13 07:36:23 2024, max compression
```

## Comparing `test_core_package-0.0.5.tar` & `test_core_package-0.0.6.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 07:31:45.159911 test_core_package-0.0.5/
--rw-rw-rw-   0        0        0        0 2024-04-29 09:27:23.000000 test_core_package-0.0.5/LICENCE.txt
--rw-rw-rw-   0        0        0      241 2024-05-13 07:31:45.158673 test_core_package-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-29 09:27:23.000000 test_core_package-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-13 07:31:45.099569 test_core_package-0.0.5/qa_qc_check/
--rw-rw-rw-   0        0        0        0 2024-05-07 12:52:35.000000 test_core_package-0.0.5/qa_qc_check/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 07:31:45.110131 test_core_package-0.0.5/qa_qc_check/controller/
--rw-rw-rw-   0        0        0        0 2024-05-02 09:51:13.000000 test_core_package-0.0.5/qa_qc_check/controller/__init__.py
--rw-rw-rw-   0        0        0     4161 2024-05-06 12:22:37.000000 test_core_package-0.0.5/qa_qc_check/controller/checks.json
--rw-rw-rw-   0        0        0     4310 2024-05-13 06:11:44.000000 test_core_package-0.0.5/qa_qc_check/controller/meta_data.py
--rw-rw-rw-   0        0        0     9348 2024-05-13 07:31:05.000000 test_core_package-0.0.5/qa_qc_check/controller/meta_data_extractor.py
--rw-rw-rw-   0        0        0     1951 2024-05-07 07:45:01.000000 test_core_package-0.0.5/qa_qc_check/controller/meta_data_validator.py
--rw-rw-rw-   0        0        0      932 2024-05-07 07:38:44.000000 test_core_package-0.0.5/qa_qc_check/controller/metadata_model.py
--rw-rw-rw-   0        0        0     1587 2024-05-13 07:08:30.000000 test_core_package-0.0.5/qa_qc_check/controller/qa_qc.py
-drwxrwxrwx   0        0        0        0 2024-05-13 07:31:45.113129 test_core_package-0.0.5/qa_qc_check/tests/
--rw-rw-rw-   0        0        0        0 2024-05-07 11:46:23.000000 test_core_package-0.0.5/qa_qc_check/tests/__init__.py
--rw-rw-rw-   0        0        0     1296 2024-05-07 12:24:28.000000 test_core_package-0.0.5/qa_qc_check/tests/test_meta_data_extractor.py
-drwxrwxrwx   0        0        0        0 2024-05-13 07:31:45.116546 test_core_package-0.0.5/satelite/
--rw-rw-rw-   0        0        0        0 2024-05-07 11:29:36.000000 test_core_package-0.0.5/satelite/__init__.py
--rw-rw-rw-   0        0        0      651 2024-05-07 11:29:36.000000 test_core_package-0.0.5/satelite/config.py
-drwxrwxrwx   0        0        0        0 2024-05-13 07:31:45.122547 test_core_package-0.0.5/satelite/sentinel2/
--rw-rw-rw-   0        0        0      160 2024-05-07 11:29:36.000000 test_core_package-0.0.5/satelite/sentinel2/__init__.py
--rw-rw-rw-   0        0        0     2486 2024-05-07 11:29:36.000000 test_core_package-0.0.5/satelite/sentinel2/fetch_unique_tile_date.py
--rw-rw-rw-   0        0        0     1679 2024-05-07 11:29:36.000000 test_core_package-0.0.5/satelite/sentinel2/fetch_unique_tile_date_pystac.py
--rw-rw-rw-   0        0        0     3086 2024-05-07 11:29:36.000000 test_core_package-0.0.5/satelite/sentinel2/get_tiles.py
-drwxrwxrwx   0        0        0        0 2024-05-13 07:31:45.124578 test_core_package-0.0.5/satelite/tests/
--rw-rw-rw-   0        0        0        0 2024-05-07 11:29:36.000000 test_core_package-0.0.5/satelite/tests/__init__.py
--rw-rw-rw-   0        0        0      772 2024-05-07 11:29:36.000000 test_core_package-0.0.5/satelite/tests/conftest.py
-drwxrwxrwx   0        0        0        0 2024-05-13 07:31:45.130598 test_core_package-0.0.5/satelite/tests/sentinel2/
--rw-rw-rw-   0        0        0        0 2024-05-07 11:29:36.000000 test_core_package-0.0.5/satelite/tests/sentinel2/__init__.py
--rw-rw-rw-   0        0        0      396 2024-05-07 11:29:36.000000 test_core_package-0.0.5/satelite/tests/sentinel2/test_fetch_unique_tile_date.py
--rw-rw-rw-   0        0        0      443 2024-05-07 11:29:36.000000 test_core_package-0.0.5/satelite/tests/sentinel2/test_fetch_unique_tile_date_pystac.py
--rw-rw-rw-   0        0        0     1362 2024-05-07 11:29:36.000000 test_core_package-0.0.5/satelite/tests/sentinel2/test_get_tile.py
--rw-rw-rw-   0        0        0       42 2024-05-13 07:31:45.160918 test_core_package-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      898 2024-05-13 07:31:35.000000 test_core_package-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-13 07:31:45.157670 test_core_package-0.0.5/test_core_package.egg-info/
--rw-rw-rw-   0        0        0      241 2024-05-13 07:31:45.000000 test_core_package-0.0.5/test_core_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1057 2024-05-13 07:31:45.000000 test_core_package-0.0.5/test_core_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 07:31:45.000000 test_core_package-0.0.5/test_core_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      289 2024-05-13 07:31:45.000000 test_core_package-0.0.5/test_core_package.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2024-05-13 07:31:45.000000 test_core_package-0.0.5/test_core_package.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-13 07:36:23.741207 test_core_package-0.0.6/
+-rw-rw-rw-   0        0        0        0 2024-04-29 09:27:23.000000 test_core_package-0.0.6/LICENCE.txt
+-rw-rw-rw-   0        0        0      241 2024-05-13 07:36:23.740198 test_core_package-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-29 09:27:23.000000 test_core_package-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 07:36:23.559841 test_core_package-0.0.6/qa_qc_check/
+-rw-rw-rw-   0        0        0        0 2024-05-07 12:52:35.000000 test_core_package-0.0.6/qa_qc_check/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 07:36:23.585119 test_core_package-0.0.6/qa_qc_check/controller/
+-rw-rw-rw-   0        0        0        0 2024-05-02 09:51:13.000000 test_core_package-0.0.6/qa_qc_check/controller/__init__.py
+-rw-rw-rw-   0        0        0     4161 2024-05-06 12:22:37.000000 test_core_package-0.0.6/qa_qc_check/controller/checks.json
+-rw-rw-rw-   0        0        0     4310 2024-05-13 06:11:44.000000 test_core_package-0.0.6/qa_qc_check/controller/meta_data.py
+-rw-rw-rw-   0        0        0     9348 2024-05-13 07:36:04.000000 test_core_package-0.0.6/qa_qc_check/controller/meta_data_extractor.py
+-rw-rw-rw-   0        0        0     1951 2024-05-07 07:45:01.000000 test_core_package-0.0.6/qa_qc_check/controller/meta_data_validator.py
+-rw-rw-rw-   0        0        0      932 2024-05-07 07:38:44.000000 test_core_package-0.0.6/qa_qc_check/controller/metadata_model.py
+-rw-rw-rw-   0        0        0     1587 2024-05-13 07:08:30.000000 test_core_package-0.0.6/qa_qc_check/controller/qa_qc.py
+drwxrwxrwx   0        0        0        0 2024-05-13 07:36:23.588135 test_core_package-0.0.6/qa_qc_check/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-07 11:46:23.000000 test_core_package-0.0.6/qa_qc_check/tests/__init__.py
+-rw-rw-rw-   0        0        0     1296 2024-05-07 12:24:28.000000 test_core_package-0.0.6/qa_qc_check/tests/test_meta_data_extractor.py
+drwxrwxrwx   0        0        0        0 2024-05-13 07:36:23.661906 test_core_package-0.0.6/satelite/
+-rw-rw-rw-   0        0        0        0 2024-05-07 11:29:36.000000 test_core_package-0.0.6/satelite/__init__.py
+-rw-rw-rw-   0        0        0      651 2024-05-07 11:29:36.000000 test_core_package-0.0.6/satelite/config.py
+drwxrwxrwx   0        0        0        0 2024-05-13 07:36:23.699541 test_core_package-0.0.6/satelite/sentinel2/
+-rw-rw-rw-   0        0        0      160 2024-05-07 11:29:36.000000 test_core_package-0.0.6/satelite/sentinel2/__init__.py
+-rw-rw-rw-   0        0        0     2486 2024-05-07 11:29:36.000000 test_core_package-0.0.6/satelite/sentinel2/fetch_unique_tile_date.py
+-rw-rw-rw-   0        0        0     1679 2024-05-07 11:29:36.000000 test_core_package-0.0.6/satelite/sentinel2/fetch_unique_tile_date_pystac.py
+-rw-rw-rw-   0        0        0     3086 2024-05-07 11:29:36.000000 test_core_package-0.0.6/satelite/sentinel2/get_tiles.py
+drwxrwxrwx   0        0        0        0 2024-05-13 07:36:23.704480 test_core_package-0.0.6/satelite/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-07 11:29:36.000000 test_core_package-0.0.6/satelite/tests/__init__.py
+-rw-rw-rw-   0        0        0      772 2024-05-07 11:29:36.000000 test_core_package-0.0.6/satelite/tests/conftest.py
+drwxrwxrwx   0        0        0        0 2024-05-13 07:36:23.711463 test_core_package-0.0.6/satelite/tests/sentinel2/
+-rw-rw-rw-   0        0        0        0 2024-05-07 11:29:36.000000 test_core_package-0.0.6/satelite/tests/sentinel2/__init__.py
+-rw-rw-rw-   0        0        0      396 2024-05-07 11:29:36.000000 test_core_package-0.0.6/satelite/tests/sentinel2/test_fetch_unique_tile_date.py
+-rw-rw-rw-   0        0        0      443 2024-05-07 11:29:36.000000 test_core_package-0.0.6/satelite/tests/sentinel2/test_fetch_unique_tile_date_pystac.py
+-rw-rw-rw-   0        0        0     1362 2024-05-07 11:29:36.000000 test_core_package-0.0.6/satelite/tests/sentinel2/test_get_tile.py
+-rw-rw-rw-   0        0        0       42 2024-05-13 07:36:23.741207 test_core_package-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      898 2024-05-13 07:36:21.000000 test_core_package-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 07:36:23.737195 test_core_package-0.0.6/test_core_package.egg-info/
+-rw-rw-rw-   0        0        0      241 2024-05-13 07:36:23.000000 test_core_package-0.0.6/test_core_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1057 2024-05-13 07:36:23.000000 test_core_package-0.0.6/test_core_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 07:36:23.000000 test_core_package-0.0.6/test_core_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      289 2024-05-13 07:36:23.000000 test_core_package-0.0.6/test_core_package.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2024-05-13 07:36:23.000000 test_core_package-0.0.6/test_core_package.egg-info/top_level.txt
```

### Comparing `test_core_package-0.0.5/qa_qc_check/controller/checks.json` & `test_core_package-0.0.6/qa_qc_check/controller/checks.json`

 * *Files identical despite different names*

### Comparing `test_core_package-0.0.5/qa_qc_check/controller/meta_data.py` & `test_core_package-0.0.6/qa_qc_check/controller/meta_data.py`

 * *Files identical despite different names*

### Comparing `test_core_package-0.0.5/qa_qc_check/controller/meta_data_extractor.py` & `test_core_package-0.0.6/qa_qc_check/controller/meta_data_extractor.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,14 @@
         Args:
             file (str): S3 File Path
             check_type (str): QA/QC check type
         """
         self.file = file
         self.check_type = check_type
         # self.checks_json = json.load(open("checks.json", "r"))
-        self.product = self._fetch_product()
         self.checks_json = {
             "ndvi": {
                 "entry": {},
                 "exit": {
                     "filename_parts_count": 3,
                     "filename_endswith": ".tif",
                     "filename_date_chars": 8,
@@ -149,14 +148,15 @@
                     "values_range": [0, 1],
                     "compression_type": "LZW",
                 },
                 "product_list": ["CH"],
                 "s3_bucket_names": ["satsure-products"],
             },
         }
+        self.product = self._fetch_product()
 
     def _fetch_product(self):
         """
         Fetch product name from file path
 
         Returns:
             str: name of the product for the input file
```

### Comparing `test_core_package-0.0.5/qa_qc_check/controller/meta_data_validator.py` & `test_core_package-0.0.6/qa_qc_check/controller/meta_data_validator.py`

 * *Files identical despite different names*

### Comparing `test_core_package-0.0.5/qa_qc_check/controller/metadata_model.py` & `test_core_package-0.0.6/qa_qc_check/controller/metadata_model.py`

 * *Files identical despite different names*

### Comparing `test_core_package-0.0.5/qa_qc_check/controller/qa_qc.py` & `test_core_package-0.0.6/qa_qc_check/controller/qa_qc.py`

 * *Files identical despite different names*

### Comparing `test_core_package-0.0.5/qa_qc_check/tests/test_meta_data_extractor.py` & `test_core_package-0.0.6/qa_qc_check/tests/test_meta_data_extractor.py`

 * *Files identical despite different names*

### Comparing `test_core_package-0.0.5/satelite/config.py` & `test_core_package-0.0.6/satelite/config.py`

 * *Files identical despite different names*

### Comparing `test_core_package-0.0.5/satelite/sentinel2/fetch_unique_tile_date.py` & `test_core_package-0.0.6/satelite/sentinel2/fetch_unique_tile_date.py`

 * *Files identical despite different names*

### Comparing `test_core_package-0.0.5/satelite/sentinel2/fetch_unique_tile_date_pystac.py` & `test_core_package-0.0.6/satelite/sentinel2/fetch_unique_tile_date_pystac.py`

 * *Files identical despite different names*

### Comparing `test_core_package-0.0.5/satelite/sentinel2/get_tiles.py` & `test_core_package-0.0.6/satelite/sentinel2/get_tiles.py`

 * *Files identical despite different names*

### Comparing `test_core_package-0.0.5/satelite/tests/conftest.py` & `test_core_package-0.0.6/satelite/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `test_core_package-0.0.5/satelite/tests/sentinel2/test_get_tile.py` & `test_core_package-0.0.6/satelite/tests/sentinel2/test_get_tile.py`

 * *Files identical despite different names*

### Comparing `test_core_package-0.0.5/setup.py` & `test_core_package-0.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="test_core_package",
-    version="0.0.5",
+    version="0.0.6",
     description="satsure core package",
     author="Satsure",
     author_email="kmstpm@email.com",
     packages=find_packages(),
     install_requires=[
         "requests",
         "fiona",
```

### Comparing `test_core_package-0.0.5/test_core_package.egg-info/SOURCES.txt` & `test_core_package-0.0.6/test_core_package.egg-info/SOURCES.txt`

 * *Files identical despite different names*

