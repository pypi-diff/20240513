# Comparing `tmp/smartboiler-0.1.8.tar.gz` & `tmp/smartboiler-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartboiler-0.1.8.tar", last modified: Mon May 13 19:32:32 2024, max compression
+gzip compressed data, was "smartboiler-0.1.9.tar", last modified: Mon May 13 19:56:09 2024, max compression
```

## Comparing `smartboiler-0.1.8.tar` & `smartboiler-0.1.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:32:32.538576 smartboiler-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-13 19:32:32.534576 smartboiler-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-13 19:32:29.000000 smartboiler-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 19:32:32.538576 smartboiler-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-13 19:32:31.000000 smartboiler-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:32:32.534576 smartboiler-0.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:32:32.534576 smartboiler-0.1.8/src/smartboiler/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-13 19:32:29.000000 smartboiler-0.1.8/src/smartboiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13583 2024-05-13 19:32:29.000000 smartboiler-0.1.8/src/smartboiler/boiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     9688 2024-05-13 19:32:29.000000 smartboiler-0.1.8/src/smartboiler/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)    31760 2024-05-13 19:32:29.000000 smartboiler-0.1.8/src/smartboiler/data_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5541 2024-05-13 19:32:29.000000 smartboiler-0.1.8/src/smartboiler/event_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)    15561 2024-05-13 19:32:29.000000 smartboiler-0.1.8/src/smartboiler/forecast.py
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-05-13 19:32:29.000000 smartboiler-0.1.8/src/smartboiler/fotovoltaics.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 19:32:29.000000 smartboiler-0.1.8/src/smartboiler/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-13 19:32:29.000000 smartboiler-0.1.8/src/smartboiler/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-13 19:32:29.000000 smartboiler-0.1.8/src/smartboiler/time_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:32:32.534576 smartboiler-0.1.8/src/smartboiler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-13 19:32:32.000000 smartboiler-0.1.8/src/smartboiler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-13 19:32:32.000000 smartboiler-0.1.8/src/smartboiler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 19:32:32.000000 smartboiler-0.1.8/src/smartboiler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-13 19:32:32.000000 smartboiler-0.1.8/src/smartboiler.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-13 19:32:32.000000 smartboiler-0.1.8/src/smartboiler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-13 19:32:32.000000 smartboiler-0.1.8/src/smartboiler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:56:09.632419 smartboiler-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-13 19:56:09.632419 smartboiler-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-13 19:56:07.000000 smartboiler-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 19:56:09.632419 smartboiler-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-13 19:56:09.000000 smartboiler-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:56:09.628419 smartboiler-0.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:56:09.632419 smartboiler-0.1.9/src/smartboiler/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-13 19:56:07.000000 smartboiler-0.1.9/src/smartboiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13583 2024-05-13 19:56:07.000000 smartboiler-0.1.9/src/smartboiler/boiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9984 2024-05-13 19:56:07.000000 smartboiler-0.1.9/src/smartboiler/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31760 2024-05-13 19:56:07.000000 smartboiler-0.1.9/src/smartboiler/data_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5541 2024-05-13 19:56:07.000000 smartboiler-0.1.9/src/smartboiler/event_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15561 2024-05-13 19:56:07.000000 smartboiler-0.1.9/src/smartboiler/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-05-13 19:56:07.000000 smartboiler-0.1.9/src/smartboiler/fotovoltaics.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 19:56:07.000000 smartboiler-0.1.9/src/smartboiler/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-13 19:56:07.000000 smartboiler-0.1.9/src/smartboiler/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-13 19:56:07.000000 smartboiler-0.1.9/src/smartboiler/time_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:56:09.632419 smartboiler-0.1.9/src/smartboiler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-13 19:56:09.000000 smartboiler-0.1.9/src/smartboiler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-13 19:56:09.000000 smartboiler-0.1.9/src/smartboiler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 19:56:09.000000 smartboiler-0.1.9/src/smartboiler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-13 19:56:09.000000 smartboiler-0.1.9/src/smartboiler.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-13 19:56:09.000000 smartboiler-0.1.9/src/smartboiler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-13 19:56:09.000000 smartboiler-0.1.9/src/smartboiler.egg-info/top_level.txt
```

### Comparing `smartboiler-0.1.8/PKG-INFO` & `smartboiler-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartboiler
-Version: 0.1.8
+Version: 0.1.9
 Summary: Smart boiling of household
 Home-page: https://github.com/grinwi/smartboiler
 Author: Adam GRUNWALD
 Author-email: grunwald.adam24@gmail.com
 Keywords: energy,management,optimization,hass
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `smartboiler-0.1.8/README.md` & `smartboiler-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `smartboiler-0.1.8/setup.py` & `smartboiler-0.1.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
 
 setup(
     name="smartboiler",  # Required
-    version="0.1.8",  # Required
+    version="0.1.9",  # Required
     description="Smart boiling of household",  # Optional
     long_description=long_description,  # Optional
     long_description_content_type="text/markdown",  # Optional (see note above)
     url="https://github.com/grinwi/smartboiler",  # Optional
     author="Adam GRUNWALD",  # Optional
     author_email="grunwald.adam24@gmail.com",  # Optional
     classifiers=[  # Optional
```

### Comparing `smartboiler-0.1.8/src/smartboiler/boiler.py` & `smartboiler-0.1.9/src/smartboiler/boiler.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.1.8/src/smartboiler/controller.py` & `smartboiler-0.1.9/src/smartboiler/controller.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # Faculty of Information Technology, Brno University of Technology, 2024
 # Author: Adam Grünwald
 #
 # This module is used for controlling the boiler with use of the predictions in combination with the smart heating algotithm.
 
 
 from pathlib import Path
+from matplotlib.font_manager import json_load
 import pytz
 from datetime import datetime, timedelta
 
 import os.path
 import logging
 import time
 import os
@@ -169,14 +170,16 @@
 
     data_path = Path(DATA_PATH)
 
     start_of_data_measurement = datetime(2023, 10, 1, 0, 0, 0, 0)
 
     shelly_ip = options["shelly_ip"]
     boiler_switch_id = options["boiler_switch_id"]
+    
+    google_calendar_token = options["google_calendar_token"]
 
     home_longitude = options["home_longitude"]
     home_latitude = options["home_latitude"]
     device_tracker_entity_id = options["device_tracker_entity_id"]
     device_tracker_entity_id_2 = options["device_tracker_entity_id_2"]
 
     influxdb_host = options["influxdb_host"]
@@ -211,14 +214,18 @@
     if model_type == "smaller_household":
         model_path = "/app/model_form.weights.h5"
         scaler_path = "/app/scaler_form.pkl"
     else:
         model_path = "/app/model_zuka.weights.h5"
         scaler_path = "/app/scaler_zuka.pkl"
 
+    if google_calendar_token:
+        google_calendar_token = json.loads(google_calendar_token)
+    with open("/app/token.json", "w") as f:
+        json.dump(google_calendar_token, f)
     model_path = Path(model_path)
     scaler_path = Path(scaler_path)
 
     dataHandler = DataHandler(
         influx_id=influxdb_host,
         db_name=influxdb_name,
         db_username=influxdb_user,
```

### Comparing `smartboiler-0.1.8/src/smartboiler/data_handler.py` & `smartboiler-0.1.9/src/smartboiler/data_handler.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.1.8/src/smartboiler/event_checker.py` & `smartboiler-0.1.9/src/smartboiler/event_checker.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.1.8/src/smartboiler/forecast.py` & `smartboiler-0.1.9/src/smartboiler/forecast.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.1.8/src/smartboiler/fotovoltaics.py` & `smartboiler-0.1.9/src/smartboiler/fotovoltaics.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.1.8/src/smartboiler/switch.py` & `smartboiler-0.1.9/src/smartboiler/switch.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.1.8/src/smartboiler/time_handler.py` & `smartboiler-0.1.9/src/smartboiler/time_handler.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.1.8/src/smartboiler.egg-info/PKG-INFO` & `smartboiler-0.1.9/src/smartboiler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartboiler
-Version: 0.1.8
+Version: 0.1.9
 Summary: Smart boiling of household
 Home-page: https://github.com/grinwi/smartboiler
 Author: Adam GRUNWALD
 Author-email: grunwald.adam24@gmail.com
 Keywords: energy,management,optimization,hass
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `smartboiler-0.1.8/src/smartboiler.egg-info/SOURCES.txt` & `smartboiler-0.1.9/src/smartboiler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

