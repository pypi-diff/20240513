# Comparing `tmp/smartboiler-0.1.7.tar.gz` & `tmp/smartboiler-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartboiler-0.1.7.tar", last modified: Mon May 13 19:07:50 2024, max compression
+gzip compressed data, was "smartboiler-0.1.8.tar", last modified: Mon May 13 19:32:32 2024, max compression
```

## Comparing `smartboiler-0.1.7.tar` & `smartboiler-0.1.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:07:50.316017 smartboiler-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-13 19:07:50.316017 smartboiler-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-13 19:07:46.000000 smartboiler-0.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 19:07:50.316017 smartboiler-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-13 19:07:48.000000 smartboiler-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:07:50.312017 smartboiler-0.1.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:07:50.316017 smartboiler-0.1.7/src/smartboiler/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-13 19:07:46.000000 smartboiler-0.1.7/src/smartboiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13583 2024-05-13 19:07:46.000000 smartboiler-0.1.7/src/smartboiler/boiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     9915 2024-05-13 19:07:46.000000 smartboiler-0.1.7/src/smartboiler/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)    31760 2024-05-13 19:07:46.000000 smartboiler-0.1.7/src/smartboiler/data_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5541 2024-05-13 19:07:46.000000 smartboiler-0.1.7/src/smartboiler/event_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)    15561 2024-05-13 19:07:46.000000 smartboiler-0.1.7/src/smartboiler/forecast.py
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-05-13 19:07:46.000000 smartboiler-0.1.7/src/smartboiler/fotovoltaics.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 19:07:46.000000 smartboiler-0.1.7/src/smartboiler/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-13 19:07:46.000000 smartboiler-0.1.7/src/smartboiler/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-13 19:07:46.000000 smartboiler-0.1.7/src/smartboiler/time_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:07:50.316017 smartboiler-0.1.7/src/smartboiler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-13 19:07:50.000000 smartboiler-0.1.7/src/smartboiler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-13 19:07:50.000000 smartboiler-0.1.7/src/smartboiler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 19:07:50.000000 smartboiler-0.1.7/src/smartboiler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-13 19:07:50.000000 smartboiler-0.1.7/src/smartboiler.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-13 19:07:50.000000 smartboiler-0.1.7/src/smartboiler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-13 19:07:50.000000 smartboiler-0.1.7/src/smartboiler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:32:32.538576 smartboiler-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-13 19:32:32.534576 smartboiler-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-13 19:32:29.000000 smartboiler-0.1.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 19:32:32.538576 smartboiler-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-13 19:32:31.000000 smartboiler-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:32:32.534576 smartboiler-0.1.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:32:32.534576 smartboiler-0.1.8/src/smartboiler/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-13 19:32:29.000000 smartboiler-0.1.8/src/smartboiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13583 2024-05-13 19:32:29.000000 smartboiler-0.1.8/src/smartboiler/boiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9688 2024-05-13 19:32:29.000000 smartboiler-0.1.8/src/smartboiler/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31760 2024-05-13 19:32:29.000000 smartboiler-0.1.8/src/smartboiler/data_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5541 2024-05-13 19:32:29.000000 smartboiler-0.1.8/src/smartboiler/event_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15561 2024-05-13 19:32:29.000000 smartboiler-0.1.8/src/smartboiler/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-05-13 19:32:29.000000 smartboiler-0.1.8/src/smartboiler/fotovoltaics.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 19:32:29.000000 smartboiler-0.1.8/src/smartboiler/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-13 19:32:29.000000 smartboiler-0.1.8/src/smartboiler/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-13 19:32:29.000000 smartboiler-0.1.8/src/smartboiler/time_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:32:32.534576 smartboiler-0.1.8/src/smartboiler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-13 19:32:32.000000 smartboiler-0.1.8/src/smartboiler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-13 19:32:32.000000 smartboiler-0.1.8/src/smartboiler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 19:32:32.000000 smartboiler-0.1.8/src/smartboiler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-13 19:32:32.000000 smartboiler-0.1.8/src/smartboiler.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-13 19:32:32.000000 smartboiler-0.1.8/src/smartboiler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-13 19:32:32.000000 smartboiler-0.1.8/src/smartboiler.egg-info/top_level.txt
```

### Comparing `smartboiler-0.1.7/PKG-INFO` & `smartboiler-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartboiler
-Version: 0.1.7
+Version: 0.1.8
 Summary: Smart boiling of household
 Home-page: https://github.com/grinwi/smartboiler
 Author: Adam GRUNWALD
 Author-email: grunwald.adam24@gmail.com
 Keywords: energy,management,optimization,hass
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `smartboiler-0.1.7/README.md` & `smartboiler-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `smartboiler-0.1.7/setup.py` & `smartboiler-0.1.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
 
 setup(
     name="smartboiler",  # Required
-    version="0.1.7",  # Required
+    version="0.1.8",  # Required
     description="Smart boiling of household",  # Optional
     long_description=long_description,  # Optional
     long_description_content_type="text/markdown",  # Optional (see note above)
     url="https://github.com/grinwi/smartboiler",  # Optional
     author="Adam GRUNWALD",  # Optional
     author_email="grunwald.adam24@gmail.com",  # Optional
     classifiers=[  # Optional
```

### Comparing `smartboiler-0.1.7/src/smartboiler/boiler.py` & `smartboiler-0.1.8/src/smartboiler/boiler.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.1.7/src/smartboiler/controller.py` & `smartboiler-0.1.8/src/smartboiler/controller.py`

 * *Files 3% similar despite different names*

```diff
@@ -182,20 +182,17 @@
     influxdb_host = options["influxdb_host"]
     influxdb_port: 8086
     influxdb_user = options["influxdb_user"]
     influxdb_pass = options["influxdb_pass"]
     influxdb_name = options["influxdb_name"]
 
     boiler_case_tmp_entity_id = options["boiler_case_tmp_entity_id"]
-    boiler_case_tmp_measurement = options["boiler_case_tmp_measurement"]
     boiler_water_flow_entity_id = options["boiler_water_flow_entity_id"]
-    boiler_water_flow_measurement = options["boiler_water_flow_measurement"]
     boiler_water_temp_entity_id = options["boiler_water_temp_entity_id"]
     boiler_water_temp_entity_id_2 = options["boiler_water_temp_entity_id_2"]
-    boiler_water_temp_measurement = options["boiler_water_temp_measurement"]
     boiler_volume = options["boiler_volume"]
     boiler_set_tmp = options["boiler_set_tmp"]
     boiler_min_operation_tmp = options["boiler_min_operation_tmp"]
     average_boiler_surroundings_temp = options["average_boiler_surroundings_temp"]
     boiler_case_max_tmp = options["boiler_case_max_tmp"]
     boiler_watt_power = options["boiler_watt_power"]
```

### Comparing `smartboiler-0.1.7/src/smartboiler/data_handler.py` & `smartboiler-0.1.8/src/smartboiler/data_handler.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.1.7/src/smartboiler/event_checker.py` & `smartboiler-0.1.8/src/smartboiler/event_checker.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.1.7/src/smartboiler/forecast.py` & `smartboiler-0.1.8/src/smartboiler/forecast.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.1.7/src/smartboiler/fotovoltaics.py` & `smartboiler-0.1.8/src/smartboiler/fotovoltaics.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.1.7/src/smartboiler/switch.py` & `smartboiler-0.1.8/src/smartboiler/switch.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.1.7/src/smartboiler/time_handler.py` & `smartboiler-0.1.8/src/smartboiler/time_handler.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.1.7/src/smartboiler.egg-info/PKG-INFO` & `smartboiler-0.1.8/src/smartboiler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartboiler
-Version: 0.1.7
+Version: 0.1.8
 Summary: Smart boiling of household
 Home-page: https://github.com/grinwi/smartboiler
 Author: Adam GRUNWALD
 Author-email: grunwald.adam24@gmail.com
 Keywords: energy,management,optimization,hass
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `smartboiler-0.1.7/src/smartboiler.egg-info/SOURCES.txt` & `smartboiler-0.1.8/src/smartboiler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

