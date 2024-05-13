# Comparing `tmp/grader_helper-0.1.7.tar.gz` & `tmp/grader_helper-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grader_helper-0.1.7.tar", max compression
+gzip compressed data, was "grader_helper-0.1.9.tar", max compression
```

## Comparing `grader_helper-0.1.7.tar` & `grader_helper-0.1.9.tar`

### file list

```diff
@@ -1,13 +1,15 @@
--rw-r--r--   0        0        0      122 2024-05-08 22:46:49.302642 grader_helper-0.1.7/grader_helper/.gitignore
--rw-r--r--   0        0        0      794 2024-05-06 22:37:50.633298 grader_helper-0.1.7/grader_helper/__init__.py
--rw-r--r--   0        0        0     1607 2024-05-06 19:47:00.017889 grader_helper-0.1.7/grader_helper/distribute_feedback_sheets.py
--rw-r--r--   0        0        0     2592 2024-05-06 19:47:00.030900 grader_helper-0.1.7/grader_helper/distribute_graders_groups.py
--rw-r--r--   0        0        0     1967 2024-05-06 19:46:59.931883 grader_helper-0.1.7/grader_helper/distribute_graders_individual.py
--rw-r--r--   0        0        0     1483 2024-05-06 19:47:00.070903 grader_helper-0.1.7/grader_helper/import_brightspace_classlist.py
--rw-r--r--   0        0        0      644 2024-05-06 20:26:06.293171 grader_helper-0.1.7/grader_helper/load_graders.py
--rw-r--r--   0        0        0     4817 2024-05-06 23:29:36.953441 grader_helper-0.1.7/grader_helper/rename_folders.py
--rw-r--r--   0        0        0     1617 2024-05-08 22:41:41.876957 grader_helper-0.1.7/grader_helper/save_distributed_graders.py
--rw-r--r--   0        0        0     2191 2024-05-08 22:42:13.520463 grader_helper-0.1.7/grader_helper/save_grader_sheets.py
--rw-r--r--   0        0        0      462 2024-05-08 22:47:32.584277 grader_helper-0.1.7/pyproject.toml
--rw-r--r--   0        0        0       18 2024-05-08 22:45:14.968398 grader_helper-0.1.7/README.md
--rw-r--r--   0        0        0      538 1970-01-01 00:00:00.000000 grader_helper-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0      122 2024-05-08 22:46:49.000000 grader_helper-0.1.9/grader_helper/.gitignore
+-rw-r--r--   0        0        0      937 2024-05-13 10:04:56.402355 grader_helper-0.1.9/grader_helper/__init__.py
+-rw-r--r--   0        0        0      224 2024-05-13 10:08:26.349982 grader_helper-0.1.9/grader_helper/ask_to_rename.py
+-rw-r--r--   0        0        0     1607 2024-05-06 19:47:00.000000 grader_helper-0.1.9/grader_helper/distribute_feedback_sheets.py
+-rw-r--r--   0        0        0     2592 2024-05-06 19:47:00.000000 grader_helper-0.1.9/grader_helper/distribute_graders_groups.py
+-rw-r--r--   0        0        0     1967 2024-05-06 19:46:59.000000 grader_helper-0.1.9/grader_helper/distribute_graders_individual.py
+-rw-r--r--   0        0        0     1483 2024-05-06 19:47:00.000000 grader_helper-0.1.9/grader_helper/import_brightspace_classlist.py
+-rw-r--r--   0        0        0      218 2024-05-13 10:05:33.693000 grader_helper-0.1.9/grader_helper/is_already_renamed.py
+-rw-r--r--   0        0        0      644 2024-05-06 20:26:06.000000 grader_helper-0.1.9/grader_helper/load_graders.py
+-rw-r--r--   0        0        0     4684 2024-05-13 10:06:10.923321 grader_helper-0.1.9/grader_helper/rename_folders.py
+-rw-r--r--   0        0        0     1617 2024-05-08 22:41:41.000000 grader_helper-0.1.9/grader_helper/save_distributed_graders.py
+-rw-r--r--   0        0        0     2191 2024-05-08 22:42:13.000000 grader_helper-0.1.9/grader_helper/save_grader_sheets.py
+-rw-r--r--   0        0        0      485 2024-05-13 10:48:11.960364 grader_helper-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      208 2024-05-10 13:44:07.291096 grader_helper-0.1.9/README.md
+-rw-r--r--   0        0        0      822 1970-01-01 00:00:00.000000 grader_helper-0.1.9/PKG-INFO
```

### Comparing `grader_helper-0.1.7/grader_helper/distribute_feedback_sheets.py` & `grader_helper-0.1.9/grader_helper/distribute_feedback_sheets.py`

 * *Files identical despite different names*

### Comparing `grader_helper-0.1.7/grader_helper/distribute_graders_groups.py` & `grader_helper-0.1.9/grader_helper/distribute_graders_groups.py`

 * *Files identical despite different names*

### Comparing `grader_helper-0.1.7/grader_helper/distribute_graders_individual.py` & `grader_helper-0.1.9/grader_helper/distribute_graders_individual.py`

 * *Files identical despite different names*

### Comparing `grader_helper-0.1.7/grader_helper/import_brightspace_classlist.py` & `grader_helper-0.1.9/grader_helper/import_brightspace_classlist.py`

 * *Files identical despite different names*

### Comparing `grader_helper-0.1.7/grader_helper/load_graders.py` & `grader_helper-0.1.9/grader_helper/load_graders.py`

 * *Files identical despite different names*

### Comparing `grader_helper-0.1.7/grader_helper/rename_folders.py` & `grader_helper-0.1.9/grader_helper/rename_folders.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 import pandas as pd
 import pathlib as pl
-
+import re
+from .ask_to_rename import ask_to_rename
+from .is_already_renamed import is_already_renamed
 
 def rename_folders(df, subs_folder):
     """
     Renames folders in subs_folder based on a DataFrame mapping of names to student IDs.
     
     Args:
         df (pd.DataFrame): DataFrame containing columns 'Last Name', 'First Name', and 'Student ID'.
-        subs_folder (Path): pathlib.Path object pointing to the directory containing the folders to be renamed.
+        subs_folder (pl.Path): pathlib.Path object pointing to the directory containing the folders to be renamed.
     """
     # Convert DataFrame to a dictionary for easier lookup
     name_id_map = {(row['Last Name'].upper(), row['First Name'].upper()): row['Student ID'] for _, row in df.iterrows()}
-    
-    def ask_to_rename(folder_name, suggested_name):
-        """Prompts user for rename confirmation."""
-        response = input(f"Rename '{folder_name}' to '{suggested_name}'? (y/n): ").strip().lower()
-        return response == 'y'
 
     rename_attempts = []  # Initialize a list to keep track of rename attempts
 
     for folder in subs_folder.iterdir():
-        if folder.is_dir():
+        if folder.is_dir() and not is_already_renamed(folder.name.upper()):
             folder_name_upper = folder.name.upper()
             matched = False
             
             for (last_name, first_name), student_id in name_id_map.items():
                 if last_name in folder_name_upper and first_name in folder_name_upper:
                     new_folder_name = f"{last_name}, {first_name} ({student_id})"
                     try:
@@ -72,12 +69,11 @@
 
             if not matched:
                 rename_attempts.append({'Original Name': folder.name, 'Suggested Name': 'N/A', 'Outcome': 'No Match Found'})
 
     # Log rename attempts
     rename_log_df = pd.DataFrame(rename_attempts)
     log_path = subs_folder / "folder_rename_log.csv"
-    if log_path.exists():
-        renames = pd.read_csv(log_path)
-        rename_log_df = pd.concat([renames, rename_log_df], ignore_index=True)
-    rename_log_df.to_csv(log_path, index=False)
+    
+    # Append to log file if it exists or create a new one
+    rename_log_df.to_csv(log_path, mode='a', header=not log_path.exists(), index=False)
     print("Folder rename operations logged to folder_rename_log.csv.")
```

### Comparing `grader_helper-0.1.7/grader_helper/save_distributed_graders.py` & `grader_helper-0.1.9/grader_helper/save_distributed_graders.py`

 * *Files identical despite different names*

### Comparing `grader_helper-0.1.7/grader_helper/save_grader_sheets.py` & `grader_helper-0.1.9/grader_helper/save_grader_sheets.py`

 * *Files identical despite different names*

### Comparing `grader_helper-0.1.7/PKG-INFO` & `grader_helper-0.1.9/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 Metadata-Version: 2.1
 Name: grader-helper
-Version: 0.1.7
+Version: 0.1.9
 Summary: Functions to help manage assignments from UL which are hosted on Brightspace
 License: MIT
 Author: Kevin O Malley
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: ipykernel (>=6.29.4,<7.0.0)
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
 Requires-Dist: pandas (>=2.2.2,<3.0.0)
 Requires-Dist: pathlib (>=1.0.1,<2.0.0)
 Description-Content-Type: text/markdown
 
 # grader_helper
  
+Need to make the renaming folders function skip folders that have already been renamed so that I can run the function multiple times without renaming the same folders over and over again. 
+
```

