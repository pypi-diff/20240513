# Comparing `tmp/medicafe-0.240513.0.tar.gz` & `tmp/medicafe-0.240513.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medicafe-0.240513.0.tar", last modified: Mon May 13 07:22:23 2024, max compression
+gzip compressed data, was "medicafe-0.240513.1.tar", last modified: Mon May 13 14:09:41 2024, max compression
```

## Comparing `medicafe-0.240513.0.tar` & `medicafe-0.240513.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 07:22:23.571000 medicafe-0.240513.0/
--rw-rw-rw-   0        0        0     1096 2024-04-16 02:27:27.000000 medicafe-0.240513.0/LICENSE
--rw-rw-rw-   0        0        0       64 2024-04-19 20:12:06.000000 medicafe-0.240513.0/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2024-05-13 07:22:22.930000 medicafe-0.240513.0/MediBot/
--rwxrwxrwx   0        0        0     5972 2024-05-12 18:02:44.000000 medicafe-0.240513.0/MediBot/MediBot.bat
--rw-rw-rw-   0        0        0    17343 2024-05-12 16:32:17.000000 medicafe-0.240513.0/MediBot/MediBot.py
--rw-rw-rw-   0        0        0     1963 2024-04-17 03:06:31.000000 medicafe-0.240513.0/MediBot/MediBot_Charges.py
--rw-rw-rw-   0        0        0    33980 2024-05-12 16:14:26.000000 medicafe-0.240513.0/MediBot/MediBot_Preprocessor.py
--rw-rw-rw-   0        0        0     4589 2024-05-12 17:14:28.000000 medicafe-0.240513.0/MediBot/MediBot_Preprocessor_lib.py
--rw-rw-rw-   0        0        0    10660 2024-05-09 04:53:27.000000 medicafe-0.240513.0/MediBot/MediBot_UI.py
--rw-rw-rw-   0        0        0     8636 2024-05-12 16:11:39.000000 medicafe-0.240513.0/MediBot/MediBot_dataformat_library.py
--rw-rw-rw-   0        0        0      336 2024-04-18 22:50:25.000000 medicafe-0.240513.0/MediBot/MediPost.py
--rw-rw-rw-   0        0        0     8799 2024-01-30 04:51:58.000000 medicafe-0.240513.0/MediBot/PDF_to_CSV_Cleaner.py
--rw-rw-rw-   0        0        0        0 2024-04-19 02:51:16.000000 medicafe-0.240513.0/MediBot/__init__.py
--rw-rw-rw-   0        0        0     1557 2024-04-12 16:06:52.000000 medicafe-0.240513.0/MediBot/update_json.py
--rw-rw-rw-   0        0        0     2249 2024-05-10 17:47:37.000000 medicafe-0.240513.0/MediBot/update_medicafe.py
-drwxrwxrwx   0        0        0        0 2024-05-13 07:22:23.384000 medicafe-0.240513.0/MediLink/
--rw-rw-rw-   0        0        0    19263 2024-05-13 06:46:25.000000 medicafe-0.240513.0/MediLink/MediLink.py
--rw-rw-rw-   0        0        0     4358 2024-04-13 18:24:36.000000 medicafe-0.240513.0/MediLink/MediLink_277_decoder.py
--rw-rw-rw-   0        0        0    26188 2024-05-13 06:12:51.000000 medicafe-0.240513.0/MediLink/MediLink_837p_encoder.py
--rw-rw-rw-   0        0        0    39298 2024-05-13 06:41:12.000000 medicafe-0.240513.0/MediLink/MediLink_837p_encoder_library.py
--rw-rw-rw-   0        0        0     3914 2024-05-09 02:18:58.000000 medicafe-0.240513.0/MediLink/MediLink_ConfigLoader.py
--rw-rw-rw-   0        0        0    11857 2024-05-12 18:32:20.000000 medicafe-0.240513.0/MediLink/MediLink_DataMgmt.py
--rw-rw-rw-   0        0        0     7264 2024-05-08 01:45:53.000000 medicafe-0.240513.0/MediLink/MediLink_Down.py
--rw-rw-rw-   0        0        0     8724 2024-05-01 03:44:46.000000 medicafe-0.240513.0/MediLink/MediLink_ERA_decoder.py
--rw-rw-rw-   0        0        0     6236 2024-05-10 16:45:40.000000 medicafe-0.240513.0/MediLink/MediLink_Gmail.py
--rw-rw-rw-   0        0        0     6040 2024-04-18 22:53:51.000000 medicafe-0.240513.0/MediLink/MediLink_Scheduler.py
--rw-rw-rw-   0        0        0      222 2024-04-13 17:51:42.000000 medicafe-0.240513.0/MediLink/MediLink_StatusCheck.py
--rw-rw-rw-   0        0        0     5181 2024-05-12 16:36:09.000000 medicafe-0.240513.0/MediLink/MediLink_UI.py
--rw-rw-rw-   0        0        0    18988 2024-05-13 05:01:21.000000 medicafe-0.240513.0/MediLink/MediLink_Up.py
--rwxrwxrwx   0        0        0      118 2024-04-19 22:20:37.000000 medicafe-0.240513.0/MediLink/MediLink_batch.bat
--rw-rw-rw-   0        0        0      497 2024-03-15 19:39:51.000000 medicafe-0.240513.0/MediLink/Soumit_api.py
--rw-rw-rw-   0        0        0        0 2024-04-19 02:51:01.000000 medicafe-0.240513.0/MediLink/__init__.py
--rw-rw-rw-   0        0        0     3108 2024-05-13 04:52:22.000000 medicafe-0.240513.0/MediLink/test.py
--rw-rw-rw-   0        0        0     4396 2024-05-13 07:22:23.557000 medicafe-0.240513.0/PKG-INFO
--rw-rw-rw-   0        0        0      994 2024-04-16 02:33:22.000000 medicafe-0.240513.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-13 07:22:23.542000 medicafe-0.240513.0/medicafe.egg-info/
--rw-rw-rw-   0        0        0     4396 2024-05-13 07:22:22.000000 medicafe-0.240513.0/medicafe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1023 2024-05-13 07:22:22.000000 medicafe-0.240513.0/medicafe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 07:22:22.000000 medicafe-0.240513.0/medicafe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-16 03:47:58.000000 medicafe-0.240513.0/medicafe.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       60 2024-05-13 07:22:22.000000 medicafe-0.240513.0/medicafe.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-13 07:22:22.000000 medicafe-0.240513.0/medicafe.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-13 07:22:23.567000 medicafe-0.240513.0/setup.cfg
--rw-rw-rw-   0        0        0     4834 2024-05-13 07:22:19.000000 medicafe-0.240513.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:09:41.767000 medicafe-0.240513.1/
+-rw-rw-rw-   0        0        0     1096 2024-04-16 02:27:27.000000 medicafe-0.240513.1/LICENSE
+-rw-rw-rw-   0        0        0       64 2024-04-19 20:12:06.000000 medicafe-0.240513.1/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2024-05-13 14:09:40.917000 medicafe-0.240513.1/MediBot/
+-rwxrwxrwx   0        0        0     5972 2024-05-12 18:02:44.000000 medicafe-0.240513.1/MediBot/MediBot.bat
+-rw-rw-rw-   0        0        0    17343 2024-05-12 16:32:17.000000 medicafe-0.240513.1/MediBot/MediBot.py
+-rw-rw-rw-   0        0        0     1963 2024-04-17 03:06:31.000000 medicafe-0.240513.1/MediBot/MediBot_Charges.py
+-rw-rw-rw-   0        0        0    33980 2024-05-12 16:14:26.000000 medicafe-0.240513.1/MediBot/MediBot_Preprocessor.py
+-rw-rw-rw-   0        0        0     4589 2024-05-12 17:14:28.000000 medicafe-0.240513.1/MediBot/MediBot_Preprocessor_lib.py
+-rw-rw-rw-   0        0        0    10660 2024-05-09 04:53:27.000000 medicafe-0.240513.1/MediBot/MediBot_UI.py
+-rw-rw-rw-   0        0        0     8636 2024-05-12 16:11:39.000000 medicafe-0.240513.1/MediBot/MediBot_dataformat_library.py
+-rw-rw-rw-   0        0        0      336 2024-04-18 22:50:25.000000 medicafe-0.240513.1/MediBot/MediPost.py
+-rw-rw-rw-   0        0        0     8799 2024-01-30 04:51:58.000000 medicafe-0.240513.1/MediBot/PDF_to_CSV_Cleaner.py
+-rw-rw-rw-   0        0        0        0 2024-04-19 02:51:16.000000 medicafe-0.240513.1/MediBot/__init__.py
+-rw-rw-rw-   0        0        0     1557 2024-04-12 16:06:52.000000 medicafe-0.240513.1/MediBot/update_json.py
+-rw-rw-rw-   0        0        0     2249 2024-05-10 17:47:37.000000 medicafe-0.240513.1/MediBot/update_medicafe.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:09:41.563000 medicafe-0.240513.1/MediLink/
+-rw-rw-rw-   0        0        0    19263 2024-05-13 06:46:25.000000 medicafe-0.240513.1/MediLink/MediLink.py
+-rw-rw-rw-   0        0        0     4358 2024-04-13 18:24:36.000000 medicafe-0.240513.1/MediLink/MediLink_277_decoder.py
+-rw-rw-rw-   0        0        0    26271 2024-05-13 14:06:59.000000 medicafe-0.240513.1/MediLink/MediLink_837p_encoder.py
+-rw-rw-rw-   0        0        0    39298 2024-05-13 06:41:12.000000 medicafe-0.240513.1/MediLink/MediLink_837p_encoder_library.py
+-rw-rw-rw-   0        0        0     3914 2024-05-09 02:18:58.000000 medicafe-0.240513.1/MediLink/MediLink_ConfigLoader.py
+-rw-rw-rw-   0        0        0    11857 2024-05-12 18:32:20.000000 medicafe-0.240513.1/MediLink/MediLink_DataMgmt.py
+-rw-rw-rw-   0        0        0     7264 2024-05-08 01:45:53.000000 medicafe-0.240513.1/MediLink/MediLink_Down.py
+-rw-rw-rw-   0        0        0     8724 2024-05-01 03:44:46.000000 medicafe-0.240513.1/MediLink/MediLink_ERA_decoder.py
+-rw-rw-rw-   0        0        0     6236 2024-05-10 16:45:40.000000 medicafe-0.240513.1/MediLink/MediLink_Gmail.py
+-rw-rw-rw-   0        0        0     6040 2024-04-18 22:53:51.000000 medicafe-0.240513.1/MediLink/MediLink_Scheduler.py
+-rw-rw-rw-   0        0        0      222 2024-04-13 17:51:42.000000 medicafe-0.240513.1/MediLink/MediLink_StatusCheck.py
+-rw-rw-rw-   0        0        0     5181 2024-05-12 16:36:09.000000 medicafe-0.240513.1/MediLink/MediLink_UI.py
+-rw-rw-rw-   0        0        0    18988 2024-05-13 05:01:21.000000 medicafe-0.240513.1/MediLink/MediLink_Up.py
+-rwxrwxrwx   0        0        0      118 2024-04-19 22:20:37.000000 medicafe-0.240513.1/MediLink/MediLink_batch.bat
+-rw-rw-rw-   0        0        0      497 2024-03-15 19:39:51.000000 medicafe-0.240513.1/MediLink/Soumit_api.py
+-rw-rw-rw-   0        0        0        0 2024-04-19 02:51:01.000000 medicafe-0.240513.1/MediLink/__init__.py
+-rw-rw-rw-   0        0        0     3108 2024-05-13 04:52:22.000000 medicafe-0.240513.1/MediLink/test.py
+-rw-rw-rw-   0        0        0     4396 2024-05-13 14:09:41.752000 medicafe-0.240513.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2960 2024-05-13 07:31:39.000000 medicafe-0.240513.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 14:09:41.735000 medicafe-0.240513.1/medicafe.egg-info/
+-rw-rw-rw-   0        0        0     4396 2024-05-13 14:09:40.000000 medicafe-0.240513.1/medicafe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1023 2024-05-13 14:09:40.000000 medicafe-0.240513.1/medicafe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 14:09:40.000000 medicafe-0.240513.1/medicafe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-16 03:47:58.000000 medicafe-0.240513.1/medicafe.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       60 2024-05-13 14:09:40.000000 medicafe-0.240513.1/medicafe.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-13 14:09:40.000000 medicafe-0.240513.1/medicafe.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 14:09:41.763000 medicafe-0.240513.1/setup.cfg
+-rw-rw-rw-   0        0        0     4834 2024-05-13 14:09:36.000000 medicafe-0.240513.1/setup.py
```

### Comparing `medicafe-0.240513.0/LICENSE` & `medicafe-0.240513.1/LICENSE`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.0/MediBot/MediBot.bat` & `medicafe-0.240513.1/MediBot/MediBot.bat`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.0/MediBot/MediBot.py` & `medicafe-0.240513.1/MediBot/MediBot.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.0/MediBot/MediBot_Charges.py` & `medicafe-0.240513.1/MediBot/MediBot_Charges.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.0/MediBot/MediBot_Preprocessor.py` & `medicafe-0.240513.1/MediBot/MediBot_Preprocessor.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.0/MediBot/MediBot_Preprocessor_lib.py` & `medicafe-0.240513.1/MediBot/MediBot_Preprocessor_lib.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.0/MediBot/MediBot_UI.py` & `medicafe-0.240513.1/MediBot/MediBot_UI.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.0/MediBot/MediBot_dataformat_library.py` & `medicafe-0.240513.1/MediBot/MediBot_dataformat_library.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.0/MediBot/PDF_to_CSV_Cleaner.py` & `medicafe-0.240513.1/MediBot/PDF_to_CSV_Cleaner.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.0/MediBot/update_json.py` & `medicafe-0.240513.1/MediBot/update_json.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.0/MediBot/update_medicafe.py` & `medicafe-0.240513.1/MediBot/update_medicafe.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.0/MediLink/MediLink.py` & `medicafe-0.240513.1/MediLink/MediLink.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.0/MediLink/MediLink_277_decoder.py` & `medicafe-0.240513.1/MediLink/MediLink_277_decoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.0/MediLink/MediLink_837p_encoder.py` & `medicafe-0.240513.1/MediLink/MediLink_837p_encoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -301,20 +301,17 @@
     # This shouldn't need to exist.
     output_directory = winscp_validate_output_directory(output_directory)
     
     if not os.path.isdir(output_directory):
         print("Output directory does not exist. Please check the configuration.")
         return None
 
-    # Initialize document segments with headers
-    isa_header, gs_header = create_interchange_elements(config, endpoint, 1)
-    document_segments = [isa_header, gs_header]
-
-    # Initialize the transaction set control number
+    # Initialize the transaction set control number and document segments
     transaction_set_control_number = 1
+    document_segments = []
 
     # Process each patient's data in the list
     for patient_data in patient_data_list:
         # Validate each patient's data
         is_valid, validation_errors = validate_claim_data(patient_data, config)
         if is_valid:
             # Format the claim if data is valid
@@ -334,16 +331,20 @@
                 MediLink_ConfigLoader.log("Skipped processing of transaction set {} due to user decision.".format(transaction_set_control_number), config, level="INFO")
                 continue  # Skip the current patient and do not increment the transaction set number
             else:
                 print("Processing halted due to validation errors.")
                 MediLink_ConfigLoader.log("Processing halted at transaction set {} due to unresolved validation errors.".format(transaction_set_control_number), config, level="ERROR")
                 sys.exit()  # Optionally halt further processing
 
-    # Append interchange trailer
-    ge_trailer, iea_trailer = MediLink_837p_encoder_library.create_interchange_trailer(config, transaction_set_control_number - 1, isa_header['isa_13'])
+    # Create interchange elements with the final transaction set control number
+    isa_header, gs_header, ge_trailer, iea_trailer = create_interchange_elements(config, endpoint, transaction_set_control_number - 1)
+
+    # Insert headers at the beginning and append trailers at the end of document segments
+    document_segments.insert(0, gs_header)
+    document_segments.insert(0, isa_header)
     document_segments.extend([ge_trailer, iea_trailer])
 
     # Write the complete 837P document to an output file and return its path
     return write_output_file(document_segments, output_directory, endpoint, patient_data_list[0]['file_path'], config)
 
 # Validation Function checks the completeness and correctness of each claim's data
 def validate_claim_data(parsed_data, config, required_fields=[]):
```

### Comparing `medicafe-0.240513.0/MediLink/MediLink_837p_encoder_library.py` & `medicafe-0.240513.1/MediLink/MediLink_837p_encoder_library.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.0/MediLink/MediLink_ConfigLoader.py` & `medicafe-0.240513.1/MediLink/MediLink_ConfigLoader.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.0/MediLink/MediLink_DataMgmt.py` & `medicafe-0.240513.1/MediLink/MediLink_DataMgmt.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.0/MediLink/MediLink_Down.py` & `medicafe-0.240513.1/MediLink/MediLink_Down.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.0/MediLink/MediLink_ERA_decoder.py` & `medicafe-0.240513.1/MediLink/MediLink_ERA_decoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.0/MediLink/MediLink_Gmail.py` & `medicafe-0.240513.1/MediLink/MediLink_Gmail.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.0/MediLink/MediLink_Scheduler.py` & `medicafe-0.240513.1/MediLink/MediLink_Scheduler.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.0/MediLink/MediLink_UI.py` & `medicafe-0.240513.1/MediLink/MediLink_UI.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.0/MediLink/MediLink_Up.py` & `medicafe-0.240513.1/MediLink/MediLink_Up.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.0/MediLink/test.py` & `medicafe-0.240513.1/MediLink/test.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.0/PKG-INFO` & `medicafe-0.240513.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medicafe
-Version: 0.240513.0
+Version: 0.240513.1
 Summary: MediCafe
 Home-page: https://github.com/katanada2
 Author: Daniel Vidaud
 Author-email: daniel@personalizedtransformation.com
 License: MIT
 Keywords: medicafe python34 medibot medilink
 Description-Content-Type: text/markdown
```

### Comparing `medicafe-0.240513.0/medicafe.egg-info/PKG-INFO` & `medicafe-0.240513.1/medicafe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medicafe
-Version: 0.240513.0
+Version: 0.240513.1
 Summary: MediCafe
 Home-page: https://github.com/katanada2
 Author: Daniel Vidaud
 Author-email: daniel@personalizedtransformation.com
 License: MIT
 Keywords: medicafe python34 medibot medilink
 Description-Content-Type: text/markdown
```

### Comparing `medicafe-0.240513.0/medicafe.egg-info/SOURCES.txt` & `medicafe-0.240513.1/medicafe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.0/setup.py` & `medicafe-0.240513.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='medicafe',
-    version="0.240513.0",
+    version="0.240513.1",
     description='MediCafe',
     long_description="""
     # Project Overview: MediCafe
 
     ## Project Description
     MediCafe is a comprehensive suite designed to automate and streamline several aspects of medical administrative tasks within Medisoft, a popular medical practice management software. The system consists of two main components: MediBot and MediLink, each serving distinct functions but integrated to enhance the workflow of medical practices.
```

