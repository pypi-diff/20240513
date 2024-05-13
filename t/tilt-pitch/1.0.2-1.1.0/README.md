# Comparing `tmp/tilt-pitch-1.0.2.tar.gz` & `tmp/tilt-pitch-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tilt-pitch-1.0.2.tar", last modified: Tue Oct 31 12:14:13 2023, max compression
+gzip compressed data, was "dist/tilt-pitch-1.1.0.tar", last modified: Mon May 13 14:44:10 2024, max compression
```

## Comparing `tilt-pitch-1.0.2.tar` & `tilt-pitch-1.1.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 12:14:13.000000 tilt-pitch-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2023-10-31 12:13:32.000000 tilt-pitch-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    17267 2023-10-31 12:14:13.000000 tilt-pitch-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16720 2023-10-31 12:13:32.000000 tilt-pitch-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 12:14:13.000000 tilt-pitch-1.0.2/pitch/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2023-10-31 12:13:32.000000 tilt-pitch-1.0.2/pitch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2023-10-31 12:13:32.000000 tilt-pitch-1.0.2/pitch/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 12:14:13.000000 tilt-pitch-1.0.2/pitch/abstractions/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2023-10-31 12:13:32.000000 tilt-pitch-1.0.2/pitch/abstractions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      241 2023-10-31 12:13:32.000000 tilt-pitch-1.0.2/pitch/abstractions/cloud_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 12:14:13.000000 tilt-pitch-1.0.2/pitch/configuration/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2023-10-31 12:13:32.000000 tilt-pitch-1.0.2/pitch/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2717 2023-10-31 12:13:32.000000 tilt-pitch-1.0.2/pitch/configuration/pitch_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 12:14:13.000000 tilt-pitch-1.0.2/pitch/models/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2023-10-31 12:13:32.000000 tilt-pitch-1.0.2/pitch/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-10-31 12:13:32.000000 tilt-pitch-1.0.2/pitch/models/json_serialize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1826 2023-10-31 12:13:32.000000 tilt-pitch-1.0.2/pitch/models/tilt_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     7239 2023-10-31 12:13:32.000000 tilt-pitch-1.0.2/pitch/pitch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 12:14:13.000000 tilt-pitch-1.0.2/pitch/providers/
--rw-r--r--   0 runner    (1001) docker     (127)      607 2023-10-31 12:13:32.000000 tilt-pitch-1.0.2/pitch/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2023-10-31 12:13:32.000000 tilt-pitch-1.0.2/pitch/providers/azure_iothub.py
--rw-r--r--   0 runner    (1001) docker     (127)     2412 2023-10-31 12:13:32.000000 tilt-pitch-1.0.2/pitch/providers/brewersfriend_custom_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2023-10-31 12:13:32.000000 tilt-pitch-1.0.2/pitch/providers/brewfather_custom_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2023-10-31 12:13:32.000000 tilt-pitch-1.0.2/pitch/providers/calibration.py
--rw-r--r--   0 runner    (1001) docker     (127)      881 2023-10-31 12:13:32.000000 tilt-pitch-1.0.2/pitch/providers/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2023-10-31 12:13:32.000000 tilt-pitch-1.0.2/pitch/providers/grainfather_custom_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2023-10-31 12:13:32.000000 tilt-pitch-1.0.2/pitch/providers/influxdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     1951 2023-10-31 12:13:32.000000 tilt-pitch-1.0.2/pitch/providers/influxdb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2023-10-31 12:13:32.000000 tilt-pitch-1.0.2/pitch/providers/prometheus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2023-10-31 12:13:32.000000 tilt-pitch-1.0.2/pitch/providers/taplistio_custom_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)      897 2023-10-31 12:13:32.000000 tilt-pitch-1.0.2/pitch/providers/webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2023-10-31 12:13:32.000000 tilt-pitch-1.0.2/pitch/rate_limiter.py
--rw-r--r--   0 runner    (1001) docker     (127)      891 2023-10-31 12:13:32.000000 tilt-pitch-1.0.2/pitch/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-31 12:14:13.000000 tilt-pitch-1.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 12:14:13.000000 tilt-pitch-1.0.2/test/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2023-10-31 12:13:32.000000 tilt-pitch-1.0.2/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2023-10-31 12:13:32.000000 tilt-pitch-1.0.2/test/test_tilt_status.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 12:14:13.000000 tilt-pitch-1.0.2/tilt_pitch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17267 2023-10-31 12:14:13.000000 tilt-pitch-1.0.2/tilt_pitch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      944 2023-10-31 12:14:13.000000 tilt-pitch-1.0.2/tilt_pitch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-31 12:14:13.000000 tilt-pitch-1.0.2/tilt_pitch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      140 2023-10-31 12:14:13.000000 tilt-pitch-1.0.2/tilt_pitch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-10-31 12:14:13.000000 tilt-pitch-1.0.2/tilt_pitch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:44:10.000000 tilt-pitch-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-13 14:43:48.000000 tilt-pitch-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    17267 2024-05-13 14:44:10.000000 tilt-pitch-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16720 2024-05-13 14:43:48.000000 tilt-pitch-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:44:10.000000 tilt-pitch-1.1.0/pitch/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-13 14:43:48.000000 tilt-pitch-1.1.0/pitch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-13 14:43:48.000000 tilt-pitch-1.1.0/pitch/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:44:10.000000 tilt-pitch-1.1.0/pitch/abstractions/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-13 14:43:48.000000 tilt-pitch-1.1.0/pitch/abstractions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-13 14:43:48.000000 tilt-pitch-1.1.0/pitch/abstractions/cloud_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:44:10.000000 tilt-pitch-1.1.0/pitch/configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-13 14:43:48.000000 tilt-pitch-1.1.0/pitch/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-05-13 14:43:48.000000 tilt-pitch-1.1.0/pitch/configuration/pitch_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:44:10.000000 tilt-pitch-1.1.0/pitch/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-13 14:43:48.000000 tilt-pitch-1.1.0/pitch/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-13 14:43:48.000000 tilt-pitch-1.1.0/pitch/models/json_serialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-05-13 14:43:48.000000 tilt-pitch-1.1.0/pitch/models/tilt_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7239 2024-05-13 14:43:48.000000 tilt-pitch-1.1.0/pitch/pitch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:44:10.000000 tilt-pitch-1.1.0/pitch/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-13 14:43:48.000000 tilt-pitch-1.1.0/pitch/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-13 14:43:48.000000 tilt-pitch-1.1.0/pitch/providers/azure_iothub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-05-13 14:43:48.000000 tilt-pitch-1.1.0/pitch/providers/brewersfriend_custom_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-05-13 14:43:48.000000 tilt-pitch-1.1.0/pitch/providers/brewfather_custom_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-13 14:43:48.000000 tilt-pitch-1.1.0/pitch/providers/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-13 14:43:48.000000 tilt-pitch-1.1.0/pitch/providers/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-05-13 14:43:48.000000 tilt-pitch-1.1.0/pitch/providers/grainfather_custom_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-05-13 14:43:48.000000 tilt-pitch-1.1.0/pitch/providers/influxdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-05-13 14:43:48.000000 tilt-pitch-1.1.0/pitch/providers/influxdb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-05-13 14:43:48.000000 tilt-pitch-1.1.0/pitch/providers/prometheus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-13 14:43:48.000000 tilt-pitch-1.1.0/pitch/providers/taplistio_custom_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-13 14:43:48.000000 tilt-pitch-1.1.0/pitch/providers/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-13 14:43:48.000000 tilt-pitch-1.1.0/pitch/rate_limiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-13 14:43:48.000000 tilt-pitch-1.1.0/pitch/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 14:44:10.000000 tilt-pitch-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:44:10.000000 tilt-pitch-1.1.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-13 14:43:48.000000 tilt-pitch-1.1.0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-13 14:43:48.000000 tilt-pitch-1.1.0/test/test_tilt_status.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:44:10.000000 tilt-pitch-1.1.0/tilt_pitch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17267 2024-05-13 14:44:09.000000 tilt-pitch-1.1.0/tilt_pitch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-13 14:44:09.000000 tilt-pitch-1.1.0/tilt_pitch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 14:44:09.000000 tilt-pitch-1.1.0/tilt_pitch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-13 14:44:09.000000 tilt-pitch-1.1.0/tilt_pitch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-13 14:44:09.000000 tilt-pitch-1.1.0/tilt_pitch.egg-info/top_level.txt
```

### Comparing `tilt-pitch-1.0.2/LICENSE` & `tilt-pitch-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tilt-pitch-1.0.2/PKG-INFO` & `tilt-pitch-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tilt-pitch
-Version: 1.0.2
+Version: 1.1.0
 Summary: Simple replacement for the Tilt Hydrometer mobile apps and TiltPi with lots of features
 Home-page: https://github.com/linjmeyer/tilt-pitch/
 Author: Lin Meyer
 Author-email: lin@linmeyer.net
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tilt-pitch-1.0.2/README.md` & `tilt-pitch-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `tilt-pitch-1.0.2/pitch/__main__.py` & `tilt-pitch-1.1.0/pitch/__main__.py`

 * *Files identical despite different names*

### Comparing `tilt-pitch-1.0.2/pitch/configuration/pitch_config.py` & `tilt-pitch-1.1.0/pitch/configuration/pitch_config.py`

 * *Files identical despite different names*

### Comparing `tilt-pitch-1.0.2/pitch/models/tilt_status.py` & `tilt-pitch-1.1.0/pitch/models/tilt_status.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,26 +5,38 @@
 
 class TiltStatus(JsonSerialize):
 
     def __init__(self, color, temp_fahrenheit, current_gravity, config: PitchConfig):
         self.timestamp = datetime.datetime.now()
         self.color = color
         self.name = config.get_brew_name(color)
+        self.hd = current_gravity > 2  # Tilt Pro?
+
+        # With Tilt Pro values have more precision, which has to be adjusted
+        if self.hd:
+            current_gravity /= 10
+            temp_fahrenheit /= 10
+
         self.temp_fahrenheit = temp_fahrenheit + config.get_temp_offset(color)
-        self.temp_celsius = TiltStatus.get_celsius(temp_fahrenheit)
+        self.temp_celsius = TiltStatus.get_celsius(self.temp_fahrenheit)
         self.original_gravity = config.get_original_gravity(color)
         self.gravity = current_gravity + config.get_gravity_offset(color)
+        self.degrees_plato = TiltStatus.get_degrees_plato(self.gravity)
         self.alcohol_by_volume = TiltStatus.get_alcohol_by_volume(self.original_gravity, self.gravity)
         self.apparent_attenuation = TiltStatus.get_apparent_attenuation(self.original_gravity, self.gravity)
         self.temp_valid = (config.temp_range_min < self.temp_fahrenheit and self.temp_fahrenheit < config.temp_range_max)
         self.gravity_valid = (config.gravity_range_min < self.gravity and self.gravity < config.gravity_range_max)
 
     @staticmethod
     def get_celsius(temp_fahrenheit):
-        return round((temp_fahrenheit - 32) * 5.0/9.0)
+        return round((temp_fahrenheit - 32) * 5.0/9.0, 1)
+
+    @staticmethod
+    def get_degrees_plato(gravity):
+        return round(1111.14 * gravity - 630.272 * gravity ** 2 + 135.997 * gravity ** 3 - 616.868, 1)
 
     @staticmethod
     def get_alcohol_by_volume(original_gravity, current_gravity):
         if original_gravity is None:
             return 0
         alcohol_by_volume = (original_gravity - current_gravity) * 131.25
         return round(alcohol_by_volume, 2)
```

### Comparing `tilt-pitch-1.0.2/pitch/pitch.py` & `tilt-pitch-1.1.0/pitch/pitch.py`

 * *Files identical despite different names*

### Comparing `tilt-pitch-1.0.2/pitch/providers/__init__.py` & `tilt-pitch-1.1.0/pitch/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `tilt-pitch-1.0.2/pitch/providers/azure_iothub.py` & `tilt-pitch-1.1.0/pitch/providers/azure_iothub.py`

 * *Files identical despite different names*

### Comparing `tilt-pitch-1.0.2/pitch/providers/brewersfriend_custom_stream.py` & `tilt-pitch-1.1.0/pitch/providers/brewersfriend_custom_stream.py`

 * *Files identical despite different names*

### Comparing `tilt-pitch-1.0.2/pitch/providers/brewfather_custom_stream.py` & `tilt-pitch-1.1.0/pitch/providers/brewfather_custom_stream.py`

 * *Files identical despite different names*

### Comparing `tilt-pitch-1.0.2/pitch/providers/calibration.py` & `tilt-pitch-1.1.0/pitch/providers/calibration.py`

 * *Files identical despite different names*

### Comparing `tilt-pitch-1.0.2/pitch/providers/file.py` & `tilt-pitch-1.1.0/pitch/providers/file.py`

 * *Files identical despite different names*

### Comparing `tilt-pitch-1.0.2/pitch/providers/grainfather_custom_stream.py` & `tilt-pitch-1.1.0/pitch/providers/grainfather_custom_stream.py`

 * *Files identical despite different names*

### Comparing `tilt-pitch-1.0.2/pitch/providers/influxdb.py` & `tilt-pitch-1.1.0/pitch/providers/influxdb.py`

 * *Files identical despite different names*

### Comparing `tilt-pitch-1.0.2/pitch/providers/influxdb2.py` & `tilt-pitch-1.1.0/pitch/providers/influxdb2.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         return self.str_name
 
     def start(self):
         self.client = InfluxDBClient(
             url=self.config.influxdb2_url,
             token=self.config.influxdb2_token,
             org=self.config.influxdb2_org,
-            timeout=self.config.influxdb_timeout_seconds)
+            timeout=self.config.influxdb_timeout_seconds*1000)
         self.write_api = self.client.write_api(write_options=SYNCHRONOUS)
 
     def update(self, tilt_status: TiltStatus):
         self.batch.append(self.get_point(tilt_status))
         if len(self.batch) < self.config.influxdb_batch_size:
             return
         # Batch size has been met, update and clear
@@ -45,11 +45,12 @@
                 "color": tilt_status.color,
                 "name": tilt_status.name
             },
             "fields": {
                 "temp_fahrenheit": tilt_status.temp_fahrenheit,
                 "temp_celsius": tilt_status.temp_celsius,
                 "gravity": tilt_status.gravity,
+                "degrees_plato": tilt_status.degrees_plato,
                 "alcohol_by_volume": tilt_status.alcohol_by_volume,
                 "apparent_attenuation": tilt_status.apparent_attenuation
             }
         }
```

### Comparing `tilt-pitch-1.0.2/pitch/providers/prometheus.py` & `tilt-pitch-1.1.0/pitch/providers/prometheus.py`

 * *Files identical despite different names*

### Comparing `tilt-pitch-1.0.2/pitch/providers/taplistio_custom_stream.py` & `tilt-pitch-1.1.0/pitch/providers/taplistio_custom_stream.py`

 * *Files identical despite different names*

### Comparing `tilt-pitch-1.0.2/pitch/providers/webhook.py` & `tilt-pitch-1.1.0/pitch/providers/webhook.py`

 * *Files identical despite different names*

### Comparing `tilt-pitch-1.0.2/pitch/rate_limiter.py` & `tilt-pitch-1.1.0/pitch/rate_limiter.py`

 * *Files identical despite different names*

### Comparing `tilt-pitch-1.0.2/pitch/setup.py` & `tilt-pitch-1.1.0/pitch/setup.py`

 * *Files identical despite different names*

### Comparing `tilt-pitch-1.0.2/test/test_tilt_status.py` & `tilt-pitch-1.1.0/test/test_tilt_status.py`

 * *Files identical despite different names*

### Comparing `tilt-pitch-1.0.2/tilt_pitch.egg-info/PKG-INFO` & `tilt-pitch-1.1.0/tilt_pitch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tilt-pitch
-Version: 1.0.2
+Version: 1.1.0
 Summary: Simple replacement for the Tilt Hydrometer mobile apps and TiltPi with lots of features
 Home-page: https://github.com/linjmeyer/tilt-pitch/
 Author: Lin Meyer
 Author-email: lin@linmeyer.net
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tilt-pitch-1.0.2/tilt_pitch.egg-info/SOURCES.txt` & `tilt-pitch-1.1.0/tilt_pitch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

