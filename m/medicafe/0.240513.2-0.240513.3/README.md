# Comparing `tmp/medicafe-0.240513.2.tar.gz` & `tmp/medicafe-0.240513.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medicafe-0.240513.2.tar", last modified: Mon May 13 14:57:53 2024, max compression
+gzip compressed data, was "medicafe-0.240513.3.tar", last modified: Mon May 13 15:29:48 2024, max compression
```

## Comparing `medicafe-0.240513.2.tar` & `medicafe-0.240513.3.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 14:57:53.328000 medicafe-0.240513.2/
--rw-rw-rw-   0        0        0     1096 2024-04-16 02:27:27.000000 medicafe-0.240513.2/LICENSE
--rw-rw-rw-   0        0        0       64 2024-04-19 20:12:06.000000 medicafe-0.240513.2/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2024-05-13 14:57:52.493000 medicafe-0.240513.2/MediBot/
--rwxrwxrwx   0        0        0     5972 2024-05-12 18:02:44.000000 medicafe-0.240513.2/MediBot/MediBot.bat
--rw-rw-rw-   0        0        0    17343 2024-05-12 16:32:17.000000 medicafe-0.240513.2/MediBot/MediBot.py
--rw-rw-rw-   0        0        0     1963 2024-04-17 03:06:31.000000 medicafe-0.240513.2/MediBot/MediBot_Charges.py
--rw-rw-rw-   0        0        0    33980 2024-05-12 16:14:26.000000 medicafe-0.240513.2/MediBot/MediBot_Preprocessor.py
--rw-rw-rw-   0        0        0     4589 2024-05-12 17:14:28.000000 medicafe-0.240513.2/MediBot/MediBot_Preprocessor_lib.py
--rw-rw-rw-   0        0        0    10660 2024-05-09 04:53:27.000000 medicafe-0.240513.2/MediBot/MediBot_UI.py
--rw-rw-rw-   0        0        0     8636 2024-05-12 16:11:39.000000 medicafe-0.240513.2/MediBot/MediBot_dataformat_library.py
--rw-rw-rw-   0        0        0      336 2024-04-18 22:50:25.000000 medicafe-0.240513.2/MediBot/MediPost.py
--rw-rw-rw-   0        0        0     8799 2024-01-30 04:51:58.000000 medicafe-0.240513.2/MediBot/PDF_to_CSV_Cleaner.py
--rw-rw-rw-   0        0        0        0 2024-04-19 02:51:16.000000 medicafe-0.240513.2/MediBot/__init__.py
--rw-rw-rw-   0        0        0     1557 2024-04-12 16:06:52.000000 medicafe-0.240513.2/MediBot/update_json.py
--rw-rw-rw-   0        0        0     2249 2024-05-10 17:47:37.000000 medicafe-0.240513.2/MediBot/update_medicafe.py
-drwxrwxrwx   0        0        0        0 2024-05-13 14:57:53.078000 medicafe-0.240513.2/MediLink/
--rw-rw-rw-   0        0        0    19263 2024-05-13 06:46:25.000000 medicafe-0.240513.2/MediLink/MediLink.py
--rw-rw-rw-   0        0        0     4358 2024-04-13 18:24:36.000000 medicafe-0.240513.2/MediLink/MediLink_277_decoder.py
--rw-rw-rw-   0        0        0    26271 2024-05-13 14:06:59.000000 medicafe-0.240513.2/MediLink/MediLink_837p_encoder.py
--rw-rw-rw-   0        0        0    39431 2024-05-13 14:41:19.000000 medicafe-0.240513.2/MediLink/MediLink_837p_encoder_library.py
--rw-rw-rw-   0        0        0     3914 2024-05-09 02:18:58.000000 medicafe-0.240513.2/MediLink/MediLink_ConfigLoader.py
--rw-rw-rw-   0        0        0    11857 2024-05-12 18:32:20.000000 medicafe-0.240513.2/MediLink/MediLink_DataMgmt.py
--rw-rw-rw-   0        0        0     7264 2024-05-08 01:45:53.000000 medicafe-0.240513.2/MediLink/MediLink_Down.py
--rw-rw-rw-   0        0        0     8724 2024-05-01 03:44:46.000000 medicafe-0.240513.2/MediLink/MediLink_ERA_decoder.py
--rw-rw-rw-   0        0        0     6236 2024-05-10 16:45:40.000000 medicafe-0.240513.2/MediLink/MediLink_Gmail.py
--rw-rw-rw-   0        0        0     6040 2024-04-18 22:53:51.000000 medicafe-0.240513.2/MediLink/MediLink_Scheduler.py
--rw-rw-rw-   0        0        0      222 2024-04-13 17:51:42.000000 medicafe-0.240513.2/MediLink/MediLink_StatusCheck.py
--rw-rw-rw-   0        0        0     5181 2024-05-12 16:36:09.000000 medicafe-0.240513.2/MediLink/MediLink_UI.py
--rw-rw-rw-   0        0        0    19252 2024-05-13 14:56:52.000000 medicafe-0.240513.2/MediLink/MediLink_Up.py
--rwxrwxrwx   0        0        0      118 2024-04-19 22:20:37.000000 medicafe-0.240513.2/MediLink/MediLink_batch.bat
--rw-rw-rw-   0        0        0      497 2024-03-15 19:39:51.000000 medicafe-0.240513.2/MediLink/Soumit_api.py
--rw-rw-rw-   0        0        0        0 2024-04-19 02:51:01.000000 medicafe-0.240513.2/MediLink/__init__.py
--rw-rw-rw-   0        0        0     3108 2024-05-13 04:52:22.000000 medicafe-0.240513.2/MediLink/test.py
--rw-rw-rw-   0        0        0     4396 2024-05-13 14:57:53.278000 medicafe-0.240513.2/PKG-INFO
--rw-rw-rw-   0        0        0     2960 2024-05-13 07:31:39.000000 medicafe-0.240513.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-13 14:57:53.259000 medicafe-0.240513.2/medicafe.egg-info/
--rw-rw-rw-   0        0        0     4396 2024-05-13 14:57:51.000000 medicafe-0.240513.2/medicafe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1023 2024-05-13 14:57:51.000000 medicafe-0.240513.2/medicafe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 14:57:51.000000 medicafe-0.240513.2/medicafe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-16 03:47:58.000000 medicafe-0.240513.2/medicafe.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       60 2024-05-13 14:57:51.000000 medicafe-0.240513.2/medicafe.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-13 14:57:51.000000 medicafe-0.240513.2/medicafe.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-13 14:57:53.291000 medicafe-0.240513.2/setup.cfg
--rw-rw-rw-   0        0        0     4834 2024-05-13 14:57:50.000000 medicafe-0.240513.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 15:29:48.410000 medicafe-0.240513.3/
+-rw-rw-rw-   0        0        0     1096 2024-04-16 02:27:27.000000 medicafe-0.240513.3/LICENSE
+-rw-rw-rw-   0        0        0       64 2024-04-19 20:12:06.000000 medicafe-0.240513.3/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2024-05-13 15:29:47.668000 medicafe-0.240513.3/MediBot/
+-rwxrwxrwx   0        0        0     5972 2024-05-12 18:02:44.000000 medicafe-0.240513.3/MediBot/MediBot.bat
+-rw-rw-rw-   0        0        0    17343 2024-05-12 16:32:17.000000 medicafe-0.240513.3/MediBot/MediBot.py
+-rw-rw-rw-   0        0        0     1963 2024-04-17 03:06:31.000000 medicafe-0.240513.3/MediBot/MediBot_Charges.py
+-rw-rw-rw-   0        0        0    33980 2024-05-12 16:14:26.000000 medicafe-0.240513.3/MediBot/MediBot_Preprocessor.py
+-rw-rw-rw-   0        0        0     4589 2024-05-12 17:14:28.000000 medicafe-0.240513.3/MediBot/MediBot_Preprocessor_lib.py
+-rw-rw-rw-   0        0        0    10660 2024-05-09 04:53:27.000000 medicafe-0.240513.3/MediBot/MediBot_UI.py
+-rw-rw-rw-   0        0        0     8636 2024-05-12 16:11:39.000000 medicafe-0.240513.3/MediBot/MediBot_dataformat_library.py
+-rw-rw-rw-   0        0        0      336 2024-04-18 22:50:25.000000 medicafe-0.240513.3/MediBot/MediPost.py
+-rw-rw-rw-   0        0        0     8799 2024-01-30 04:51:58.000000 medicafe-0.240513.3/MediBot/PDF_to_CSV_Cleaner.py
+-rw-rw-rw-   0        0        0        0 2024-04-19 02:51:16.000000 medicafe-0.240513.3/MediBot/__init__.py
+-rw-rw-rw-   0        0        0     1557 2024-04-12 16:06:52.000000 medicafe-0.240513.3/MediBot/update_json.py
+-rw-rw-rw-   0        0        0     2249 2024-05-10 17:47:37.000000 medicafe-0.240513.3/MediBot/update_medicafe.py
+drwxrwxrwx   0        0        0        0 2024-05-13 15:29:48.196000 medicafe-0.240513.3/MediLink/
+-rw-rw-rw-   0        0        0    20013 2024-05-13 15:28:44.000000 medicafe-0.240513.3/MediLink/MediLink.py
+-rw-rw-rw-   0        0        0     4358 2024-04-13 18:24:36.000000 medicafe-0.240513.3/MediLink/MediLink_277_decoder.py
+-rw-rw-rw-   0        0        0    26271 2024-05-13 14:06:59.000000 medicafe-0.240513.3/MediLink/MediLink_837p_encoder.py
+-rw-rw-rw-   0        0        0    39431 2024-05-13 14:41:19.000000 medicafe-0.240513.3/MediLink/MediLink_837p_encoder_library.py
+-rw-rw-rw-   0        0        0     3914 2024-05-09 02:18:58.000000 medicafe-0.240513.3/MediLink/MediLink_ConfigLoader.py
+-rw-rw-rw-   0        0        0    11857 2024-05-12 18:32:20.000000 medicafe-0.240513.3/MediLink/MediLink_DataMgmt.py
+-rw-rw-rw-   0        0        0     7264 2024-05-08 01:45:53.000000 medicafe-0.240513.3/MediLink/MediLink_Down.py
+-rw-rw-rw-   0        0        0     8724 2024-05-01 03:44:46.000000 medicafe-0.240513.3/MediLink/MediLink_ERA_decoder.py
+-rw-rw-rw-   0        0        0     6236 2024-05-10 16:45:40.000000 medicafe-0.240513.3/MediLink/MediLink_Gmail.py
+-rw-rw-rw-   0        0        0     6040 2024-04-18 22:53:51.000000 medicafe-0.240513.3/MediLink/MediLink_Scheduler.py
+-rw-rw-rw-   0        0        0      222 2024-04-13 17:51:42.000000 medicafe-0.240513.3/MediLink/MediLink_StatusCheck.py
+-rw-rw-rw-   0        0        0     5181 2024-05-12 16:36:09.000000 medicafe-0.240513.3/MediLink/MediLink_UI.py
+-rw-rw-rw-   0        0        0    19252 2024-05-13 14:56:52.000000 medicafe-0.240513.3/MediLink/MediLink_Up.py
+-rwxrwxrwx   0        0        0      118 2024-04-19 22:20:37.000000 medicafe-0.240513.3/MediLink/MediLink_batch.bat
+-rw-rw-rw-   0        0        0      497 2024-03-15 19:39:51.000000 medicafe-0.240513.3/MediLink/Soumit_api.py
+-rw-rw-rw-   0        0        0        0 2024-04-19 02:51:01.000000 medicafe-0.240513.3/MediLink/__init__.py
+-rw-rw-rw-   0        0        0     3108 2024-05-13 04:52:22.000000 medicafe-0.240513.3/MediLink/test.py
+-rw-rw-rw-   0        0        0     4396 2024-05-13 15:29:48.394000 medicafe-0.240513.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2960 2024-05-13 07:31:39.000000 medicafe-0.240513.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 15:29:48.376000 medicafe-0.240513.3/medicafe.egg-info/
+-rw-rw-rw-   0        0        0     4396 2024-05-13 15:29:46.000000 medicafe-0.240513.3/medicafe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1023 2024-05-13 15:29:47.000000 medicafe-0.240513.3/medicafe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 15:29:46.000000 medicafe-0.240513.3/medicafe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-16 03:47:58.000000 medicafe-0.240513.3/medicafe.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       60 2024-05-13 15:29:46.000000 medicafe-0.240513.3/medicafe.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-13 15:29:46.000000 medicafe-0.240513.3/medicafe.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 15:29:48.406000 medicafe-0.240513.3/setup.cfg
+-rw-rw-rw-   0        0        0     4834 2024-05-13 15:29:45.000000 medicafe-0.240513.3/setup.py
```

### Comparing `medicafe-0.240513.2/LICENSE` & `medicafe-0.240513.3/LICENSE`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.2/MediBot/MediBot.bat` & `medicafe-0.240513.3/MediBot/MediBot.bat`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.2/MediBot/MediBot.py` & `medicafe-0.240513.3/MediBot/MediBot.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.2/MediBot/MediBot_Charges.py` & `medicafe-0.240513.3/MediBot/MediBot_Charges.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.2/MediBot/MediBot_Preprocessor.py` & `medicafe-0.240513.3/MediBot/MediBot_Preprocessor.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.2/MediBot/MediBot_Preprocessor_lib.py` & `medicafe-0.240513.3/MediBot/MediBot_Preprocessor_lib.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.2/MediBot/MediBot_UI.py` & `medicafe-0.240513.3/MediBot/MediBot_UI.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.2/MediBot/MediBot_dataformat_library.py` & `medicafe-0.240513.3/MediBot/MediBot_dataformat_library.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.2/MediBot/PDF_to_CSV_Cleaner.py` & `medicafe-0.240513.3/MediBot/PDF_to_CSV_Cleaner.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.2/MediBot/update_json.py` & `medicafe-0.240513.3/MediBot/update_json.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.2/MediBot/update_medicafe.py` & `medicafe-0.240513.3/MediBot/update_medicafe.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.2/MediLink/MediLink.py` & `medicafe-0.240513.3/MediLink/MediLink.py`

 * *Files 3% similar despite different names*

```diff
@@ -121,36 +121,45 @@
     - A comprehensive data structure retaining detailed patient claim details needed for processing,
       including new key-value pairs for file path, surgery date, patient name, and primary insurance.
     """
     detailed_patient_data = []
     
     # Load insurance data from MAINS to create a mapping from insurance names to their respective IDs
     insurance_to_id = load_insurance_data_from_mains(config)
-    
+    MediLink_ConfigLoader.log("Insurance data loaded from MAINS. {} insurance providers found.".format(len(insurance_to_id)))
+
     for personal_info, insurance_info, service_info in MediLink_837p_encoder.read_fixed_width_data(file_path, config.get('MediLink_Config', {})):
         parsed_data = MediLink_837p_encoder.parse_fixed_width_data(personal_info, insurance_info, service_info, config.get('MediLink_Config', {}))
         
         primary_insurance = parsed_data.get('INAME')
         
         # Retrieve the insurance ID associated with the primary insurance
         insurance_id = insurance_to_id.get(primary_insurance)
-        
+        MediLink_ConfigLoader.log("Primary insurance ID retrieved for '{}': {}".format(primary_insurance, insurance_id))
+
         # Use insurance ID to retrieve the payer ID(s) associated with the insurance
         payer_ids = []
         if insurance_id:
             for payer_id, payer_data in crosswalk.get('payer_id', {}).items():
                 if insurance_id in payer_data.get('medisoft_id', []):
                     payer_ids.append(payer_id)
+        if payer_ids:
+            MediLink_ConfigLoader.log("Payer IDs retrieved for insurance '{}': {}".format(primary_insurance, payer_ids))
+        else:
+            MediLink_ConfigLoader.log("No payer IDs found for insurance '{}'".format(primary_insurance)))
         
         # Find the suggested endpoint from the crosswalk based on the payer IDs
         suggested_endpoint = 'AVAILITY'  # Default endpoint if no matching payer IDs found
         for payer_id in payer_ids:
             if payer_id in crosswalk.get('payer_id', {}):
                 suggested_endpoint = crosswalk['payer_id'][payer_id]['endpoint']
+                MediLink_ConfigLoader.log("Suggested endpoint for payer ID '{}': {}".format(payer_id, suggested_endpoint))
                 break
+        else:
+            MediLink_ConfigLoader.log("No suggested endpoint found for payer IDs: {}".format(payer_ids)))
         
         # Enrich detailed patient data with additional information and suggested endpoint
         detailed_data = parsed_data.copy()  # Copy parsed_data to avoid modifying the original dictionary
         detailed_data.update({
             'file_path': file_path,
             'patient_id': parsed_data.get('CHART'),
             'surgery_date': parsed_data.get('DATE'),
```

### Comparing `medicafe-0.240513.2/MediLink/MediLink_277_decoder.py` & `medicafe-0.240513.3/MediLink/MediLink_277_decoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.2/MediLink/MediLink_837p_encoder.py` & `medicafe-0.240513.3/MediLink/MediLink_837p_encoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.2/MediLink/MediLink_837p_encoder_library.py` & `medicafe-0.240513.3/MediLink/MediLink_837p_encoder_library.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.2/MediLink/MediLink_ConfigLoader.py` & `medicafe-0.240513.3/MediLink/MediLink_ConfigLoader.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.2/MediLink/MediLink_DataMgmt.py` & `medicafe-0.240513.3/MediLink/MediLink_DataMgmt.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.2/MediLink/MediLink_Down.py` & `medicafe-0.240513.3/MediLink/MediLink_Down.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.2/MediLink/MediLink_ERA_decoder.py` & `medicafe-0.240513.3/MediLink/MediLink_ERA_decoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.2/MediLink/MediLink_Gmail.py` & `medicafe-0.240513.3/MediLink/MediLink_Gmail.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.2/MediLink/MediLink_Scheduler.py` & `medicafe-0.240513.3/MediLink/MediLink_Scheduler.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.2/MediLink/MediLink_UI.py` & `medicafe-0.240513.3/MediLink/MediLink_UI.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.2/MediLink/MediLink_Up.py` & `medicafe-0.240513.3/MediLink/MediLink_Up.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.2/MediLink/test.py` & `medicafe-0.240513.3/MediLink/test.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.2/PKG-INFO` & `medicafe-0.240513.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medicafe
-Version: 0.240513.2
+Version: 0.240513.3
 Summary: MediCafe
 Home-page: https://github.com/katanada2
 Author: Daniel Vidaud
 Author-email: daniel@personalizedtransformation.com
 License: MIT
 Keywords: medicafe python34 medibot medilink
 Description-Content-Type: text/markdown
```

### Comparing `medicafe-0.240513.2/README.md` & `medicafe-0.240513.3/README.md`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.2/medicafe.egg-info/PKG-INFO` & `medicafe-0.240513.3/medicafe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medicafe
-Version: 0.240513.2
+Version: 0.240513.3
 Summary: MediCafe
 Home-page: https://github.com/katanada2
 Author: Daniel Vidaud
 Author-email: daniel@personalizedtransformation.com
 License: MIT
 Keywords: medicafe python34 medibot medilink
 Description-Content-Type: text/markdown
```

### Comparing `medicafe-0.240513.2/medicafe.egg-info/SOURCES.txt` & `medicafe-0.240513.3/medicafe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.2/setup.py` & `medicafe-0.240513.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='medicafe',
-    version="0.240513.2",
+    version="0.240513.3",
     description='MediCafe',
     long_description="""
     # Project Overview: MediCafe
 
     ## Project Description
     MediCafe is a comprehensive suite designed to automate and streamline several aspects of medical administrative tasks within Medisoft, a popular medical practice management software. The system consists of two main components: MediBot and MediLink, each serving distinct functions but integrated to enhance the workflow of medical practices.
```

