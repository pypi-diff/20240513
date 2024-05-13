# Comparing `tmp/smartboiler-0.1.2.tar.gz` & `tmp/smartboiler-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartboiler-0.1.2.tar", last modified: Mon May 13 10:37:43 2024, max compression
+gzip compressed data, was "smartboiler-0.1.3.tar", last modified: Mon May 13 10:53:51 2024, max compression
```

## Comparing `smartboiler-0.1.2.tar` & `smartboiler-0.1.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:37:43.640676 smartboiler-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-13 10:37:43.640676 smartboiler-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-13 10:37:40.000000 smartboiler-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 10:37:43.640676 smartboiler-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-13 10:37:42.000000 smartboiler-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:37:43.640676 smartboiler-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:37:43.640676 smartboiler-0.1.2/src/smartboiler/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-13 10:37:40.000000 smartboiler-0.1.2/src/smartboiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13942 2024-05-13 10:37:40.000000 smartboiler-0.1.2/src/smartboiler/boiler.py
--rw-r--r--   0 runner    (1001) docker     (127)    10712 2024-05-13 10:37:40.000000 smartboiler-0.1.2/src/smartboiler/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)    32021 2024-05-13 10:37:40.000000 smartboiler-0.1.2/src/smartboiler/data_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5584 2024-05-13 10:37:40.000000 smartboiler-0.1.2/src/smartboiler/event_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)    15307 2024-05-13 10:37:40.000000 smartboiler-0.1.2/src/smartboiler/forecast.py
--rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-05-13 10:37:40.000000 smartboiler-0.1.2/src/smartboiler/fotovoltaics.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 10:37:40.000000 smartboiler-0.1.2/src/smartboiler/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-05-13 10:37:40.000000 smartboiler-0.1.2/src/smartboiler/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-13 10:37:40.000000 smartboiler-0.1.2/src/smartboiler/time_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:37:43.640676 smartboiler-0.1.2/src/smartboiler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-13 10:37:43.000000 smartboiler-0.1.2/src/smartboiler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-13 10:37:43.000000 smartboiler-0.1.2/src/smartboiler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 10:37:43.000000 smartboiler-0.1.2/src/smartboiler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-13 10:37:43.000000 smartboiler-0.1.2/src/smartboiler.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-13 10:37:43.000000 smartboiler-0.1.2/src/smartboiler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-13 10:37:43.000000 smartboiler-0.1.2/src/smartboiler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:53:51.627890 smartboiler-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-13 10:53:51.627890 smartboiler-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-13 10:53:49.000000 smartboiler-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 10:53:51.627890 smartboiler-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-13 10:53:51.000000 smartboiler-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:53:51.623890 smartboiler-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:53:51.627890 smartboiler-0.1.3/src/smartboiler/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-13 10:53:49.000000 smartboiler-0.1.3/src/smartboiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13942 2024-05-13 10:53:49.000000 smartboiler-0.1.3/src/smartboiler/boiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10488 2024-05-13 10:53:49.000000 smartboiler-0.1.3/src/smartboiler/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32021 2024-05-13 10:53:49.000000 smartboiler-0.1.3/src/smartboiler/data_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5584 2024-05-13 10:53:49.000000 smartboiler-0.1.3/src/smartboiler/event_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15307 2024-05-13 10:53:49.000000 smartboiler-0.1.3/src/smartboiler/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-05-13 10:53:49.000000 smartboiler-0.1.3/src/smartboiler/fotovoltaics.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 10:53:49.000000 smartboiler-0.1.3/src/smartboiler/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-05-13 10:53:49.000000 smartboiler-0.1.3/src/smartboiler/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-13 10:53:49.000000 smartboiler-0.1.3/src/smartboiler/time_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:53:51.627890 smartboiler-0.1.3/src/smartboiler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-13 10:53:51.000000 smartboiler-0.1.3/src/smartboiler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-13 10:53:51.000000 smartboiler-0.1.3/src/smartboiler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 10:53:51.000000 smartboiler-0.1.3/src/smartboiler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-13 10:53:51.000000 smartboiler-0.1.3/src/smartboiler.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-13 10:53:51.000000 smartboiler-0.1.3/src/smartboiler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-13 10:53:51.000000 smartboiler-0.1.3/src/smartboiler.egg-info/top_level.txt
```

### Comparing `smartboiler-0.1.2/PKG-INFO` & `smartboiler-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartboiler
-Version: 0.1.2
+Version: 0.1.3
 Summary: Smart boiling of household
 Home-page: https://github.com/grinwi/smartboiler
 Author: Adam GRUNWALD
 Author-email: grunwald.adam24@gmail.com
 Keywords: energy,management,optimization,hass
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `smartboiler-0.1.2/README.md` & `smartboiler-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `smartboiler-0.1.2/setup.py` & `smartboiler-0.1.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
 
 setup(
     name="smartboiler",  # Required
-    version="0.1.2",  # Required
+    version="0.1.3",  # Required
     description="Smart boiling of household",  # Optional
     long_description=long_description,  # Optional
     long_description_content_type="text/markdown",  # Optional (see note above)
     url="https://github.com/grinwi/smartboiler",  # Optional
     author="Adam GRUNWALD",  # Optional
     author_email="grunwald.adam24@gmail.com",  # Optional
     classifiers=[  # Optional
```

### Comparing `smartboiler-0.1.2/src/smartboiler/boiler.py` & `smartboiler-0.1.3/src/smartboiler/boiler.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.1.2/src/smartboiler/controller.py` & `smartboiler-0.1.3/src/smartboiler/controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,19 +193,15 @@
     boiler_water_temp_entity_id_2 = options["boiler_water_temp_entity_id_2"]
     boiler_water_temp_measurement = options["boiler_water_temp_measurement"]
     boiler_volume = options["boiler_volume"]
     boiler_set_tmp = options["boiler_set_tmp"]
     boiler_min_operation_tmp = options["boiler_min_operation_tmp"]
     average_boiler_surroundings_temp = options["average_boiler_surroundings_temp"]
     boiler_case_max_tmp = options["boiler_case_max_tmp"]
-    one_shower_volume = options["one_shower_volume"]
     boiler_watt_power = options["boiler_watt_power"]
-    household_floor_size = options["household_floor_size"]
-    household_members = options["household_members"]
-    thermostat_entity_id = options["thermostat_entity_id"]
     logging_level = options["logging_level"]
     load_model = options["load_model"]
     learning = options["learning"]
     hdo = options["hdo"]
     has_fotovoltaics = options["has_fotovoltaics"]
     fve_solax_sn = options["fve_solax_sn"]
     fve_solax_token = options["fve_solax_token"]
```

### Comparing `smartboiler-0.1.2/src/smartboiler/data_handler.py` & `smartboiler-0.1.3/src/smartboiler/data_handler.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.1.2/src/smartboiler/event_checker.py` & `smartboiler-0.1.3/src/smartboiler/event_checker.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.1.2/src/smartboiler/forecast.py` & `smartboiler-0.1.3/src/smartboiler/forecast.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.1.2/src/smartboiler/fotovoltaics.py` & `smartboiler-0.1.3/src/smartboiler/fotovoltaics.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.1.2/src/smartboiler/switch.py` & `smartboiler-0.1.3/src/smartboiler/switch.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.1.2/src/smartboiler/time_handler.py` & `smartboiler-0.1.3/src/smartboiler/time_handler.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.1.2/src/smartboiler.egg-info/PKG-INFO` & `smartboiler-0.1.3/src/smartboiler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartboiler
-Version: 0.1.2
+Version: 0.1.3
 Summary: Smart boiling of household
 Home-page: https://github.com/grinwi/smartboiler
 Author: Adam GRUNWALD
 Author-email: grunwald.adam24@gmail.com
 Keywords: energy,management,optimization,hass
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `smartboiler-0.1.2/src/smartboiler.egg-info/SOURCES.txt` & `smartboiler-0.1.3/src/smartboiler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

