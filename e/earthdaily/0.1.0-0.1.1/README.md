# Comparing `tmp/earthdaily-0.1.0.tar.gz` & `tmp/earthdaily-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "earthdaily-0.1.0.tar", last modified: Fri Apr 19 09:46:40 2024, max compression
+gzip compressed data, was "earthdaily-0.1.1.tar", last modified: Mon May 13 14:06:33 2024, max compression
```

## Comparing `earthdaily-0.1.0.tar` & `earthdaily-0.1.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:46:40.738356 earthdaily-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-19 09:46:40.000000 earthdaily-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4842 2024-04-19 09:46:40.738356 earthdaily-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-04-19 09:46:40.000000 earthdaily-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:46:40.734356 earthdaily-0.1.0/earthdaily/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-19 09:46:40.000000 earthdaily-0.1.0/earthdaily/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:46:40.734356 earthdaily-0.1.0/earthdaily/accessor/
--rw-r--r--   0 runner    (1001) docker     (127)     9473 2024-04-19 09:46:40.000000 earthdaily-0.1.0/earthdaily/accessor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:46:40.734356 earthdaily-0.1.0/earthdaily/accessor/whittaker/
--rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-04-19 09:46:40.000000 earthdaily-0.1.0/earthdaily/accessor/whittaker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7226 2024-04-19 09:46:40.000000 earthdaily-0.1.0/earthdaily/accessor/whittaker/_pywapor_core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:46:40.734356 earthdaily-0.1.0/earthdaily/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-19 09:46:40.000000 earthdaily-0.1.0/earthdaily/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:46:40.734356 earthdaily-0.1.0/earthdaily/datasets/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 09:46:40.000000 earthdaily-0.1.0/earthdaily/datasets/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-04-19 09:46:40.000000 earthdaily-0.1.0/earthdaily/datasets/data/pivot.geojson
--rw-r--r--   0 runner    (1001) docker     (127)     6517 2024-04-19 09:46:40.000000 earthdaily-0.1.0/earthdaily/datasets/data/pivot_corumba.geojson
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:46:40.734356 earthdaily-0.1.0/earthdaily/earthdatastore/
--rw-r--r--   0 runner    (1001) docker     (127)    37396 2024-04-19 09:46:40.000000 earthdaily-0.1.0/earthdaily/earthdatastore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-19 09:46:40.000000 earthdaily-0.1.0/earthdaily/earthdatastore/_scales_collections.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:46:40.734356 earthdaily-0.1.0/earthdaily/earthdatastore/cube_utils/
--rw-r--r--   0 runner    (1001) docker     (127)    15898 2024-04-19 09:46:40.000000 earthdaily-0.1.0/earthdaily/earthdatastore/cube_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7429 2024-04-19 09:46:40.000000 earthdaily-0.1.0/earthdaily/earthdatastore/cube_utils/_zonal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:46:40.738356 earthdaily-0.1.0/earthdaily/earthdatastore/cube_utils/asset_mapper/
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-04-19 09:46:40.000000 earthdaily-0.1.0/earthdaily/earthdatastore/cube_utils/asset_mapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-19 09:46:40.000000 earthdaily-0.1.0/earthdaily/earthdatastore/cube_utils/asset_mapper/__update_asset_mapper_config_json.py
--rw-r--r--   0 runner    (1001) docker     (127)    25336 2024-04-19 09:46:40.000000 earthdaily-0.1.0/earthdaily/earthdatastore/cube_utils/asset_mapper/asset_mapper_config.json
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-19 09:46:40.000000 earthdaily-0.1.0/earthdaily/earthdatastore/cube_utils/custom_reducers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-04-19 09:46:40.000000 earthdaily-0.1.0/earthdaily/earthdatastore/cube_utils/geometry_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:46:40.738356 earthdaily-0.1.0/earthdaily/earthdatastore/cube_utils/harmonizer/
--rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-04-19 09:46:40.000000 earthdaily-0.1.0/earthdaily/earthdatastore/cube_utils/harmonizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-19 09:46:40.000000 earthdaily-0.1.0/earthdaily/earthdatastore/cube_utils/preprocessing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:46:40.738356 earthdaily-0.1.0/earthdaily/earthdatastore/mask/
--rw-r--r--   0 runner    (1001) docker     (127)     7682 2024-04-19 09:46:40.000000 earthdaily-0.1.0/earthdaily/earthdatastore/mask/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:46:40.734356 earthdaily-0.1.0/earthdaily.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4842 2024-04-19 09:46:40.000000 earthdaily-0.1.0/earthdaily.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-19 09:46:40.000000 earthdaily-0.1.0/earthdaily.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 09:46:40.000000 earthdaily-0.1.0/earthdaily.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 09:46:40.000000 earthdaily-0.1.0/earthdaily.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-19 09:46:40.000000 earthdaily-0.1.0/earthdaily.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-19 09:46:40.000000 earthdaily-0.1.0/earthdaily.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 09:46:40.738356 earthdaily-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-04-19 09:46:40.000000 earthdaily-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:06:33.509983 earthdaily-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-13 14:06:33.000000 earthdaily-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4842 2024-05-13 14:06:33.509983 earthdaily-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-05-13 14:06:33.000000 earthdaily-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:06:33.505983 earthdaily-0.1.1/earthdaily/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-13 14:06:33.000000 earthdaily-0.1.1/earthdaily/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:06:33.505983 earthdaily-0.1.1/earthdaily/accessor/
+-rw-r--r--   0 runner    (1001) docker     (127)    10068 2024-05-13 14:06:33.000000 earthdaily-0.1.1/earthdaily/accessor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:06:33.505983 earthdaily-0.1.1/earthdaily/accessor/whittaker/
+-rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-05-13 14:06:33.000000 earthdaily-0.1.1/earthdaily/accessor/whittaker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7226 2024-05-13 14:06:33.000000 earthdaily-0.1.1/earthdaily/accessor/whittaker/_pywapor_core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:06:33.505983 earthdaily-0.1.1/earthdaily/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-13 14:06:33.000000 earthdaily-0.1.1/earthdaily/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:06:33.509983 earthdaily-0.1.1/earthdaily/datasets/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 14:06:33.000000 earthdaily-0.1.1/earthdaily/datasets/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-05-13 14:06:33.000000 earthdaily-0.1.1/earthdaily/datasets/data/pivot.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)     6517 2024-05-13 14:06:33.000000 earthdaily-0.1.1/earthdaily/datasets/data/pivot_corumba.geojson
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:06:33.509983 earthdaily-0.1.1/earthdaily/earthdatastore/
+-rw-r--r--   0 runner    (1001) docker     (127)    37428 2024-05-13 14:06:33.000000 earthdaily-0.1.1/earthdaily/earthdatastore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-13 14:06:33.000000 earthdaily-0.1.1/earthdaily/earthdatastore/_scales_collections.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:06:33.509983 earthdaily-0.1.1/earthdaily/earthdatastore/cube_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)    15898 2024-05-13 14:06:33.000000 earthdaily-0.1.1/earthdaily/earthdatastore/cube_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7429 2024-05-13 14:06:33.000000 earthdaily-0.1.1/earthdaily/earthdatastore/cube_utils/_zonal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:06:33.509983 earthdaily-0.1.1/earthdaily/earthdatastore/cube_utils/asset_mapper/
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-05-13 14:06:33.000000 earthdaily-0.1.1/earthdaily/earthdatastore/cube_utils/asset_mapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-13 14:06:33.000000 earthdaily-0.1.1/earthdaily/earthdatastore/cube_utils/asset_mapper/__update_asset_mapper_config_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25336 2024-05-13 14:06:33.000000 earthdaily-0.1.1/earthdaily/earthdatastore/cube_utils/asset_mapper/asset_mapper_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-13 14:06:33.000000 earthdaily-0.1.1/earthdaily/earthdatastore/cube_utils/custom_reducers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-05-13 14:06:33.000000 earthdaily-0.1.1/earthdaily/earthdatastore/cube_utils/geometry_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:06:33.509983 earthdaily-0.1.1/earthdaily/earthdatastore/cube_utils/harmonizer/
+-rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-05-13 14:06:33.000000 earthdaily-0.1.1/earthdaily/earthdatastore/cube_utils/harmonizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-13 14:06:33.000000 earthdaily-0.1.1/earthdaily/earthdatastore/cube_utils/preprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:06:33.509983 earthdaily-0.1.1/earthdaily/earthdatastore/mask/
+-rw-r--r--   0 runner    (1001) docker     (127)     7682 2024-05-13 14:06:33.000000 earthdaily-0.1.1/earthdaily/earthdatastore/mask/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:06:33.505983 earthdaily-0.1.1/earthdaily.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4842 2024-05-13 14:06:33.000000 earthdaily-0.1.1/earthdaily.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-13 14:06:33.000000 earthdaily-0.1.1/earthdaily.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 14:06:33.000000 earthdaily-0.1.1/earthdaily.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 14:06:33.000000 earthdaily-0.1.1/earthdaily.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-13 14:06:33.000000 earthdaily-0.1.1/earthdaily.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-13 14:06:33.000000 earthdaily-0.1.1/earthdaily.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 14:06:33.509983 earthdaily-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-13 14:06:33.000000 earthdaily-0.1.1/setup.py
```

### Comparing `earthdaily-0.1.0/LICENSE` & `earthdaily-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `earthdaily-0.1.0/PKG-INFO` & `earthdaily-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: earthdaily
-Version: 0.1.0
+Version: 0.1.1
 Summary: earthdaily: easy authentication, search and retrieval of Earth Data Store collections data
 Home-page: UNKNOWN
 Author: EarthDaily Agro
 License: MIT
 Keywords: Earth Data Store,earthdaily,earthdailyagro,stac
 Platform: UNKNOWN
 Requires-Python: >=3.10
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_pe8l2cfi_/tmpfxmddvj__TarContainer/0/2", line 25, column 36: Levels of opening and closing headings don't match*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: earthdaily Version: 0.1.0 Summary: earthdaily: easy
+Metadata-Version: 2.1 Name: earthdaily Version: 0.1.1 Summary: earthdaily: easy
 authentication, search and retrieval of Earth Data Store collections data Home-
 page: UNKNOWN Author: EarthDaily Agro License: MIT Keywords: Earth Data
 Store,earthdaily,earthdailyagro,stac Platform: UNKNOWN Requires-Python: >=3.10
 Description-Content-Type: text/markdown License-File: LICENSE
 
 ************ EEaarrtthhDDaaiillyy PPyytthhoonn CClliieenntt ************
 Your gateway to the Earth Data Store STAC Catalog.
```

### Comparing `earthdaily-0.1.0/README.md` & `earthdaily-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `earthdaily-0.1.0/earthdaily/accessor/__init__.py` & `earthdaily-0.1.1/earthdaily/accessor/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -125,14 +125,26 @@
 
     def clip(self, geom):
         return _xr_rio_clip(self._obj, geom)
 
     def _max_time_wrap(self, wish=5, col="time"):
         return np.min((wish, self._obj[col].size))
 
+    def drop_unfrozen_coords(self, keep_spatial_ref=True):
+        unfrozen_coords = [
+            coord
+            for coord in self._obj.coords
+            if coord not in list(self._obj.sizes.keys())
+        ]
+        if keep_spatial_ref and "spatial_ref" in unfrozen_coords:
+            unfrozen_coords.pop(
+                np.argwhere(np.in1d(unfrozen_coords, "spatial_ref"))[0][0]
+            )
+        return self._obj.drop(unfrozen_coords)
+
     def plot_rgb(
         self,
         red: str = "red",
         green: str = "green",
         blue: str = "blue",
         col="time",
         col_wrap=5,
@@ -286,25 +298,30 @@
         min_value: float = -np.inf,
         max_value: float = np.inf,
         max_iter: int = 10,
         time="time",
     ):
         from . import whittaker
 
-        return whittaker.xr_wt(
+        data_crs = self._obj.rio.crs
+
+        self._obj = whittaker.xr_wt(
             self._obj,
             lmbd,
             time=time,
             weights=weights,
             a=a,
             min_value=min_value,
             max_value=max_value,
             max_iter=max_iter,
         )
 
+        self._obj = self._obj.rio.set_crs(data_crs).rio.write_crs(data_crs)
+        return self._obj
+
     def zonal_stats(
         self,
         geometry,
         operations: list = ["mean"],
         raise_missing_geometry: bool = False,
     ):
         from ..earthdatastore.cube_utils import zonal_stats, GeometryManager
```

### Comparing `earthdaily-0.1.0/earthdaily/accessor/whittaker/__init__.py` & `earthdaily-0.1.1/earthdaily/accessor/whittaker/__init__.py`

 * *Files identical despite different names*

### Comparing `earthdaily-0.1.0/earthdaily/accessor/whittaker/_pywapor_core.py` & `earthdaily-0.1.1/earthdaily/accessor/whittaker/_pywapor_core.py`

 * *Files identical despite different names*

### Comparing `earthdaily-0.1.0/earthdaily/datasets/__init__.py` & `earthdaily-0.1.1/earthdaily/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `earthdaily-0.1.0/earthdaily/datasets/data/pivot.geojson` & `earthdaily-0.1.1/earthdaily/datasets/data/pivot.geojson`

 * *Files identical despite different names*

### Comparing `earthdaily-0.1.0/earthdaily/datasets/data/pivot_corumba.geojson` & `earthdaily-0.1.1/earthdaily/datasets/data/pivot_corumba.geojson`

 * *Files identical despite different names*

### Comparing `earthdaily-0.1.0/earthdaily/earthdatastore/__init__.py` & `earthdaily-0.1.1/earthdaily/earthdatastore/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -531,15 +531,15 @@
         mask_statistics: bool | int = False,
         clear_cover: (int | float) = None,
         prefer_alternate: (str | bool) = "download",
         search_kwargs: dict = {},
         add_default_scale_factor: bool = True,
         common_band_names=True,
         cross_calibration_collection: (None | str) = None,
-        properties: (bool | str | list) = None,
+        properties: (bool | str | list) = False,
         groupby_date: str = "mean",
         **kwargs,
     ) -> xr.Dataset:
         """
         Create a datacube.
 
         Parameters
@@ -603,15 +603,15 @@
         add_default_scale_factor : bool, optional
             DESCRIPTION. The default is True.
         common_band_names : TYPE, optional
             DESCRIPTION. The default is True.
         cross_calibration_collection : (None | str), optional
             DESCRIPTION. The default is None.
         properties : (bool | str | list), optional
-            Retrieve properties per item.
+            Retrieve properties per item. The default is False.
         **kwargs : TYPE
             DESCRIPTION.
          : TYPE
             DESCRIPTION.
 
         Raises
         ------
@@ -622,15 +622,15 @@
 
         Returns
         -------
         xr_datacube : TYPE
             DESCRIPTION.
 
         """
-        if properties is not None and groupby_date is not None:
+        if properties not in (None, False) and groupby_date is not None:
             raise NotImplementedError(
                 "You must set `groupby_date=None` to have properties per item."
             )
 
         if isinstance(collections, str):
             collections = [collections]
```

### Comparing `earthdaily-0.1.0/earthdaily/earthdatastore/_scales_collections.py` & `earthdaily-0.1.1/earthdaily/earthdatastore/_scales_collections.py`

 * *Files identical despite different names*

### Comparing `earthdaily-0.1.0/earthdaily/earthdatastore/cube_utils/__init__.py` & `earthdaily-0.1.1/earthdaily/earthdatastore/cube_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `earthdaily-0.1.0/earthdaily/earthdatastore/cube_utils/_zonal.py` & `earthdaily-0.1.1/earthdaily/earthdatastore/cube_utils/_zonal.py`

 * *Files identical despite different names*

### Comparing `earthdaily-0.1.0/earthdaily/earthdatastore/cube_utils/asset_mapper/__init__.py` & `earthdaily-0.1.1/earthdaily/earthdatastore/cube_utils/asset_mapper/__init__.py`

 * *Files identical despite different names*

### Comparing `earthdaily-0.1.0/earthdaily/earthdatastore/cube_utils/asset_mapper/__update_asset_mapper_config_json.py` & `earthdaily-0.1.1/earthdaily/earthdatastore/cube_utils/asset_mapper/__update_asset_mapper_config_json.py`

 * *Files identical despite different names*

### Comparing `earthdaily-0.1.0/earthdaily/earthdatastore/cube_utils/asset_mapper/asset_mapper_config.json` & `earthdaily-0.1.1/earthdaily/earthdatastore/cube_utils/asset_mapper/asset_mapper_config.json`

 * *Files identical despite different names*

### Comparing `earthdaily-0.1.0/earthdaily/earthdatastore/cube_utils/custom_reducers.py` & `earthdaily-0.1.1/earthdaily/earthdatastore/cube_utils/custom_reducers.py`

 * *Files identical despite different names*

### Comparing `earthdaily-0.1.0/earthdaily/earthdatastore/cube_utils/geometry_manager.py` & `earthdaily-0.1.1/earthdaily/earthdatastore/cube_utils/geometry_manager.py`

 * *Files identical despite different names*

### Comparing `earthdaily-0.1.0/earthdaily/earthdatastore/cube_utils/harmonizer/__init__.py` & `earthdaily-0.1.1/earthdaily/earthdatastore/cube_utils/harmonizer/__init__.py`

 * *Files identical despite different names*

### Comparing `earthdaily-0.1.0/earthdaily/earthdatastore/cube_utils/preprocessing.py` & `earthdaily-0.1.1/earthdaily/earthdatastore/cube_utils/preprocessing.py`

 * *Files identical despite different names*

### Comparing `earthdaily-0.1.0/earthdaily/earthdatastore/mask/__init__.py` & `earthdaily-0.1.1/earthdaily/earthdatastore/mask/__init__.py`

 * *Files identical despite different names*

### Comparing `earthdaily-0.1.0/earthdaily.egg-info/PKG-INFO` & `earthdaily-0.1.1/earthdaily.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: earthdaily
-Version: 0.1.0
+Version: 0.1.1
 Summary: earthdaily: easy authentication, search and retrieval of Earth Data Store collections data
 Home-page: UNKNOWN
 Author: EarthDaily Agro
 License: MIT
 Keywords: Earth Data Store,earthdaily,earthdailyagro,stac
 Platform: UNKNOWN
 Requires-Python: >=3.10
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_pe8l2cfi_/tmpfxmddvj__TarContainer/0/35", line 25, column 36: Levels of opening and closing headings don't match*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: earthdaily Version: 0.1.0 Summary: earthdaily: easy
+Metadata-Version: 2.1 Name: earthdaily Version: 0.1.1 Summary: earthdaily: easy
 authentication, search and retrieval of Earth Data Store collections data Home-
 page: UNKNOWN Author: EarthDaily Agro License: MIT Keywords: Earth Data
 Store,earthdaily,earthdailyagro,stac Platform: UNKNOWN Requires-Python: >=3.10
 Description-Content-Type: text/markdown License-File: LICENSE
 
 ************ EEaarrtthhDDaaiillyy PPyytthhoonn CClliieenntt ************
 Your gateway to the Earth Data Store STAC Catalog.
```

### Comparing `earthdaily-0.1.0/earthdaily.egg-info/SOURCES.txt` & `earthdaily-0.1.1/earthdaily.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `earthdaily-0.1.0/setup.py` & `earthdaily-0.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         "requests",
         "xarray",
         "rasterio",
         "rioxarray",
         "tqdm",
         "python-dotenv",
         "rich",
-        "dask",
+        "dask>=2024.5",
         "spyndex",
         "dask-image",
         "numba",
         "geocube"
     ],
     include_package_data=True,
     package_data={"":['*.geojson','*.json']},
```

