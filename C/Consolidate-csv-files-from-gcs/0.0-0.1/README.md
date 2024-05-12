# Comparing `tmp/Consolidate_csv_files_from_gcs-0.0.tar.gz` & `tmp/Consolidate_csv_files_from_gcs-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Consolidate_csv_files_from_gcs-0.0.tar", last modified: Sat May 11 03:06:45 2024, max compression
+gzip compressed data, was "Consolidate_csv_files_from_gcs-0.1.tar", last modified: Sun May 12 22:39:48 2024, max compression
```

## Comparing `Consolidate_csv_files_from_gcs-0.0.tar` & `Consolidate_csv_files_from_gcs-0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 preyaaatri   (501) staff       (20)        0 2024-05-11 03:06:45.868634 Consolidate_csv_files_from_gcs-0.0/
-drwxr-xr-x   0 preyaaatri   (501) staff       (20)        0 2024-05-11 03:06:45.867616 Consolidate_csv_files_from_gcs-0.0/Consolidate_csv_files_from_gcs/
--rw-r--r--   0 preyaaatri   (501) staff       (20)       43 2024-05-10 21:18:29.000000 Consolidate_csv_files_from_gcs-0.0/Consolidate_csv_files_from_gcs/__init__.py
--rw-r--r--   0 preyaaatri   (501) staff       (20)     2218 2024-05-10 21:14:19.000000 Consolidate_csv_files_from_gcs-0.0/Consolidate_csv_files_from_gcs/main.py
-drwxr-xr-x   0 preyaaatri   (501) staff       (20)        0 2024-05-11 03:06:45.868356 Consolidate_csv_files_from_gcs-0.0/Consolidate_csv_files_from_gcs.egg-info/
--rw-r--r--   0 preyaaatri   (501) staff       (20)     2887 2024-05-11 03:06:45.000000 Consolidate_csv_files_from_gcs-0.0/Consolidate_csv_files_from_gcs.egg-info/PKG-INFO
--rw-r--r--   0 preyaaatri   (501) staff       (20)      373 2024-05-11 03:06:45.000000 Consolidate_csv_files_from_gcs-0.0/Consolidate_csv_files_from_gcs.egg-info/SOURCES.txt
--rw-r--r--   0 preyaaatri   (501) staff       (20)        1 2024-05-11 03:06:45.000000 Consolidate_csv_files_from_gcs-0.0/Consolidate_csv_files_from_gcs.egg-info/dependency_links.txt
--rw-r--r--   0 preyaaatri   (501) staff       (20)      107 2024-05-11 03:06:45.000000 Consolidate_csv_files_from_gcs-0.0/Consolidate_csv_files_from_gcs.egg-info/entry_points.txt
--rw-r--r--   0 preyaaatri   (501) staff       (20)       31 2024-05-11 03:06:45.000000 Consolidate_csv_files_from_gcs-0.0/Consolidate_csv_files_from_gcs.egg-info/top_level.txt
--rw-r--r--   0 preyaaatri   (501) staff       (20)     2887 2024-05-11 03:06:45.868517 Consolidate_csv_files_from_gcs-0.0/PKG-INFO
--rw-r--r--   0 preyaaatri   (501) staff       (20)     2774 2024-05-10 21:14:04.000000 Consolidate_csv_files_from_gcs-0.0/README.md
--rw-r--r--   0 preyaaatri   (501) staff       (20)       38 2024-05-11 03:06:45.868668 Consolidate_csv_files_from_gcs-0.0/setup.cfg
--rw-r--r--   0 preyaaatri   (501) staff       (20)      476 2024-05-10 22:18:04.000000 Consolidate_csv_files_from_gcs-0.0/setup.py
+drwxr-xr-x   0 preyaaatri   (501) staff       (20)        0 2024-05-12 22:39:48.556427 Consolidate_csv_files_from_gcs-0.1/
+drwxr-xr-x   0 preyaaatri   (501) staff       (20)        0 2024-05-12 22:39:48.555369 Consolidate_csv_files_from_gcs-0.1/Consolidate_csv_files_from_gcs/
+-rw-r--r--   0 preyaaatri   (501) staff       (20)       43 2024-05-10 21:18:29.000000 Consolidate_csv_files_from_gcs-0.1/Consolidate_csv_files_from_gcs/__init__.py
+-rw-r--r--   0 preyaaatri   (501) staff       (20)     2218 2024-05-10 21:14:19.000000 Consolidate_csv_files_from_gcs-0.1/Consolidate_csv_files_from_gcs/main.py
+drwxr-xr-x   0 preyaaatri   (501) staff       (20)        0 2024-05-12 22:39:48.556148 Consolidate_csv_files_from_gcs-0.1/Consolidate_csv_files_from_gcs.egg-info/
+-rw-r--r--   0 preyaaatri   (501) staff       (20)     3194 2024-05-12 22:39:48.000000 Consolidate_csv_files_from_gcs-0.1/Consolidate_csv_files_from_gcs.egg-info/PKG-INFO
+-rw-r--r--   0 preyaaatri   (501) staff       (20)      373 2024-05-12 22:39:48.000000 Consolidate_csv_files_from_gcs-0.1/Consolidate_csv_files_from_gcs.egg-info/SOURCES.txt
+-rw-r--r--   0 preyaaatri   (501) staff       (20)        1 2024-05-12 22:39:48.000000 Consolidate_csv_files_from_gcs-0.1/Consolidate_csv_files_from_gcs.egg-info/dependency_links.txt
+-rw-r--r--   0 preyaaatri   (501) staff       (20)      107 2024-05-12 22:39:48.000000 Consolidate_csv_files_from_gcs-0.1/Consolidate_csv_files_from_gcs.egg-info/entry_points.txt
+-rw-r--r--   0 preyaaatri   (501) staff       (20)       31 2024-05-12 22:39:48.000000 Consolidate_csv_files_from_gcs-0.1/Consolidate_csv_files_from_gcs.egg-info/top_level.txt
+-rw-r--r--   0 preyaaatri   (501) staff       (20)     3194 2024-05-12 22:39:48.556309 Consolidate_csv_files_from_gcs-0.1/PKG-INFO
+-rw-r--r--   0 preyaaatri   (501) staff       (20)     3081 2024-05-12 22:39:08.000000 Consolidate_csv_files_from_gcs-0.1/README.md
+-rw-r--r--   0 preyaaatri   (501) staff       (20)       38 2024-05-12 22:39:48.556463 Consolidate_csv_files_from_gcs-0.1/setup.cfg
+-rw-r--r--   0 preyaaatri   (501) staff       (20)      476 2024-05-12 22:39:29.000000 Consolidate_csv_files_from_gcs-0.1/setup.py
```

### Comparing `Consolidate_csv_files_from_gcs-0.0/Consolidate_csv_files_from_gcs/main.py` & `Consolidate_csv_files_from_gcs-0.1/Consolidate_csv_files_from_gcs/main.py`

 * *Files identical despite different names*

### Comparing `Consolidate_csv_files_from_gcs-0.0/Consolidate_csv_files_from_gcs.egg-info/PKG-INFO` & `Consolidate_csv_files_from_gcs-0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: Consolidate-csv-files-from-gcs
-Version: 0.0
+Name: Consolidate_csv_files_from_gcs
+Version: 0.1
 Description-Content-Type: text/markdown
 
 Python Library for Merging CSV Files from Google Cloud Storage
 
 This library provides a function consolidate_csv_from_gcs that simplifies the process of merging multiple CSV files from a Google Cloud Storage (GCS) bucket into a single file.
 
 **1. consolidate_csv_from_gcs(bucket_name, prefix, merged_file_name, output_bucket_name, output_bucket_name_prefix):**
@@ -20,14 +20,29 @@
 5. output_bucket_name_prefix = "merged/data/"  # Optional, defaults to prefix
 
 
 Return Value:
 
 There is no return value as the result can be seen in the GCS bucket.
 
+**Usage:**
+
+```Python
+
+from Consolidate_csv_files_from_gcs import consolidate_csv_from_gcs
+
+consolidate_csv_from_gcs(
+    bucket_name='source-bucket',
+    prefix='data/',
+    merged_file_name='consolidated.csv',
+    output_bucket_name='destination-bucket',
+    output_bucket_name_prefix='processed/'
+)
+
+```
 
 *Explanation:*
 
 The consolidate_csv_from_gcs function takes the following arguments:
 1. bucket_name: (str) The name of the GCS bucket containing the CSV files.
 2. prefix: (str) The prefix to filter files within the bucket (e.g., "path/to/your/csv/files/"). Include a trailing slash.
 3. merged_file_name: (str) The desired name for the output merged CSV file.
```

### Comparing `Consolidate_csv_files_from_gcs-0.0/PKG-INFO` & `Consolidate_csv_files_from_gcs-0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,7 @@
-Metadata-Version: 2.1
-Name: Consolidate_csv_files_from_gcs
-Version: 0.0
-Description-Content-Type: text/markdown
-
 Python Library for Merging CSV Files from Google Cloud Storage
 
 This library provides a function consolidate_csv_from_gcs that simplifies the process of merging multiple CSV files from a Google Cloud Storage (GCS) bucket into a single file.
 
 **1. consolidate_csv_from_gcs(bucket_name, prefix, merged_file_name, output_bucket_name, output_bucket_name_prefix):**
 
 The consolidate_csv_from_gcs function takes the following arguments:
@@ -20,14 +15,29 @@
 5. output_bucket_name_prefix = "merged/data/"  # Optional, defaults to prefix
 
 
 Return Value:
 
 There is no return value as the result can be seen in the GCS bucket.
 
+**Usage:**
+
+```Python
+
+from Consolidate_csv_files_from_gcs import consolidate_csv_from_gcs
+
+consolidate_csv_from_gcs(
+    bucket_name='source-bucket',
+    prefix='data/',
+    merged_file_name='consolidated.csv',
+    output_bucket_name='destination-bucket',
+    output_bucket_name_prefix='processed/'
+)
+
+```
 
 *Explanation:*
 
 The consolidate_csv_from_gcs function takes the following arguments:
 1. bucket_name: (str) The name of the GCS bucket containing the CSV files.
 2. prefix: (str) The prefix to filter files within the bucket (e.g., "path/to/your/csv/files/"). Include a trailing slash.
 3. merged_file_name: (str) The desired name for the output merged CSV file.
```

### Comparing `Consolidate_csv_files_from_gcs-0.0/README.md` & `Consolidate_csv_files_from_gcs-0.1/Consolidate_csv_files_from_gcs.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+Metadata-Version: 2.1
+Name: Consolidate-csv-files-from-gcs
+Version: 0.1
+Description-Content-Type: text/markdown
+
 Python Library for Merging CSV Files from Google Cloud Storage
 
 This library provides a function consolidate_csv_from_gcs that simplifies the process of merging multiple CSV files from a Google Cloud Storage (GCS) bucket into a single file.
 
 **1. consolidate_csv_from_gcs(bucket_name, prefix, merged_file_name, output_bucket_name, output_bucket_name_prefix):**
 
 The consolidate_csv_from_gcs function takes the following arguments:
@@ -15,14 +20,29 @@
 5. output_bucket_name_prefix = "merged/data/"  # Optional, defaults to prefix
 
 
 Return Value:
 
 There is no return value as the result can be seen in the GCS bucket.
 
+**Usage:**
+
+```Python
+
+from Consolidate_csv_files_from_gcs import consolidate_csv_from_gcs
+
+consolidate_csv_from_gcs(
+    bucket_name='source-bucket',
+    prefix='data/',
+    merged_file_name='consolidated.csv',
+    output_bucket_name='destination-bucket',
+    output_bucket_name_prefix='processed/'
+)
+
+```
 
 *Explanation:*
 
 The consolidate_csv_from_gcs function takes the following arguments:
 1. bucket_name: (str) The name of the GCS bucket containing the CSV files.
 2. prefix: (str) The prefix to filter files within the bucket (e.g., "path/to/your/csv/files/"). Include a trailing slash.
 3. merged_file_name: (str) The desired name for the output merged CSV file.
```

