# Comparing `tmp/garmin-fit-sdk-21.133.0.tar.gz` & `tmp/garmin-fit-sdk-21.141.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/fit-python-sdk/fit-python-sdk/dist/tmpuzmoxm_1/garmin-fit-sdk-21.133.0.tar", last modified: Tue Feb 13 18:15:44 2024, max compression
+gzip compressed data, was "/home/runner/work/fit-python-sdk/fit-python-sdk/dist/tmp2s2d82qz/garmin-fit-sdk-21.141.0.tar", last modified: Mon May 13 20:33:22 2024, max compression
```

## Comparing `garmin-fit-sdk-21.133.0.tar` & `garmin-fit-sdk-21.141.0.tar`

### file list

```diff
@@ -1,43 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 18:15:44.000000 garmin-fit-sdk-21.133.0/
--rw-r--r--   0 runner    (1001) docker     (127)     8928 2024-02-13 18:15:32.000000 garmin-fit-sdk-21.133.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     9022 2024-02-13 18:15:44.000000 garmin-fit-sdk-21.133.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 18:15:44.000000 garmin-fit-sdk-21.133.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 18:15:44.000000 garmin-fit-sdk-21.133.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-02-13 18:15:32.000000 garmin-fit-sdk-21.133.0/.github/workflows/run_tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-02-13 18:15:32.000000 garmin-fit-sdk-21.133.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-02-13 18:15:44.000000 garmin-fit-sdk-21.133.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 18:15:44.000000 garmin-fit-sdk-21.133.0/garmin_fit_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9022 2024-02-13 18:15:44.000000 garmin-fit-sdk-21.133.0/garmin_fit_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-13 18:15:44.000000 garmin-fit-sdk-21.133.0/garmin_fit_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-02-13 18:15:44.000000 garmin-fit-sdk-21.133.0/garmin_fit_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-13 18:15:44.000000 garmin-fit-sdk-21.133.0/garmin_fit_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-13 18:15:44.000000 garmin-fit-sdk-21.133.0/garmin_fit_sdk.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 18:15:44.000000 garmin-fit-sdk-21.133.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 18:15:44.000000 garmin-fit-sdk-21.133.0/tests/fits/
--rw-r--r--   0 runner    (1001) docker     (127)    94199 2024-02-13 18:15:32.000000 garmin-fit-sdk-21.133.0/tests/fits/ActivityDevFields.fit
--rw-r--r--   0 runner    (1001) docker     (127)    90970 2024-02-13 18:15:32.000000 garmin-fit-sdk-21.133.0/tests/fits/WithGearChangeData.fit
--rw-r--r--   0 runner    (1001) docker     (127)    25121 2024-02-13 18:15:32.000000 garmin-fit-sdk-21.133.0/tests/fits/HrmPluginTestActivity.fit
--rw-r--r--   0 runner    (1001) docker     (127)    37792 2024-02-13 18:15:32.000000 garmin-fit-sdk-21.133.0/tests/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    11160 2024-02-13 18:15:32.000000 garmin-fit-sdk-21.133.0/tests/test_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     5222 2024-02-13 18:15:32.000000 garmin-fit-sdk-21.133.0/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-02-13 18:15:32.000000 garmin-fit-sdk-21.133.0/tests/test_crc_calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)   328393 2024-02-13 18:15:32.000000 garmin-fit-sdk-21.133.0/tests/data_expand_hr_mesgs.py
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-02-13 18:15:32.000000 garmin-fit-sdk-21.133.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-02-13 18:15:32.000000 garmin-fit-sdk-21.133.0/tests/test_hr_mesg_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-02-13 18:15:32.000000 garmin-fit-sdk-21.133.0/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     5565 2024-02-13 18:15:32.000000 garmin-fit-sdk-21.133.0/tests/test_bitstream.py
--rw-r--r--   0 runner    (1001) docker     (127)    25241 2024-02-13 18:15:32.000000 garmin-fit-sdk-21.133.0/tests/test_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-02-13 18:15:32.000000 garmin-fit-sdk-21.133.0/tests/test_accumulator.py
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-02-13 18:15:32.000000 garmin-fit-sdk-21.133.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 18:15:44.000000 garmin-fit-sdk-21.133.0/garmin_fit_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)   768516 2024-02-13 18:15:32.000000 garmin-fit-sdk-21.133.0/garmin_fit_sdk/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    32063 2024-02-13 18:15:32.000000 garmin-fit-sdk-21.133.0/garmin_fit_sdk/decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-02-13 18:15:32.000000 garmin-fit-sdk-21.133.0/garmin_fit_sdk/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3341 2024-02-13 18:15:32.000000 garmin-fit-sdk-21.133.0/garmin_fit_sdk/bitstream.py
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-02-13 18:15:32.000000 garmin-fit-sdk-21.133.0/garmin_fit_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6513 2024-02-13 18:15:32.000000 garmin-fit-sdk-21.133.0/garmin_fit_sdk/hr_mesg_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3851 2024-02-13 18:15:32.000000 garmin-fit-sdk-21.133.0/garmin_fit_sdk/fit.py
--rw-r--r--   0 runner    (1001) docker     (127)     6791 2024-02-13 18:15:32.000000 garmin-fit-sdk-21.133.0/garmin_fit_sdk/stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-02-13 18:15:32.000000 garmin-fit-sdk-21.133.0/garmin_fit_sdk/crc_calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-02-13 18:15:32.000000 garmin-fit-sdk-21.133.0/garmin_fit_sdk/accumulator.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-13 18:15:32.000000 garmin-fit-sdk-21.133.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:33:22.000000 garmin-fit-sdk-21.141.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:33:22.000000 garmin-fit-sdk-21.141.0/garmin_fit_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 20:33:22.000000 garmin-fit-sdk-21.141.0/garmin_fit_sdk.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     9022 2024-05-13 20:33:22.000000 garmin-fit-sdk-21.141.0/garmin_fit_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-13 20:33:22.000000 garmin-fit-sdk-21.141.0/garmin_fit_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-13 20:33:22.000000 garmin-fit-sdk-21.141.0/garmin_fit_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 20:33:22.000000 garmin-fit-sdk-21.141.0/garmin_fit_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8928 2024-05-13 20:33:10.000000 garmin-fit-sdk-21.141.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:33:22.000000 garmin-fit-sdk-21.141.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-05-13 20:33:10.000000 garmin-fit-sdk-21.141.0/tests/test_hr_mesg_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25241 2024-05-13 20:33:10.000000 garmin-fit-sdk-21.141.0/tests/test_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11160 2024-05-13 20:33:10.000000 garmin-fit-sdk-21.141.0/tests/test_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-13 20:33:10.000000 garmin-fit-sdk-21.141.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-13 20:33:10.000000 garmin-fit-sdk-21.141.0/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-13 20:33:10.000000 garmin-fit-sdk-21.141.0/tests/test_accumulator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:33:22.000000 garmin-fit-sdk-21.141.0/tests/fits/
+-rw-r--r--   0 runner    (1001) docker     (127)    94199 2024-05-13 20:33:10.000000 garmin-fit-sdk-21.141.0/tests/fits/ActivityDevFields.fit
+-rw-r--r--   0 runner    (1001) docker     (127)    25121 2024-05-13 20:33:10.000000 garmin-fit-sdk-21.141.0/tests/fits/HrmPluginTestActivity.fit
+-rw-r--r--   0 runner    (1001) docker     (127)    90970 2024-05-13 20:33:10.000000 garmin-fit-sdk-21.141.0/tests/fits/WithGearChangeData.fit
+-rw-r--r--   0 runner    (1001) docker     (127)   328393 2024-05-13 20:33:10.000000 garmin-fit-sdk-21.141.0/tests/data_expand_hr_mesgs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-05-13 20:33:10.000000 garmin-fit-sdk-21.141.0/tests/test_crc_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5565 2024-05-13 20:33:10.000000 garmin-fit-sdk-21.141.0/tests/test_bitstream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37792 2024-05-13 20:33:10.000000 garmin-fit-sdk-21.141.0/tests/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9022 2024-05-13 20:33:22.000000 garmin-fit-sdk-21.141.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-13 20:33:10.000000 garmin-fit-sdk-21.141.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:33:22.000000 garmin-fit-sdk-21.141.0/garmin_fit_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)     6791 2024-05-13 20:33:10.000000 garmin-fit-sdk-21.141.0/garmin_fit_sdk/stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3851 2024-05-13 20:33:10.000000 garmin-fit-sdk-21.141.0/garmin_fit_sdk/fit.py
+-rw-r--r--   0 runner    (1001) docker     (127)   772027 2024-05-13 20:33:10.000000 garmin-fit-sdk-21.141.0/garmin_fit_sdk/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-05-13 20:33:10.000000 garmin-fit-sdk-21.141.0/garmin_fit_sdk/accumulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-05-13 20:33:10.000000 garmin-fit-sdk-21.141.0/garmin_fit_sdk/crc_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32059 2024-05-13 20:33:10.000000 garmin-fit-sdk-21.141.0/garmin_fit_sdk/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-13 20:33:10.000000 garmin-fit-sdk-21.141.0/garmin_fit_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3341 2024-05-13 20:33:10.000000 garmin-fit-sdk-21.141.0/garmin_fit_sdk/bitstream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-05-13 20:33:10.000000 garmin-fit-sdk-21.141.0/garmin_fit_sdk/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6513 2024-05-13 20:33:10.000000 garmin-fit-sdk-21.141.0/garmin_fit_sdk/hr_mesg_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-13 20:33:22.000000 garmin-fit-sdk-21.141.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-13 20:33:10.000000 garmin-fit-sdk-21.141.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:33:22.000000 garmin-fit-sdk-21.141.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:33:22.000000 garmin-fit-sdk-21.141.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-13 20:33:10.000000 garmin-fit-sdk-21.141.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-13 20:33:10.000000 garmin-fit-sdk-21.141.0/.github/workflows/run_tests.yml
```

### Comparing `garmin-fit-sdk-21.133.0/README.md` & `garmin-fit-sdk-21.141.0/README.md`

 * *Files identical despite different names*

### Comparing `garmin-fit-sdk-21.133.0/PKG-INFO` & `garmin-fit-sdk-21.141.0/garmin_fit_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garmin-fit-sdk
-Version: 21.133.0
+Version: 21.141.0
 Summary: Garmin FIT Python SDK
 Home-page: https://github.com/garmin/fit-python-sdk
 Author: Garmin International, Inc.
 License: UNKNOWN
 Keywords: garmin,fit sdk,fit
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `garmin-fit-sdk-21.133.0/.github/workflows/run_tests.yml` & `garmin-fit-sdk-21.141.0/.github/workflows/run_tests.yml`

 * *Files identical despite different names*

### Comparing `garmin-fit-sdk-21.133.0/.github/workflows/publish.yml` & `garmin-fit-sdk-21.141.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `garmin-fit-sdk-21.133.0/setup.cfg` & `garmin-fit-sdk-21.141.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = garmin-fit-sdk
-version = 21.133.0
+version = 21.141.0
 author = Garmin International, Inc.
 url = https://github.com/garmin/fit-python-sdk
 description = Garmin FIT Python SDK
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = garmin, fit sdk, fit
 license_files = LICENSE.txt
```

### Comparing `garmin-fit-sdk-21.133.0/garmin_fit_sdk.egg-info/PKG-INFO` & `garmin-fit-sdk-21.141.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garmin-fit-sdk
-Version: 21.133.0
+Version: 21.141.0
 Summary: Garmin FIT Python SDK
 Home-page: https://github.com/garmin/fit-python-sdk
 Author: Garmin International, Inc.
 License: UNKNOWN
 Keywords: garmin,fit sdk,fit
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `garmin-fit-sdk-21.133.0/garmin_fit_sdk.egg-info/SOURCES.txt` & `garmin-fit-sdk-21.141.0/garmin_fit_sdk.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,13 @@
 tests/__init__.py
 tests/data.py
 tests/data_expand_hr_mesgs.py
 tests/test_accumulator.py
 tests/test_bitstream.py
 tests/test_crc_calculator.py
 tests/test_decoder.py
-tests/test_errors.py
 tests/test_hr_mesg_utils.py
 tests/test_stream.py
 tests/test_util.py
 tests/fits/ActivityDevFields.fit
 tests/fits/HrmPluginTestActivity.fit
 tests/fits/WithGearChangeData.fit
```

### Comparing `garmin-fit-sdk-21.133.0/tests/fits/ActivityDevFields.fit` & `garmin-fit-sdk-21.141.0/tests/fits/ActivityDevFields.fit`

 * *Files identical despite different names*

### Comparing `garmin-fit-sdk-21.133.0/tests/fits/WithGearChangeData.fit` & `garmin-fit-sdk-21.141.0/tests/fits/WithGearChangeData.fit`

 * *Files identical despite different names*

### Comparing `garmin-fit-sdk-21.133.0/tests/fits/HrmPluginTestActivity.fit` & `garmin-fit-sdk-21.141.0/tests/fits/HrmPluginTestActivity.fit`

 * *Files identical despite different names*

### Comparing `garmin-fit-sdk-21.133.0/tests/data.py` & `garmin-fit-sdk-21.141.0/tests/data.py`

 * *Files identical despite different names*

### Comparing `garmin-fit-sdk-21.133.0/tests/test_stream.py` & `garmin-fit-sdk-21.141.0/tests/test_stream.py`

 * *Files identical despite different names*

### Comparing `garmin-fit-sdk-21.133.0/tests/test_crc_calculator.py` & `garmin-fit-sdk-21.141.0/tests/test_crc_calculator.py`

 * *Files identical despite different names*

### Comparing `garmin-fit-sdk-21.133.0/tests/data_expand_hr_mesgs.py` & `garmin-fit-sdk-21.141.0/tests/data_expand_hr_mesgs.py`

 * *Files identical despite different names*

### Comparing `garmin-fit-sdk-21.133.0/tests/test_hr_mesg_utils.py` & `garmin-fit-sdk-21.141.0/tests/test_hr_mesg_utils.py`

 * *Files identical despite different names*

### Comparing `garmin-fit-sdk-21.133.0/tests/test_util.py` & `garmin-fit-sdk-21.141.0/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `garmin-fit-sdk-21.133.0/tests/test_bitstream.py` & `garmin-fit-sdk-21.141.0/tests/test_bitstream.py`

 * *Files identical despite different names*

### Comparing `garmin-fit-sdk-21.133.0/tests/test_decoder.py` & `garmin-fit-sdk-21.141.0/tests/test_decoder.py`

 * *Files identical despite different names*

### Comparing `garmin-fit-sdk-21.133.0/tests/test_accumulator.py` & `garmin-fit-sdk-21.141.0/tests/test_accumulator.py`

 * *Files identical despite different names*

### Comparing `garmin-fit-sdk-21.133.0/garmin_fit_sdk/profile.py` & `garmin-fit-sdk-21.141.0/garmin_fit_sdk/profile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 ###########################################################################################
 # Copyright 2024 Garmin International, Inc.
 # Licensed under the Flexible and Interoperable Data Transfer (FIT) Protocol License; you
 # may not use this file except in compliance with the Flexible and Interoperable Data
 # Transfer (FIT) Protocol License.
 ###########################################################################################
 # ****WARNING****  This file is auto-generated!  Do NOT edit this file.
-# Profile Version = 21.133.0Release
-# Tag = production/release/21.133.0-0-g6002091
+# Profile Version = 21.141.0Release
+# Tag = production/release/21.141.0-0-g2aa27e1
 ############################################################################################
 
 
 Profile = {
     'version': {
         'major': 21,
-        'minor': 133,
+        'minor': 141,
         'patch': 0,
         'type': "Release"
     },
     'common_fields': {
         'part_index': 250,
         'timestamp': 253,
         'message_index': 254
@@ -6481,14 +6481,42 @@
             'units': "Flow",
             'bits': [],
             'components': [],
             'is_accumulated': False,
             'has_components': False,
 			'sub_fields': []
             },
+        192: {
+            'num': 192, # A 0-100 scale representing how a user felt while performing a workout. Low values are considered feeling bad, while high values are good.
+            'name': "workout_feel",
+            'type': "uint8",
+            'array': "false",
+            'scale': [1],
+            'offset': [0],
+            'units': "",
+            'bits': [],
+            'components': [],
+            'is_accumulated': False,
+            'has_components': False,
+			'sub_fields': []
+            },
+        193: {
+            'num': 193, # Common Borg CR10 / 0-10 RPE scale, multiplied 10x.. Aggregate score for all workouts in a single session.
+            'name': "workout_rpe",
+            'type': "uint8",
+            'array': "false",
+            'scale': [1],
+            'offset': [0],
+            'units': "",
+            'bits': [],
+            'components': [],
+            'is_accumulated': False,
+            'has_components': False,
+			'sub_fields': []
+            },
         194: {
             'num': 194, # Average SPO2 for the monitoring session
             'name': "avg_spo2",
             'type': "uint8",
             'array': "false",
             'scale': [1],
             'offset': [0],
@@ -21477,14 +21505,91 @@
             'components': [],
             'is_accumulated': False,
             'has_components': False,
 			'sub_fields': []
             },
     },
 },
+        398: {
+        'num': "398",
+        'name': "skin_temp_overnight",
+        'messages_key': "skin_temp_overnight_mesgs",
+        'fields': {
+        253: {
+            'num': 253,
+            'name': "timestamp",
+            'type': "date_time",
+            'array': "false",
+            'scale': [1],
+            'offset': [0],
+            'units': "",
+            'bits': [],
+            'components': [],
+            'is_accumulated': False,
+            'has_components': False,
+			'sub_fields': []
+            },
+        0: {
+            'num': 0,
+            'name': "local_timestamp",
+            'type': "local_date_time",
+            'array': "false",
+            'scale': [1],
+            'offset': [0],
+            'units': "",
+            'bits': [],
+            'components': [],
+            'is_accumulated': False,
+            'has_components': False,
+			'sub_fields': []
+            },
+        1: {
+            'num': 1, # The average overnight deviation from baseline temperature in degrees C
+            'name': "average_deviation",
+            'type': "float32",
+            'array': "false",
+            'scale': [1],
+            'offset': [0],
+            'units': "",
+            'bits': [],
+            'components': [],
+            'is_accumulated': False,
+            'has_components': False,
+			'sub_fields': []
+            },
+        2: {
+            'num': 2, # The average 7 day overnight deviation from baseline temperature in degrees C
+            'name': "average_7_day_deviation",
+            'type': "float32",
+            'array': "false",
+            'scale': [1],
+            'offset': [0],
+            'units': "",
+            'bits': [],
+            'components': [],
+            'is_accumulated': False,
+            'has_components': False,
+			'sub_fields': []
+            },
+        4: {
+            'num': 4, # Final overnight temperature value
+            'name': "nightly_value",
+            'type': "float32",
+            'array': "false",
+            'scale': [1],
+            'offset': [0],
+            'units': "",
+            'bits': [],
+            'components': [],
+            'is_accumulated': False,
+            'has_components': False,
+			'sub_fields': []
+            },
+    },
+},
         105: {
         'num': "105",
         'name': "pad",
         'messages_key': "pad_mesgs",
         'fields': {
     },
 },
@@ -21627,14 +21732,15 @@
         '372': 'raw_bbi',
         '375': 'device_aux_battery_info',
         '376': 'hsa_gyroscope_data',
         '387': 'chrono_shot_session',
         '388': 'chrono_shot_data',
         '389': 'hsa_configuration_data',
         '393': 'dive_apnea_alarm',
+        '398': 'skin_temp_overnight',
         '409': 'hsa_wrist_temperature_data', # Message number for the HSA wrist temperature data message
         '0xFF00': 'mfg_range_min', # 0xFF00 - 0xFFFE reserved for manufacturer specific messages
         '0xFFFE': 'mfg_range_max', # 0xFF00 - 0xFFFE reserved for manufacturer specific messages
         },
     'checksum': {
         '0': 'clear', # Allows clear of checksum for flash memory where can only write 1 to 0 without erasing sector.
         '1': 'ok', # Set to mark checksum as valid if computes to invalid values 0 or 0xFF. Checksum can also be set to ok to save encoding computation time.
@@ -22672,14 +22778,15 @@
         '322': 'shanyue',
         '323': 'spinning_mda',
         '324': 'hilldating',
         '325': 'aero_sensor',
         '326': 'nike',
         '327': 'magicshine',
         '328': 'ictrainer',
+        '329': 'absolute_cycling',
         '5759': 'actigraphcorp',
         },
     'garmin_product': {
         '1': 'hrm1',
         '2': 'axh01', # AXH01 HRM chipset
         '3': 'axb01',
         '4': 'axb02',
@@ -23091,14 +23198,16 @@
         '4341': 'enduro2',
         '4374': 'fenix7s_pro_solar',
         '4375': 'fenix7_pro_solar',
         '4376': 'fenix7x_pro_solar',
         '4380': 'lily2',
         '4394': 'instinct_2x',
         '4426': 'vivoactive5',
+        '4432': 'fr165',
+        '4433': 'fr165_music',
         '4442': 'descent_t2',
         '4446': 'hrm_fit',
         '4472': 'marq_gen2_commander',
         '4556': 'd2_mach1_pro',
         '10007': 'sdm4', # SDM4 footpod
         '10014': 'edge_remote',
         '20533': 'tacx_training_app_win',
@@ -23505,16 +23614,20 @@
         '2': 'connections',
         '3': 'group',
         '4': 'challenger',
         '5': 'kom',
         '6': 'qom',
         '7': 'pr',
         '8': 'goal',
-        '9': 'rival',
+        '9': 'carrot',
         '10': 'club_leader',
+        '11': 'rival',
+        '12': 'last',
+        '13': 'recent_best',
+        '14': 'course_record',
         },
     'segment_delete_status': {
         '0': 'do_not_delete',
         '1': 'delete_one',
         '2': 'delete_all',
         },
     'segment_selection_type': {
@@ -25599,10 +25712,11 @@
         'RAW_BBI': 372,
         'RESPIRATION_RATE': 297,
         'CHRONO_SHOT_SESSION': 387,
         'CHRONO_SHOT_DATA': 388,
         'TANK_UPDATE': 319,
         'TANK_SUMMARY': 323,
         'SLEEP_ASSESSMENT': 346,
+        'SKIN_TEMP_OVERNIGHT': 398,
         'PAD': 105,
     }
 }
```

### Comparing `garmin-fit-sdk-21.133.0/garmin_fit_sdk/decoder.py` & `garmin-fit-sdk-21.141.0/garmin_fit_sdk/decoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 ###########################################################################################
 # Copyright 2024 Garmin International, Inc.
 # Licensed under the Flexible and Interoperable Data Transfer (FIT) Protocol License; you
 # may not use this file except in compliance with the Flexible and Interoperable Data
 # Transfer (FIT) Protocol License.
 ###########################################################################################
 # ****WARNING****  This file is auto-generated!  Do NOT edit this file.
-# Profile Version = 21.133.0Release
-# Tag = production/release/21.133.0-0-g6002091
+# Profile Version = 21.141.0Release
+# Tag = production/release/21.141.0-0-g2aa27e1
 ############################################################################################
 
 
 import copy
 
 from . import Accumulator, BitStream, CrcCalculator
 from . import fit as FIT
@@ -89,15 +89,15 @@
                 return False
 
             file_header = self.read_file_header()
 
             if file_header.header_size + file_header.data_size + _CRCSIZE > self._stream.get_length():
                 return False
 
-            if file_header.header_size is 14 and file_header.header_crc != CrcCalculator.calculate_crc(self._stream.slice(0, 12), 0, 12):
+            if file_header.header_size == 14 and file_header.header_crc != CrcCalculator.calculate_crc(self._stream.slice(0, 12), 0, 12):
                 return False
 
             file_crc = CrcCalculator.calculate_crc(self._stream.read_bytes(file_header.file_total_size),0, file_header.file_total_size)
             crc_from_file = self._stream.read_byte() + (self._stream.read_byte() << 8)
             if crc_from_file != file_crc:
                 return False
 
@@ -312,15 +312,15 @@
             self.__add_field_description_to_profile(message)
 
         else:
             message = self.__apply_profile(mesg_def, message)
 
         self.__clean_message(message)
 
-        if len(developer_fields) is not 0:
+        if len(developer_fields) != 0:
             message['developer_fields'] = developer_fields
 
         # Append decoded message
         self._messages[messages_key].append(message)
 
         if self._mesg_listener is not None:
             self._mesg_listener(mesg_def['global_mesg_num'], message)
@@ -697,15 +697,15 @@
                 self.protocol_version = stream.read_byte()
                 self.profile_version = stream.read_unint_16("little")
                 self.data_size = stream.read_unint_32("little")
                 self.data_type = stream.read_string(4)
                 self.header_crc = 0
                 self.file_total_size = self.header_size + self.data_size
 
-                if self.header_size is 14:
+                if self.header_size == 14:
                     self.header_crc = stream.read_unint_16("little")
 
             def get_dict(self):
                 dict = {}
                 dict["header_size"] = self.header_size
                 dict["protocol_version"] = (self.protocol_version >> 4) + ((self.protocol_version & 0x0F) / 10)
                 dict["profile_version"] = self.profile_version / 1000 if self.profile_version > 2199 else 100
```

### Comparing `garmin-fit-sdk-21.133.0/garmin_fit_sdk/util.py` & `garmin-fit-sdk-21.141.0/garmin_fit_sdk/util.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 ###########################################################################################
 # Copyright 2024 Garmin International, Inc.
 # Licensed under the Flexible and Interoperable Data Transfer (FIT) Protocol License; you
 # may not use this file except in compliance with the Flexible and Interoperable Data
 # Transfer (FIT) Protocol License.
 ###########################################################################################
 # ****WARNING****  This file is auto-generated!  Do NOT edit this file.
-# Profile Version = 21.133.0Release
-# Tag = production/release/21.133.0-0-g6002091
+# Profile Version = 21.141.0Release
+# Tag = production/release/21.141.0-0-g2aa27e1
 ############################################################################################
 
 
 from datetime import datetime, timezone
 
 FIT_EPOCH_S = 631065600
```

### Comparing `garmin-fit-sdk-21.133.0/garmin_fit_sdk/bitstream.py` & `garmin-fit-sdk-21.141.0/garmin_fit_sdk/bitstream.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 ###########################################################################################
 # Copyright 2024 Garmin International, Inc.
 # Licensed under the Flexible and Interoperable Data Transfer (FIT) Protocol License; you
 # may not use this file except in compliance with the Flexible and Interoperable Data
 # Transfer (FIT) Protocol License.
 ###########################################################################################
 # ****WARNING****  This file is auto-generated!  Do NOT edit this file.
-# Profile Version = 21.133.0Release
-# Tag = production/release/21.133.0-0-g6002091
+# Profile Version = 21.141.0Release
+# Tag = production/release/21.141.0-0-g2aa27e1
 ############################################################################################
 
 
 from . import fit as FIT
 
 
 class BitStream:
```

### Comparing `garmin-fit-sdk-21.133.0/garmin_fit_sdk/__init__.py` & `garmin-fit-sdk-21.141.0/garmin_fit_sdk/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 ###########################################################################################
 # Copyright 2024 Garmin International, Inc.
 # Licensed under the Flexible and Interoperable Data Transfer (FIT) Protocol License; you
 # may not use this file except in compliance with the Flexible and Interoperable Data
 # Transfer (FIT) Protocol License.
 ###########################################################################################
 # ****WARNING****  This file is auto-generated!  Do NOT edit this file.
-# Profile Version = 21.133.0Release
-# Tag = production/release/21.133.0-0-g6002091
+# Profile Version = 21.141.0Release
+# Tag = production/release/21.141.0-0-g2aa27e1
 ############################################################################################
 
 
 from garmin_fit_sdk.accumulator import Accumulator
 from garmin_fit_sdk.bitstream import BitStream
 from garmin_fit_sdk.crc_calculator import CrcCalculator
 from garmin_fit_sdk.decoder import Decoder
 from garmin_fit_sdk.fit import BASE_TYPE, BASE_TYPE_DEFINITIONS
 from garmin_fit_sdk.hr_mesg_utils import expand_heart_rates
 from garmin_fit_sdk.profile import Profile
 from garmin_fit_sdk.stream import Stream
 from garmin_fit_sdk.util import FIT_EPOCH_S, convert_timestamp_to_datetime
 
-__version__ = '21.133.0'
+__version__ = '21.141.0'
```

### Comparing `garmin-fit-sdk-21.133.0/garmin_fit_sdk/hr_mesg_utils.py` & `garmin-fit-sdk-21.141.0/garmin_fit_sdk/hr_mesg_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 ###########################################################################################
 # Copyright 2024 Garmin International, Inc.
 # Licensed under the Flexible and Interoperable Data Transfer (FIT) Protocol License; you
 # may not use this file except in compliance with the Flexible and Interoperable Data
 # Transfer (FIT) Protocol License.
 ###########################################################################################
 # ****WARNING****  This file is auto-generated!  Do NOT edit this file.
-# Profile Version = 21.133.0Release
-# Tag = production/release/21.133.0-0-g6002091
+# Profile Version = 21.141.0Release
+# Tag = production/release/21.141.0-0-g2aa27e1
 ############################################################################################
 
 
 from datetime import datetime
 
 from . import util
```

### Comparing `garmin-fit-sdk-21.133.0/garmin_fit_sdk/fit.py` & `garmin-fit-sdk-21.141.0/garmin_fit_sdk/fit.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 ###########################################################################################
 # Copyright 2024 Garmin International, Inc.
 # Licensed under the Flexible and Interoperable Data Transfer (FIT) Protocol License; you
 # may not use this file except in compliance with the Flexible and Interoperable Data
 # Transfer (FIT) Protocol License.
 ###########################################################################################
 # ****WARNING****  This file is auto-generated!  Do NOT edit this file.
-# Profile Version = 21.133.0Release
-# Tag = production/release/21.133.0-0-g6002091
+# Profile Version = 21.141.0Release
+# Tag = production/release/21.141.0-0-g2aa27e1
 ############################################################################################
 
 
 BASE_TYPE = {
     "ENUM": 0x00,
     "SINT8": 0x01,
     "UINT8": 0x02,
```

### Comparing `garmin-fit-sdk-21.133.0/garmin_fit_sdk/stream.py` & `garmin-fit-sdk-21.141.0/garmin_fit_sdk/stream.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 ###########################################################################################
 # Copyright 2024 Garmin International, Inc.
 # Licensed under the Flexible and Interoperable Data Transfer (FIT) Protocol License; you
 # may not use this file except in compliance with the Flexible and Interoperable Data
 # Transfer (FIT) Protocol License.
 ###########################################################################################
 # ****WARNING****  This file is auto-generated!  Do NOT edit this file.
-# Profile Version = 21.133.0Release
-# Tag = production/release/21.133.0-0-g6002091
+# Profile Version = 21.141.0Release
+# Tag = production/release/21.141.0-0-g2aa27e1
 ############################################################################################
 
 
 import os
 from enum import Enum
 from io import BufferedReader, BytesIO
 from struct import unpack
```

### Comparing `garmin-fit-sdk-21.133.0/garmin_fit_sdk/crc_calculator.py` & `garmin-fit-sdk-21.141.0/garmin_fit_sdk/crc_calculator.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 ###########################################################################################
 # Copyright 2024 Garmin International, Inc.
 # Licensed under the Flexible and Interoperable Data Transfer (FIT) Protocol License; you
 # may not use this file except in compliance with the Flexible and Interoperable Data
 # Transfer (FIT) Protocol License.
 ###########################################################################################
 # ****WARNING****  This file is auto-generated!  Do NOT edit this file.
-# Profile Version = 21.133.0Release
-# Tag = production/release/21.133.0-0-g6002091
+# Profile Version = 21.141.0Release
+# Tag = production/release/21.141.0-0-g2aa27e1
 ############################################################################################
 
 
 _CRC_TABLE = [
     0x0000, 0xCC01, 0xD801, 0x1400, 0xF001, 0x3C00, 0x2800, 0xE401,
     0xA001, 0x6C00, 0x7800, 0xB401, 0x5000, 0x9C01, 0x8801, 0x4400
 ]
```

### Comparing `garmin-fit-sdk-21.133.0/garmin_fit_sdk/accumulator.py` & `garmin-fit-sdk-21.141.0/garmin_fit_sdk/accumulator.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 ###########################################################################################
 # Copyright 2024 Garmin International, Inc.
 # Licensed under the Flexible and Interoperable Data Transfer (FIT) Protocol License; you
 # may not use this file except in compliance with the Flexible and Interoperable Data
 # Transfer (FIT) Protocol License.
 ###########################################################################################
 # ****WARNING****  This file is auto-generated!  Do NOT edit this file.
-# Profile Version = 21.133.0Release
-# Tag = production/release/21.133.0-0-g6002091
+# Profile Version = 21.141.0Release
+# Tag = production/release/21.141.0-0-g2aa27e1
 ############################################################################################
 
 
 class AccumulatedField:
     '''A class that accumulates a value for a particular field.
         Attributes:
             _accumulated_value: Resulting accumulated value
```

