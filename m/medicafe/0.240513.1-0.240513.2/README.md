# Comparing `tmp/medicafe-0.240513.1.tar.gz` & `tmp/medicafe-0.240513.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medicafe-0.240513.1.tar", last modified: Mon May 13 14:09:41 2024, max compression
+gzip compressed data, was "medicafe-0.240513.2.tar", last modified: Mon May 13 14:57:53 2024, max compression
```

## Comparing `medicafe-0.240513.1.tar` & `medicafe-0.240513.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 14:09:41.767000 medicafe-0.240513.1/
--rw-rw-rw-   0        0        0     1096 2024-04-16 02:27:27.000000 medicafe-0.240513.1/LICENSE
--rw-rw-rw-   0        0        0       64 2024-04-19 20:12:06.000000 medicafe-0.240513.1/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2024-05-13 14:09:40.917000 medicafe-0.240513.1/MediBot/
--rwxrwxrwx   0        0        0     5972 2024-05-12 18:02:44.000000 medicafe-0.240513.1/MediBot/MediBot.bat
--rw-rw-rw-   0        0        0    17343 2024-05-12 16:32:17.000000 medicafe-0.240513.1/MediBot/MediBot.py
--rw-rw-rw-   0        0        0     1963 2024-04-17 03:06:31.000000 medicafe-0.240513.1/MediBot/MediBot_Charges.py
--rw-rw-rw-   0        0        0    33980 2024-05-12 16:14:26.000000 medicafe-0.240513.1/MediBot/MediBot_Preprocessor.py
--rw-rw-rw-   0        0        0     4589 2024-05-12 17:14:28.000000 medicafe-0.240513.1/MediBot/MediBot_Preprocessor_lib.py
--rw-rw-rw-   0        0        0    10660 2024-05-09 04:53:27.000000 medicafe-0.240513.1/MediBot/MediBot_UI.py
--rw-rw-rw-   0        0        0     8636 2024-05-12 16:11:39.000000 medicafe-0.240513.1/MediBot/MediBot_dataformat_library.py
--rw-rw-rw-   0        0        0      336 2024-04-18 22:50:25.000000 medicafe-0.240513.1/MediBot/MediPost.py
--rw-rw-rw-   0        0        0     8799 2024-01-30 04:51:58.000000 medicafe-0.240513.1/MediBot/PDF_to_CSV_Cleaner.py
--rw-rw-rw-   0        0        0        0 2024-04-19 02:51:16.000000 medicafe-0.240513.1/MediBot/__init__.py
--rw-rw-rw-   0        0        0     1557 2024-04-12 16:06:52.000000 medicafe-0.240513.1/MediBot/update_json.py
--rw-rw-rw-   0        0        0     2249 2024-05-10 17:47:37.000000 medicafe-0.240513.1/MediBot/update_medicafe.py
-drwxrwxrwx   0        0        0        0 2024-05-13 14:09:41.563000 medicafe-0.240513.1/MediLink/
--rw-rw-rw-   0        0        0    19263 2024-05-13 06:46:25.000000 medicafe-0.240513.1/MediLink/MediLink.py
--rw-rw-rw-   0        0        0     4358 2024-04-13 18:24:36.000000 medicafe-0.240513.1/MediLink/MediLink_277_decoder.py
--rw-rw-rw-   0        0        0    26271 2024-05-13 14:06:59.000000 medicafe-0.240513.1/MediLink/MediLink_837p_encoder.py
--rw-rw-rw-   0        0        0    39298 2024-05-13 06:41:12.000000 medicafe-0.240513.1/MediLink/MediLink_837p_encoder_library.py
--rw-rw-rw-   0        0        0     3914 2024-05-09 02:18:58.000000 medicafe-0.240513.1/MediLink/MediLink_ConfigLoader.py
--rw-rw-rw-   0        0        0    11857 2024-05-12 18:32:20.000000 medicafe-0.240513.1/MediLink/MediLink_DataMgmt.py
--rw-rw-rw-   0        0        0     7264 2024-05-08 01:45:53.000000 medicafe-0.240513.1/MediLink/MediLink_Down.py
--rw-rw-rw-   0        0        0     8724 2024-05-01 03:44:46.000000 medicafe-0.240513.1/MediLink/MediLink_ERA_decoder.py
--rw-rw-rw-   0        0        0     6236 2024-05-10 16:45:40.000000 medicafe-0.240513.1/MediLink/MediLink_Gmail.py
--rw-rw-rw-   0        0        0     6040 2024-04-18 22:53:51.000000 medicafe-0.240513.1/MediLink/MediLink_Scheduler.py
--rw-rw-rw-   0        0        0      222 2024-04-13 17:51:42.000000 medicafe-0.240513.1/MediLink/MediLink_StatusCheck.py
--rw-rw-rw-   0        0        0     5181 2024-05-12 16:36:09.000000 medicafe-0.240513.1/MediLink/MediLink_UI.py
--rw-rw-rw-   0        0        0    18988 2024-05-13 05:01:21.000000 medicafe-0.240513.1/MediLink/MediLink_Up.py
--rwxrwxrwx   0        0        0      118 2024-04-19 22:20:37.000000 medicafe-0.240513.1/MediLink/MediLink_batch.bat
--rw-rw-rw-   0        0        0      497 2024-03-15 19:39:51.000000 medicafe-0.240513.1/MediLink/Soumit_api.py
--rw-rw-rw-   0        0        0        0 2024-04-19 02:51:01.000000 medicafe-0.240513.1/MediLink/__init__.py
--rw-rw-rw-   0        0        0     3108 2024-05-13 04:52:22.000000 medicafe-0.240513.1/MediLink/test.py
--rw-rw-rw-   0        0        0     4396 2024-05-13 14:09:41.752000 medicafe-0.240513.1/PKG-INFO
--rw-rw-rw-   0        0        0     2960 2024-05-13 07:31:39.000000 medicafe-0.240513.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-13 14:09:41.735000 medicafe-0.240513.1/medicafe.egg-info/
--rw-rw-rw-   0        0        0     4396 2024-05-13 14:09:40.000000 medicafe-0.240513.1/medicafe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1023 2024-05-13 14:09:40.000000 medicafe-0.240513.1/medicafe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 14:09:40.000000 medicafe-0.240513.1/medicafe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-16 03:47:58.000000 medicafe-0.240513.1/medicafe.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       60 2024-05-13 14:09:40.000000 medicafe-0.240513.1/medicafe.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-13 14:09:40.000000 medicafe-0.240513.1/medicafe.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-13 14:09:41.763000 medicafe-0.240513.1/setup.cfg
--rw-rw-rw-   0        0        0     4834 2024-05-13 14:09:36.000000 medicafe-0.240513.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:57:53.328000 medicafe-0.240513.2/
+-rw-rw-rw-   0        0        0     1096 2024-04-16 02:27:27.000000 medicafe-0.240513.2/LICENSE
+-rw-rw-rw-   0        0        0       64 2024-04-19 20:12:06.000000 medicafe-0.240513.2/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2024-05-13 14:57:52.493000 medicafe-0.240513.2/MediBot/
+-rwxrwxrwx   0        0        0     5972 2024-05-12 18:02:44.000000 medicafe-0.240513.2/MediBot/MediBot.bat
+-rw-rw-rw-   0        0        0    17343 2024-05-12 16:32:17.000000 medicafe-0.240513.2/MediBot/MediBot.py
+-rw-rw-rw-   0        0        0     1963 2024-04-17 03:06:31.000000 medicafe-0.240513.2/MediBot/MediBot_Charges.py
+-rw-rw-rw-   0        0        0    33980 2024-05-12 16:14:26.000000 medicafe-0.240513.2/MediBot/MediBot_Preprocessor.py
+-rw-rw-rw-   0        0        0     4589 2024-05-12 17:14:28.000000 medicafe-0.240513.2/MediBot/MediBot_Preprocessor_lib.py
+-rw-rw-rw-   0        0        0    10660 2024-05-09 04:53:27.000000 medicafe-0.240513.2/MediBot/MediBot_UI.py
+-rw-rw-rw-   0        0        0     8636 2024-05-12 16:11:39.000000 medicafe-0.240513.2/MediBot/MediBot_dataformat_library.py
+-rw-rw-rw-   0        0        0      336 2024-04-18 22:50:25.000000 medicafe-0.240513.2/MediBot/MediPost.py
+-rw-rw-rw-   0        0        0     8799 2024-01-30 04:51:58.000000 medicafe-0.240513.2/MediBot/PDF_to_CSV_Cleaner.py
+-rw-rw-rw-   0        0        0        0 2024-04-19 02:51:16.000000 medicafe-0.240513.2/MediBot/__init__.py
+-rw-rw-rw-   0        0        0     1557 2024-04-12 16:06:52.000000 medicafe-0.240513.2/MediBot/update_json.py
+-rw-rw-rw-   0        0        0     2249 2024-05-10 17:47:37.000000 medicafe-0.240513.2/MediBot/update_medicafe.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:57:53.078000 medicafe-0.240513.2/MediLink/
+-rw-rw-rw-   0        0        0    19263 2024-05-13 06:46:25.000000 medicafe-0.240513.2/MediLink/MediLink.py
+-rw-rw-rw-   0        0        0     4358 2024-04-13 18:24:36.000000 medicafe-0.240513.2/MediLink/MediLink_277_decoder.py
+-rw-rw-rw-   0        0        0    26271 2024-05-13 14:06:59.000000 medicafe-0.240513.2/MediLink/MediLink_837p_encoder.py
+-rw-rw-rw-   0        0        0    39431 2024-05-13 14:41:19.000000 medicafe-0.240513.2/MediLink/MediLink_837p_encoder_library.py
+-rw-rw-rw-   0        0        0     3914 2024-05-09 02:18:58.000000 medicafe-0.240513.2/MediLink/MediLink_ConfigLoader.py
+-rw-rw-rw-   0        0        0    11857 2024-05-12 18:32:20.000000 medicafe-0.240513.2/MediLink/MediLink_DataMgmt.py
+-rw-rw-rw-   0        0        0     7264 2024-05-08 01:45:53.000000 medicafe-0.240513.2/MediLink/MediLink_Down.py
+-rw-rw-rw-   0        0        0     8724 2024-05-01 03:44:46.000000 medicafe-0.240513.2/MediLink/MediLink_ERA_decoder.py
+-rw-rw-rw-   0        0        0     6236 2024-05-10 16:45:40.000000 medicafe-0.240513.2/MediLink/MediLink_Gmail.py
+-rw-rw-rw-   0        0        0     6040 2024-04-18 22:53:51.000000 medicafe-0.240513.2/MediLink/MediLink_Scheduler.py
+-rw-rw-rw-   0        0        0      222 2024-04-13 17:51:42.000000 medicafe-0.240513.2/MediLink/MediLink_StatusCheck.py
+-rw-rw-rw-   0        0        0     5181 2024-05-12 16:36:09.000000 medicafe-0.240513.2/MediLink/MediLink_UI.py
+-rw-rw-rw-   0        0        0    19252 2024-05-13 14:56:52.000000 medicafe-0.240513.2/MediLink/MediLink_Up.py
+-rwxrwxrwx   0        0        0      118 2024-04-19 22:20:37.000000 medicafe-0.240513.2/MediLink/MediLink_batch.bat
+-rw-rw-rw-   0        0        0      497 2024-03-15 19:39:51.000000 medicafe-0.240513.2/MediLink/Soumit_api.py
+-rw-rw-rw-   0        0        0        0 2024-04-19 02:51:01.000000 medicafe-0.240513.2/MediLink/__init__.py
+-rw-rw-rw-   0        0        0     3108 2024-05-13 04:52:22.000000 medicafe-0.240513.2/MediLink/test.py
+-rw-rw-rw-   0        0        0     4396 2024-05-13 14:57:53.278000 medicafe-0.240513.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2960 2024-05-13 07:31:39.000000 medicafe-0.240513.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 14:57:53.259000 medicafe-0.240513.2/medicafe.egg-info/
+-rw-rw-rw-   0        0        0     4396 2024-05-13 14:57:51.000000 medicafe-0.240513.2/medicafe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1023 2024-05-13 14:57:51.000000 medicafe-0.240513.2/medicafe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 14:57:51.000000 medicafe-0.240513.2/medicafe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-16 03:47:58.000000 medicafe-0.240513.2/medicafe.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       60 2024-05-13 14:57:51.000000 medicafe-0.240513.2/medicafe.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-13 14:57:51.000000 medicafe-0.240513.2/medicafe.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 14:57:53.291000 medicafe-0.240513.2/setup.cfg
+-rw-rw-rw-   0        0        0     4834 2024-05-13 14:57:50.000000 medicafe-0.240513.2/setup.py
```

### Comparing `medicafe-0.240513.1/LICENSE` & `medicafe-0.240513.2/LICENSE`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.1/MediBot/MediBot.bat` & `medicafe-0.240513.2/MediBot/MediBot.bat`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.1/MediBot/MediBot.py` & `medicafe-0.240513.2/MediBot/MediBot.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.1/MediBot/MediBot_Charges.py` & `medicafe-0.240513.2/MediBot/MediBot_Charges.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.1/MediBot/MediBot_Preprocessor.py` & `medicafe-0.240513.2/MediBot/MediBot_Preprocessor.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.1/MediBot/MediBot_Preprocessor_lib.py` & `medicafe-0.240513.2/MediBot/MediBot_Preprocessor_lib.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.1/MediBot/MediBot_UI.py` & `medicafe-0.240513.2/MediBot/MediBot_UI.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.1/MediBot/MediBot_dataformat_library.py` & `medicafe-0.240513.2/MediBot/MediBot_dataformat_library.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.1/MediBot/PDF_to_CSV_Cleaner.py` & `medicafe-0.240513.2/MediBot/PDF_to_CSV_Cleaner.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.1/MediBot/update_json.py` & `medicafe-0.240513.2/MediBot/update_json.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.1/MediBot/update_medicafe.py` & `medicafe-0.240513.2/MediBot/update_medicafe.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.1/MediLink/MediLink.py` & `medicafe-0.240513.2/MediLink/MediLink.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.1/MediLink/MediLink_277_decoder.py` & `medicafe-0.240513.2/MediLink/MediLink_277_decoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.1/MediLink/MediLink_837p_encoder.py` & `medicafe-0.240513.2/MediLink/MediLink_837p_encoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.1/MediLink/MediLink_837p_encoder_library.py` & `medicafe-0.240513.2/MediLink/MediLink_837p_encoder_library.py`

 * *Files 2% similar despite different names*

```diff
@@ -547,22 +547,25 @@
         "LM": "Liability Medical",
         "MA": "Medicare Part A",
         "MB": "Medicare Part B",
         "MC": "Medicaid",
         "OF": "Other Federal Program",
         "TV": "Title V",
         "VA": "Veterans Affairs Plan",
-        "WC": "Workers’ Compensation Health Claim",
+        "WC": "Workers Compensation Health Claim",
         "ZZ": "Mutually Defined"
     }
 
     # Function to display full list of insurance options
     def display_insurance_options(options):
         print("Insurance Type Options:")
-        for code, description in options.items():
+        # Sorting the dictionary keys to ensure consistent order
+        sorted_keys = sorted(options.keys())
+        for code in sorted_keys:
+            description = options[code]
             print("{} - {}".format(code, description))
 
     # Prompt to display full list
     display_full_list = input("Do you want to see the full list of insurance options? (yes/no): ").strip().lower()
 
     # Display full list if user confirms
     if display_full_list in ['yes', 'y']:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `medicafe-0.240513.1/MediLink/MediLink_ConfigLoader.py` & `medicafe-0.240513.2/MediLink/MediLink_ConfigLoader.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.1/MediLink/MediLink_DataMgmt.py` & `medicafe-0.240513.2/MediLink/MediLink_DataMgmt.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.1/MediLink/MediLink_Down.py` & `medicafe-0.240513.2/MediLink/MediLink_Down.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.1/MediLink/MediLink_ERA_decoder.py` & `medicafe-0.240513.2/MediLink/MediLink_ERA_decoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.1/MediLink/MediLink_Gmail.py` & `medicafe-0.240513.2/MediLink/MediLink_Gmail.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.1/MediLink/MediLink_Scheduler.py` & `medicafe-0.240513.2/MediLink/MediLink_Scheduler.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.1/MediLink/MediLink_UI.py` & `medicafe-0.240513.2/MediLink/MediLink_UI.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.1/MediLink/MediLink_Up.py` & `medicafe-0.240513.2/MediLink/MediLink_Up.py`

 * *Files 1% similar despite different names*

```diff
@@ -225,22 +225,24 @@
                 patient['success'] = success
             
             receipt_data[endpoint]["patients"].extend(patient_data)
     
     validate_data(receipt_data)
     return receipt_data
 
-def validate_data(patient_data):
+def validate_data(receipt_data):
     # Simple validation to check if data fields are correctly populated
-    for index, data in enumerate(patient_data, start=1):
-        missing_fields = [field for field in ('name', 'service_date', 'amount_billed', 'success') if not data.get(field)]
-        
-        if missing_fields:
-            # Log the missing fields without revealing PHI
-            log("Receipt Data validation error for patient {}: Missing information in fields: {}".format(index, ", ".join(missing_fields)))
+    for endpoint, data in receipt_data.items():
+        patients = data.get("patients", [])
+        for index, patient in enumerate(patients, start=1):
+            missing_fields = [field for field in ('name', 'service_date', 'amount_billed', 'success') if not patient.get(field)]
+            
+            if missing_fields:
+                # Log the missing fields without revealing PHI
+                log("Receipt Data validation error for endpoint '{}', patient {}: Missing information in fields: {}".format(endpoint, index, ", ".join(missing_fields)))
     return True
 
 def parse_837p_file(file_path):
     """
     Parse an 837p file to extract patient details and date of submission.
 
     This function reads the specified 837p file, extracts patient details such as name, service date, and amount billed,
@@ -302,27 +304,31 @@
         print("Error reading or parsing the 837p file: {0}".format(str(e)))
     
     # Optionally, return also date_of_submission as a separate variable  
     return patient_details, date_of_submission
 
 def build_receipt_content(receipt_data):
     # Build the receipt content in a human-readable ASCII format
-    # Format the receipt content to display endpoint-wise with associated patient information
-    # Use ASCII art or other formatting techniques to make the receipt visually appealing
+    # Improved layout with tabular data presentation for patient information
     receipt_lines = ["Submission Receipt", "="*60, ""]  # Header
     for endpoint, data in receipt_data.items():
         header = "Endpoint: {0} (Submitted: {1})".format(endpoint, data['date_of_submission'])
         receipt_lines.extend([header, "-"*len(header)])
         
-        # Adding patient information
+        # Table headers
+        table_header = "{:<20} | {:<15} | {:<15} | {:<10}".format("Patient", "Service Date", "Amount Billed", "Status")
+        receipt_lines.append(table_header)
+        receipt_lines.append("-"*len(table_header))
+        
+        # Adding patient information in a tabular format
         for patient in data["patients"]:
             success_status = "SUCCESS" if patient['success'] else "FAILED"
-            patient_info = "Patient: {0}, Service Date: {1}, Amount Billed: ${2}, Submission Status: {3}".format(patient['name'], patient['service_date'], patient['amount_billed'], success_status)
+            patient_info = "{:<20} | {:<15} | ${:<14} | {:<10}".format(patient['name'], patient['service_date'], patient['amount_billed'], success_status)
             receipt_lines.append(patient_info)
-            
+        
         receipt_lines.append("")  # Blank line for separation
     
     receipt_content = "\n".join(receipt_lines)
     return receipt_content
 
 def save_receipt_to_file(receipt_content, config):
     try:
```

### Comparing `medicafe-0.240513.1/MediLink/test.py` & `medicafe-0.240513.2/MediLink/test.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.1/PKG-INFO` & `medicafe-0.240513.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medicafe
-Version: 0.240513.1
+Version: 0.240513.2
 Summary: MediCafe
 Home-page: https://github.com/katanada2
 Author: Daniel Vidaud
 Author-email: daniel@personalizedtransformation.com
 License: MIT
 Keywords: medicafe python34 medibot medilink
 Description-Content-Type: text/markdown
```

### Comparing `medicafe-0.240513.1/README.md` & `medicafe-0.240513.2/README.md`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.1/medicafe.egg-info/PKG-INFO` & `medicafe-0.240513.2/medicafe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medicafe
-Version: 0.240513.1
+Version: 0.240513.2
 Summary: MediCafe
 Home-page: https://github.com/katanada2
 Author: Daniel Vidaud
 Author-email: daniel@personalizedtransformation.com
 License: MIT
 Keywords: medicafe python34 medibot medilink
 Description-Content-Type: text/markdown
```

### Comparing `medicafe-0.240513.1/medicafe.egg-info/SOURCES.txt` & `medicafe-0.240513.2/medicafe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `medicafe-0.240513.1/setup.py` & `medicafe-0.240513.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='medicafe',
-    version="0.240513.1",
+    version="0.240513.2",
     description='MediCafe',
     long_description="""
     # Project Overview: MediCafe
 
     ## Project Description
     MediCafe is a comprehensive suite designed to automate and streamline several aspects of medical administrative tasks within Medisoft, a popular medical practice management software. The system consists of two main components: MediBot and MediLink, each serving distinct functions but integrated to enhance the workflow of medical practices.
```

