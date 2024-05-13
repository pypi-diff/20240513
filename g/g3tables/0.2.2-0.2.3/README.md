# Comparing `tmp/g3tables-0.2.2.tar.gz` & `tmp/g3tables-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "g3tables-0.2.2.tar", last modified: Sat May  4 20:13:16 2024, max compression
+gzip compressed data, was "g3tables-0.2.3.tar", last modified: Mon May 13 09:41:58 2024, max compression
```

## Comparing `g3tables-0.2.2.tar` & `g3tables-0.2.3.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 20:13:16.488160 g3tables-0.2.2/
--rw-rw-rw-   0        0        0     1091 2024-04-29 08:48:33.000000 g3tables-0.2.2/LICENCE
--rw-rw-rw-   0        0        0     1325 2024-05-04 20:13:16.488160 g3tables-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0       81 2024-04-29 08:48:33.000000 g3tables-0.2.2/README.md
--rw-rw-rw-   0        0        0     1679 2024-05-02 05:59:12.000000 g3tables-0.2.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-04 20:13:16.488160 g3tables-0.2.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-04 20:13:16.387880 g3tables-0.2.2/src/
-drwxrwxrwx   0        0        0        0 2024-05-04 20:13:16.403516 g3tables-0.2.2/src/g3tables/
--rw-rw-rw-   0        0        0      550 2024-04-29 08:48:33.000000 g3tables-0.2.2/src/g3tables/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-04 20:13:16.434757 g3tables-0.2.2/src/g3tables/plc_composition_io_table/
--rw-rw-rw-   0        0        0      361 2024-04-29 08:48:33.000000 g3tables-0.2.2/src/g3tables/plc_composition_io_table/__init__.py
--rw-rw-rw-   0        0        0    14539 2024-04-29 08:48:33.000000 g3tables-0.2.2/src/g3tables/plc_composition_io_table/_extend_table.py
--rw-rw-rw-   0        0        0    21360 2024-04-30 11:02:43.000000 g3tables-0.2.2/src/g3tables/plc_composition_io_table/_table.py
--rw-rw-rw-   0        0        0     5780 2024-04-29 08:48:33.000000 g3tables-0.2.2/src/g3tables/plc_composition_io_table/io_signals.json
--rw-rw-rw-   0        0        0        0 2024-04-29 08:48:33.000000 g3tables-0.2.2/src/g3tables/py.typed
-drwxrwxrwx   0        0        0        0 2024-05-04 20:13:16.434757 g3tables-0.2.2/src/g3tables/sw_definition_table/
--rw-rw-rw-   0        0        0      182 2024-04-29 08:48:33.000000 g3tables-0.2.2/src/g3tables/sw_definition_table/__init__.py
--rw-rw-rw-   0        0        0    54470 2024-04-30 11:02:43.000000 g3tables-0.2.2/src/g3tables/sw_definition_table/_table.py
-drwxrwxrwx   0        0        0        0 2024-05-04 20:13:16.450378 g3tables-0.2.2/src/g3tables/system_config/
--rw-rw-rw-   0        0        0      225 2024-04-29 08:48:33.000000 g3tables-0.2.2/src/g3tables/system_config/__init__.py
--rw-rw-rw-   0        0        0    15259 2024-04-30 11:02:43.000000 g3tables-0.2.2/src/g3tables/system_config/_cli.py
--rw-rw-rw-   0        0        0    22338 2024-04-30 11:02:43.000000 g3tables-0.2.2/src/g3tables/system_config/_g3core_updater.py
--rw-rw-rw-   0        0        0      972 2024-04-30 11:02:43.000000 g3tables-0.2.2/src/g3tables/system_config/_hw_connections.py
--rw-rw-rw-   0        0        0     8599 2024-04-30 11:02:43.000000 g3tables-0.2.2/src/g3tables/system_config/_iomap_updater.py
--rw-rw-rw-   0        0        0       74 2024-04-29 08:48:33.000000 g3tables-0.2.2/src/g3tables/system_config/_logger.py
--rw-rw-rw-   0        0        0     7326 2024-04-30 11:02:43.000000 g3tables-0.2.2/src/g3tables/system_config/_sw_system_dict_wrapper.py
--rw-rw-rw-   0        0        0     4132 2024-04-29 08:48:33.000000 g3tables-0.2.2/src/g3tables/system_config/_system_config_processor.py
--rw-rw-rw-   0        0        0     1192 2024-04-29 08:48:33.000000 g3tables-0.2.2/src/g3tables/system_config/type_hinting.py
-drwxrwxrwx   0        0        0        0 2024-05-04 20:13:16.472517 g3tables-0.2.2/src/g3tables/utils/
--rw-rw-rw-   0        0        0      146 2024-04-29 08:48:33.000000 g3tables-0.2.2/src/g3tables/utils/__init__.py
--rw-rw-rw-   0        0        0     1552 2024-04-29 08:48:33.000000 g3tables-0.2.2/src/g3tables/utils/_d2nd.py
--rw-rw-rw-   0        0        0     3706 2024-04-29 08:48:33.000000 g3tables-0.2.2/src/g3tables/utils/_interval.py
-drwxrwxrwx   0        0        0        0 2024-05-04 20:13:16.472517 g3tables-0.2.2/src/g3tables/utils/gdrive/
--rw-rw-rw-   0        0        0      365 2024-04-29 08:48:33.000000 g3tables-0.2.2/src/g3tables/utils/gdrive/__init__.py
--rw-rw-rw-   0        0        0     5172 2024-04-29 08:48:33.000000 g3tables-0.2.2/src/g3tables/utils/gdrive/_gdrive.py
--rw-rw-rw-   0        0        0     1263 2024-04-29 08:48:33.000000 g3tables-0.2.2/src/g3tables/utils/gdrive/_update_creds.py
-drwxrwxrwx   0        0        0        0 2024-05-04 20:13:16.472517 g3tables-0.2.2/src/g3tables/visualization_table/
--rw-rw-rw-   0        0        0      207 2024-04-29 08:48:33.000000 g3tables-0.2.2/src/g3tables/visualization_table/__init__.py
--rw-rw-rw-   0        0        0    14819 2024-04-30 13:14:34.000000 g3tables-0.2.2/src/g3tables/visualization_table/_table.py
-drwxrwxrwx   0        0        0        0 2024-05-04 20:13:16.488160 g3tables-0.2.2/src/g3tables.egg-info/
--rw-rw-rw-   0        0        0     1325 2024-05-04 20:13:16.000000 g3tables-0.2.2/src/g3tables.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1290 2024-05-04 20:13:16.000000 g3tables-0.2.2/src/g3tables.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 20:13:16.000000 g3tables-0.2.2/src/g3tables.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      207 2024-05-04 20:13:16.000000 g3tables-0.2.2/src/g3tables.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       79 2024-05-04 20:13:16.000000 g3tables-0.2.2/src/g3tables.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-04 20:13:16.000000 g3tables-0.2.2/src/g3tables.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-13 09:41:58.776576 g3tables-0.2.3/
+-rw-rw-rw-   0        0        0     1091 2024-04-29 08:48:33.000000 g3tables-0.2.3/LICENCE
+-rw-rw-rw-   0        0        0     1325 2024-05-13 09:41:58.776576 g3tables-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0       81 2024-04-29 08:48:33.000000 g3tables-0.2.3/README.md
+-rw-rw-rw-   0        0        0     1679 2024-05-13 09:39:47.000000 g3tables-0.2.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-13 09:41:58.776576 g3tables-0.2.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-13 09:41:58.698450 g3tables-0.2.3/src/
+drwxrwxrwx   0        0        0        0 2024-05-13 09:41:58.714093 g3tables-0.2.3/src/g3tables/
+-rw-rw-rw-   0        0        0      550 2024-04-29 08:48:33.000000 g3tables-0.2.3/src/g3tables/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 09:41:58.729703 g3tables-0.2.3/src/g3tables/plc_composition_io_table/
+-rw-rw-rw-   0        0        0      361 2024-04-29 08:48:33.000000 g3tables-0.2.3/src/g3tables/plc_composition_io_table/__init__.py
+-rw-rw-rw-   0        0        0    14539 2024-04-29 08:48:33.000000 g3tables-0.2.3/src/g3tables/plc_composition_io_table/_extend_table.py
+-rw-rw-rw-   0        0        0    21360 2024-04-30 11:02:43.000000 g3tables-0.2.3/src/g3tables/plc_composition_io_table/_table.py
+-rw-rw-rw-   0        0        0     5780 2024-04-29 08:48:33.000000 g3tables-0.2.3/src/g3tables/plc_composition_io_table/io_signals.json
+-rw-rw-rw-   0        0        0        0 2024-04-29 08:48:33.000000 g3tables-0.2.3/src/g3tables/py.typed
+drwxrwxrwx   0        0        0        0 2024-05-13 09:41:58.729703 g3tables-0.2.3/src/g3tables/sw_definition_table/
+-rw-rw-rw-   0        0        0      182 2024-04-29 08:48:33.000000 g3tables-0.2.3/src/g3tables/sw_definition_table/__init__.py
+-rw-rw-rw-   0        0        0    54470 2024-05-13 09:37:12.000000 g3tables-0.2.3/src/g3tables/sw_definition_table/_table.py
+drwxrwxrwx   0        0        0        0 2024-05-13 09:41:58.745326 g3tables-0.2.3/src/g3tables/system_config/
+-rw-rw-rw-   0        0        0      225 2024-04-29 08:48:33.000000 g3tables-0.2.3/src/g3tables/system_config/__init__.py
+-rw-rw-rw-   0        0        0    15259 2024-05-13 09:37:18.000000 g3tables-0.2.3/src/g3tables/system_config/_cli.py
+-rw-rw-rw-   0        0        0    22338 2024-04-30 11:02:43.000000 g3tables-0.2.3/src/g3tables/system_config/_g3core_updater.py
+-rw-rw-rw-   0        0        0      972 2024-04-30 11:02:43.000000 g3tables-0.2.3/src/g3tables/system_config/_hw_connections.py
+-rw-rw-rw-   0        0        0     8599 2024-04-30 11:02:43.000000 g3tables-0.2.3/src/g3tables/system_config/_iomap_updater.py
+-rw-rw-rw-   0        0        0       74 2024-04-29 08:48:33.000000 g3tables-0.2.3/src/g3tables/system_config/_logger.py
+-rw-rw-rw-   0        0        0     7326 2024-04-30 11:02:43.000000 g3tables-0.2.3/src/g3tables/system_config/_sw_system_dict_wrapper.py
+-rw-rw-rw-   0        0        0     4132 2024-04-29 08:48:33.000000 g3tables-0.2.3/src/g3tables/system_config/_system_config_processor.py
+-rw-rw-rw-   0        0        0     1192 2024-04-29 08:48:33.000000 g3tables-0.2.3/src/g3tables/system_config/type_hinting.py
+drwxrwxrwx   0        0        0        0 2024-05-13 09:41:58.745326 g3tables-0.2.3/src/g3tables/utils/
+-rw-rw-rw-   0        0        0      146 2024-04-29 08:48:33.000000 g3tables-0.2.3/src/g3tables/utils/__init__.py
+-rw-rw-rw-   0        0        0     1552 2024-04-29 08:48:33.000000 g3tables-0.2.3/src/g3tables/utils/_d2nd.py
+-rw-rw-rw-   0        0        0     3706 2024-04-29 08:48:33.000000 g3tables-0.2.3/src/g3tables/utils/_interval.py
+drwxrwxrwx   0        0        0        0 2024-05-13 09:41:58.760955 g3tables-0.2.3/src/g3tables/utils/gdrive/
+-rw-rw-rw-   0        0        0      365 2024-04-29 08:48:33.000000 g3tables-0.2.3/src/g3tables/utils/gdrive/__init__.py
+-rw-rw-rw-   0        0        0     5172 2024-04-29 08:48:33.000000 g3tables-0.2.3/src/g3tables/utils/gdrive/_gdrive.py
+-rw-rw-rw-   0        0        0     1263 2024-04-29 08:48:33.000000 g3tables-0.2.3/src/g3tables/utils/gdrive/_update_creds.py
+drwxrwxrwx   0        0        0        0 2024-05-13 09:41:58.760955 g3tables-0.2.3/src/g3tables/visualization_table/
+-rw-rw-rw-   0        0        0      207 2024-04-29 08:48:33.000000 g3tables-0.2.3/src/g3tables/visualization_table/__init__.py
+-rw-rw-rw-   0        0        0    14812 2024-05-12 17:57:40.000000 g3tables-0.2.3/src/g3tables/visualization_table/_table.py
+drwxrwxrwx   0        0        0        0 2024-05-13 09:41:58.760955 g3tables-0.2.3/src/g3tables.egg-info/
+-rw-rw-rw-   0        0        0     1325 2024-05-13 09:41:58.000000 g3tables-0.2.3/src/g3tables.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1290 2024-05-13 09:41:58.000000 g3tables-0.2.3/src/g3tables.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 09:41:58.000000 g3tables-0.2.3/src/g3tables.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      207 2024-05-13 09:41:58.000000 g3tables-0.2.3/src/g3tables.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       79 2024-05-13 09:41:58.000000 g3tables-0.2.3/src/g3tables.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-13 09:41:58.000000 g3tables-0.2.3/src/g3tables.egg-info/top_level.txt
```

### Comparing `g3tables-0.2.2/LICENCE` & `g3tables-0.2.3/LICENCE`

 * *Files identical despite different names*

### Comparing `g3tables-0.2.2/PKG-INFO` & `g3tables-0.2.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g3tables
-Version: 0.2.2
+Version: 0.2.3
 Summary: G3 SW Definition, HW and PLC components, and Visualisation tables parser
 Author: Elektroline a.s.
 Project-URL: Homepage, https://gitlab.elektroline.cz/plc/systemg3-py/SystemG3Tables
 Keywords: Elektroline,Google Drive,Project table
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Other Audience
```

### Comparing `g3tables-0.2.2/pyproject.toml` & `g3tables-0.2.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "g3tables"
-version = "0.2.2"
+version = "0.2.3"
 description = "G3 SW Definition, HW and PLC components, and Visualisation tables parser"
 readme = "README.md"
 license = {file = "LICENSE"}
 authors = [
   { name="Elektroline a.s." },
 ]
 classifiers = [
```

### Comparing `g3tables-0.2.2/src/g3tables/__init__.py` & `g3tables-0.2.3/src/g3tables/__init__.py`

 * *Files identical despite different names*

### Comparing `g3tables-0.2.2/src/g3tables/plc_composition_io_table/_extend_table.py` & `g3tables-0.2.3/src/g3tables/plc_composition_io_table/_extend_table.py`

 * *Files identical despite different names*

### Comparing `g3tables-0.2.2/src/g3tables/plc_composition_io_table/_table.py` & `g3tables-0.2.3/src/g3tables/plc_composition_io_table/_table.py`

 * *Files identical despite different names*

### Comparing `g3tables-0.2.2/src/g3tables/plc_composition_io_table/io_signals.json` & `g3tables-0.2.3/src/g3tables/plc_composition_io_table/io_signals.json`

 * *Files identical despite different names*

### Comparing `g3tables-0.2.2/src/g3tables/sw_definition_table/_table.py` & `g3tables-0.2.3/src/g3tables/sw_definition_table/_table.py`

 * *Files identical despite different names*

### Comparing `g3tables-0.2.2/src/g3tables/system_config/_cli.py` & `g3tables-0.2.3/src/g3tables/system_config/_cli.py`

 * *Files identical despite different names*

### Comparing `g3tables-0.2.2/src/g3tables/system_config/_g3core_updater.py` & `g3tables-0.2.3/src/g3tables/system_config/_g3core_updater.py`

 * *Files identical despite different names*

### Comparing `g3tables-0.2.2/src/g3tables/system_config/_hw_connections.py` & `g3tables-0.2.3/src/g3tables/system_config/_hw_connections.py`

 * *Files identical despite different names*

### Comparing `g3tables-0.2.2/src/g3tables/system_config/_iomap_updater.py` & `g3tables-0.2.3/src/g3tables/system_config/_iomap_updater.py`

 * *Files identical despite different names*

### Comparing `g3tables-0.2.2/src/g3tables/system_config/_sw_system_dict_wrapper.py` & `g3tables-0.2.3/src/g3tables/system_config/_sw_system_dict_wrapper.py`

 * *Files identical despite different names*

### Comparing `g3tables-0.2.2/src/g3tables/system_config/_system_config_processor.py` & `g3tables-0.2.3/src/g3tables/system_config/_system_config_processor.py`

 * *Files identical despite different names*

### Comparing `g3tables-0.2.2/src/g3tables/system_config/type_hinting.py` & `g3tables-0.2.3/src/g3tables/system_config/type_hinting.py`

 * *Files identical despite different names*

### Comparing `g3tables-0.2.2/src/g3tables/utils/_d2nd.py` & `g3tables-0.2.3/src/g3tables/utils/_d2nd.py`

 * *Files identical despite different names*

### Comparing `g3tables-0.2.2/src/g3tables/utils/_interval.py` & `g3tables-0.2.3/src/g3tables/utils/_interval.py`

 * *Files identical despite different names*

### Comparing `g3tables-0.2.2/src/g3tables/utils/gdrive/_gdrive.py` & `g3tables-0.2.3/src/g3tables/utils/gdrive/_gdrive.py`

 * *Files identical despite different names*

### Comparing `g3tables-0.2.2/src/g3tables/utils/gdrive/_update_creds.py` & `g3tables-0.2.3/src/g3tables/utils/gdrive/_update_creds.py`

 * *Files identical despite different names*

### Comparing `g3tables-0.2.2/src/g3tables/visualization_table/_table.py` & `g3tables-0.2.3/src/g3tables/visualization_table/_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,24 +144,24 @@
                 with data from the specified local Excel file.
         """
         logger.info('Reading Visualization table from local path: %s', path)
         xls = pd.ExcelFile(path)
         with warnings.catch_warnings():
             warnings.filterwarnings('ignore', category=UserWarning)
             parameters_sheet = pd.read_excel(
-                xls, header=3, sheet_name='Parameters'
+                xls, header=2, sheet_name='Parameters'
                 )
             gate_table_sheet = pd.read_excel(
-                xls, header=3, sheet_name='Requestor table'
+                xls, header=2, sheet_name='Gate table'
                 )
             heating_table_sheet = pd.read_excel(
-                xls, header=3, sheet_name='Requestor table'
+                xls, header=2, sheet_name='Heating table'
                 )
             requestor_table_sheet = pd.read_excel(
-                xls, header=3, sheet_name='Requestor table'
+                xls, header=2, sheet_name='Requestor table'
                 )
         params_formatter = VisualizationTableFormatter.format_params_sheet
         table_formatter = VisualizationTableFormatter.format_table_sheet
         return cls(
             parameters_sheet_data=params_formatter(parameters_sheet),
             gate_table_sheet_data=table_formatter(gate_table_sheet),
             heating_table_sheet_data=table_formatter(heating_table_sheet),
```

### Comparing `g3tables-0.2.2/src/g3tables.egg-info/PKG-INFO` & `g3tables-0.2.3/src/g3tables.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g3tables
-Version: 0.2.2
+Version: 0.2.3
 Summary: G3 SW Definition, HW and PLC components, and Visualisation tables parser
 Author: Elektroline a.s.
 Project-URL: Homepage, https://gitlab.elektroline.cz/plc/systemg3-py/SystemG3Tables
 Keywords: Elektroline,Google Drive,Project table
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Other Audience
```

### Comparing `g3tables-0.2.2/src/g3tables.egg-info/SOURCES.txt` & `g3tables-0.2.3/src/g3tables.egg-info/SOURCES.txt`

 * *Files identical despite different names*

