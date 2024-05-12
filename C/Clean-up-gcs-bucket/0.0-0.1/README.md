# Comparing `tmp/Clean_up_gcs_bucket-0.0.tar.gz` & `tmp/Clean_up_gcs_bucket-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Clean_up_gcs_bucket-0.0.tar", last modified: Sat May 11 05:15:01 2024, max compression
+gzip compressed data, was "Clean_up_gcs_bucket-0.1.tar", last modified: Sun May 12 22:44:59 2024, max compression
```

## Comparing `Clean_up_gcs_bucket-0.0.tar` & `Clean_up_gcs_bucket-0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 preyaaatri   (501) staff       (20)        0 2024-05-11 05:15:01.344389 Clean_up_gcs_bucket-0.0/
-drwxr-xr-x   0 preyaaatri   (501) staff       (20)        0 2024-05-11 05:15:01.343455 Clean_up_gcs_bucket-0.0/Clean_up_gcs_bucket/
--rw-r--r--   0 preyaaatri   (501) staff       (20)       47 2024-05-11 05:13:57.000000 Clean_up_gcs_bucket-0.0/Clean_up_gcs_bucket/__init__.py
--rw-r--r--   0 preyaaatri   (501) staff       (20)      730 2024-05-11 05:13:53.000000 Clean_up_gcs_bucket-0.0/Clean_up_gcs_bucket/main.py
-drwxr-xr-x   0 preyaaatri   (501) staff       (20)        0 2024-05-11 05:15:01.344111 Clean_up_gcs_bucket-0.0/Clean_up_gcs_bucket.egg-info/
--rw-r--r--   0 preyaaatri   (501) staff       (20)     2438 2024-05-11 05:15:01.000000 Clean_up_gcs_bucket-0.0/Clean_up_gcs_bucket.egg-info/PKG-INFO
--rw-r--r--   0 preyaaatri   (501) staff       (20)      296 2024-05-11 05:15:01.000000 Clean_up_gcs_bucket-0.0/Clean_up_gcs_bucket.egg-info/SOURCES.txt
--rw-r--r--   0 preyaaatri   (501) staff       (20)        1 2024-05-11 05:15:01.000000 Clean_up_gcs_bucket-0.0/Clean_up_gcs_bucket.egg-info/dependency_links.txt
--rw-r--r--   0 preyaaatri   (501) staff       (20)       88 2024-05-11 05:15:01.000000 Clean_up_gcs_bucket-0.0/Clean_up_gcs_bucket.egg-info/entry_points.txt
--rw-r--r--   0 preyaaatri   (501) staff       (20)       20 2024-05-11 05:15:01.000000 Clean_up_gcs_bucket-0.0/Clean_up_gcs_bucket.egg-info/top_level.txt
--rw-r--r--   0 preyaaatri   (501) staff       (20)     2438 2024-05-11 05:15:01.344270 Clean_up_gcs_bucket-0.0/PKG-INFO
--rw-r--r--   0 preyaaatri   (501) staff       (20)     2336 2024-05-11 05:13:43.000000 Clean_up_gcs_bucket-0.0/README.md
--rw-r--r--   0 preyaaatri   (501) staff       (20)       38 2024-05-11 05:15:01.344423 Clean_up_gcs_bucket-0.0/setup.cfg
--rw-r--r--   0 preyaaatri   (501) staff       (20)      446 2024-05-11 05:13:48.000000 Clean_up_gcs_bucket-0.0/setup.py
+drwxr-xr-x   0 preyaaatri   (501) staff       (20)        0 2024-05-12 22:44:59.899204 Clean_up_gcs_bucket-0.1/
+drwxr-xr-x   0 preyaaatri   (501) staff       (20)        0 2024-05-12 22:44:59.898250 Clean_up_gcs_bucket-0.1/Clean_up_gcs_bucket/
+-rw-r--r--   0 preyaaatri   (501) staff       (20)       39 2024-05-12 22:44:13.000000 Clean_up_gcs_bucket-0.1/Clean_up_gcs_bucket/__init__.py
+-rw-r--r--   0 preyaaatri   (501) staff       (20)      722 2024-05-12 22:44:10.000000 Clean_up_gcs_bucket-0.1/Clean_up_gcs_bucket/main.py
+drwxr-xr-x   0 preyaaatri   (501) staff       (20)        0 2024-05-12 22:44:59.898921 Clean_up_gcs_bucket-0.1/Clean_up_gcs_bucket.egg-info/
+-rw-r--r--   0 preyaaatri   (501) staff       (20)     2438 2024-05-12 22:44:59.000000 Clean_up_gcs_bucket-0.1/Clean_up_gcs_bucket.egg-info/PKG-INFO
+-rw-r--r--   0 preyaaatri   (501) staff       (20)      296 2024-05-12 22:44:59.000000 Clean_up_gcs_bucket-0.1/Clean_up_gcs_bucket.egg-info/SOURCES.txt
+-rw-r--r--   0 preyaaatri   (501) staff       (20)        1 2024-05-12 22:44:59.000000 Clean_up_gcs_bucket-0.1/Clean_up_gcs_bucket.egg-info/dependency_links.txt
+-rw-r--r--   0 preyaaatri   (501) staff       (20)       88 2024-05-12 22:44:59.000000 Clean_up_gcs_bucket-0.1/Clean_up_gcs_bucket.egg-info/entry_points.txt
+-rw-r--r--   0 preyaaatri   (501) staff       (20)       20 2024-05-12 22:44:59.000000 Clean_up_gcs_bucket-0.1/Clean_up_gcs_bucket.egg-info/top_level.txt
+-rw-r--r--   0 preyaaatri   (501) staff       (20)     2438 2024-05-12 22:44:59.899088 Clean_up_gcs_bucket-0.1/PKG-INFO
+-rw-r--r--   0 preyaaatri   (501) staff       (20)     2336 2024-05-11 05:13:43.000000 Clean_up_gcs_bucket-0.1/README.md
+-rw-r--r--   0 preyaaatri   (501) staff       (20)       38 2024-05-12 22:44:59.899239 Clean_up_gcs_bucket-0.1/setup.cfg
+-rw-r--r--   0 preyaaatri   (501) staff       (20)      446 2024-05-12 22:44:27.000000 Clean_up_gcs_bucket-0.1/setup.py
```

### Comparing `Clean_up_gcs_bucket-0.0/Clean_up_gcs_bucket/main.py` & `Clean_up_gcs_bucket-0.1/Clean_up_gcs_bucket/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from google.cloud import storage
 
-def remove_all_files_gcs_bucket(bucket_name, folder_path='', substring=''):
+def clean_up_gcs_bucket(bucket_name, folder_path='', substring=''):
     # Create a client to interact with Google Cloud Storage
     client = storage.Client()
 
     # Get the bucket
     bucket = client.get_bucket(bucket_name)
 
     # List all blobs in the bucket
```

### Comparing `Clean_up_gcs_bucket-0.0/Clean_up_gcs_bucket.egg-info/PKG-INFO` & `Clean_up_gcs_bucket-0.1/Clean_up_gcs_bucket.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Clean-up-gcs-bucket
-Version: 0.0
+Version: 0.1
 Description-Content-Type: text/markdown
 
 Python Library for Deleting Objects in Google Cloud Storage Buckets
 
 This library provides a function clean_up_gcs_bucket that helps you delete unwanted objects from a Google Cloud Storage (GCS) bucket based on a folder path and substring criteria.
```

### Comparing `Clean_up_gcs_bucket-0.0/PKG-INFO` & `Clean_up_gcs_bucket-0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Clean_up_gcs_bucket
-Version: 0.0
+Version: 0.1
 Description-Content-Type: text/markdown
 
 Python Library for Deleting Objects in Google Cloud Storage Buckets
 
 This library provides a function clean_up_gcs_bucket that helps you delete unwanted objects from a Google Cloud Storage (GCS) bucket based on a folder path and substring criteria.
```

### Comparing `Clean_up_gcs_bucket-0.0/README.md` & `Clean_up_gcs_bucket-0.1/README.md`

 * *Files identical despite different names*

