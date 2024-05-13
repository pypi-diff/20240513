# Comparing `tmp/medicafe-0.240512.9.tar.gz` & `tmp/medicafe-0.240513.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medicafe-0.240512.9.tar", last modified: Sun May 12 18:48:23 2024, max compression
+gzip compressed data, was "medicafe-0.240513.0.tar", last modified: Mon May 13 07:22:23 2024, max compression
```

## Comparing `medicafe-0.240512.9.tar` & `medicafe-0.240513.0.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 18:48:23.165000 medicafe-0.240512.9/
--rw-rw-rw-   0        0        0     1096 2024-04-16 02:27:27.000000 medicafe-0.240512.9/LICENSE
--rw-rw-rw-   0        0        0       64 2024-04-19 20:12:06.000000 medicafe-0.240512.9/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2024-05-12 18:48:21.379000 medicafe-0.240512.9/MediBot/
--rwxrwxrwx   0        0        0     5972 2024-05-12 18:02:44.000000 medicafe-0.240512.9/MediBot/MediBot.bat
--rw-rw-rw-   0        0        0    17343 2024-05-12 16:32:17.000000 medicafe-0.240512.9/MediBot/MediBot.py
--rw-rw-rw-   0        0        0     1963 2024-04-17 03:06:31.000000 medicafe-0.240512.9/MediBot/MediBot_Charges.py
--rw-rw-rw-   0        0        0    33980 2024-05-12 16:14:26.000000 medicafe-0.240512.9/MediBot/MediBot_Preprocessor.py
--rw-rw-rw-   0        0        0     4589 2024-05-12 17:14:28.000000 medicafe-0.240512.9/MediBot/MediBot_Preprocessor_lib.py
--rw-rw-rw-   0        0        0    10660 2024-05-09 04:53:27.000000 medicafe-0.240512.9/MediBot/MediBot_UI.py
--rw-rw-rw-   0        0        0     8636 2024-05-12 16:11:39.000000 medicafe-0.240512.9/MediBot/MediBot_dataformat_library.py
--rw-rw-rw-   0        0        0      336 2024-04-18 22:50:25.000000 medicafe-0.240512.9/MediBot/MediPost.py
--rw-rw-rw-   0        0        0     8799 2024-01-30 04:51:58.000000 medicafe-0.240512.9/MediBot/PDF_to_CSV_Cleaner.py
--rw-rw-rw-   0        0        0        0 2024-04-19 02:51:16.000000 medicafe-0.240512.9/MediBot/__init__.py
--rw-rw-rw-   0        0        0     1557 2024-04-12 16:06:52.000000 medicafe-0.240512.9/MediBot/update_json.py
--rw-rw-rw-   0        0        0     2249 2024-05-10 17:47:37.000000 medicafe-0.240512.9/MediBot/update_medicafe.py
-drwxrwxrwx   0        0        0        0 2024-05-12 18:48:22.626000 medicafe-0.240512.9/MediLink/
--rw-rw-rw-   0        0        0    18258 2024-05-12 05:05:14.000000 medicafe-0.240512.9/MediLink/MediLink.py
--rw-rw-rw-   0        0        0     4358 2024-04-13 18:24:36.000000 medicafe-0.240512.9/MediLink/MediLink_277_decoder.py
--rw-rw-rw-   0        0        0    25854 2024-05-12 17:24:38.000000 medicafe-0.240512.9/MediLink/MediLink_837p_encoder.py
--rw-rw-rw-   0        0        0    39204 2024-05-12 16:27:25.000000 medicafe-0.240512.9/MediLink/MediLink_837p_encoder_library.py
--rw-rw-rw-   0        0        0     3914 2024-05-09 02:18:58.000000 medicafe-0.240512.9/MediLink/MediLink_ConfigLoader.py
--rw-rw-rw-   0        0        0    11857 2024-05-12 18:32:20.000000 medicafe-0.240512.9/MediLink/MediLink_DataMgmt.py
--rw-rw-rw-   0        0        0     7264 2024-05-08 01:45:53.000000 medicafe-0.240512.9/MediLink/MediLink_Down.py
--rw-rw-rw-   0        0        0     8724 2024-05-01 03:44:46.000000 medicafe-0.240512.9/MediLink/MediLink_ERA_decoder.py
--rw-rw-rw-   0        0        0     6236 2024-05-10 16:45:40.000000 medicafe-0.240512.9/MediLink/MediLink_Gmail.py
--rw-rw-rw-   0        0        0     6040 2024-04-18 22:53:51.000000 medicafe-0.240512.9/MediLink/MediLink_Scheduler.py
--rw-rw-rw-   0        0        0      222 2024-04-13 17:51:42.000000 medicafe-0.240512.9/MediLink/MediLink_StatusCheck.py
--rw-rw-rw-   0        0        0     5181 2024-05-12 16:36:09.000000 medicafe-0.240512.9/MediLink/MediLink_UI.py
--rw-rw-rw-   0        0        0    16331 2024-05-12 18:46:57.000000 medicafe-0.240512.9/MediLink/MediLink_Up.py
--rwxrwxrwx   0        0        0      118 2024-04-19 22:20:37.000000 medicafe-0.240512.9/MediLink/MediLink_batch.bat
--rw-rw-rw-   0        0        0      497 2024-03-15 19:39:51.000000 medicafe-0.240512.9/MediLink/Soumit_api.py
--rw-rw-rw-   0        0        0        0 2024-04-19 02:51:01.000000 medicafe-0.240512.9/MediLink/__init__.py
--rw-rw-rw-   0        0        0      730 2024-05-12 18:48:23.132000 medicafe-0.240512.9/PKG-INFO
--rw-rw-rw-   0        0        0      994 2024-04-16 02:33:22.000000 medicafe-0.240512.9/README.md
-drwxrwxrwx   0        0        0        0 2024-05-12 18:48:23.089000 medicafe-0.240512.9/medicafe.egg-info/
--rw-rw-rw-   0        0        0      730 2024-05-12 18:48:19.000000 medicafe-0.240512.9/medicafe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1006 2024-05-12 18:48:20.000000 medicafe-0.240512.9/medicafe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 18:48:19.000000 medicafe-0.240512.9/medicafe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-16 03:47:58.000000 medicafe-0.240512.9/medicafe.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       60 2024-05-12 18:48:19.000000 medicafe-0.240512.9/medicafe.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-12 18:48:19.000000 medicafe-0.240512.9/medicafe.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-12 18:48:23.157000 medicafe-0.240512.9/setup.cfg
--rw-rw-rw-   0        0        0     1164 2024-05-12 18:48:17.000000 medicafe-0.240512.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 07:22:23.571000 medicafe-0.240513.0/
+-rw-rw-rw-   0        0        0     1096 2024-04-16 02:27:27.000000 medicafe-0.240513.0/LICENSE
+-rw-rw-rw-   0        0        0       64 2024-04-19 20:12:06.000000 medicafe-0.240513.0/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2024-05-13 07:22:22.930000 medicafe-0.240513.0/MediBot/
+-rwxrwxrwx   0        0        0     5972 2024-05-12 18:02:44.000000 medicafe-0.240513.0/MediBot/MediBot.bat
+-rw-rw-rw-   0        0        0    17343 2024-05-12 16:32:17.000000 medicafe-0.240513.0/MediBot/MediBot.py
+-rw-rw-rw-   0        0        0     1963 2024-04-17 03:06:31.000000 medicafe-0.240513.0/MediBot/MediBot_Charges.py
+-rw-rw-rw-   0        0        0    33980 2024-05-12 16:14:26.000000 medicafe-0.240513.0/MediBot/MediBot_Preprocessor.py
+-rw-rw-rw-   0        0        0     4589 2024-05-12 17:14:28.000000 medicafe-0.240513.0/MediBot/MediBot_Preprocessor_lib.py
+-rw-rw-rw-   0        0        0    10660 2024-05-09 04:53:27.000000 medicafe-0.240513.0/MediBot/MediBot_UI.py
+-rw-rw-rw-   0        0        0     8636 2024-05-12 16:11:39.000000 medicafe-0.240513.0/MediBot/MediBot_dataformat_library.py
+-rw-rw-rw-   0        0        0      336 2024-04-18 22:50:25.000000 medicafe-0.240513.0/MediBot/MediPost.py
+-rw-rw-rw-   0        0        0     8799 2024-01-30 04:51:58.000000 medicafe-0.240513.0/MediBot/PDF_to_CSV_Cleaner.py
+-rw-rw-rw-   0        0        0        0 2024-04-19 02:51:16.000000 medicafe-0.240513.0/MediBot/__init__.py
+-rw-rw-rw-   0        0        0     1557 2024-04-12 16:06:52.000000 medicafe-0.240513.0/MediBot/update_json.py
+-rw-rw-rw-   0        0        0     2249 2024-05-10 17:47:37.000000 medicafe-0.240513.0/MediBot/update_medicafe.py
+drwxrwxrwx   0        0        0        0 2024-05-13 07:22:23.384000 medicafe-0.240513.0/MediLink/
+-rw-rw-rw-   0        0        0    19263 2024-05-13 06:46:25.000000 medicafe-0.240513.0/MediLink/MediLink.py
+-rw-rw-rw-   0        0        0     4358 2024-04-13 18:24:36.000000 medicafe-0.240513.0/MediLink/MediLink_277_decoder.py
+-rw-rw-rw-   0        0        0    26188 2024-05-13 06:12:51.000000 medicafe-0.240513.0/MediLink/MediLink_837p_encoder.py
+-rw-rw-rw-   0        0        0    39298 2024-05-13 06:41:12.000000 medicafe-0.240513.0/MediLink/MediLink_837p_encoder_library.py
+-rw-rw-rw-   0        0        0     3914 2024-05-09 02:18:58.000000 medicafe-0.240513.0/MediLink/MediLink_ConfigLoader.py
+-rw-rw-rw-   0        0        0    11857 2024-05-12 18:32:20.000000 medicafe-0.240513.0/MediLink/MediLink_DataMgmt.py
+-rw-rw-rw-   0        0        0     7264 2024-05-08 01:45:53.000000 medicafe-0.240513.0/MediLink/MediLink_Down.py
+-rw-rw-rw-   0        0        0     8724 2024-05-01 03:44:46.000000 medicafe-0.240513.0/MediLink/MediLink_ERA_decoder.py
+-rw-rw-rw-   0        0        0     6236 2024-05-10 16:45:40.000000 medicafe-0.240513.0/MediLink/MediLink_Gmail.py
+-rw-rw-rw-   0        0        0     6040 2024-04-18 22:53:51.000000 medicafe-0.240513.0/MediLink/MediLink_Scheduler.py
+-rw-rw-rw-   0        0        0      222 2024-04-13 17:51:42.000000 medicafe-0.240513.0/MediLink/MediLink_StatusCheck.py
+-rw-rw-rw-   0        0        0     5181 2024-05-12 16:36:09.000000 medicafe-0.240513.0/MediLink/MediLink_UI.py
+-rw-rw-rw-   0        0        0    18988 2024-05-13 05:01:21.000000 medicafe-0.240513.0/MediLink/MediLink_Up.py
+-rwxrwxrwx   0        0        0      118 2024-04-19 22:20:37.000000 medicafe-0.240513.0/MediLink/MediLink_batch.bat
+-rw-rw-rw-   0        0        0      497 2024-03-15 19:39:51.000000 medicafe-0.240513.0/MediLink/Soumit_api.py
+-rw-rw-rw-   0        0        0        0 2024-04-19 02:51:01.000000 medicafe-0.240513.0/MediLink/__init__.py
+-rw-rw-rw-   0        0        0     3108 2024-05-13 04:52:22.000000 medicafe-0.240513.0/MediLink/test.py
+-rw-rw-rw-   0        0        0     4396 2024-05-13 07:22:23.557000 medicafe-0.240513.0/PKG-INFO
+-rw-rw-rw-   0        0        0      994 2024-04-16 02:33:22.000000 medicafe-0.240513.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 07:22:23.542000 medicafe-0.240513.0/medicafe.egg-info/
+-rw-rw-rw-   0        0        0     4396 2024-05-13 07:22:22.000000 medicafe-0.240513.0/medicafe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1023 2024-05-13 07:22:22.000000 medicafe-0.240513.0/medicafe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 07:22:22.000000 medicafe-0.240513.0/medicafe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-16 03:47:58.000000 medicafe-0.240513.0/medicafe.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       60 2024-05-13 07:22:22.000000 medicafe-0.240513.0/medicafe.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-13 07:22:22.000000 medicafe-0.240513.0/medicafe.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 07:22:23.567000 medicafe-0.240513.0/setup.cfg
+-rw-rw-rw-   0        0        0     4834 2024-05-13 07:22:19.000000 medicafe-0.240513.0/setup.py
```

### Comparing `medicafe-0.240512.9/LICENSE` & `medicafe-0.240513.0/LICENSE`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.9/MediBot/MediBot.bat` & `medicafe-0.240513.0/MediBot/MediBot.bat`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.9/MediBot/MediBot.py` & `medicafe-0.240513.0/MediBot/MediBot.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.9/MediBot/MediBot_Charges.py` & `medicafe-0.240513.0/MediBot/MediBot_Charges.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.9/MediBot/MediBot_Preprocessor.py` & `medicafe-0.240513.0/MediBot/MediBot_Preprocessor.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.9/MediBot/MediBot_Preprocessor_lib.py` & `medicafe-0.240513.0/MediBot/MediBot_Preprocessor_lib.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.9/MediBot/MediBot_UI.py` & `medicafe-0.240513.0/MediBot/MediBot_UI.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.9/MediBot/MediBot_dataformat_library.py` & `medicafe-0.240513.0/MediBot/MediBot_dataformat_library.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.9/MediBot/PDF_to_CSV_Cleaner.py` & `medicafe-0.240513.0/MediBot/PDF_to_CSV_Cleaner.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.9/MediBot/update_json.py` & `medicafe-0.240513.0/MediBot/update_json.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.9/MediBot/update_medicafe.py` & `medicafe-0.240513.0/MediBot/update_medicafe.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.9/MediLink/MediLink.py` & `medicafe-0.240513.0/MediLink/MediLink.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,27 @@
 import os
+
 import MediLink_Down
 import MediLink_Up
 import MediLink_ConfigLoader
 import MediLink_837p_encoder
 
 # For UI Functions
 import os
 import MediLink_UI  # Import UI module for handling all user interfaces
 from tqdm import tqdm
 
+# Add parent directory of the project to the Python path
+import sys
+project_dir = os.path.abspath(os.path.join(os.path.dirname(__file__), ".."))
+sys.path.append(project_dir)
+
+from MediBot.MediBot_Preprocessor import load_insurance_data_from_mains
+
+
 """
 Development Tasks for Backend Enhancement in MediSoft Claims Submittal (MediLink) Script:
 
 Implement dynamic configurations for multiple endpoints (Availity, Optum, PNT Data) with environmental settings support.
 Enhance file detection with detailed logging and introduce integrity checks for pre-processing validation.
 Verify file transmissions via WinSCP log analysis for successful endpoint acknowledgments and secure data transfer.
 Automate response file handling from endpoints and integrate feedback into MediSoft with exception alerts.
@@ -110,30 +119,40 @@
 
     Returns:
     - A comprehensive data structure retaining detailed patient claim details needed for processing,
       including new key-value pairs for file path, surgery date, patient name, and primary insurance.
     """
     detailed_patient_data = []
     
+    # Load insurance data from MAINS to create a mapping from insurance names to their respective IDs
+    insurance_to_id = load_insurance_data_from_mains(config)
+    
     for personal_info, insurance_info, service_info in MediLink_837p_encoder.read_fixed_width_data(file_path, config.get('MediLink_Config', {})):
         parsed_data = MediLink_837p_encoder.parse_fixed_width_data(personal_info, insurance_info, service_info, config.get('MediLink_Config', {}))
         
         primary_insurance = parsed_data.get('INAME')
         
-        # TODO (High Crosswalk) This suggested endpoint should be a payerid_to_endpoint_mapping.
-        # No, we've completely changed this structure so the whole thing is wrong.
-        # We're going to have something like payer_id {endpoint:'AVAILITY', insurance_id: {105, 12}}
-        # we'll need MAINS to map primary_insurance to insurance_id first and then look for the number in the values.
-        try:
-            # Fix this soon. new json format.
-            suggested_endpoint = crosswalk['insurance_to_endpoint_mapping'][primary_insurance]
-        except KeyError:
-            suggested_endpoint = 'AVAILITY'
-
-        # Directly enrich detailed patient data with additional information and suggested endpoint
+        # Retrieve the insurance ID associated with the primary insurance
+        insurance_id = insurance_to_id.get(primary_insurance)
+        
+        # Use insurance ID to retrieve the payer ID(s) associated with the insurance
+        payer_ids = []
+        if insurance_id:
+            for payer_id, payer_data in crosswalk.get('payer_id', {}).items():
+                if insurance_id in payer_data.get('medisoft_id', []):
+                    payer_ids.append(payer_id)
+        
+        # Find the suggested endpoint from the crosswalk based on the payer IDs
+        suggested_endpoint = 'AVAILITY'  # Default endpoint if no matching payer IDs found
+        for payer_id in payer_ids:
+            if payer_id in crosswalk.get('payer_id', {}):
+                suggested_endpoint = crosswalk['payer_id'][payer_id]['endpoint']
+                break
+        
+        # Enrich detailed patient data with additional information and suggested endpoint
         detailed_data = parsed_data.copy()  # Copy parsed_data to avoid modifying the original dictionary
         detailed_data.update({
             'file_path': file_path,
             'patient_id': parsed_data.get('CHART'),
             'surgery_date': parsed_data.get('DATE'),
             'patient_name': ' '.join([parsed_data.get(key, '') for key in ['FIRST', 'MIDDLE', 'LAST']]),
             'amount': parsed_data.get('AMOUNT'),
@@ -174,15 +193,16 @@
             if 'remote_directory_down' in endpoint_info:  # Check if the 'remote_directory_down' key exists
                 #print("Processing endpoint: ", endpoint_info['name']) 
                 # BUG (Debug and verbosity removal) this is really for debug only. Positive statements can be muted.
                 try:
                     ERA_path = MediLink_Down.main(desired_endpoint=endpoint_key)
                     processed_endpoints.append((endpoint_info['name'], ERA_path))
                     MediLink_ConfigLoader.log("Results for {} saved to: {}".format(endpoint_info['name'], ERA_path))
-                    # TODO (Low SFTP) This needs to check to see if this actually worked maybe winscplog before saying it completed successfully 
+                    # TODO (Low SFTP - Download side) This needs to check to see if this actually worked maybe winscplog before saying it completed successfully 
+                    # Check if there is commonality with the upload side so we can use the same validation function.
                 except Exception as e:
                     print("An error occurred while checking remittances for {}: {}".format(endpoint_info['name'], e))
             else:
                 MediLink_ConfigLoader.log("Skipping endpoint '{}' as it does not have 'remote_directory_down' configured.".format(endpoint_info['name']))
     else:
         print("Error: Endpoint config is not a 'dictionary' as expected.")
     # Check if all ERA paths are the same
@@ -204,15 +224,16 @@
 
 def user_decision_on_suggestions(detailed_patient_data, config):
     """
     Presents the user with all patient summaries and suggested endpoints,
     then asks for confirmation to proceed with all or specify adjustments manually.
     
     BUG (Med suggested_endpoint) The display summary suggested_endpoint key isn't updating per the user's decision 
-    although the user decision is persisting.
+    although the user decision is persisting. Possibly consider making the current/suggested/confirmed endpoint 
+    part of a class that the user can interact with via these menus. Probably better handling that way.
     """
     # Display summaries of patient details and endpoints.
     MediLink_UI.display_patient_summaries(detailed_patient_data)
 
     # Ask the user if they want to proceed with all suggested endpoints.
     proceed = MediLink_UI.ask_for_proceeding_with_endpoints()
 
@@ -232,17 +253,17 @@
             data['confirmed_endpoint'] = data['suggested_endpoint']
     return detailed_patient_data
 
 def select_and_adjust_files(detailed_patient_data, config):
     """
     Allows users to select patients and adjust their endpoints by interfacing with UI functions.
     
-    BUG (Med suggested_endpoint) After the user is done making their selection, suggested_endpoint should update to persist the 
-    user selection as priority over its original suggestion. Also, the crosswalk should persist the change 
-    in the endpoint as well.
+    BUG (Med suggested_endpoint) After the user is done making their selection (probably via a class?), 
+    Then suggested_endpoint should update to persist the user selection as priority over its original suggestion. 
+    Which means the crosswalk should persist the change in the endpoint as well.
     """
     # Display options for patients
     MediLink_UI.display_patient_options(detailed_patient_data)
 
     # Get user-selected indices for adjustment
     selected_indices = MediLink_UI.get_selected_indices(len(detailed_patient_data))
```

### Comparing `medicafe-0.240512.9/MediLink/MediLink_277_decoder.py` & `medicafe-0.240513.0/MediLink/MediLink_277_decoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.9/MediLink/MediLink_837p_encoder.py` & `medicafe-0.240513.0/MediLink/MediLink_837p_encoder.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,14 @@
     - transaction_set_control_number: The starting transaction set control number.
 
     Returns:
     - Tuple containing (ISA header, GS header, GE trailer, IEA trailer).
     """
     endpoint_config = config['endpoints'].get(endpoint.upper(), {})
     
-    # BUG NASTY!!! This is duplicated in process_claim.
     # Get the current system time and format it as 'HHMMSS' in 24-hour clock.
     current_time = datetime.now().strftime('%H%M%S')
     isa13 = '000' + current_time  # Format ISA13 with '000HHMMSS'.
 
     # Check if isa13 could not be generated from the current time
     if len(isa13) != 9:
         # If isa13 cannot be generated from the current time, use the configured value.
@@ -125,14 +124,17 @@
 
     # Optionally, print or log the formatted 837P for debugging or verification
     # TODO (Low UI/usability) Add chart number to this.
     MediLink_ConfigLoader.log("Formatted 837P for endpoint {}.".format(endpoint), config, level="INFO")
 
     return formatted_837p
 
+import os
+from datetime import datetime
+
 def write_output_file(document_segments, output_directory, endpoint_key, input_file_path, config):
     """
     Writes formatted 837P document segments to an output file with a dynamically generated name.
     
     Development Roadmap:
     - Ensure input `document_segments` is a non-empty list to avoid creating empty files.
     - Verify `output_directory` exists and is writable before proceeding. Create the directory if it does not exist.
@@ -146,28 +148,45 @@
     - output_directory: String specifying the directory where the output file will be saved.
     - endpoint_key: String specifying the endpoint for which the claim is processed, used in naming the output file.
     - input_file_path: String specifying the path to the input file being processed, used in naming the output file.
     
     Returns:
     - String specifying the path to the successfully created output file. Consider returning a tuple (path, status) for enhanced error handling.
     """
-    formatted_837p = '\n'.join(document_segments)
+    # Check if document segments are empty
+    if not document_segments:
+        MediLink_ConfigLoader.log("Error: Empty document segments provided. No output file created.", config, level="ERROR")
+        return None
+    
+    # Check if the output directory exists and is writable
+    if not os.path.exists(output_directory):
+        try:
+            os.makedirs(output_directory)
+        except OSError as e:
+            MediLink_ConfigLoader.log("Error: Failed to create output directory. {}".format(e), config, level="ERROR")
+            return None
+    elif not os.access(output_directory, os.W_OK):
+        MediLink_ConfigLoader.log("Error: Output directory is not writable.", config, level="ERROR")
+        return None
+    
+    # Generate new output file path
     base_name = os.path.splitext(os.path.basename(input_file_path))[0]
     timestamp = datetime.now().strftime("%m%d%H%M")
     new_output_file_name = "{}_{}_{}.txt".format(base_name, endpoint_key.lower(), timestamp)
     new_output_file_path = os.path.join(output_directory, new_output_file_name)
 
-    with open(new_output_file_path, 'w') as output_file:
-        output_file.write(formatted_837p)
-
-    # need to pass config here. for what?   
-    # BUG Validate that the output file path has no spaces in it, Unless this is no issue (skip)
-    MediLink_ConfigLoader.log("Successfully converted and saved to {}".format(new_output_file_path), config, level="INFO")
-    
-    return new_output_file_path
+    # Write formatted 837P document to the output file
+    try:
+        with open(new_output_file_path, 'w') as output_file:
+            output_file.write('\n'.join(document_segments))
+        MediLink_ConfigLoader.log("Successfully converted and saved to {}".format(new_output_file_path), config, level="INFO")
+        return new_output_file_path
+    except Exception as e:
+        MediLink_ConfigLoader.log("Error: Failed to write output file. {}".format(e), config, level="ERROR")
+        return None
 
 def process_file(file_path, config, endpoint_key, transaction_set_control_number):
     """
     Reads, validates, and formats claim data from a given file into the 837P format.
 
     :param file_path: The path to the file containing claim data.
     :param config: Configuration settings loaded from a JSON file.
@@ -282,26 +301,16 @@
     # This shouldn't need to exist.
     output_directory = winscp_validate_output_directory(output_directory)
     
     if not os.path.isdir(output_directory):
         print("Output directory does not exist. Please check the configuration.")
         return None
 
-    # BUG NASTY!!!
-    # Get the current system time and format it as 'HHMMSS' in 24-hour clock.
-    current_time = datetime.now().strftime('%H%M%S')
-    isa13 = '000' + current_time  # Format ISA13 with '000HHMMSS'.
-
-    # Check if isa13 could not be generated from the current time
-    if len(isa13) != 9:
-        # If isa13 cannot be generated from the current time, use the configured value.
-        isa13 = endpoint_config.get('isa_13_value', '000000001')
-
     # Initialize document segments with headers
-    isa_header, gs_header = MediLink_837p_encoder_library.create_interchange_header(config, endpoint, isa13)
+    isa_header, gs_header = create_interchange_elements(config, endpoint, 1)
     document_segments = [isa_header, gs_header]
 
     # Initialize the transaction set control number
     transaction_set_control_number = 1
 
     # Process each patient's data in the list
     for patient_data in patient_data_list:
@@ -326,15 +335,15 @@
                 continue  # Skip the current patient and do not increment the transaction set number
             else:
                 print("Processing halted due to validation errors.")
                 MediLink_ConfigLoader.log("Processing halted at transaction set {} due to unresolved validation errors.".format(transaction_set_control_number), config, level="ERROR")
                 sys.exit()  # Optionally halt further processing
 
     # Append interchange trailer
-    ge_trailer, iea_trailer = MediLink_837p_encoder_library.create_interchange_trailer(config, transaction_set_control_number - 1, isa13)
+    ge_trailer, iea_trailer = MediLink_837p_encoder_library.create_interchange_trailer(config, transaction_set_control_number - 1, isa_header['isa_13'])
     document_segments.extend([ge_trailer, iea_trailer])
 
     # Write the complete 837P document to an output file and return its path
     return write_output_file(document_segments, output_directory, endpoint, patient_data_list[0]['file_path'], config)
 
 # Validation Function checks the completeness and correctness of each claim's data
 def validate_claim_data(parsed_data, config, required_fields=[]):
```

### Comparing `medicafe-0.240512.9/MediLink/MediLink_837p_encoder_library.py` & `medicafe-0.240513.0/MediLink/MediLink_837p_encoder_library.py`

 * *Files 2% similar despite different names*

```diff
@@ -490,54 +490,49 @@
     insurance_type_code = insurance_type_selection(parsed_data)
 
     # Construct the SBR segment using the determined codes
     sbr_segment = "SBR*{responsibility_code}*18*******{insurance_type_code}~".format(
         responsibility_code=responsibility_code,
         insurance_type_code=insurance_type_code
     )
-
     return sbr_segment
 
 def insurance_type_selection(parsed_data):
     """
-    TODO (HIGH SBR09) Finish making this function. This should integrate into a menu for now and then figure 
-    out the automated/API method to getting this.
-    
-    This menu flow probably needs to be alongside the suggested endpoint flow.
-    Default should be PPO (12), then CI, then FI as most common options , followed by the rest. 
-    
-    This is going to be really ugly and a terrible implementation but, for now, lets make a print menu in here that 
-    asks prompts the user for which insurance type the patient last_name=parsed_data['LAST'] is?
-    
-    This is the full list of options that should be available to the user. Show them this list. Explain that they need to input the 2 character code.
-    
+    Quick Fix: This funtion selects the insurance type for a patient based on predefined codes.
     
+    TODO (HIGH SBR09) Finish making this function. 
+    This should  eventually integrate into a menu upstream. This menu flow probably needs to be alongside the suggested endpoint flow.
+    For now let's make a menu here and then figure out the automated/API method to getting this per patient as there are no
+    useful historical patterns other than to say that the default should be PPO (12), then CI, then FI as most common options, 
+    followed by the rest. 
     
     Present a user-selectable menu of insurance types based on predefined codes.
+    User needs to input the desired 2 character code for that patient or default to PPO.
     
-    This function currently implements a simple text-based selection menu to choose
+    Currently implements a simple text-based selection menu to choose
     an insurance type for a patient. The default selection is '12' for PPO, but the user
     can input other codes as per the options listed. This initial implementation uses
     simple input/output functions for selection and can be replaced in the future by a 
     more dynamic interface or API-driven selection method.
 
     Future Enhancements:
-    - Implement a graphical user interface or web-based form for selections.
-    - Automate selection via an API that fetches user's most common choices or suggests based on historical data.
+    - Automate selection via an API that fetches patient data directly and auto-assigns the insurance type.
     - Error handling to manage incorrect inputs and retry mechanisms.
     
     Parameters:
     - parsed_data (dict): Contains patient's last name under key 'LAST'.
     
     Returns:
     - str: The insurance type code selected by the user.
     
     """
-    print("\nSelect the insurance type for patient {}: ".format(parsed_data['LAST']))
+    print("\nHorrible Temporary Menu: Select the insurance type for patient {}: ".format(parsed_data['LAST']))
 
+    # Define insurance options with codes and descriptions
     insurance_options = {
         "11": "Other Non-Federal Programs",
         "12": "Preferred Provider Organization (PPO)",
         "13": "Point of Service (POS)",
         "14": "Exclusive Provider Organization (EPO)",
         "15": "Indemnity Insurance",
         "16": "Health Maintenance Organization (HMO) Medicare Risk",
@@ -558,26 +553,30 @@
         "VA": "Veterans Affairs Plan",
         "WC": "Workers’ Compensation Health Claim",
         "ZZ": "Mutually Defined"
     }
 
     # Function to display full list of insurance options
     def display_insurance_options(options):
+        print("Insurance Type Options:")
         for code, description in options.items():
             print("{} - {}".format(code, description))
 
     # Prompt to display full list
     display_full_list = input("Do you want to see the full list of insurance options? (yes/no): ").strip().lower()
 
-    if display_full_list == 'yes':
+    # Display full list if user confirms
+    if display_full_list in ['yes', 'y']:
         display_insurance_options(insurance_options)
 
     # Default selection
     insurance_type_code = '12'
-    user_input = input("Enter the 2 character code for the insurance type (default '12' for PPO): ").strip()
+
+    # User input for insurance type
+    user_input = input("Enter the 2-character code for the insurance type (or press Enter to default to '12' for PPO): ").strip().upper()
 
     # Validate input and set the insurance type code
     if user_input in insurance_options:
         insurance_type_code = user_input
     else:
         print("Invalid input. Defaulting to Preferred Provider Organization (PPO)")
 
@@ -614,15 +613,15 @@
     return "DMG*D8*{}*{}~".format(
         convert_date_format(parsed_data['BDAY']),  
         parsed_data['SEX'] # ensure it returns a string instead of a list if it only returns one segment
     )
 
 def create_nm1_rendering_provider_segment(config, is_rendering_provider_different=False):
     """
-    #BUG This is getting placed incorrectly.
+    # BUG This is getting placed incorrectly. Has this been fixed??
     
     Constructs the NM1 segment for the rendering provider in the 2310B loop using configuration data.
     
     Parameters:
     - config: Configuration dictionary including rendering provider details.
     - is_rendering_provider_different: Boolean indicating if rendering provider differs from billing provider.
```

### Comparing `medicafe-0.240512.9/MediLink/MediLink_ConfigLoader.py` & `medicafe-0.240513.0/MediLink/MediLink_ConfigLoader.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.9/MediLink/MediLink_DataMgmt.py` & `medicafe-0.240513.0/MediLink/MediLink_DataMgmt.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.9/MediLink/MediLink_Down.py` & `medicafe-0.240513.0/MediLink/MediLink_Down.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.9/MediLink/MediLink_ERA_decoder.py` & `medicafe-0.240513.0/MediLink/MediLink_ERA_decoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.9/MediLink/MediLink_Gmail.py` & `medicafe-0.240513.0/MediLink/MediLink_Gmail.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.9/MediLink/MediLink_Scheduler.py` & `medicafe-0.240513.0/MediLink/MediLink_Scheduler.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.9/MediLink/MediLink_UI.py` & `medicafe-0.240513.0/MediLink/MediLink_UI.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.9/MediLink/MediLink_Up.py` & `medicafe-0.240513.0/MediLink/MediLink_Up.py`

 * *Files 8% similar despite different names*

```diff
@@ -207,78 +207,122 @@
     
     Returns:
     - dict: Organized data for receipt preparation, including both successful and failed submission details.
     """
     receipt_data = {}
     for endpoint, files in submission_results.items():
         for file_path, success in files.items():
-            # Parse the 837p file for patient data, regardless of success
-            patient_data = parse_837p_file(file_path)
-            date_of_submission = datetime.now().strftime("%Y-%m-%d %H:%M:%S")  # Placeholder for actual submission date from file
+            # Parse the 837p file for patient data, regardless of success.
+            patient_data, date_of_submission = parse_837p_file(file_path)
             
             if endpoint not in receipt_data:
                 receipt_data[endpoint] = {
                     "date_of_submission": date_of_submission,
                     "patients": []
                 }
 
             # Enhance patient data with success status
             for patient in patient_data:
                 patient['success'] = success
             
             receipt_data[endpoint]["patients"].extend(patient_data)
-
+    
+    validate_data(receipt_data)
     return receipt_data
 
+def validate_data(patient_data):
+    # Simple validation to check if data fields are correctly populated
+    for index, data in enumerate(patient_data, start=1):
+        missing_fields = [field for field in ('name', 'service_date', 'amount_billed', 'success') if not data.get(field)]
+        
+        if missing_fields:
+            # Log the missing fields without revealing PHI
+            log("Receipt Data validation error for patient {}: Missing information in fields: {}".format(index, ", ".join(missing_fields)))
+    return True
+
 def parse_837p_file(file_path):
+    """
+    Parse an 837p file to extract patient details and date of submission.
+
+    This function reads the specified 837p file, extracts patient details such as name, service date, and amount billed,
+    and retrieves the date of submission from the GS segment. It then organizes this information into a list of dictionaries
+    containing patient data. If the GS segment is not found, it falls back to using the current date and time.
+
+    Parameters:
+    - file_path (str): The path to the 837p file to parse.
+
+    Returns:
+    - tuple: A tuple containing two elements:
+        - A list of dictionaries, where each dictionary represents patient details including name, service date, and amount billed.
+        - A string representing the date and time of submission in the format 'YYYY-MM-DD HH:MM:SS'.
+    """
     patient_details = []
+    date_of_submission = None
     try:
         with open(file_path, 'r') as file:
             content = file.read()
             log("Parsing submitted 837p...")
-            
-            # Patient Names
-            names = re.findall(r'NM1\*[^*]*\*1\*([^\*]+)\*([^\*]+)\*([^\*]+)', content)  # Updated regex to include middle name
-            
-            # Service Dates
-            dates = re.findall(r'DTP\*472\D8\*([0-9]{8})', content)
-            
-            # Amounts Billed
-            amounts = re.findall(r'CLM\*[^\*]*\*([0-9]+\.?[0-9]*)\*', content)
-            
-            # Assuming each match is aligned across the three lists
-            for name, date, amount in zip(names, dates, amounts):
-                patient_name = "{0} {1} {2}".format(name[1], name[0], name[2])  # First, Middle, and Last Name
-                service_date = "{0}-{1}-{2}".format(date[:4], date[4:6], date[6:])  # Convert YYYYMMDD to YYYY-MM-DD
-                amount_billed = float(amount)
+
+            # Extract the submission date from the GS segment
+            gs_match = re.search(r'GS\*HC\*[^*]*\*[^*]*\*([0-9]{8})\*([0-9]{4})', content)
+            if gs_match:
+                date = gs_match.group(1)
+                time = gs_match.group(2)
+                date_of_submission = datetime.strptime("{}{}".format(date, time), "%Y%m%d%H%M").strftime("%Y-%m-%d %H:%M:%S")
+            else:
+                # Fallback to the current date and time if GS segment is not found
+                date_of_submission = datetime.now().strftime("%Y-%m-%d %H:%M:%S")
+
+            # Split content using 'SE*{count}*{control_number}~' as delimiter
+            patient_records = re.split(r'SE\*\d+\*\d{4}~', content)
+            
+            # Remove any empty strings from list that may have been added from split
+            patient_records = [record for record in patient_records if record.strip()]
+            
+            for record in patient_records:
+                # Extract patient name
+                name_match = re.search(r'NM1\*IL\*1\*([^*]+)\*([^*]+)\*([^*]*)', record)
+                # Extract service date
+                service_date_match = re.search(r'DTP\*472\D*8\*([0-9]{8})', record)
+                # Extract claim amount
+                amount_match = re.search(r'CLM\*[^\*]*\*([0-9]+\.?[0-9]*)', record)
                 
-                patient_details.append({
-                    "name": patient_name,
-                    "service_date": service_date,
-                    "amount_billed": amount_billed
-                })
+                if name_match and service_date_match and amount_match:
+                    # Handle optional middle name
+                    middle_name = name_match.group(3).strip() if name_match.group(3) else ""
+                    patient_name = "{} {} {}".format(name_match.group(2), middle_name, name_match.group(1)).strip()
+                    service_date = "{}-{}-{}".format(service_date_match.group(1)[:4], service_date_match.group(1)[4:6], service_date_match.group(1)[6:])
+                    amount_billed = float(amount_match.group(1))
+                    
+                    patient_details.append({
+                        "name": patient_name,
+                        "service_date": service_date,
+                        "amount_billed": amount_billed
+                    })
     except Exception as e:
-        print("Error reading or parsing the 837p file {0}: {1}".format(file_path, str(e)))
-
-    return patient_details
+        print("Error reading or parsing the 837p file: {0}".format(str(e)))
+    
+    # Optionally, return also date_of_submission as a separate variable  
+    return patient_details, date_of_submission
 
 def build_receipt_content(receipt_data):
     # Build the receipt content in a human-readable ASCII format
     # Format the receipt content to display endpoint-wise with associated patient information
     # Use ASCII art or other formatting techniques to make the receipt visually appealing
     receipt_lines = ["Submission Receipt", "="*60, ""]  # Header
     for endpoint, data in receipt_data.items():
         header = "Endpoint: {0} (Submitted: {1})".format(endpoint, data['date_of_submission'])
         receipt_lines.extend([header, "-"*len(header)])
         
         # Adding patient information
         for patient in data["patients"]:
-            patient_info = "Patient: {0}, Service Date: {1}, Amount Billed: ${2}".format(patient['name'], patient['service_date'], patient['amount_billed'])
+            success_status = "SUCCESS" if patient['success'] else "FAILED"
+            patient_info = "Patient: {0}, Service Date: {1}, Amount Billed: ${2}, Submission Status: {3}".format(patient['name'], patient['service_date'], patient['amount_billed'], success_status)
             receipt_lines.append(patient_info)
-        
+            
         receipt_lines.append("")  # Blank line for separation
     
     receipt_content = "\n".join(receipt_lines)
     return receipt_content
 
 def save_receipt_to_file(receipt_content, config):
     try:
```

### Comparing `medicafe-0.240512.9/README.md` & `medicafe-0.240513.0/README.md`

 * *Files identical despite different names*

### Comparing `medicafe-0.240512.9/medicafe.egg-info/SOURCES.txt` & `medicafe-0.240513.0/medicafe.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -26,13 +26,14 @@
 MediLink/MediLink_Scheduler.py
 MediLink/MediLink_StatusCheck.py
 MediLink/MediLink_UI.py
 MediLink/MediLink_Up.py
 MediLink/MediLink_batch.bat
 MediLink/Soumit_api.py
 MediLink/__init__.py
+MediLink/test.py
 medicafe.egg-info/PKG-INFO
 medicafe.egg-info/SOURCES.txt
 medicafe.egg-info/dependency_links.txt
 medicafe.egg-info/not-zip-safe
 medicafe.egg-info/requires.txt
 medicafe.egg-info/top_level.txt
```

