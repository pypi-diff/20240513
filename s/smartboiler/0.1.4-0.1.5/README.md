# Comparing `tmp/smartboiler-0.1.4.tar.gz` & `tmp/smartboiler-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartboiler-0.1.4.tar", last modified: Mon May 13 16:27:10 2024, max compression
+gzip compressed data, was "smartboiler-0.1.5.tar", last modified: Mon May 13 16:49:03 2024, max compression
```

## Comparing `smartboiler-0.1.4.tar` & `smartboiler-0.1.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:27:10.869680 smartboiler-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-13 16:27:10.869680 smartboiler-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-13 16:27:06.000000 smartboiler-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 16:27:10.869680 smartboiler-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-13 16:27:09.000000 smartboiler-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:27:10.865680 smartboiler-0.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:27:10.869680 smartboiler-0.1.4/src/smartboiler/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-13 16:27:06.000000 smartboiler-0.1.4/src/smartboiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13942 2024-05-13 16:27:06.000000 smartboiler-0.1.4/src/smartboiler/boiler.py
--rw-r--r--   0 runner    (1001) docker     (127)    10412 2024-05-13 16:27:06.000000 smartboiler-0.1.4/src/smartboiler/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)    32021 2024-05-13 16:27:06.000000 smartboiler-0.1.4/src/smartboiler/data_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5584 2024-05-13 16:27:06.000000 smartboiler-0.1.4/src/smartboiler/event_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)    15307 2024-05-13 16:27:06.000000 smartboiler-0.1.4/src/smartboiler/forecast.py
--rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-05-13 16:27:06.000000 smartboiler-0.1.4/src/smartboiler/fotovoltaics.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 16:27:06.000000 smartboiler-0.1.4/src/smartboiler/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-05-13 16:27:06.000000 smartboiler-0.1.4/src/smartboiler/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-13 16:27:06.000000 smartboiler-0.1.4/src/smartboiler/time_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:27:10.869680 smartboiler-0.1.4/src/smartboiler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-13 16:27:10.000000 smartboiler-0.1.4/src/smartboiler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-13 16:27:10.000000 smartboiler-0.1.4/src/smartboiler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 16:27:10.000000 smartboiler-0.1.4/src/smartboiler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-13 16:27:10.000000 smartboiler-0.1.4/src/smartboiler.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-13 16:27:10.000000 smartboiler-0.1.4/src/smartboiler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-13 16:27:10.000000 smartboiler-0.1.4/src/smartboiler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:49:03.340579 smartboiler-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-13 16:49:03.340579 smartboiler-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-13 16:49:01.000000 smartboiler-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 16:49:03.340579 smartboiler-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-13 16:49:02.000000 smartboiler-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:49:03.336579 smartboiler-0.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:49:03.336579 smartboiler-0.1.5/src/smartboiler/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-13 16:49:01.000000 smartboiler-0.1.5/src/smartboiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13942 2024-05-13 16:49:01.000000 smartboiler-0.1.5/src/smartboiler/boiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10412 2024-05-13 16:49:01.000000 smartboiler-0.1.5/src/smartboiler/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32013 2024-05-13 16:49:01.000000 smartboiler-0.1.5/src/smartboiler/data_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5584 2024-05-13 16:49:01.000000 smartboiler-0.1.5/src/smartboiler/event_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15569 2024-05-13 16:49:01.000000 smartboiler-0.1.5/src/smartboiler/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-05-13 16:49:01.000000 smartboiler-0.1.5/src/smartboiler/fotovoltaics.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 16:49:01.000000 smartboiler-0.1.5/src/smartboiler/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-05-13 16:49:01.000000 smartboiler-0.1.5/src/smartboiler/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-13 16:49:01.000000 smartboiler-0.1.5/src/smartboiler/time_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:49:03.340579 smartboiler-0.1.5/src/smartboiler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-13 16:49:03.000000 smartboiler-0.1.5/src/smartboiler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-13 16:49:03.000000 smartboiler-0.1.5/src/smartboiler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 16:49:03.000000 smartboiler-0.1.5/src/smartboiler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-13 16:49:03.000000 smartboiler-0.1.5/src/smartboiler.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-13 16:49:03.000000 smartboiler-0.1.5/src/smartboiler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-13 16:49:03.000000 smartboiler-0.1.5/src/smartboiler.egg-info/top_level.txt
```

### Comparing `smartboiler-0.1.4/PKG-INFO` & `smartboiler-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartboiler
-Version: 0.1.4
+Version: 0.1.5
 Summary: Smart boiling of household
 Home-page: https://github.com/grinwi/smartboiler
 Author: Adam GRUNWALD
 Author-email: grunwald.adam24@gmail.com
 Keywords: energy,management,optimization,hass
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `smartboiler-0.1.4/README.md` & `smartboiler-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `smartboiler-0.1.4/setup.py` & `smartboiler-0.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
 
 setup(
     name="smartboiler",  # Required
-    version="0.1.4",  # Required
+    version="0.1.5",  # Required
     description="Smart boiling of household",  # Optional
     long_description=long_description,  # Optional
     long_description_content_type="text/markdown",  # Optional (see note above)
     url="https://github.com/grinwi/smartboiler",  # Optional
     author="Adam GRUNWALD",  # Optional
     author_email="grunwald.adam24@gmail.com",  # Optional
     classifiers=[  # Optional
```

### Comparing `smartboiler-0.1.4/src/smartboiler/boiler.py` & `smartboiler-0.1.5/src/smartboiler/boiler.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.1.4/src/smartboiler/controller.py` & `smartboiler-0.1.5/src/smartboiler/controller.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.1.4/src/smartboiler/data_handler.py` & `smartboiler-0.1.5/src/smartboiler/data_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -703,21 +703,21 @@
         df = df[
             [
                 "longtime_mean",
                 "last_3_week_skew",
                 "last_3_week_std",
                 "distance_from_home",
                 "speed_towards_home",
-                # "distance_from_home_2",
-                # "speed_towards_home_2",
+                "distance_from_home_2",
+                "speed_towards_home_2",
                 "count",
                 "heading_to_home_sin",
                 "heading_to_home_cos",
-                # "heading_to_home_sin_2",
-                # "heading_to_home_cos_2",
+                "heading_to_home_sin_2",
+                "heading_to_home_cos_2",
                 "temperature",
                 "humidity",
                 "wind_speed",
                 "weekday_sin",
                 "weekday_cos",
                 "hour_sin",
                 "hour_cos",
```

### Comparing `smartboiler-0.1.4/src/smartboiler/event_checker.py` & `smartboiler-0.1.5/src/smartboiler/event_checker.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.1.4/src/smartboiler/forecast.py` & `smartboiler-0.1.5/src/smartboiler/forecast.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,15 +43,15 @@
             predicted_columns (Optional[list], optional): List of columns for prediction. Defaults to None.
         """
         self.batch_size = 16
         self.lookback = 32
         self.delay = 1
         self.step = 1
 
-        self.num_of_features = 14
+        self.num_of_features = 18
 
         self.predicted_columns = predicted_columns
         self.dataHandler = dataHandler
         self.scaler = RobustScaler()
         self.start_of_data = start_of_data
 
         self.model_path = model_path
@@ -215,20 +215,24 @@
             data=[
                 [
                     predicted_value,  # longtime_mean
                     prev_week_values[1],  # 3 week skew
                     prev_week_values[2],  # 3 weeak std
                     last_row_values[3],  # distance_from_home
                     last_row_values[4],  # speed_towards_home
-                    last_row_values[5],  # count
-                    last_row_values[6],  # heading to home sin
-                    last_row_values[7],  # heading to home cos
-                    last_row_values[8],  # temperature
-                    last_row_values[9],  # humidity
-                    last_row_values[10],  # wind_speed
+                    last_row_values[5],  # distance_from_home 2
+                    last_row_values[6],  # speed_towards_home 2
+                    last_row_values[7],  # count
+                    last_row_values[8],  # heading to home sin
+                    last_row_values[9],  # heading to home cos
+                    last_row_values[10],  # heading to home sin 2
+                    last_row_values[11],  # heading to home cos 2
+                    last_row_values[12],  # temperature
+                    last_row_values[13],  # humidity
+                    last_row_values[14],  # wind_speed
                     np.sin(2 * np.pi * date_time.weekday() / 7),
                     np.cos(2 * np.pi * date_time.weekday() / 7),
                     np.sin(2 * np.pi * date_time.hour / 24),
                     np.cos(2 * np.pi * date_time.hour / 24),
                 ]
             ],
         )
```

### Comparing `smartboiler-0.1.4/src/smartboiler/fotovoltaics.py` & `smartboiler-0.1.5/src/smartboiler/fotovoltaics.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.1.4/src/smartboiler/switch.py` & `smartboiler-0.1.5/src/smartboiler/switch.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.1.4/src/smartboiler/time_handler.py` & `smartboiler-0.1.5/src/smartboiler/time_handler.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.1.4/src/smartboiler.egg-info/PKG-INFO` & `smartboiler-0.1.5/src/smartboiler.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartboiler
-Version: 0.1.4
+Version: 0.1.5
 Summary: Smart boiling of household
 Home-page: https://github.com/grinwi/smartboiler
 Author: Adam GRUNWALD
 Author-email: grunwald.adam24@gmail.com
 Keywords: energy,management,optimization,hass
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `smartboiler-0.1.4/src/smartboiler.egg-info/SOURCES.txt` & `smartboiler-0.1.5/src/smartboiler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

