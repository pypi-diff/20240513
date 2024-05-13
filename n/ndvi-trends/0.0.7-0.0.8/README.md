# Comparing `tmp/ndvi_trends-0.0.7.tar.gz` & `tmp/ndvi_trends-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ndvi_trends-0.0.7.tar", last modified: Wed Apr 24 02:41:29 2024, max compression
+gzip compressed data, was "ndvi_trends-0.0.8.tar", last modified: Mon May 13 18:02:06 2024, max compression
```

## Comparing `ndvi_trends-0.0.7.tar` & `ndvi_trends-0.0.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 brookieguzder-williams   (501) staff       (20)        0 2024-04-24 02:41:29.880318 ndvi_trends-0.0.7/
--rw-r--r--   0 brookieguzder-williams   (501) staff       (20)     2193 2024-02-23 18:28:00.000000 ndvi_trends-0.0.7/LICENSE.md
--rw-r--r--   0 brookieguzder-williams   (501) staff       (20)     3127 2024-04-24 02:41:29.880264 ndvi_trends-0.0.7/PKG-INFO
--rw-r--r--   0 brookieguzder-williams   (501) staff       (20)     3006 2024-03-22 16:26:36.000000 ndvi_trends-0.0.7/README.md
-drwxr-xr-x   0 brookieguzder-williams   (501) staff       (20)        0 2024-04-24 02:41:29.878791 ndvi_trends-0.0.7/ndvi_trends/
--rw-r--r--   0 brookieguzder-williams   (501) staff       (20)       14 2024-03-22 16:16:19.000000 ndvi_trends-0.0.7/ndvi_trends/__init__.py
--rw-r--r--   0 brookieguzder-williams   (501) staff       (20)      262 2024-03-22 16:16:45.000000 ndvi_trends-0.0.7/ndvi_trends/calc.py
--rw-r--r--   0 brookieguzder-williams   (501) staff       (20)    11979 2024-03-31 16:45:05.000000 ndvi_trends-0.0.7/ndvi_trends/data.py
--rw-r--r--   0 brookieguzder-williams   (501) staff       (20)    22814 2024-04-24 02:37:00.000000 ndvi_trends-0.0.7/ndvi_trends/smoothing.py
-drwxr-xr-x   0 brookieguzder-williams   (501) staff       (20)        0 2024-04-24 02:41:29.879817 ndvi_trends-0.0.7/ndvi_trends/utils/
--rw-r--r--   0 brookieguzder-williams   (501) staff       (20)       14 2024-03-22 16:16:18.000000 ndvi_trends-0.0.7/ndvi_trends/utils/__init__.py
--rw-r--r--   0 brookieguzder-williams   (501) staff       (20)     2139 2024-03-22 16:16:54.000000 ndvi_trends-0.0.7/ndvi_trends/utils/ee.py
--rw-r--r--   0 brookieguzder-williams   (501) staff       (20)    10757 2024-04-22 18:29:55.000000 ndvi_trends-0.0.7/ndvi_trends/utils/npxr.py
-drwxr-xr-x   0 brookieguzder-williams   (501) staff       (20)        0 2024-04-24 02:41:29.880116 ndvi_trends-0.0.7/ndvi_trends.egg-info/
--rw-r--r--   0 brookieguzder-williams   (501) staff       (20)     3127 2024-04-24 02:41:29.000000 ndvi_trends-0.0.7/ndvi_trends.egg-info/PKG-INFO
--rw-r--r--   0 brookieguzder-williams   (501) staff       (20)      354 2024-04-24 02:41:29.000000 ndvi_trends-0.0.7/ndvi_trends.egg-info/SOURCES.txt
--rw-r--r--   0 brookieguzder-williams   (501) staff       (20)        1 2024-04-24 02:41:29.000000 ndvi_trends-0.0.7/ndvi_trends.egg-info/dependency_links.txt
--rw-r--r--   0 brookieguzder-williams   (501) staff       (20)       12 2024-04-24 02:41:29.000000 ndvi_trends-0.0.7/ndvi_trends.egg-info/top_level.txt
--rw-r--r--   0 brookieguzder-williams   (501) staff       (20)      240 2024-04-24 02:38:23.000000 ndvi_trends-0.0.7/pyproject.toml
--rw-r--r--   0 brookieguzder-williams   (501) staff       (20)      114 2024-04-24 02:41:29.880496 ndvi_trends-0.0.7/setup.cfg
+drwxr-xr-x   0 brookieguzder-williams   (501) staff       (20)        0 2024-05-13 18:02:06.725192 ndvi_trends-0.0.8/
+-rw-r--r--   0 brookieguzder-williams   (501) staff       (20)     2193 2024-02-23 18:28:00.000000 ndvi_trends-0.0.8/LICENSE.md
+-rw-r--r--   0 brookieguzder-williams   (501) staff       (20)     3127 2024-05-13 18:02:06.725135 ndvi_trends-0.0.8/PKG-INFO
+-rw-r--r--   0 brookieguzder-williams   (501) staff       (20)     3006 2024-03-22 16:26:36.000000 ndvi_trends-0.0.8/README.md
+drwxr-xr-x   0 brookieguzder-williams   (501) staff       (20)        0 2024-05-13 18:02:06.723162 ndvi_trends-0.0.8/ndvi_trends/
+-rw-r--r--   0 brookieguzder-williams   (501) staff       (20)       14 2024-03-22 16:16:19.000000 ndvi_trends-0.0.8/ndvi_trends/__init__.py
+-rw-r--r--   0 brookieguzder-williams   (501) staff       (20)      262 2024-03-22 16:16:45.000000 ndvi_trends-0.0.8/ndvi_trends/calc.py
+-rw-r--r--   0 brookieguzder-williams   (501) staff       (20)    11984 2024-05-13 17:24:21.000000 ndvi_trends-0.0.8/ndvi_trends/data.py
+-rw-r--r--   0 brookieguzder-williams   (501) staff       (20)    22906 2024-05-13 17:59:28.000000 ndvi_trends-0.0.8/ndvi_trends/smoothing.py
+drwxr-xr-x   0 brookieguzder-williams   (501) staff       (20)        0 2024-05-13 18:02:06.724547 ndvi_trends-0.0.8/ndvi_trends/utils/
+-rw-r--r--   0 brookieguzder-williams   (501) staff       (20)       14 2024-03-22 16:16:18.000000 ndvi_trends-0.0.8/ndvi_trends/utils/__init__.py
+-rw-r--r--   0 brookieguzder-williams   (501) staff       (20)     2139 2024-03-22 16:16:54.000000 ndvi_trends-0.0.8/ndvi_trends/utils/ee.py
+-rw-r--r--   0 brookieguzder-williams   (501) staff       (20)    10757 2024-04-22 18:29:55.000000 ndvi_trends-0.0.8/ndvi_trends/utils/npxr.py
+drwxr-xr-x   0 brookieguzder-williams   (501) staff       (20)        0 2024-05-13 18:02:06.724948 ndvi_trends-0.0.8/ndvi_trends.egg-info/
+-rw-r--r--   0 brookieguzder-williams   (501) staff       (20)     3127 2024-05-13 18:02:06.000000 ndvi_trends-0.0.8/ndvi_trends.egg-info/PKG-INFO
+-rw-r--r--   0 brookieguzder-williams   (501) staff       (20)      354 2024-05-13 18:02:06.000000 ndvi_trends-0.0.8/ndvi_trends.egg-info/SOURCES.txt
+-rw-r--r--   0 brookieguzder-williams   (501) staff       (20)        1 2024-05-13 18:02:06.000000 ndvi_trends-0.0.8/ndvi_trends.egg-info/dependency_links.txt
+-rw-r--r--   0 brookieguzder-williams   (501) staff       (20)       12 2024-05-13 18:02:06.000000 ndvi_trends-0.0.8/ndvi_trends.egg-info/top_level.txt
+-rw-r--r--   0 brookieguzder-williams   (501) staff       (20)      240 2024-05-13 18:01:18.000000 ndvi_trends-0.0.8/pyproject.toml
+-rw-r--r--   0 brookieguzder-williams   (501) staff       (20)      114 2024-05-13 18:02:06.725406 ndvi_trends-0.0.8/setup.cfg
```

### Comparing `ndvi_trends-0.0.7/LICENSE.md` & `ndvi_trends-0.0.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ndvi_trends-0.0.7/PKG-INFO` & `ndvi_trends-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ndvi_trends
-Version: 0.0.7
+Version: 0.0.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 #### NDVI TRENDS
 
 A module for studying NDVI Trends (from S2/LSAT) with a particular emphasis on determining or deriving relvant features for cover-cropping.
```

### Comparing `ndvi_trends-0.0.7/README.md` & `ndvi_trends-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `ndvi_trends-0.0.7/ndvi_trends/data.py` & `ndvi_trends-0.0.8/ndvi_trends/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 MAX_ERR = 1
 
 
 #
 # ASSETS
 #
 if EE_INITIALIZED:
-    S2 = ee.ImageCollection("COPERNICUS/S2_HARMONIZED")
+    S2 = ee.ImageCollection("COPERNICUS/S2_SR_HARMONIZED")
     S2_CSP = ee.ImageCollection("GOOGLE/CLOUD_SCORE_PLUS/V1/S2_HARMONIZED")
     HLSL = ee.ImageCollection("NASA/HLS/HLSL30/v002")
     FIELDS_FC = ee.FeatureCollection("projects/yield-predict/assets/KnoxFields")
 
 
 #
 # MAIN
@@ -112,15 +112,15 @@
         data_filter = ee.Filter.bounds(geom)
     else:
         data_filter = ee.Filter.And(
             ee.Filter.date(start_date, end_date),
             ee.Filter.bounds(geom))
     ndvi_ic = s2_lsat_ndvi_ic(data_filter)
     if source:
-        ndvi_i = ndvi_ic.filter(ee.Filter.eq('source', source))
+        ndvi_ic  = ndvi_ic.filter(ee.Filter.eq('source', source))
     ndvi_ic = ndvi_ic.sort('system:time_start')
     source_values = ndvi_ic.aggregate_array('source').getInfo()
     is_s2 = np.array([int(s == 'S2') for s in source_values])
     nb_s2 = is_s2.sum()
     nb_lsat = (1 - is_s2).sum()
     ds = get_ee_xrr(ndvi_ic, geom, attrs={'nb_s2': nb_s2, 'nb_landsat': nb_lsat})
     ds['is_sentinel_2'] = 'time', is_s2
```

### Comparing `ndvi_trends-0.0.7/ndvi_trends/smoothing.py` & `ndvi_trends-0.0.8/ndvi_trends/smoothing.py`

 * *Files 1% similar despite different names*

```diff
@@ -387,14 +387,19 @@
         smoothing_radius (int):
             radius used in `linear_window_smoothing`
 
     Returns:
         data with drops removed and replaced by nan
     """
     data = data.copy()
+    # compute if dask array
+    try:
+        data = data.compute()
+    except:
+        pass
     test_data = nan_mean_window_smoothing(data, radius=smoothing_radius)
     test = (data / test_data) < drop_threshold
     data[test] = np.nan
     return data
 
 
 @npxr
```

### Comparing `ndvi_trends-0.0.7/ndvi_trends/utils/ee.py` & `ndvi_trends-0.0.8/ndvi_trends/utils/ee.py`

 * *Files identical despite different names*

### Comparing `ndvi_trends-0.0.7/ndvi_trends/utils/npxr.py` & `ndvi_trends-0.0.8/ndvi_trends/utils/npxr.py`

 * *Files identical despite different names*

### Comparing `ndvi_trends-0.0.7/ndvi_trends.egg-info/PKG-INFO` & `ndvi_trends-0.0.8/ndvi_trends.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ndvi_trends
-Version: 0.0.7
+Version: 0.0.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 #### NDVI TRENDS
 
 A module for studying NDVI Trends (from S2/LSAT) with a particular emphasis on determining or deriving relvant features for cover-cropping.
```

