# Comparing `tmp/Compress_csv_files_gcs_bucket-0.0.tar.gz` & `tmp/Compress_csv_files_gcs_bucket-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Compress_csv_files_gcs_bucket-0.0.tar", last modified: Sat May 11 04:55:18 2024, max compression
+gzip compressed data, was "Compress_csv_files_gcs_bucket-0.1.tar", last modified: Sun May 12 22:52:53 2024, max compression
```

## Comparing `Compress_csv_files_gcs_bucket-0.0.tar` & `Compress_csv_files_gcs_bucket-0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 preyaaatri   (501) staff       (20)        0 2024-05-11 04:55:18.318551 Compress_csv_files_gcs_bucket-0.0/
-drwxr-xr-x   0 preyaaatri   (501) staff       (20)        0 2024-05-11 04:55:18.317459 Compress_csv_files_gcs_bucket-0.0/Compress_csv_files_gcs_bucket/
--rw-r--r--   0 preyaaatri   (501) staff       (20)       44 2024-05-11 04:25:36.000000 Compress_csv_files_gcs_bucket-0.0/Compress_csv_files_gcs_bucket/__init__.py
--rw-r--r--   0 preyaaatri   (501) staff       (20)     1506 2024-05-11 04:25:23.000000 Compress_csv_files_gcs_bucket-0.0/Compress_csv_files_gcs_bucket/main.py
-drwxr-xr-x   0 preyaaatri   (501) staff       (20)        0 2024-05-11 04:55:18.318229 Compress_csv_files_gcs_bucket-0.0/Compress_csv_files_gcs_bucket.egg-info/
--rw-r--r--   0 preyaaatri   (501) staff       (20)     3028 2024-05-11 04:55:18.000000 Compress_csv_files_gcs_bucket-0.0/Compress_csv_files_gcs_bucket.egg-info/PKG-INFO
--rw-r--r--   0 preyaaatri   (501) staff       (20)      366 2024-05-11 04:55:18.000000 Compress_csv_files_gcs_bucket-0.0/Compress_csv_files_gcs_bucket.egg-info/SOURCES.txt
--rw-r--r--   0 preyaaatri   (501) staff       (20)        1 2024-05-11 04:55:18.000000 Compress_csv_files_gcs_bucket-0.0/Compress_csv_files_gcs_bucket.egg-info/dependency_links.txt
--rw-r--r--   0 preyaaatri   (501) staff       (20)      106 2024-05-11 04:55:18.000000 Compress_csv_files_gcs_bucket-0.0/Compress_csv_files_gcs_bucket.egg-info/entry_points.txt
--rw-r--r--   0 preyaaatri   (501) staff       (20)       30 2024-05-11 04:55:18.000000 Compress_csv_files_gcs_bucket-0.0/Compress_csv_files_gcs_bucket.egg-info/top_level.txt
--rw-r--r--   0 preyaaatri   (501) staff       (20)     3028 2024-05-11 04:55:18.318418 Compress_csv_files_gcs_bucket-0.0/PKG-INFO
--rw-r--r--   0 preyaaatri   (501) staff       (20)     2916 2024-05-11 04:47:05.000000 Compress_csv_files_gcs_bucket-0.0/README.md
--rw-r--r--   0 preyaaatri   (501) staff       (20)       38 2024-05-11 04:55:18.318590 Compress_csv_files_gcs_bucket-0.0/setup.cfg
--rw-r--r--   0 preyaaatri   (501) staff       (20)      474 2024-05-11 04:54:35.000000 Compress_csv_files_gcs_bucket-0.0/setup.py
+drwxr-xr-x   0 preyaaatri   (501) staff       (20)        0 2024-05-12 22:52:53.316200 Compress_csv_files_gcs_bucket-0.1/
+drwxr-xr-x   0 preyaaatri   (501) staff       (20)        0 2024-05-12 22:52:53.315237 Compress_csv_files_gcs_bucket-0.1/Compress_csv_files_gcs_bucket/
+-rw-r--r--   0 preyaaatri   (501) staff       (20)       48 2024-05-12 22:52:33.000000 Compress_csv_files_gcs_bucket-0.1/Compress_csv_files_gcs_bucket/__init__.py
+-rw-r--r--   0 preyaaatri   (501) staff       (20)     1510 2024-05-12 22:52:28.000000 Compress_csv_files_gcs_bucket-0.1/Compress_csv_files_gcs_bucket/main.py
+drwxr-xr-x   0 preyaaatri   (501) staff       (20)        0 2024-05-12 22:52:53.315905 Compress_csv_files_gcs_bucket-0.1/Compress_csv_files_gcs_bucket.egg-info/
+-rw-r--r--   0 preyaaatri   (501) staff       (20)     3052 2024-05-12 22:52:53.000000 Compress_csv_files_gcs_bucket-0.1/Compress_csv_files_gcs_bucket.egg-info/PKG-INFO
+-rw-r--r--   0 preyaaatri   (501) staff       (20)      366 2024-05-12 22:52:53.000000 Compress_csv_files_gcs_bucket-0.1/Compress_csv_files_gcs_bucket.egg-info/SOURCES.txt
+-rw-r--r--   0 preyaaatri   (501) staff       (20)        1 2024-05-12 22:52:53.000000 Compress_csv_files_gcs_bucket-0.1/Compress_csv_files_gcs_bucket.egg-info/dependency_links.txt
+-rw-r--r--   0 preyaaatri   (501) staff       (20)      110 2024-05-12 22:52:53.000000 Compress_csv_files_gcs_bucket-0.1/Compress_csv_files_gcs_bucket.egg-info/entry_points.txt
+-rw-r--r--   0 preyaaatri   (501) staff       (20)       30 2024-05-12 22:52:53.000000 Compress_csv_files_gcs_bucket-0.1/Compress_csv_files_gcs_bucket.egg-info/top_level.txt
+-rw-r--r--   0 preyaaatri   (501) staff       (20)     3052 2024-05-12 22:52:53.316078 Compress_csv_files_gcs_bucket-0.1/PKG-INFO
+-rw-r--r--   0 preyaaatri   (501) staff       (20)     2940 2024-05-12 22:52:18.000000 Compress_csv_files_gcs_bucket-0.1/README.md
+-rw-r--r--   0 preyaaatri   (501) staff       (20)       38 2024-05-12 22:52:53.316239 Compress_csv_files_gcs_bucket-0.1/setup.cfg
+-rw-r--r--   0 preyaaatri   (501) staff       (20)      478 2024-05-12 22:52:24.000000 Compress_csv_files_gcs_bucket-0.1/setup.py
```

### Comparing `Compress_csv_files_gcs_bucket-0.0/Compress_csv_files_gcs_bucket/main.py` & `Compress_csv_files_gcs_bucket-0.1/Compress_csv_files_gcs_bucket/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import io
 import zipfile
 from google.cloud import storage
 
 
-def compress_gcs_bucket_files(bucket_name, prefix, output_zip_name, output_zip_prefix=None):
+def compress_csv_files_gcs_bucket(bucket_name, prefix, output_zip_name, output_zip_prefix=None):
     # Create a client to interact with Google Cloud Storage
     client = storage.Client()
 
     # Get the bucket containing the files
     bucket = client.get_bucket(bucket_name)
 
     # Create an in-memory buffer to store the zip file
```

### Comparing `Compress_csv_files_gcs_bucket-0.0/Compress_csv_files_gcs_bucket.egg-info/PKG-INFO` & `Compress_csv_files_gcs_bucket-0.1/Compress_csv_files_gcs_bucket.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 Metadata-Version: 2.1
 Name: Compress-csv-files-gcs-bucket
-Version: 0.0
+Version: 0.1
 Description-Content-Type: text/markdown
 
 Python Library for Compressing Files in Google Cloud Storage
 
-This library provides a function compress_gcs_bucket_files that simplifies the process of compressing multiple CSV files from a Google Cloud Storage (GCS) bucket into a single ZIP archive. The archive is then uploaded back to the same bucket.
+This library provides a function compress_csv_files_gcs_bucket that simplifies the process of compressing multiple CSV files from a Google Cloud Storage (GCS) bucket into a single ZIP archive. The archive is then uploaded back to the same bucket.
 
 
-**1. compress_gcs_bucket_files(bucket_name, prefix, output_zip_name, output_zip_prefix):**
+**1. compress_csv_files_gcs_bucket(bucket_name, prefix, output_zip_name, output_zip_prefix):**
 
-The compress_gcs_bucket_files function takes the following arguments:
+The compress_csv_files_gcs_bucket function takes the following arguments:
 
 *Parameters:*
 
 1. bucket_name: (str) The name of the GCS bucket containing the CSV files.
 2. prefix: (str) The prefix to filter files within the bucket (e.g., "path/to/your/csv/files/"). Include a trailing slash.
 3. output_zip_name: (str) The desired name for the output ZIP archive.
 4. output_zip_prefix (str, optional): An optional prefix to add to the filename within the output bucket. Defaults to saving the ZIP file in the same bucket as the source files.
 
 
 *Example Usage:*
 
 ```Python
 
-from compress_gcs_bucket_files import compress_gcs_bucket_files
+from Compress_csv_files_gcs_bucket import compress_csv_files_gcs_bucket
 
 # Replace with your information
 bucket_name = "your-bucket-name"
 prefix = "path/to/your/csv/files/"  # Include trailing slash
 output_zip_name = "compressed_data.zip"
 output_zip_prefix = "archived/data/"  # Optional, defaults to none
                                        # (saves in the same bucket)
 
-compress_gcs_bucket_files(bucket_name, prefix, output_zip_name, output_zip_prefix)
+compress_csv_files_gcs_bucket(bucket_name, prefix, output_zip_name, output_zip_prefix)
 
 ```
 
 
 *Function Behavior*
 1. Connects to GCS using storage.Client.
 2. Retrieves the bucket specified by bucket_name.
```

### Comparing `Compress_csv_files_gcs_bucket-0.0/PKG-INFO` & `Compress_csv_files_gcs_bucket-0.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,43 +1,38 @@
-Metadata-Version: 2.1
-Name: Compress_csv_files_gcs_bucket
-Version: 0.0
-Description-Content-Type: text/markdown
-
 Python Library for Compressing Files in Google Cloud Storage
 
-This library provides a function compress_gcs_bucket_files that simplifies the process of compressing multiple CSV files from a Google Cloud Storage (GCS) bucket into a single ZIP archive. The archive is then uploaded back to the same bucket.
+This library provides a function compress_csv_files_gcs_bucket that simplifies the process of compressing multiple CSV files from a Google Cloud Storage (GCS) bucket into a single ZIP archive. The archive is then uploaded back to the same bucket.
 
 
-**1. compress_gcs_bucket_files(bucket_name, prefix, output_zip_name, output_zip_prefix):**
+**1. compress_csv_files_gcs_bucket(bucket_name, prefix, output_zip_name, output_zip_prefix):**
 
-The compress_gcs_bucket_files function takes the following arguments:
+The compress_csv_files_gcs_bucket function takes the following arguments:
 
 *Parameters:*
 
 1. bucket_name: (str) The name of the GCS bucket containing the CSV files.
 2. prefix: (str) The prefix to filter files within the bucket (e.g., "path/to/your/csv/files/"). Include a trailing slash.
 3. output_zip_name: (str) The desired name for the output ZIP archive.
 4. output_zip_prefix (str, optional): An optional prefix to add to the filename within the output bucket. Defaults to saving the ZIP file in the same bucket as the source files.
 
 
 *Example Usage:*
 
 ```Python
 
-from compress_gcs_bucket_files import compress_gcs_bucket_files
+from Compress_csv_files_gcs_bucket import compress_csv_files_gcs_bucket
 
 # Replace with your information
 bucket_name = "your-bucket-name"
 prefix = "path/to/your/csv/files/"  # Include trailing slash
 output_zip_name = "compressed_data.zip"
 output_zip_prefix = "archived/data/"  # Optional, defaults to none
                                        # (saves in the same bucket)
 
-compress_gcs_bucket_files(bucket_name, prefix, output_zip_name, output_zip_prefix)
+compress_csv_files_gcs_bucket(bucket_name, prefix, output_zip_name, output_zip_prefix)
 
 ```
 
 
 *Function Behavior*
 1. Connects to GCS using storage.Client.
 2. Retrieves the bucket specified by bucket_name.
```

### Comparing `Compress_csv_files_gcs_bucket-0.0/README.md` & `Compress_csv_files_gcs_bucket-0.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,38 +1,43 @@
+Metadata-Version: 2.1
+Name: Compress_csv_files_gcs_bucket
+Version: 0.1
+Description-Content-Type: text/markdown
+
 Python Library for Compressing Files in Google Cloud Storage
 
-This library provides a function compress_gcs_bucket_files that simplifies the process of compressing multiple CSV files from a Google Cloud Storage (GCS) bucket into a single ZIP archive. The archive is then uploaded back to the same bucket.
+This library provides a function compress_csv_files_gcs_bucket that simplifies the process of compressing multiple CSV files from a Google Cloud Storage (GCS) bucket into a single ZIP archive. The archive is then uploaded back to the same bucket.
 
 
-**1. compress_gcs_bucket_files(bucket_name, prefix, output_zip_name, output_zip_prefix):**
+**1. compress_csv_files_gcs_bucket(bucket_name, prefix, output_zip_name, output_zip_prefix):**
 
-The compress_gcs_bucket_files function takes the following arguments:
+The compress_csv_files_gcs_bucket function takes the following arguments:
 
 *Parameters:*
 
 1. bucket_name: (str) The name of the GCS bucket containing the CSV files.
 2. prefix: (str) The prefix to filter files within the bucket (e.g., "path/to/your/csv/files/"). Include a trailing slash.
 3. output_zip_name: (str) The desired name for the output ZIP archive.
 4. output_zip_prefix (str, optional): An optional prefix to add to the filename within the output bucket. Defaults to saving the ZIP file in the same bucket as the source files.
 
 
 *Example Usage:*
 
 ```Python
 
-from compress_gcs_bucket_files import compress_gcs_bucket_files
+from Compress_csv_files_gcs_bucket import compress_csv_files_gcs_bucket
 
 # Replace with your information
 bucket_name = "your-bucket-name"
 prefix = "path/to/your/csv/files/"  # Include trailing slash
 output_zip_name = "compressed_data.zip"
 output_zip_prefix = "archived/data/"  # Optional, defaults to none
                                        # (saves in the same bucket)
 
-compress_gcs_bucket_files(bucket_name, prefix, output_zip_name, output_zip_prefix)
+compress_csv_files_gcs_bucket(bucket_name, prefix, output_zip_name, output_zip_prefix)
 
 ```
 
 
 *Function Behavior*
 1. Connects to GCS using storage.Client.
 2. Retrieves the bucket specified by bucket_name.
```

