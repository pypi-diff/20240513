# Comparing `tmp/landcover_assignment-0.2.1.tar.gz` & `tmp/landcover_assignment-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "landcover_assignment-0.2.1.tar", max compression
+gzip compressed data, was "landcover_assignment-0.2.2.tar", max compression
```

## Comparing `landcover_assignment-0.2.1.tar` & `landcover_assignment-0.2.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1088 2023-05-25 19:51:14.000000 landcover_assignment-0.2.1/LICENSE
--rw-r--r--   0        0        0     5207 2024-04-29 07:30:36.759766 landcover_assignment-0.2.1/README.md
--rw-r--r--   0        0        0      479 2024-04-29 07:30:36.775766 landcover_assignment-0.2.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-21 12:33:17.659500 landcover_assignment-0.2.1/src/landcover_assignment/__init__.py
--rw-r--r--   0        0        0     7671 2024-02-21 12:33:17.659500 landcover_assignment-0.2.1/src/landcover_assignment/afforestation.py
--rw-r--r--   0        0        0      222 2024-02-21 12:33:17.659500 landcover_assignment-0.2.1/src/landcover_assignment/database/__init__.py
--rw-r--r--   0        0        0   102400 2024-04-29 07:30:36.775766 landcover_assignment-0.2.1/src/landcover_assignment/database/land_use_database.db
--rw-r--r--   0        0        0    10270 2024-02-21 12:33:17.659500 landcover_assignment-0.2.1/src/landcover_assignment/distribution.py
--rw-r--r--   0        0        0        0 2024-02-21 12:33:17.659500 landcover_assignment-0.2.1/src/landcover_assignment/geo_landcover_assignment/__init__.py
--rw-r--r--   0        0        0    23520 2024-02-21 12:33:17.659500 landcover_assignment-0.2.1/src/landcover_assignment/geo_landcover_assignment/catchment_landcover.py
--rw-r--r--   0        0        0     7652 2024-02-21 12:33:17.659500 landcover_assignment-0.2.1/src/landcover_assignment/geo_landcover_assignment/geo_afforestation.py
--rw-r--r--   0        0        0     9690 2024-02-21 12:33:17.659500 landcover_assignment-0.2.1/src/landcover_assignment/geo_landcover_assignment/geo_distribution.py
--rw-r--r--   0        0        0    20183 2024-02-21 12:33:17.659500 landcover_assignment-0.2.1/src/landcover_assignment/geo_landcover_assignment/geo_landcover.py
--rw-r--r--   0        0        0     8483 2024-02-21 12:33:17.659500 landcover_assignment-0.2.1/src/landcover_assignment/geo_landcover_assignment/geo_transition_matrix.py
--rw-r--r--   0        0        0    22423 2024-02-21 12:33:17.659500 landcover_assignment-0.2.1/src/landcover_assignment/landcover.py
--rw-r--r--   0        0        0     4390 2024-02-21 12:33:17.663501 landcover_assignment-0.2.1/src/landcover_assignment/landcover_data_manager.py
--rw-r--r--   0        0        0    31010 2024-02-21 12:33:17.663501 landcover_assignment-0.2.1/src/landcover_assignment/national_landcover.py
--rw-r--r--   0        0        0        0 2024-02-21 12:33:17.663501 landcover_assignment-0.2.1/src/landcover_assignment/resource_manager/__init__.py
--rw-r--r--   0        0        0     3516 2024-02-21 12:33:17.663501 landcover_assignment-0.2.1/src/landcover_assignment/resource_manager/data_loader.py
--rw-r--r--   0        0        0     5746 2024-02-21 12:33:17.663501 landcover_assignment-0.2.1/src/landcover_assignment/resource_manager/database_manager.py
--rw-r--r--   0        0        0     5994 2024-02-21 12:33:17.663501 landcover_assignment-0.2.1/src/landcover_assignment/resource_manager/scenario_data_fetcher.py
--rw-r--r--   0        0        0    17134 2024-02-21 12:33:17.663501 landcover_assignment-0.2.1/src/landcover_assignment/resource_manager/transition_data_fetcher.py
--rw-r--r--   0        0        0     8034 2024-02-12 13:07:15.410030 landcover_assignment-0.2.1/src/landcover_assignment/transition_matrix.py
--rw-r--r--   0        0        0     5842 1970-01-01 00:00:00.000000 landcover_assignment-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1088 2023-05-25 19:51:14.000000 landcover_assignment-0.2.2/LICENSE
+-rw-r--r--   0        0        0     5207 2024-04-29 07:30:36.759766 landcover_assignment-0.2.2/README.md
+-rw-r--r--   0        0        0      478 2024-05-13 10:41:12.665489 landcover_assignment-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-02-21 12:33:17.659500 landcover_assignment-0.2.2/src/landcover_assignment/__init__.py
+-rw-r--r--   0        0        0     7671 2024-02-21 12:33:17.659500 landcover_assignment-0.2.2/src/landcover_assignment/afforestation.py
+-rw-r--r--   0        0        0      222 2024-02-21 12:33:17.659500 landcover_assignment-0.2.2/src/landcover_assignment/database/__init__.py
+-rw-r--r--   0        0        0   102400 2024-04-29 07:30:36.775766 landcover_assignment-0.2.2/src/landcover_assignment/database/land_use_database.db
+-rw-r--r--   0        0        0    10270 2024-02-21 12:33:17.659500 landcover_assignment-0.2.2/src/landcover_assignment/distribution.py
+-rw-r--r--   0        0        0        0 2024-02-21 12:33:17.659500 landcover_assignment-0.2.2/src/landcover_assignment/geo_landcover_assignment/__init__.py
+-rw-r--r--   0        0        0    26151 2024-05-13 10:41:12.665489 landcover_assignment-0.2.2/src/landcover_assignment/geo_landcover_assignment/catchment_landcover.py
+-rw-r--r--   0        0        0     7652 2024-02-21 12:33:17.659500 landcover_assignment-0.2.2/src/landcover_assignment/geo_landcover_assignment/geo_afforestation.py
+-rw-r--r--   0        0        0     9690 2024-02-21 12:33:17.659500 landcover_assignment-0.2.2/src/landcover_assignment/geo_landcover_assignment/geo_distribution.py
+-rw-r--r--   0        0        0    20183 2024-02-21 12:33:17.659500 landcover_assignment-0.2.2/src/landcover_assignment/geo_landcover_assignment/geo_landcover.py
+-rw-r--r--   0        0        0     8483 2024-02-21 12:33:17.659500 landcover_assignment-0.2.2/src/landcover_assignment/geo_landcover_assignment/geo_transition_matrix.py
+-rw-r--r--   0        0        0    22423 2024-02-21 12:33:17.659500 landcover_assignment-0.2.2/src/landcover_assignment/landcover.py
+-rw-r--r--   0        0        0     4390 2024-02-21 12:33:17.663500 landcover_assignment-0.2.2/src/landcover_assignment/landcover_data_manager.py
+-rw-r--r--   0        0        0    31010 2024-02-21 12:33:17.663500 landcover_assignment-0.2.2/src/landcover_assignment/national_landcover.py
+-rw-r--r--   0        0        0        0 2024-02-21 12:33:17.663500 landcover_assignment-0.2.2/src/landcover_assignment/resource_manager/__init__.py
+-rw-r--r--   0        0        0     3516 2024-02-21 12:33:17.663500 landcover_assignment-0.2.2/src/landcover_assignment/resource_manager/data_loader.py
+-rw-r--r--   0        0        0     5746 2024-02-21 12:33:17.663500 landcover_assignment-0.2.2/src/landcover_assignment/resource_manager/database_manager.py
+-rw-r--r--   0        0        0     5994 2024-02-21 12:33:17.663500 landcover_assignment-0.2.2/src/landcover_assignment/resource_manager/scenario_data_fetcher.py
+-rw-r--r--   0        0        0    17134 2024-02-21 12:33:17.663500 landcover_assignment-0.2.2/src/landcover_assignment/resource_manager/transition_data_fetcher.py
+-rw-r--r--   0        0        0     8034 2024-02-12 13:07:15.410030 landcover_assignment-0.2.2/src/landcover_assignment/transition_matrix.py
+-rw-r--r--   0        0        0     5835 1970-01-01 00:00:00.000000 landcover_assignment-0.2.2/PKG-INFO
```

### Comparing `landcover_assignment-0.2.1/LICENSE` & `landcover_assignment-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `landcover_assignment-0.2.1/README.md` & `landcover_assignment-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `landcover_assignment-0.2.1/src/landcover_assignment/afforestation.py` & `landcover_assignment-0.2.2/src/landcover_assignment/afforestation.py`

 * *Files identical despite different names*

### Comparing `landcover_assignment-0.2.1/src/landcover_assignment/database/land_use_database.db` & `landcover_assignment-0.2.2/src/landcover_assignment/database/land_use_database.db`

 * *Files identical despite different names*

### Comparing `landcover_assignment-0.2.1/src/landcover_assignment/distribution.py` & `landcover_assignment-0.2.2/src/landcover_assignment/distribution.py`

 * *Files identical despite different names*

### Comparing `landcover_assignment-0.2.1/src/landcover_assignment/geo_landcover_assignment/catchment_landcover.py` & `landcover_assignment-0.2.2/src/landcover_assignment/geo_landcover_assignment/catchment_landcover.py`

 * *Files 11% similar despite different names*

```diff
@@ -104,102 +104,138 @@
         :param catchment: The name of the catchment area.
         :type catchment: str
         :return: A pandas DataFrame summarizing the forest area details.
         :rtype: pd.DataFrame
         """
         forest_df = self.api.get_catchment_forest_data_by_catchment_name(catchment)
 
+        # Check if the DataFrame is empty
+        if forest_df.empty:
+            summary_data = {
+                'area_ha': 0,
+                'share_mineral': 0,
+                'share_organic': 0,
+                'share_organic_mineral': 0,
+                'share_burnt': 0  # Assuming a default value; replace with an appropriate call if needed
+            }
+            return pd.DataFrame([summary_data])
+
         # Filter for specific types of forests and then group
         forest_types = ['Broadleaved Forest and Woodland', 'Coniferous Forest', 'Mixed Forest']
         filtered_df = forest_df[forest_df['cover_type'].isin(forest_types)]
         grouped_df = filtered_df.groupby(['cover_type', 'soil_type']).sum()
 
-        # Calculating totals for different soil types
+        # Safely get totals for different soil types, using 0 if the category is missing
         total_area = grouped_df['total_hectares'].sum()
-        total_mineral = grouped_df.xs('mineral', level='soil_type')['total_hectares'].sum() + \
-                        grouped_df.xs('misc', level='soil_type')['total_hectares'].sum()
-        total_peat = grouped_df.xs('peat', level='soil_type')['total_hectares'].sum()
-        total_mineral_peat = grouped_df.xs('peaty_mineral', level='soil_type')['total_hectares'].sum()
+        total_mineral = grouped_df.xs('mineral', level='soil_type')['total_hectares'].sum() if 'mineral' in grouped_df.index.get_level_values('soil_type') else 0
+        total_mineral += grouped_df.xs('misc', level='soil_type')['total_hectares'].sum() if 'misc' in grouped_df.index.get_level_values('soil_type') else 0
+        total_peat = grouped_df.xs('peat', level='soil_type')['total_hectares'].sum() if 'peat' in grouped_df.index.get_level_values('soil_type') else 0
+        total_mineral_peat = grouped_df.xs('peaty_mineral', level='soil_type')['total_hectares'].sum() if 'peaty_mineral' in grouped_df.index.get_level_values('soil_type') else 0
 
-        # Creating a summary DataFrame
+        # Calculating shares, ensuring no division by zero
         summary_data = {
             'area_ha': total_area,
-            'share_mineral': total_mineral / total_area,
-            'share_organic': total_peat / total_area,
-            'share_organic_mineral': total_mineral_peat / total_area,
+            'share_mineral': total_mineral / total_area if total_area != 0 else 0,
+            'share_organic': total_peat / total_area if total_area != 0 else 0,
+            'share_organic_mineral': total_mineral_peat / total_area if total_area != 0 else 0,
             'share_burnt': self.get_national_burnt_average('forest')
         }
 
         return pd.DataFrame([summary_data])
+
     
 
     def get_catchment_peat_area(self, catchment):
         """
         Calculates the total organic area within a specified catchment, grouped by cover and soil types.
 
         :param catchment: The name of the catchment area.
         :type catchment: str
         :return: A pandas DataFrame summarizing the peat area details.
         :rtype: pd.DataFrame
         """
         peat_df = self.api.get_catchment_peat_data_by_catchment_name(catchment)
 
-        # Filter
+        # Check if the DataFrame is empty
+        if peat_df.empty:
+            summary_data = {
+                'area_ha': 0,
+                'share_mineral': 0,
+                'share_organic': 0,
+                'share_organic_mineral': 0,
+                'share_burnt': 0  # Assuming a default value; replace with an appropriate call if needed
+            }
+            return pd.DataFrame([summary_data])
+        
+        # Filter and group by cover and soil types
         grouped_df = peat_df.groupby(['cover_type', 'soil_type']).sum()
 
-        # Calculating totals for different soil types
+        # Safely get totals for different soil types, using 0 if the category is missing
         total_area = grouped_df['total_hectares'].sum()
-        total_mineral = grouped_df.xs('mineral', level='soil_type')['total_hectares'].sum() + \
-                        grouped_df.xs('misc', level='soil_type')['total_hectares'].sum()
-        total_peat = grouped_df.xs('peat', level='soil_type')['total_hectares'].sum()
-        total_mineral_peat = grouped_df.xs('peaty_mineral', level='soil_type')['total_hectares'].sum()
+        total_mineral = grouped_df.xs('mineral', level='soil_type')['total_hectares'].sum() if 'mineral' in grouped_df.index.get_level_values('soil_type') else 0
+        total_mineral += grouped_df.xs('misc', level='soil_type')['total_hectares'].sum() if 'misc' in grouped_df.index.get_level_values('soil_type') else 0
+        total_peat = grouped_df.xs('peat', level='soil_type')['total_hectares'].sum() if 'peat' in grouped_df.index.get_level_values('soil_type') else 0
+        total_mineral_peat = grouped_df.xs('peaty_mineral', level='soil_type')['total_hectares'].sum() if 'peaty_mineral' in grouped_df.index.get_level_values('soil_type') else 0
 
-        # Creating a summary DataFrame
+        # Calculating shares, ensuring no division by zero
         summary_data = {
             'area_ha': total_area,
-            'share_mineral': total_mineral / total_area,
-            'share_organic': total_peat / total_area,
-            'share_organic_mineral': total_mineral_peat / total_area,
+            'share_mineral': total_mineral / total_area if total_area != 0 else 0,
+            'share_organic': total_peat / total_area if total_area != 0 else 0,
+            'share_organic_mineral': total_mineral_peat / total_area if total_area != 0 else 0,
             'share_burnt': self.get_national_burnt_average('wetland')
         }
 
         return pd.DataFrame([summary_data])
+
     
 
     def get_catchment_crop_area(self, catchment):
         """
         Calculates the total crop area within a specified catchment, grouped by cover and soil types.
 
         :param catchment: The name of the catchment area.
         :type catchment: str
         :return: A pandas DataFrame summarizing the crop area details.
         :rtype: pd.DataFrame
         """
         cultivated_df = self.api.get_catchment_cultivated_data_by_catchment_name(catchment)
 
-        # Filter    
+        # Check if the DataFrame is empty
+        if cultivated_df.empty:
+            summary_data = {
+                'area_ha': 0,
+                'share_mineral': 0,
+                'share_organic': 0,
+                'share_organic_mineral': 0,
+                'share_burnt': 0  # Assuming a default value; replace with an appropriate call if needed
+            }
+            return pd.DataFrame([summary_data])
+        
+        # Filter and group by cover and soil types
         grouped_df = cultivated_df.groupby(['cover_type', 'soil_type']).sum()
 
-        # Calculating totals for different soil types
+        # Safely get totals for different soil types, using 0 if the category is missing
         total_area = grouped_df['total_hectares'].sum()
-        total_mineral = grouped_df.xs('mineral', level='soil_type')['total_hectares'].sum() + \
-                        grouped_df.xs('misc', level='soil_type')['total_hectares'].sum()
-        total_peat = grouped_df.xs('peat', level='soil_type')['total_hectares'].sum()
-        total_mineral_peat = grouped_df.xs('peaty_mineral', level='soil_type')['total_hectares'].sum()
+        total_mineral = grouped_df.xs('mineral', level='soil_type')['total_hectares'].sum() if 'mineral' in grouped_df.index.get_level_values('soil_type') else 0
+        total_mineral += grouped_df.xs('misc', level='soil_type')['total_hectares'].sum() if 'misc' in grouped_df.index.get_level_values('soil_type') else 0
+        total_peat = grouped_df.xs('peat', level='soil_type')['total_hectares'].sum() if 'peat' in grouped_df.index.get_level_values('soil_type') else 0
+        total_mineral_peat = grouped_df.xs('peaty_mineral', level='soil_type')['total_hectares'].sum() if 'peaty_mineral' in grouped_df.index.get_level_values('soil_type') else 0
 
-        # Creating a summary DataFrame
+        # Calculating shares, ensuring no division by zero
         summary_data = {
             'area_ha': total_area,
-            'share_mineral': total_mineral / total_area,
-            'share_organic': total_peat / total_area,
-            'share_organic_mineral': total_mineral_peat / total_area,
-            'share_burnt': self.get_national_burnt_average('cropland') 
+            'share_mineral': total_mineral / total_area if total_area != 0 else 0,
+            'share_organic': total_peat / total_area if total_area != 0 else 0,
+            'share_organic_mineral': total_mineral_peat / total_area if total_area != 0 else 0,
+            'share_burnt': self.get_national_burnt_average('cropland')
         }
 
         return pd.DataFrame([summary_data])
+
     
 
     def get_catchment_grassland_area(self, catchment, total_grassland_area):
         """
         Calculates the total grassland area within a specified catchment, using additional grassland area data from the 
         grassland_production package.
 
@@ -241,17 +277,17 @@
                 total_peat += summed_df.loc[soil].sum()
             elif soil == 'peaty_mineral':
                 total_mineral_peat += summed_df.loc[soil].sum()
 
         # Creating a summary DataFrame
         summary_data = {
             'area_ha': derived_grassland_area,
-            'share_mineral': total_mineral / total_area,
-            'share_organic': total_peat / total_area,
-            'share_organic_mineral': total_mineral_peat / total_area,
+            'share_mineral': total_mineral / total_area if total_area != 0 else 0,
+            'share_organic': total_peat / total_area if total_area != 0 else 0,
+            'share_organic_mineral': total_mineral_peat / total_area if total_area != 0 else 0,
             'share_burnt': self.get_national_burnt_average('grassland')
         }
 
         return pd.DataFrame([summary_data])
 
 
     def get_landuse_area(self, landuse, catchment, grassland_area=None):
```

### Comparing `landcover_assignment-0.2.1/src/landcover_assignment/geo_landcover_assignment/geo_afforestation.py` & `landcover_assignment-0.2.2/src/landcover_assignment/geo_landcover_assignment/geo_afforestation.py`

 * *Files identical despite different names*

### Comparing `landcover_assignment-0.2.1/src/landcover_assignment/geo_landcover_assignment/geo_distribution.py` & `landcover_assignment-0.2.2/src/landcover_assignment/geo_landcover_assignment/geo_distribution.py`

 * *Files identical despite different names*

### Comparing `landcover_assignment-0.2.1/src/landcover_assignment/geo_landcover_assignment/geo_landcover.py` & `landcover_assignment-0.2.2/src/landcover_assignment/geo_landcover_assignment/geo_landcover.py`

 * *Files identical despite different names*

### Comparing `landcover_assignment-0.2.1/src/landcover_assignment/geo_landcover_assignment/geo_transition_matrix.py` & `landcover_assignment-0.2.2/src/landcover_assignment/geo_landcover_assignment/geo_transition_matrix.py`

 * *Files identical despite different names*

### Comparing `landcover_assignment-0.2.1/src/landcover_assignment/landcover.py` & `landcover_assignment-0.2.2/src/landcover_assignment/landcover.py`

 * *Files identical despite different names*

### Comparing `landcover_assignment-0.2.1/src/landcover_assignment/landcover_data_manager.py` & `landcover_assignment-0.2.2/src/landcover_assignment/landcover_data_manager.py`

 * *Files identical despite different names*

### Comparing `landcover_assignment-0.2.1/src/landcover_assignment/national_landcover.py` & `landcover_assignment-0.2.2/src/landcover_assignment/national_landcover.py`

 * *Files identical despite different names*

### Comparing `landcover_assignment-0.2.1/src/landcover_assignment/resource_manager/data_loader.py` & `landcover_assignment-0.2.2/src/landcover_assignment/resource_manager/data_loader.py`

 * *Files identical despite different names*

### Comparing `landcover_assignment-0.2.1/src/landcover_assignment/resource_manager/database_manager.py` & `landcover_assignment-0.2.2/src/landcover_assignment/resource_manager/database_manager.py`

 * *Files identical despite different names*

### Comparing `landcover_assignment-0.2.1/src/landcover_assignment/resource_manager/scenario_data_fetcher.py` & `landcover_assignment-0.2.2/src/landcover_assignment/resource_manager/scenario_data_fetcher.py`

 * *Files identical despite different names*

### Comparing `landcover_assignment-0.2.1/src/landcover_assignment/resource_manager/transition_data_fetcher.py` & `landcover_assignment-0.2.2/src/landcover_assignment/resource_manager/transition_data_fetcher.py`

 * *Files identical despite different names*

### Comparing `landcover_assignment-0.2.1/src/landcover_assignment/transition_matrix.py` & `landcover_assignment-0.2.2/src/landcover_assignment/transition_matrix.py`

 * *Files identical despite different names*

### Comparing `landcover_assignment-0.2.1/PKG-INFO` & `landcover_assignment-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: landcover_assignment
-Version: 0.2.1
+Version: 0.2.2
 Summary: A goblin tool for the generation of areas of alternative land uses based on spared area available
 License: MIT
 Author: Colm Duffy
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: catchment_data_api (>=0.1.0,<0.2.0)
+Requires-Dist: catchment_data_api (==0.1.1)
 Requires-Dist: numpy (>=1.25.0,<2.0.0)
 Requires-Dist: pandas (==2.1.4)
 Requires-Dist: sqlalchemy (>=1.4.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # 🏘️🌳🌲🌽🍀 Land cover generator for the GOBLIN model (Ireland only)
 [![license](https://img.shields.io/badge/License-MIT-red)](https://github.com/GOBLIN-Proj/landcover_assignment/blob/0.1.0/LICENSE)
```

