# Comparing `tmp/rtisdev-2.13.0.tar.gz` & `tmp/rtisdev-2.14.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\woute\Projects\rtisdev\dist\.tmp-y9knme4e\rtisdev-2.13.0.tar", last modified: Tue Apr  9 07:01:55 2024, max compression
+gzip compressed data, was "C:\Users\woute\Projects\rtisdev\dist\.tmp-s19io4xe\rtisdev-2.14.0.tar", last modified: Mon May 13 14:54:29 2024, max compression
```

## Comparing `rtisdev-2.13.0.tar` & `rtisdev-2.14.0.tar`

### file list

```diff
@@ -1,58 +1,54 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 07:01:55.000000 rtisdev-2.13.0/
--rw-rw-rw-   0        0        0    21286 2024-04-04 14:00:40.000000 rtisdev-2.13.0/LICENSE
--rw-rw-rw-   0        0        0       52 2024-04-05 08:40:05.000000 rtisdev-2.13.0/MANIFEST.in
--rw-rw-rw-   0        0        0    34213 2024-04-09 07:01:55.000000 rtisdev-2.13.0/PKG-INFO
--rw-rw-rw-   0        0        0     8123 2024-04-05 08:00:27.000000 rtisdev-2.13.0/README.md
--rw-rw-rw-   0        0        0     1832 2024-04-09 07:00:17.000000 rtisdev-2.13.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-04-09 07:01:55.000000 rtisdev-2.13.0/rtisdev/
--rw-rw-rw-   0        0        0     7881 2024-04-05 08:47:07.000000 rtisdev-2.13.0/rtisdev/GenerateWiki.py
--rw-rw-rw-   0        0        0   223482 2024-04-09 07:00:17.000000 rtisdev-2.13.0/rtisdev/RTISDev.py
--rw-rw-rw-   0        0        0    11893 2024-04-05 08:18:48.000000 rtisdev-2.13.0/rtisdev/RTISGenerateSettings.py
--rw-rw-rw-   0        0        0     4457 2024-04-09 07:00:17.000000 rtisdev-2.13.0/rtisdev/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 07:01:55.000000 rtisdev-2.13.0/rtisdev/config/
-drwxrwxrwx   0        0        0        0 2024-04-09 07:01:55.000000 rtisdev-2.13.0/rtisdev/config/microphoneLayouts/
-drwxrwxrwx   0        0        0        0 2024-04-09 07:01:55.000000 rtisdev-2.13.0/rtisdev/config/microphoneLayouts/eRTIS_v2/
--rw-rw-rw-   0        0        0      700 2023-03-24 10:15:41.000000 rtisdev-2.13.0/rtisdev/config/microphoneLayouts/eRTIS_v2/mic_coordinates.mat
-drwxrwxrwx   0        0        0        0 2024-04-09 07:01:55.000000 rtisdev-2.13.0/rtisdev/config/microphoneLayouts/eRTIS_v2REC/
--rw-rw-rw-   0        0        0      281 2023-04-27 11:51:07.000000 rtisdev-2.13.0/rtisdev/config/microphoneLayouts/eRTIS_v2REC/mic_coordinates.mat
-drwxrwxrwx   0        0        0        0 2024-04-09 07:01:55.000000 rtisdev-2.13.0/rtisdev/config/microphoneLayouts/eRTIS_v3D1/
--rw-rw-rw-   0        0        0      699 2023-03-22 13:54:21.000000 rtisdev-2.13.0/rtisdev/config/microphoneLayouts/eRTIS_v3D1/mic_coordinates.mat
-drwxrwxrwx   0        0        0        0 2024-04-09 07:01:55.000000 rtisdev-2.13.0/rtisdev/config/microphoneLayouts/eRTIS_v3D1REC/
--rw-rw-rw-   0        0        0      266 2023-03-22 13:54:21.000000 rtisdev-2.13.0/rtisdev/config/microphoneLayouts/eRTIS_v3D1REC/mic_coordinates.mat
-drwxrwxrwx   0        0        0        0 2024-04-09 07:01:55.000000 rtisdev-2.13.0/rtisdev/config/microphoneLayouts/uRTIS_v1/
--rw-rw-rw-   0        0        0      259 2023-03-22 13:54:21.000000 rtisdev-2.13.0/rtisdev/config/microphoneLayouts/uRTIS_v1/mic_coordinates.mat
-drwxrwxrwx   0        0        0        0 2024-04-09 07:01:55.000000 rtisdev-2.13.0/rtisdev/config/microphoneLayouts/xRTIS_v1/
--rw-rw-rw-   0        0        0      318 2023-03-22 13:54:21.000000 rtisdev-2.13.0/rtisdev/config/microphoneLayouts/xRTIS_v1/mic_coordinates.mat
-drwxrwxrwx   0        0        0        0 2024-04-09 07:01:55.000000 rtisdev-2.13.0/rtisdev/config/premadeSettings/
-drwxrwxrwx   0        0        0        0 2024-04-09 07:01:55.000000 rtisdev-2.13.0/rtisdev/config/premadeSettings/processing/
--rw-rw-rw-   0        0        0      115 2023-03-22 13:54:21.000000 rtisdev-2.13.0/rtisdev/config/premadeSettings/processing/2D_5m_181.json
--rw-rw-rw-   0        0        0      114 2023-03-22 13:54:21.000000 rtisdev-2.13.0/rtisdev/config/premadeSettings/processing/2D_5m_91.json
--rw-rw-rw-   0        0        0      117 2023-03-22 13:54:21.000000 rtisdev-2.13.0/rtisdev/config/premadeSettings/processing/3D_10m_3000.json
--rw-rw-rw-   0        0        0      116 2023-03-22 13:54:21.000000 rtisdev-2.13.0/rtisdev/config/premadeSettings/processing/3D_5m_1000.json
--rw-rw-rw-   0        0        0      116 2023-03-22 13:54:21.000000 rtisdev-2.13.0/rtisdev/config/premadeSettings/processing/3D_5m_3000.json
--rw-rw-rw-   0        0        0      116 2023-03-22 13:54:21.000000 rtisdev-2.13.0/rtisdev/config/premadeSettings/processing/3D_5m_4000.json
--rw-rw-rw-   0        0        0      115 2023-03-22 13:54:21.000000 rtisdev-2.13.0/rtisdev/config/premadeSettings/processing/3D_5m_500.json
--rw-rw-rw-   0        0        0      182 2023-03-22 13:54:21.000000 rtisdev-2.13.0/rtisdev/config/premadeSettings/processing/custom_example_2D_5m_91.json
--rw-rw-rw-   0        0        0     8056 2023-03-22 13:54:21.000000 rtisdev-2.13.0/rtisdev/config/premadeSettings/processing/delaymatrix.csv
--rw-rw-rw-   0        0        0     1992 2023-03-22 13:54:21.000000 rtisdev-2.13.0/rtisdev/config/premadeSettings/processing/directions.csv
--rw-rw-rw-   0        0        0     8277 2023-03-22 13:54:21.000000 rtisdev-2.13.0/rtisdev/config/premadeSettings/processing/ranges.csv
-drwxrwxrwx   0        0        0        0 2024-04-09 07:01:55.000000 rtisdev-2.13.0/rtisdev/config/premadeSettings/recording/
--rw-rw-rw-   0        0        0      231 2023-03-22 13:54:21.000000 rtisdev-2.13.0/rtisdev/config/premadeSettings/recording/default_20_80.json
--rw-rw-rw-   0        0        0      231 2023-03-22 13:54:21.000000 rtisdev-2.13.0/rtisdev/config/premadeSettings/recording/default_25_50.json
--rw-rw-rw-   0        0        0    29236 2023-03-22 13:54:21.000000 rtisdev-2.13.0/rtisdev/config/premadeSettings/recording/flutter.csv
--rw-rw-rw-   0        0        0      180 2023-03-22 13:54:21.000000 rtisdev-2.13.0/rtisdev/config/premadeSettings/recording/flutter.json
--rw-rw-rw-   0        0        0      231 2023-03-22 13:54:21.000000 rtisdev-2.13.0/rtisdev/config/premadeSettings/recording/long_20_80.json
--rw-rw-rw-   0        0        0      231 2023-03-22 13:54:21.000000 rtisdev-2.13.0/rtisdev/config/premadeSettings/recording/long_25_50.json
--rw-rw-rw-   0        0        0      230 2023-03-22 13:54:21.000000 rtisdev-2.13.0/rtisdev/config/premadeSettings/recording/short_20_80.json
--rw-rw-rw-   0        0        0      230 2023-03-22 13:54:21.000000 rtisdev-2.13.0/rtisdev/config/premadeSettings/recording/short_25_50.json
--rw-rw-rw-   0        0        0   655360 2023-03-22 13:54:21.000000 rtisdev-2.13.0/rtisdev/simulate.bin
-drwxrwxrwx   0        0        0        0 2024-04-09 07:01:55.000000 rtisdev-2.13.0/rtisdev.egg-info/
--rw-rw-rw-   0        0        0    34213 2024-04-09 07:01:54.000000 rtisdev-2.13.0/rtisdev.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3536 2024-04-09 07:01:54.000000 rtisdev-2.13.0/rtisdev.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 07:01:54.000000 rtisdev-2.13.0/rtisdev.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2024-04-09 07:01:54.000000 rtisdev-2.13.0/rtisdev.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-04-09 07:01:54.000000 rtisdev-2.13.0/rtisdev.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-09 07:01:55.000000 rtisdev-2.13.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-09 07:01:55.000000 rtisdev-2.13.0/tests/
--rw-rw-rw-   0        0        0        0 2023-03-22 13:54:21.000000 rtisdev-2.13.0/tests/__init__.py
--rw-rw-rw-   0        0        0    22523 2024-04-05 08:26:25.000000 rtisdev-2.13.0/tests/test_rtisdev.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:54:29.000000 rtisdev-2.14.0/
+-rw-rw-rw-   0        0        0    21286 2024-04-04 14:00:40.000000 rtisdev-2.14.0/LICENSE
+-rw-rw-rw-   0        0        0       52 2024-04-05 08:40:05.000000 rtisdev-2.14.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    34213 2024-05-13 14:54:29.000000 rtisdev-2.14.0/PKG-INFO
+-rw-rw-rw-   0        0        0     8123 2024-04-05 08:00:27.000000 rtisdev-2.14.0/README.md
+-rw-rw-rw-   0        0        0     1832 2024-05-13 14:42:14.000000 rtisdev-2.14.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-05-13 14:54:29.000000 rtisdev-2.14.0/rtisdev/
+-rw-rw-rw-   0        0        0   224997 2024-05-13 14:42:14.000000 rtisdev-2.14.0/rtisdev/RTISDev.py
+-rw-rw-rw-   0        0        0    11927 2024-05-13 14:33:14.000000 rtisdev-2.14.0/rtisdev/RTISGenerateSettings.py
+-rw-rw-rw-   0        0        0     4457 2024-05-13 14:42:14.000000 rtisdev-2.14.0/rtisdev/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:54:29.000000 rtisdev-2.14.0/rtisdev/config/
+drwxrwxrwx   0        0        0        0 2024-05-13 14:54:29.000000 rtisdev-2.14.0/rtisdev/config/microphoneLayouts/
+drwxrwxrwx   0        0        0        0 2024-05-13 14:54:29.000000 rtisdev-2.14.0/rtisdev/config/microphoneLayouts/eRTIS_v2/
+-rw-rw-rw-   0        0        0      700 2023-03-24 10:15:41.000000 rtisdev-2.14.0/rtisdev/config/microphoneLayouts/eRTIS_v2/mic_coordinates.mat
+drwxrwxrwx   0        0        0        0 2024-05-13 14:54:29.000000 rtisdev-2.14.0/rtisdev/config/microphoneLayouts/eRTIS_v2REC/
+-rw-rw-rw-   0        0        0      281 2023-04-27 11:51:07.000000 rtisdev-2.14.0/rtisdev/config/microphoneLayouts/eRTIS_v2REC/mic_coordinates.mat
+drwxrwxrwx   0        0        0        0 2024-05-13 14:54:29.000000 rtisdev-2.14.0/rtisdev/config/microphoneLayouts/eRTIS_v3D1/
+-rw-rw-rw-   0        0        0      699 2023-03-22 13:54:21.000000 rtisdev-2.14.0/rtisdev/config/microphoneLayouts/eRTIS_v3D1/mic_coordinates.mat
+drwxrwxrwx   0        0        0        0 2024-05-13 14:54:29.000000 rtisdev-2.14.0/rtisdev/config/microphoneLayouts/eRTIS_v3D1REC/
+-rw-rw-rw-   0        0        0      266 2023-03-22 13:54:21.000000 rtisdev-2.14.0/rtisdev/config/microphoneLayouts/eRTIS_v3D1REC/mic_coordinates.mat
+drwxrwxrwx   0        0        0        0 2024-05-13 14:54:29.000000 rtisdev-2.14.0/rtisdev/config/microphoneLayouts/uRTIS_v1/
+-rw-rw-rw-   0        0        0      259 2023-03-22 13:54:21.000000 rtisdev-2.14.0/rtisdev/config/microphoneLayouts/uRTIS_v1/mic_coordinates.mat
+drwxrwxrwx   0        0        0        0 2024-05-13 14:54:29.000000 rtisdev-2.14.0/rtisdev/config/microphoneLayouts/xRTIS_v1/
+-rw-rw-rw-   0        0        0      318 2023-03-22 13:54:21.000000 rtisdev-2.14.0/rtisdev/config/microphoneLayouts/xRTIS_v1/mic_coordinates.mat
+drwxrwxrwx   0        0        0        0 2024-05-13 14:54:29.000000 rtisdev-2.14.0/rtisdev/config/premadeSettings/
+drwxrwxrwx   0        0        0        0 2024-05-13 14:54:29.000000 rtisdev-2.14.0/rtisdev/config/premadeSettings/processing/
+-rw-rw-rw-   0        0        0      115 2023-03-22 13:54:21.000000 rtisdev-2.14.0/rtisdev/config/premadeSettings/processing/2D_5m_181.json
+-rw-rw-rw-   0        0        0      114 2023-03-22 13:54:21.000000 rtisdev-2.14.0/rtisdev/config/premadeSettings/processing/2D_5m_91.json
+-rw-rw-rw-   0        0        0      117 2023-03-22 13:54:21.000000 rtisdev-2.14.0/rtisdev/config/premadeSettings/processing/3D_10m_3000.json
+-rw-rw-rw-   0        0        0      116 2023-03-22 13:54:21.000000 rtisdev-2.14.0/rtisdev/config/premadeSettings/processing/3D_5m_1000.json
+-rw-rw-rw-   0        0        0      116 2023-03-22 13:54:21.000000 rtisdev-2.14.0/rtisdev/config/premadeSettings/processing/3D_5m_3000.json
+-rw-rw-rw-   0        0        0      116 2023-03-22 13:54:21.000000 rtisdev-2.14.0/rtisdev/config/premadeSettings/processing/3D_5m_4000.json
+-rw-rw-rw-   0        0        0      115 2023-03-22 13:54:21.000000 rtisdev-2.14.0/rtisdev/config/premadeSettings/processing/3D_5m_500.json
+-rw-rw-rw-   0        0        0      182 2023-03-22 13:54:21.000000 rtisdev-2.14.0/rtisdev/config/premadeSettings/processing/custom_example_2D_5m_91.json
+-rw-rw-rw-   0        0        0     8056 2023-03-22 13:54:21.000000 rtisdev-2.14.0/rtisdev/config/premadeSettings/processing/delaymatrix.csv
+-rw-rw-rw-   0        0        0     1992 2023-03-22 13:54:21.000000 rtisdev-2.14.0/rtisdev/config/premadeSettings/processing/directions.csv
+-rw-rw-rw-   0        0        0     8277 2023-03-22 13:54:21.000000 rtisdev-2.14.0/rtisdev/config/premadeSettings/processing/ranges.csv
+drwxrwxrwx   0        0        0        0 2024-05-13 14:54:29.000000 rtisdev-2.14.0/rtisdev/config/premadeSettings/recording/
+-rw-rw-rw-   0        0        0      231 2023-03-22 13:54:21.000000 rtisdev-2.14.0/rtisdev/config/premadeSettings/recording/default_20_80.json
+-rw-rw-rw-   0        0        0      231 2023-03-22 13:54:21.000000 rtisdev-2.14.0/rtisdev/config/premadeSettings/recording/default_25_50.json
+-rw-rw-rw-   0        0        0    29236 2023-03-22 13:54:21.000000 rtisdev-2.14.0/rtisdev/config/premadeSettings/recording/flutter.csv
+-rw-rw-rw-   0        0        0      180 2023-03-22 13:54:21.000000 rtisdev-2.14.0/rtisdev/config/premadeSettings/recording/flutter.json
+-rw-rw-rw-   0        0        0      231 2023-03-22 13:54:21.000000 rtisdev-2.14.0/rtisdev/config/premadeSettings/recording/long_20_80.json
+-rw-rw-rw-   0        0        0      231 2023-03-22 13:54:21.000000 rtisdev-2.14.0/rtisdev/config/premadeSettings/recording/long_25_50.json
+-rw-rw-rw-   0        0        0      230 2023-03-22 13:54:21.000000 rtisdev-2.14.0/rtisdev/config/premadeSettings/recording/short_20_80.json
+-rw-rw-rw-   0        0        0      230 2023-03-22 13:54:21.000000 rtisdev-2.14.0/rtisdev/config/premadeSettings/recording/short_25_50.json
+-rw-rw-rw-   0        0        0   655360 2023-03-22 13:54:21.000000 rtisdev-2.14.0/rtisdev/simulate.bin
+drwxrwxrwx   0        0        0        0 2024-05-13 14:54:29.000000 rtisdev-2.14.0/rtisdev.egg-info/
+-rw-rw-rw-   0        0        0    34213 2024-05-13 14:54:29.000000 rtisdev-2.14.0/rtisdev.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3402 2024-05-13 14:54:29.000000 rtisdev-2.14.0/rtisdev.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 14:54:29.000000 rtisdev-2.14.0/rtisdev.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2024-05-13 14:54:29.000000 rtisdev-2.14.0/rtisdev.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-13 14:54:29.000000 rtisdev-2.14.0/rtisdev.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 14:54:29.000000 rtisdev-2.14.0/setup.cfg
```

### Comparing `rtisdev-2.13.0/LICENSE` & `rtisdev-2.14.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rtisdev-2.13.0/PKG-INFO` & `rtisdev-2.14.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rtisdev
-Version: 2.13.0
+Version: 2.14.0
 Summary: Python module to make it easy to code with RTIS devices
 Author-email: Wouter Jansen <wouter.jansen@uantwerpen.be>, Arne Aerts <arne.aerts@uantwerpen.be>, Dennis Laurijssen <dennis.laurijssen@uantwerpen.be>, Jan Steckel <jan.steckel@uantwerpen.be>
 Maintainer-email: Wouter Jansen <wouter.jansen@uantwerpen.be>
 License: Attribution-NonCommercial-ShareAlike 4.0 International
         
         =======================================================================
```

### Comparing `rtisdev-2.13.0/README.md` & `rtisdev-2.14.0/README.md`

 * *Files identical despite different names*

### Comparing `rtisdev-2.13.0/pyproject.toml` & `rtisdev-2.14.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rtisdev"
-version = "2.13.0"
+version = "2.14.0"
 description = "Python module to make it easy to code with RTIS devices"
 readme = {file = "README.md", content-type = "text/markdown"}
 authors = [{ name = "Wouter Jansen", email = "wouter.jansen@uantwerpen.be" },
            { name = "Arne Aerts", email = "arne.aerts@uantwerpen.be"},
            { name = "Dennis Laurijssen", email = "dennis.laurijssen@uantwerpen.be"},
            { name = "Jan Steckel", email = "jan.steckel@uantwerpen.be"}]
 maintainers = [{name = "Wouter Jansen", email = "wouter.jansen@uantwerpen.be"}]
```

### Comparing `rtisdev-2.13.0/rtisdev/RTISDev.py` & `rtisdev-2.14.0/rtisdev/RTISDev.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,15 +143,15 @@
 SETTINGS = {}
 WORKERS = []
 CUDA_USED = False
 PACKAGE_DIRECTORY = os.path.dirname(os.path.abspath(__file__))
 BEHAVIOUR = False
 AMPLIFIER_ACTIVE = False
 DEBUG_COUNTER = 0
-VERSION = "v2.13.0"
+VERSION = "v2.14.0"
 CURRENT_RECORDING_CONFIG = ""
 
 
 class CustomFormatter(logging.Formatter):
     grey = "\x1b[38m"
     green = "\x1b[32m"
     yellow = "\x1b[33m"
@@ -2175,15 +2175,15 @@
     if containsError:
         logger.warning(errorString + "The config name has been altered to '" + configName + "'.")
     return configName
 
 
 def __generate_valid_processing_settings(packageDirectory, microphoneLayout, mode, directions, minRange, maxRange,
                                          esSubFactor, microphoneSampleFrequency, azimuthLowLimit, azimuthHighLimit,
-                                         elevationLowLimit, elevationHighLimit):
+                                         elevationLowLimit, elevationHighLimit, elevation2DAngle):
     """The internal function to generate valid processing settings like delay, range and direction matrices.
 
        Parameters
        ----------
        packageDirectory : String
            The location of the RTIS Dev package to correctly find the microphone setting files.
 
@@ -2219,14 +2219,17 @@
 
        elevationLowLimit : float
            The lower limit of the elevation in degrees of the directions to generate. Has to be between -90 and 90.
 
        elevationHighLimit : float
            The higher limit of the elevation in degrees of the directions to generate. Has to be between -90 and 90.
 
+       elevation2DAngle : float (default = 0)
+           The angle in degrees of the elevation in the 2D mode generation. Has to be between -90 and 90.
+
        Returns
        -------
        delayMatrix : Numpy ndarray
            The array holding the delay matrix used for beamforming. (shape: nMicrophones x nDirections)
 
        directions : Numpy ndarray
            The array holding the directions in radians used of the energyscape.
@@ -2284,27 +2287,34 @@
 
     if elevationHighLimit < -90 or elevationHighLimit > 90:
         logger.error("Could not set the higher elevation direction limit to " + str(elevationHighLimit)
                      + " degrees : It has to be between -90 degrees and 90 degrees.")
         raise ValueError("Could not set the higher elevation direction limit to " + str(elevationHighLimit)
                          + " degrees : It has to be between -90 degrees and 90 degrees.")
 
+    if elevation2DAngle < -90 or elevation2DAngle > 90:
+        logger.error("Could not set the 2D mode elevation angle to " + str(elevation2DAngle)
+                     + " degrees : It has to be between -90 degrees and 90 degrees.")
+        raise ValueError("Could not set 2D mode elevation angle to " + str(elevation2DAngle)
+                         + " degrees : It has to be between -90 degrees and 90 degrees.")
+
     try:
         scipy.io.loadmat(packageDirectory + "/config/microphoneLayouts/" + microphoneLayout + "/mic_coordinates.mat")
     except FileNotFoundError:
         logger.error("Could not find the microphone layout file for " + microphoneLayout
                      + ". Use get_microphone_layout_list() to get a list of available microphone layouts.")
         raise FileNotFoundError("Could not find the microphone layout file for " + microphoneLayout
                                 + ". Use get_microphone_layout_list() to get a list of available microphone layouts.")
 
     delaymatrix, directions, ranges = generate_processing_settings(packageDirectory, microphoneLayout,
                                                                    mode, directions, minRange, maxRange,
                                                                    esSubFactor, microphoneSampleFrequency,
                                                                    azimuthLowLimit, azimuthHighLimit,
-                                                                   elevationLowLimit, elevationHighLimit)
+                                                                   elevationLowLimit, elevationHighLimit,
+                                                                   elevation2DAngle)
     return delaymatrix, directions, ranges
 
 
 def __return_and_verify_all_settings(sigADC, sigDAC, microphoneSampleFrequency, callSampleFrequency,
                                      microphoneSamples, callDuration, callMinimumFrequency,
                                      callMaximumFrequency, callEmissions, delayMatrix, directions, ranges, preFilter,
                                      postFilter, meanEnergyRangeMultiplier, maxEnergyRangeThresholdMultiplier,
@@ -2869,14 +2879,15 @@
         maxRange = 5
         directions = 181
         mode = 1
         azimuthLowLimit = -90
         azimuthHighLimit = 90
         elevationLowLimit = -90
         elevationHighLimit = 90
+        elevation2DAngle = 0
         if 'minRange' in processingConfig.keys():
             minRange = processingConfig["minRange"]
         if 'maxRange' in processingConfig.keys():
             maxRange = processingConfig["maxRange"]
         if 'directions' in processingConfig.keys():
             directions = processingConfig["directions"]
         if '2D' in processingConfig.keys():
@@ -2885,20 +2896,23 @@
             azimuthLowLimit = processingConfig["azimuthLowLimit"]
         if 'azimuthHighLimit' in processingConfig.keys():
             azimuthHighLimit = processingConfig["azimuthHighLimit"]
         if 'elevationLowLimit' in processingConfig.keys():
             elevationLowLimit = processingConfig["elevationLowLimit"]
         if 'elevationHighLimit' in processingConfig.keys():
             elevationHighLimit = processingConfig["elevationHighLimit"]
+        if 'elevation2DAngle' in processingConfig.keys():
+            elevation2DAngle = processingConfig["elevation2DAngle"]
 
         delaymatrix, directions, ranges = __generate_valid_processing_settings(PACKAGE_DIRECTORY, microphoneLayout,
                                                                                mode, directions, minRange, maxRange,
                                                                                10, microphoneSampleFrequency,
                                                                                azimuthLowLimit, azimuthHighLimit,
-                                                                               elevationLowLimit, elevationHighLimit)
+                                                                               elevationLowLimit, elevationHighLimit,
+                                                                               elevation2DAngle)
 
     return delaymatrix, directions, ranges, microphoneLayout, disableList
 
 
 ##############################
 # RTIS Dev Public Functions #
 ##############################
@@ -3222,15 +3236,15 @@
                                     "Please make sure to use correct path and filename.")
 
 
 def set_processing_settings(configName: str, premade: str = None, jsonPath: str = None, customPath: str = None,
                             microphoneLayout: str = "eRTIS_v3D1", mode: int = 1, directions: int = 181,
                             azimuthLowLimit : float = -90, azimuthHighLimit : float = 90,
                             elevationLowLimit : float = -90, elevationHighLimit : float = 90,
-                            minRange: float = 0.5, maxRange: float = 5,
+                            elevation2DAngle : float =0, minRange: float = 0.5, maxRange: float = 5,
                             pdmEnable: bool = True, preFilterEnable: bool = False, matchedFilterEnable: bool = True,
                             beamformingEnable: bool = True, postFilterEnable: bool = False,
                             enveloppeEnable: bool = True, cleanEnable: bool = True, preloadToggle: bool = True,
                             preFilter: np.ndarray = None, postFilter: np.ndarray = None,
                             meanEnergyRangeMultiplier: float = 2,
                             maxEnergyRangeThresholdMultiplier: float = 0.5) -> bool:
     """Set the processing settings. All parameters are optional and most have default values.
@@ -3273,14 +3287,17 @@
 
        elevationLowLimit : float (default = -90)
            The lower limit of the elevation in degrees of the directions to generate. Has to be between -90 and 90.
 
        elevationHighLimit : float (default = 90)
            The higher limit of the elevation in degrees of the directions to generate. Has to be between -90 and 90.
 
+       elevation2DAngle : float (default = 0)
+           The angle in degrees of the elevation in the 2D mode generation. Has to be between -90 and 90.
+
        minRange : float (default = 0.5)
            The minimum distance in meters of the energyscape to generate.
 
        maxRange : float (default = 5)
            The maximum distance in meters of the energyscape to generate.
 
        pdmEnable : bool (default = True)
@@ -3443,15 +3460,16 @@
             microphoneSampleFrequency = SETTINGS[configName].microphoneSampleFrequency
 
             delaymatrix, directions, ranges = __generate_valid_processing_settings(PACKAGE_DIRECTORY, microphoneLayout,
                                                                                    mode, directions, minRange, maxRange,
                                                                                    10, microphoneSampleFrequency,
                                                                                    azimuthLowLimit, azimuthHighLimit,
                                                                                    elevationLowLimit,
-                                                                                   elevationHighLimit)
+                                                                                   elevationHighLimit,
+                                                                                   elevation2DAngle)
 
             disableList = get_disabled_microphone_list(PACKAGE_DIRECTORY, microphoneLayout)
 
             return __set_and_verify_processing_settings(delaymatrix, directions, ranges, postFilter, preFilter,
                                                         meanEnergyRangeMultiplier, maxEnergyRangeThresholdMultiplier,
                                                         pdmEnable, preFilterEnable, matchedFilterEnable,
                                                         beamformingEnable, postFilterEnable,
@@ -3591,15 +3609,15 @@
 def get_settings(recordingPremade: str = None, recordingJsonPath: str = None, recordingCallCustom: str = None,
                  processingPremade: str = None, processingJsonPath: str = None, processingCustomPath: str = None,
                  microphoneSamples: int = 163840, microphoneSampleFrequency: int = 4500000,
                  callSampleFrequency: int = 450000, callDuration: float = 2.5, callMinimumFrequency: int = 25000,
                  callMaximumFrequency: int = 50000, callEmissions: int = 1,
                  microphoneLayout: str = "eRTIS_v3D1", mode: int = 1, directions: int = 181,
                  azimuthLowLimit: float = -90, azimuthHighLimit: float = 90,
-                 elevationLowLimit: float = -90, elevationHighLimit: float = 90,
+                 elevationLowLimit: float = -90, elevationHighLimit: float = 90, elevation2DAngle: float = 0,
                  minRange: float = 0.5, maxRange: float = 5, pdmEnable: bool = True, preFilterEnable: bool = False,
                  matchedFilterEnable: bool = True, beamformingEnable: bool = True, postFilterEnable: bool = False,
                  enveloppeEnable: bool = True, cleanEnable: bool = True, preloadToggle: bool = True,
                  preFilter: np.ndarray = None, postFilter: np.ndarray = None,
                  meanEnergyRangeMultiplier: float = 2, maxEnergyRangeThresholdMultiplier: float = 0.5,
                  configName: str = "") -> RTISSettings:
     """Returns an `RTISSettings` object with all chosen recording and processing settings based on the
@@ -3674,14 +3692,17 @@
 
        elevationLowLimit : float (default = -90)
            The lower limit of the elevation in degrees of the directions to generate. Has to be between -90 and 90.
 
        elevationHighLimit : float (default = 90)
            The higher limit of the elevation in degrees of the directions to generate. Has to be between -90 and 90.
 
+       elevation2DAngle : float (default = 0)
+           The angle in degrees of the elevation in the 2D mode generation. Has to be between -90 and 90.
+
        minRange : float (default = 0.5)
            The minimum distance in meters of the energyscape to generate.
 
        maxRange : float (default = 5)
            The maximum distance in meters of the energyscape to generate.
 
        pdmEnable : bool (default = True)
@@ -3789,15 +3810,16 @@
                                         "Please make sure to use correct path and filenames.")
         else:
             delaymatrix, directions, ranges = __generate_valid_processing_settings(PACKAGE_DIRECTORY, microphoneLayout,
                                                                                    mode, directions, minRange, maxRange,
                                                                                    10, microphoneSampleFrequency,
                                                                                    azimuthLowLimit, azimuthHighLimit,
                                                                                    elevationLowLimit,
-                                                                                   elevationHighLimit)
+                                                                                   elevationHighLimit,
+                                                                                   elevation2DAngle)
 
     elif processingPremade and processingJsonPath:
         raise RTISPremadeAndJsonSettingsError
     elif processingPremade:
         if os.path.isfile(PACKAGE_DIRECTORY + '/config/premadeSettings/processing/'
                           + processingPremade + '.json'):
             with open(PACKAGE_DIRECTORY + '/config/premadeSettings/processing/'
```

### Comparing `rtisdev-2.13.0/rtisdev/RTISGenerateSettings.py` & `rtisdev-2.14.0/rtisdev/RTISGenerateSettings.py`

 * *Files 2% similar despite different names*

```diff
@@ -251,15 +251,15 @@
 
     return disableList
 
 
 def generate_processing_settings(package_directory, mLayoutName="eRTIS_v3D1", mode=1,
                                  directions=181, rMin=0.5, rMax=5, esSubFactor=10, adcFs=4500000,
                                  azimuthLowLimit=-90, azimuthHighLimit=90,
-                                 elevationLowLimit=-90, elevationHighLimit=90):
+                                 elevationLowLimit=-90, elevationHighLimit=90, elevation2DAngle=0):
     mat = scipy.io.loadmat(package_directory + "/config/microphoneLayouts/"
                            + mLayoutName + "/mic_coordinates.mat")
     micCoordsFinal = mat["mic_pos_final_pos"]
     micCoordsFinal = np.divide(micCoordsFinal, 1000)
     micCoordinates = np.concatenate((micCoordsFinal,
                                     np.zeros((micCoordsFinal.shape[0], 1), dtype=np.float64)), axis=1)
     micCoordinates[:, 0] = micCoordinates[:, 0] - np.nanmean(micCoordinates[:, 0])
@@ -268,15 +268,15 @@
 
     adcFs = adcFs / 10
 
     if mode == 1:
         # 2D
         step = (azimuthHighLimit - azimuthLowLimit) / (directions - 1)
         azVecAzEl = np.arange(azimuthLowLimit, azimuthHighLimit + step, step)
-        elVecAzEl = np.zeros((azVecAzEl.size,))
+        elVecAzEl = np.full(azVecAzEl.size, elevation2DAngle)
     else:
         # 3D
         surfacePart = (np.deg2rad(azimuthHighLimit) - np.deg2rad(azimuthLowLimit)) * (
                        np.sin(np.deg2rad(elevationHighLimit)) - np.sin(np.deg2rad(elevationLowLimit)))
         scaler = 4 * np.pi / surfacePart
         nEqPts = np.round(directions * scaler).astype(int)
         pointsPolar = eq_point_set_polar(2, nEqPts)
```

### Comparing `rtisdev-2.13.0/rtisdev/__init__.py` & `rtisdev-2.14.0/rtisdev/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,8 +96,8 @@
     ...             axs[microphone_index_i, microphone_index_j].set_xlabel("Time (Samples)")
     ...         if microphone_index_j == 0:
     ...             axs[microphone_index_i, microphone_index_j].set_ylabel("Amplitude")
     >>> plt.show()
     >>> fig.suptitle("RTIS Dev - Microphone Signals")
 """
 from .RTISDev import *
-__version__ = "2.13.0"
+__version__ = "2.14.0"
```

### Comparing `rtisdev-2.13.0/rtisdev/config/microphoneLayouts/eRTIS_v2/mic_coordinates.mat` & `rtisdev-2.14.0/rtisdev/config/microphoneLayouts/eRTIS_v2/mic_coordinates.mat`

 * *Files identical despite different names*

### Comparing `rtisdev-2.13.0/rtisdev/config/microphoneLayouts/eRTIS_v3D1/mic_coordinates.mat` & `rtisdev-2.14.0/rtisdev/config/microphoneLayouts/eRTIS_v3D1/mic_coordinates.mat`

 * *Files identical despite different names*

### Comparing `rtisdev-2.13.0/rtisdev/config/premadeSettings/processing/delaymatrix.csv` & `rtisdev-2.14.0/rtisdev/config/premadeSettings/processing/delaymatrix.csv`

 * *Files identical despite different names*

### Comparing `rtisdev-2.13.0/rtisdev/config/premadeSettings/processing/directions.csv` & `rtisdev-2.14.0/rtisdev/config/premadeSettings/processing/directions.csv`

 * *Files identical despite different names*

### Comparing `rtisdev-2.13.0/rtisdev/config/premadeSettings/processing/ranges.csv` & `rtisdev-2.14.0/rtisdev/config/premadeSettings/processing/ranges.csv`

 * *Files identical despite different names*

### Comparing `rtisdev-2.13.0/rtisdev/config/premadeSettings/recording/flutter.csv` & `rtisdev-2.14.0/rtisdev/config/premadeSettings/recording/flutter.csv`

 * *Files identical despite different names*

### Comparing `rtisdev-2.13.0/rtisdev/simulate.bin` & `rtisdev-2.14.0/rtisdev/simulate.bin`

 * *Files identical despite different names*

### Comparing `rtisdev-2.13.0/rtisdev.egg-info/PKG-INFO` & `rtisdev-2.14.0/rtisdev.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rtisdev
-Version: 2.13.0
+Version: 2.14.0
 Summary: Python module to make it easy to code with RTIS devices
 Author-email: Wouter Jansen <wouter.jansen@uantwerpen.be>, Arne Aerts <arne.aerts@uantwerpen.be>, Dennis Laurijssen <dennis.laurijssen@uantwerpen.be>, Jan Steckel <jan.steckel@uantwerpen.be>
 Maintainer-email: Wouter Jansen <wouter.jansen@uantwerpen.be>
 License: Attribution-NonCommercial-ShareAlike 4.0 International
         
         =======================================================================
```

### Comparing `rtisdev-2.13.0/rtisdev.egg-info/SOURCES.txt` & `rtisdev-2.14.0/rtisdev.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
-./rtisdev/GenerateWiki.py
 ./rtisdev/RTISDev.py
 ./rtisdev/RTISGenerateSettings.py
 ./rtisdev/__init__.py
 ./rtisdev/simulate.bin
 ./rtisdev/config/microphoneLayouts/eRTIS_v2/mic_coordinates.mat
 ./rtisdev/config/microphoneLayouts/eRTIS_v2REC/mic_coordinates.mat
 ./rtisdev/config/microphoneLayouts/eRTIS_v3D1/mic_coordinates.mat
@@ -28,17 +27,14 @@
 ./rtisdev/config/premadeSettings/recording/default_25_50.json
 ./rtisdev/config/premadeSettings/recording/flutter.csv
 ./rtisdev/config/premadeSettings/recording/flutter.json
 ./rtisdev/config/premadeSettings/recording/long_20_80.json
 ./rtisdev/config/premadeSettings/recording/long_25_50.json
 ./rtisdev/config/premadeSettings/recording/short_20_80.json
 ./rtisdev/config/premadeSettings/recording/short_25_50.json
-./tests/__init__.py
-./tests/test_rtisdev.py
-rtisdev/GenerateWiki.py
 rtisdev/RTISDev.py
 rtisdev/RTISGenerateSettings.py
 rtisdev/__init__.py
 rtisdev/simulate.bin
 rtisdev.egg-info/PKG-INFO
 rtisdev.egg-info/SOURCES.txt
 rtisdev.egg-info/dependency_links.txt
@@ -64,10 +60,8 @@
 rtisdev/config/premadeSettings/recording/default_20_80.json
 rtisdev/config/premadeSettings/recording/default_25_50.json
 rtisdev/config/premadeSettings/recording/flutter.csv
 rtisdev/config/premadeSettings/recording/flutter.json
 rtisdev/config/premadeSettings/recording/long_20_80.json
 rtisdev/config/premadeSettings/recording/long_25_50.json
 rtisdev/config/premadeSettings/recording/short_20_80.json
-rtisdev/config/premadeSettings/recording/short_25_50.json
-tests/__init__.py
-tests/test_rtisdev.py
+rtisdev/config/premadeSettings/recording/short_25_50.json
```

