# Comparing `tmp/pdemtools-0.7.0.tar.gz` & `tmp/pdemtools-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdemtools-0.7.0.tar", last modified: Tue Apr 23 20:56:47 2024, max compression
+gzip compressed data, was "pdemtools-0.8.0.tar", last modified: Mon May 13 10:53:17 2024, max compression
```

## Comparing `pdemtools-0.7.0.tar` & `pdemtools-0.8.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2024-04-23 20:56:47.212802 pdemtools-0.7.0/
--rw-r--r--   0 tom        (501) staff       (20)     1068 2023-04-15 08:23:32.000000 pdemtools-0.7.0/LICENSE.md
--rw-r--r--   0 tom        (501) staff       (20)    23086 2024-04-23 20:56:47.212536 pdemtools-0.7.0/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)    21865 2024-04-21 17:32:26.000000 pdemtools-0.7.0/README.md
--rw-r--r--   0 tom        (501) staff       (20)     1484 2024-04-18 08:02:27.000000 pdemtools-0.7.0/pyproject.toml
--rw-r--r--   0 tom        (501) staff       (20)       38 2024-04-23 20:56:47.212852 pdemtools-0.7.0/setup.cfg
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2024-04-23 20:56:47.162209 pdemtools-0.7.0/src/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2024-04-23 20:56:47.167199 pdemtools-0.7.0/src/pdemtools/
--rw-r--r--   0 tom        (501) staff       (20)      208 2024-04-21 17:14:32.000000 pdemtools-0.7.0/src/pdemtools/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)    22424 2024-04-21 17:27:33.000000 pdemtools-0.7.0/src/pdemtools/_accessor.py
--rw-r--r--   0 tom        (501) staff       (20)    13288 2024-02-08 12:17:31.000000 pdemtools-0.7.0/src/pdemtools/_coreg.py
--rw-r--r--   0 tom        (501) staff       (20)     7754 2023-05-09 15:54:10.000000 pdemtools-0.7.0/src/pdemtools/_geomorphometry.py
--rw-r--r--   0 tom        (501) staff       (20)     9026 2024-02-16 17:10:57.000000 pdemtools-0.7.0/src/pdemtools/_index_search.py
--rw-r--r--   0 tom        (501) staff       (20)     2281 2024-01-18 15:17:17.000000 pdemtools-0.7.0/src/pdemtools/_utils.py
--rw-r--r--   0 tom        (501) staff       (20)     4784 2024-02-16 17:09:38.000000 pdemtools-0.7.0/src/pdemtools/data.py
--rw-r--r--   0 tom        (501) staff       (20)    13963 2024-04-21 17:55:33.000000 pdemtools-0.7.0/src/pdemtools/load.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2024-04-23 20:56:47.200306 pdemtools-0.7.0/src/pdemtools/mosaic_index/
--rw-r--r--   0 tom        (501) staff       (20)  8540160 2024-02-08 12:15:11.000000 pdemtools-0.7.0/src/pdemtools/mosaic_index/ArcticDEM_Mosaic_Index_v3_gpkg.gpkg
--rwx------   0 tom        (501) staff       (20)  8552448 2023-08-18 15:41:04.000000 pdemtools-0.7.0/src/pdemtools/mosaic_index/ArcticDEM_Mosaic_Index_v4_1_gpkg.gpkg
--rw-r--r--   0 tom        (501) staff       (20)  5177344 2023-04-27 17:43:28.000000 pdemtools-0.7.0/src/pdemtools/mosaic_index/REMA_Mosaic_Index_v2_gpkg.gpkg
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2024-04-23 20:56:47.206391 pdemtools-0.7.0/src/pdemtools/test_data/
--rw-r--r--   0 tom        (501) staff       (20)    91756 2024-04-14 15:24:36.000000 pdemtools-0.7.0/src/pdemtools/test_data/test_arcticdem_index_kiv_steenstrup.parquet
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2024-04-23 20:56:47.212183 pdemtools-0.7.0/src/pdemtools.egg-info/
--rw-r--r--   0 tom        (501) staff       (20)    23086 2024-04-23 20:56:47.000000 pdemtools-0.7.0/src/pdemtools.egg-info/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)      751 2024-04-23 20:56:47.000000 pdemtools-0.7.0/src/pdemtools.egg-info/SOURCES.txt
--rw-r--r--   0 tom        (501) staff       (20)        1 2024-04-23 20:56:47.000000 pdemtools-0.7.0/src/pdemtools.egg-info/dependency_links.txt
--rw-r--r--   0 tom        (501) staff       (20)       89 2024-04-23 20:56:47.000000 pdemtools-0.7.0/src/pdemtools.egg-info/requires.txt
--rw-r--r--   0 tom        (501) staff       (20)       10 2024-04-23 20:56:47.000000 pdemtools-0.7.0/src/pdemtools.egg-info/top_level.txt
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2024-04-23 20:56:47.211892 pdemtools-0.7.0/tests/
--rw-r--r--   0 tom        (501) staff       (20)      509 2024-04-14 15:24:36.000000 pdemtools-0.7.0/tests/test_download.py
--rw-r--r--   0 tom        (501) staff       (20)     4613 2024-04-14 15:24:36.000000 pdemtools-0.7.0/tests/test_processing.py
--rw-r--r--   0 tom        (501) staff       (20)      638 2024-04-14 15:24:36.000000 pdemtools-0.7.0/tests/test_search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:53:17.760110 pdemtools-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-13 10:53:13.000000 pdemtools-0.8.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6833 2024-05-13 10:53:17.760110 pdemtools-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5612 2024-05-13 10:53:13.000000 pdemtools-0.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-05-13 10:53:13.000000 pdemtools-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 10:53:17.760110 pdemtools-0.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:53:17.728110 pdemtools-0.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:53:17.732110 pdemtools-0.8.0/src/pdemtools/
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-13 10:53:13.000000 pdemtools-0.8.0/src/pdemtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23580 2024-05-13 10:53:13.000000 pdemtools-0.8.0/src/pdemtools/_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13288 2024-05-13 10:53:13.000000 pdemtools-0.8.0/src/pdemtools/_coreg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7754 2024-05-13 10:53:13.000000 pdemtools-0.8.0/src/pdemtools/_geomorphometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9026 2024-05-13 10:53:13.000000 pdemtools-0.8.0/src/pdemtools/_index_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-05-13 10:53:13.000000 pdemtools-0.8.0/src/pdemtools/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-05-13 10:53:13.000000 pdemtools-0.8.0/src/pdemtools/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13963 2024-05-13 10:53:13.000000 pdemtools-0.8.0/src/pdemtools/load.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:53:17.752110 pdemtools-0.8.0/src/pdemtools/mosaic_index/
+-rw-r--r--   0 runner    (1001) docker     (127)  8540160 2024-05-13 10:53:13.000000 pdemtools-0.8.0/src/pdemtools/mosaic_index/ArcticDEM_Mosaic_Index_v3_gpkg.gpkg
+-rwxr-xr-x   0 runner    (1001) docker     (127)  8552448 2024-05-13 10:53:13.000000 pdemtools-0.8.0/src/pdemtools/mosaic_index/ArcticDEM_Mosaic_Index_v4_1_gpkg.gpkg
+-rw-r--r--   0 runner    (1001) docker     (127)  5177344 2024-05-13 10:53:13.000000 pdemtools-0.8.0/src/pdemtools/mosaic_index/REMA_Mosaic_Index_v2_gpkg.gpkg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:53:17.760110 pdemtools-0.8.0/src/pdemtools/test_data/
+-rw-r--r--   0 runner    (1001) docker     (127)    91756 2024-05-13 10:53:13.000000 pdemtools-0.8.0/src/pdemtools/test_data/test_arcticdem_index_kiv_steenstrup.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:53:17.760110 pdemtools-0.8.0/src/pdemtools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6833 2024-05-13 10:53:17.000000 pdemtools-0.8.0/src/pdemtools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-13 10:53:17.000000 pdemtools-0.8.0/src/pdemtools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 10:53:17.000000 pdemtools-0.8.0/src/pdemtools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-13 10:53:17.000000 pdemtools-0.8.0/src/pdemtools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-13 10:53:17.000000 pdemtools-0.8.0/src/pdemtools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:53:17.760110 pdemtools-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-13 10:53:13.000000 pdemtools-0.8.0/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4613 2024-05-13 10:53:13.000000 pdemtools-0.8.0/tests/test_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-13 10:53:13.000000 pdemtools-0.8.0/tests/test_search.py
```

### Comparing `pdemtools-0.7.0/LICENSE.md` & `pdemtools-0.8.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pdemtools-0.7.0/pyproject.toml` & `pdemtools-0.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdemtools-0.7.0/src/pdemtools/_accessor.py` & `pdemtools-0.8.0/src/pdemtools/_accessor.py`

 * *Files 6% similar despite different names*

```diff
@@ -406,31 +406,36 @@
         return xds
 
     def mask_ocean(
         self,
         candidate_height_thresh_m: Optional[float] = 10,
         candidate_area_thresh_km2: Optional[float] = 1,
         near_sealevel_thresh_m: Optional[float] = 5,
+        return_sealevel_as_zero: Optional[bool] = False,
         return_mask: Optional[bool] = False,
     ) -> DataArray:
         """Returns a DEM with mélange/ocean regions filtered out, adapting the method
         of Shiggins _et al._ (2023). If no likely sea level is identified, returns the
         original DEM.
 
         WARNING: The DEM must be geoid-corrected for this function to work correctly.
 
         :param candidate_height_thresh_m: Maximum value relative to geoid to be considered
             as SL, in m, defaults to 10
         :type candidate_height_thresh_m: float
         :param candidate_area_thresh_km2: Minimum area beneath `candidate_height_thresh_m`
-            to be considered for sea level assessment, in km^2, defaults to 1
+            to be considered for sea level assessment, in km^2. Defaults to 1
         :type candidate_area_thresh_km2: float
         :param near_sealevel_thresh_m: Filter out regions below this value, in metres above
-            sea level, defaults to 5
+            sea level. Defaults to 5
         :type near_sealevel_thresh_m: float
+        :param return_sealevel_as_zero: If True, subtracts that estimated sea level from
+            the DEM, returning new height values with the estimated sea level set to 0
+            m. Necessary for calculating accurate iceberg heights. Defaults to False.
+        :type return_sealevel_as_zero: bool
         :param return_mask: Return the sea level mask rather than the masked DEM.
             Defaults to False.
         :type return_mask: bool
 
         :returns: Filtered DEM as xarray DataArray
         :rtype: DataArray
         """
@@ -453,21 +458,25 @@
         else:
             mask = self._obj > (est_sea_level + near_sealevel_thresh_m)
 
         if return_mask == True:
             if mask == None:
                 warn("No sea level detected in image. Returning `None` as mask object.")
             return mask
-
         else:
             if mask is None:
                 warn("No sea level detected in image. Returning original DEM")
                 return self._obj
             else:
-                return self._obj.where(mask)
+                if return_sealevel_as_zero == True:
+                    return self._obj.where(mask) - est_sea_level
+                elif return_sealevel_as_zero == False:
+                    return self._obj.where(mask)
+                else:
+                    raise ValueError("return_sealevel_as_zero must be True or False")
 
     def get_sea_level(
         self,
         candidate_height_thresh_m: Optional[float] = 10,
         candidate_area_thresh_km2: Optional[float] = 1,
     ) -> float:
         """Returns estimated sea level following method of Shiggins _et al._ (2023). If no
@@ -516,14 +525,21 @@
         connectivity: Literal[4, 8] = 4,
     ) -> DataArray:
         """After masking the ocean using the `mask_ocean()` function, icebergs will
         remain. This function gives you the opportunity to mask them as well by
         identifying the size of connected groups of pixels and masking above/below a
         threshold.
 
+        By default, this function masks icebergs and retains terrestrial ice/land.
+        However, by setting `retain_icebergs = True`, the function will instead mask
+        ice/land and retain icebergs, allowing iceberg area and volume to be assessed.
+        For accurate volume assessment, the DEM 0 m value must be set to the estimated
+        sea level height from the `get_sea_level()` function.  This can be automated by
+        setting `return_sealevel_as_zero = True` in the mask_ocean() function.
+
         :param area_thresh_m2: Size threshold between icebergs and terrestrial ice/land, in
             m2. Defaults to 1e6 m2 (1 km2)
         :type area_thresh_m2: float | int
         :param retain_icerbergs: By default, this function masks icebergs and retains
             terrestrial ice/land (by masking pixel groups below the threshold area). By
             switching the parameter to True, the function will instead mask out larger
             pixel groups and retain the smaller icebergs.
```

### Comparing `pdemtools-0.7.0/src/pdemtools/_coreg.py` & `pdemtools-0.8.0/src/pdemtools/_coreg.py`

 * *Files identical despite different names*

### Comparing `pdemtools-0.7.0/src/pdemtools/_geomorphometry.py` & `pdemtools-0.8.0/src/pdemtools/_geomorphometry.py`

 * *Files identical despite different names*

### Comparing `pdemtools-0.7.0/src/pdemtools/_index_search.py` & `pdemtools-0.8.0/src/pdemtools/_index_search.py`

 * *Files identical despite different names*

### Comparing `pdemtools-0.7.0/src/pdemtools/_utils.py` & `pdemtools-0.8.0/src/pdemtools/_utils.py`

 * *Files identical despite different names*

### Comparing `pdemtools-0.7.0/src/pdemtools/data.py` & `pdemtools-0.8.0/src/pdemtools/data.py`

 * *Files identical despite different names*

### Comparing `pdemtools-0.7.0/src/pdemtools/load.py` & `pdemtools-0.8.0/src/pdemtools/load.py`

 * *Files identical despite different names*

### Comparing `pdemtools-0.7.0/src/pdemtools/mosaic_index/ArcticDEM_Mosaic_Index_v3_gpkg.gpkg` & `pdemtools-0.8.0/src/pdemtools/mosaic_index/ArcticDEM_Mosaic_Index_v3_gpkg.gpkg`

 * *Files identical despite different names*

### Comparing `pdemtools-0.7.0/src/pdemtools/mosaic_index/ArcticDEM_Mosaic_Index_v4_1_gpkg.gpkg` & `pdemtools-0.8.0/src/pdemtools/mosaic_index/ArcticDEM_Mosaic_Index_v4_1_gpkg.gpkg`

 * *Files identical despite different names*

### Comparing `pdemtools-0.7.0/src/pdemtools/mosaic_index/REMA_Mosaic_Index_v2_gpkg.gpkg` & `pdemtools-0.8.0/src/pdemtools/mosaic_index/REMA_Mosaic_Index_v2_gpkg.gpkg`

 * *Files identical despite different names*

### Comparing `pdemtools-0.7.0/src/pdemtools/test_data/test_arcticdem_index_kiv_steenstrup.parquet` & `pdemtools-0.8.0/src/pdemtools/test_data/test_arcticdem_index_kiv_steenstrup.parquet`

 * *Files identical despite different names*

### Comparing `pdemtools-0.7.0/src/pdemtools.egg-info/SOURCES.txt` & `pdemtools-0.8.0/src/pdemtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pdemtools-0.7.0/tests/test_processing.py` & `pdemtools-0.8.0/tests/test_processing.py`

 * *Files identical despite different names*

### Comparing `pdemtools-0.7.0/tests/test_search.py` & `pdemtools-0.8.0/tests/test_search.py`

 * *Files identical despite different names*

