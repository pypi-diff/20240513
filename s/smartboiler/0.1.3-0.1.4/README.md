# Comparing `tmp/smartboiler-0.1.3.tar.gz` & `tmp/smartboiler-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartboiler-0.1.3.tar", last modified: Mon May 13 10:53:51 2024, max compression
+gzip compressed data, was "smartboiler-0.1.4.tar", last modified: Mon May 13 16:27:10 2024, max compression
```

## Comparing `smartboiler-0.1.3.tar` & `smartboiler-0.1.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:53:51.627890 smartboiler-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-13 10:53:51.627890 smartboiler-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-13 10:53:49.000000 smartboiler-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 10:53:51.627890 smartboiler-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-13 10:53:51.000000 smartboiler-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:53:51.623890 smartboiler-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:53:51.627890 smartboiler-0.1.3/src/smartboiler/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-13 10:53:49.000000 smartboiler-0.1.3/src/smartboiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13942 2024-05-13 10:53:49.000000 smartboiler-0.1.3/src/smartboiler/boiler.py
--rw-r--r--   0 runner    (1001) docker     (127)    10488 2024-05-13 10:53:49.000000 smartboiler-0.1.3/src/smartboiler/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)    32021 2024-05-13 10:53:49.000000 smartboiler-0.1.3/src/smartboiler/data_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5584 2024-05-13 10:53:49.000000 smartboiler-0.1.3/src/smartboiler/event_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)    15307 2024-05-13 10:53:49.000000 smartboiler-0.1.3/src/smartboiler/forecast.py
--rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-05-13 10:53:49.000000 smartboiler-0.1.3/src/smartboiler/fotovoltaics.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 10:53:49.000000 smartboiler-0.1.3/src/smartboiler/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-05-13 10:53:49.000000 smartboiler-0.1.3/src/smartboiler/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-13 10:53:49.000000 smartboiler-0.1.3/src/smartboiler/time_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:53:51.627890 smartboiler-0.1.3/src/smartboiler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-13 10:53:51.000000 smartboiler-0.1.3/src/smartboiler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-13 10:53:51.000000 smartboiler-0.1.3/src/smartboiler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 10:53:51.000000 smartboiler-0.1.3/src/smartboiler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-13 10:53:51.000000 smartboiler-0.1.3/src/smartboiler.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-13 10:53:51.000000 smartboiler-0.1.3/src/smartboiler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-13 10:53:51.000000 smartboiler-0.1.3/src/smartboiler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:27:10.869680 smartboiler-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-13 16:27:10.869680 smartboiler-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-13 16:27:06.000000 smartboiler-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 16:27:10.869680 smartboiler-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-13 16:27:09.000000 smartboiler-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:27:10.865680 smartboiler-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:27:10.869680 smartboiler-0.1.4/src/smartboiler/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-13 16:27:06.000000 smartboiler-0.1.4/src/smartboiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13942 2024-05-13 16:27:06.000000 smartboiler-0.1.4/src/smartboiler/boiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10412 2024-05-13 16:27:06.000000 smartboiler-0.1.4/src/smartboiler/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32021 2024-05-13 16:27:06.000000 smartboiler-0.1.4/src/smartboiler/data_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5584 2024-05-13 16:27:06.000000 smartboiler-0.1.4/src/smartboiler/event_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15307 2024-05-13 16:27:06.000000 smartboiler-0.1.4/src/smartboiler/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-05-13 16:27:06.000000 smartboiler-0.1.4/src/smartboiler/fotovoltaics.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 16:27:06.000000 smartboiler-0.1.4/src/smartboiler/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-05-13 16:27:06.000000 smartboiler-0.1.4/src/smartboiler/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-13 16:27:06.000000 smartboiler-0.1.4/src/smartboiler/time_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:27:10.869680 smartboiler-0.1.4/src/smartboiler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-13 16:27:10.000000 smartboiler-0.1.4/src/smartboiler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-13 16:27:10.000000 smartboiler-0.1.4/src/smartboiler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 16:27:10.000000 smartboiler-0.1.4/src/smartboiler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-13 16:27:10.000000 smartboiler-0.1.4/src/smartboiler.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-13 16:27:10.000000 smartboiler-0.1.4/src/smartboiler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-13 16:27:10.000000 smartboiler-0.1.4/src/smartboiler.egg-info/top_level.txt
```

### Comparing `smartboiler-0.1.3/PKG-INFO` & `smartboiler-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartboiler
-Version: 0.1.3
+Version: 0.1.4
 Summary: Smart boiling of household
 Home-page: https://github.com/grinwi/smartboiler
 Author: Adam GRUNWALD
 Author-email: grunwald.adam24@gmail.com
 Keywords: energy,management,optimization,hass
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `smartboiler-0.1.3/README.md` & `smartboiler-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `smartboiler-0.1.3/setup.py` & `smartboiler-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
 
 setup(
     name="smartboiler",  # Required
-    version="0.1.3",  # Required
+    version="0.1.4",  # Required
     description="Smart boiling of household",  # Optional
     long_description=long_description,  # Optional
     long_description_content_type="text/markdown",  # Optional (see note above)
     url="https://github.com/grinwi/smartboiler",  # Optional
     author="Adam GRUNWALD",  # Optional
     author_email="grunwald.adam24@gmail.com",  # Optional
     classifiers=[  # Optional
```

### Comparing `smartboiler-0.1.3/src/smartboiler/boiler.py` & `smartboiler-0.1.4/src/smartboiler/boiler.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.1.3/src/smartboiler/controller.py` & `smartboiler-0.1.4/src/smartboiler/controller.py`

 * *Files 3% similar despite different names*

```diff
@@ -166,15 +166,15 @@
 
     DATA_PATH = os.getenv("DATA_PATH", default="/app/data/")
 
     data_path = Path(DATA_PATH)
 
     start_of_data_measurement = datetime(2023, 10, 1, 0, 0, 0, 0)
 
-    hass_url = options["hass_url"]
+    shelly_ip = options["shelly_ip"]
     home_longitude = options["home_longitude"]
     home_latitude = options["home_latitude"]
     device_tracker_entity_id = options["device_tracker_entity_id"]
     device_tracker_entity_id_2 = options["device_tracker_entity_id_2"]
     model_type = options["model_type"]
     long_lived_token = options["long_lived_token"]
     influxdb_host = options["influxdb_host"]
@@ -213,18 +213,14 @@
     else:
         model_path = "/app/model_zuka.weights.h5"
         scaler_path = "/app/scaler_zuka.pkl"
 
     model_path = Path(model_path)
     scaler_path = Path(scaler_path)
 
-    base_url = hass_url
-    url = base_url + "/config"
-    web_ui = "0.0.0.0"
-
     headers = {
         "Authorization": f"Bearer {long_lived_token}",
         "content-type": "application/json",
     }
 
     dataHandler = DataHandler(
         influx_id=influxdb_host,
@@ -255,15 +251,15 @@
             battery_power=5,
         )
     else:
         fotovoltaics = None
     eventChecker = EventChecker()
     print("inicializing boiler from controller __main__")
     boiler = Boiler(
-        base_url,
+        shelly_ip,
         long_lived_token,
         headers,
         boiler_switch_entity_id=boiler_socket_switch_id,
         dataHandler=dataHandler,
         eventChecker=eventChecker,
         fotovoltaics=fotovoltaics,
         capacity=boiler_volume,
```

### Comparing `smartboiler-0.1.3/src/smartboiler/data_handler.py` & `smartboiler-0.1.4/src/smartboiler/data_handler.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.1.3/src/smartboiler/event_checker.py` & `smartboiler-0.1.4/src/smartboiler/event_checker.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.1.3/src/smartboiler/forecast.py` & `smartboiler-0.1.4/src/smartboiler/forecast.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.1.3/src/smartboiler/fotovoltaics.py` & `smartboiler-0.1.4/src/smartboiler/fotovoltaics.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.1.3/src/smartboiler/switch.py` & `smartboiler-0.1.4/src/smartboiler/switch.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.1.3/src/smartboiler/time_handler.py` & `smartboiler-0.1.4/src/smartboiler/time_handler.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.1.3/src/smartboiler.egg-info/PKG-INFO` & `smartboiler-0.1.4/src/smartboiler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartboiler
-Version: 0.1.3
+Version: 0.1.4
 Summary: Smart boiling of household
 Home-page: https://github.com/grinwi/smartboiler
 Author: Adam GRUNWALD
 Author-email: grunwald.adam24@gmail.com
 Keywords: energy,management,optimization,hass
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `smartboiler-0.1.3/src/smartboiler.egg-info/SOURCES.txt` & `smartboiler-0.1.4/src/smartboiler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

