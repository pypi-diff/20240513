# Comparing `tmp/GCS_bucket_files_or_filenames-0.4.tar.gz` & `tmp/GCS_bucket_files_or_filenames-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GCS_bucket_files_or_filenames-0.4.tar", last modified: Sun Mar 31 20:32:45 2024, max compression
+gzip compressed data, was "GCS_bucket_files_or_filenames-0.6.tar", last modified: Mon May 13 03:00:14 2024, max compression
```

## Comparing `GCS_bucket_files_or_filenames-0.4.tar` & `GCS_bucket_files_or_filenames-0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 preyaaatri   (501) staff       (20)        0 2024-03-31 20:32:45.353442 GCS_bucket_files_or_filenames-0.4/
-drwxr-xr-x   0 preyaaatri   (501) staff       (20)        0 2024-03-31 20:32:45.352457 GCS_bucket_files_or_filenames-0.4/GCS_bucket_files_or_filenames/
--rw-r--r--   0 preyaaatri   (501) staff       (20)       34 2024-03-28 02:25:21.000000 GCS_bucket_files_or_filenames-0.4/GCS_bucket_files_or_filenames/__init__.py
--rw-r--r--   0 preyaaatri   (501) staff       (20)     1746 2024-02-20 17:18:40.000000 GCS_bucket_files_or_filenames-0.4/GCS_bucket_files_or_filenames/main.py
-drwxr-xr-x   0 preyaaatri   (501) staff       (20)        0 2024-03-31 20:32:45.353162 GCS_bucket_files_or_filenames-0.4/GCS_bucket_files_or_filenames.egg-info/
--rw-r--r--   0 preyaaatri   (501) staff       (20)     2052 2024-03-31 20:32:45.000000 GCS_bucket_files_or_filenames-0.4/GCS_bucket_files_or_filenames.egg-info/PKG-INFO
--rw-r--r--   0 preyaaatri   (501) staff       (20)      366 2024-03-31 20:32:45.000000 GCS_bucket_files_or_filenames-0.4/GCS_bucket_files_or_filenames.egg-info/SOURCES.txt
--rw-r--r--   0 preyaaatri   (501) staff       (20)        1 2024-03-31 20:32:45.000000 GCS_bucket_files_or_filenames-0.4/GCS_bucket_files_or_filenames.egg-info/dependency_links.txt
--rw-r--r--   0 preyaaatri   (501) staff       (20)       96 2024-03-31 20:32:45.000000 GCS_bucket_files_or_filenames-0.4/GCS_bucket_files_or_filenames.egg-info/entry_points.txt
--rw-r--r--   0 preyaaatri   (501) staff       (20)       30 2024-03-31 20:32:45.000000 GCS_bucket_files_or_filenames-0.4/GCS_bucket_files_or_filenames.egg-info/top_level.txt
--rw-r--r--   0 preyaaatri   (501) staff       (20)     2052 2024-03-31 20:32:45.353320 GCS_bucket_files_or_filenames-0.4/PKG-INFO
--rw-r--r--   0 preyaaatri   (501) staff       (20)     1939 2024-02-20 20:18:04.000000 GCS_bucket_files_or_filenames-0.4/README.md
--rw-r--r--   0 preyaaatri   (501) staff       (20)       38 2024-03-31 20:32:45.353478 GCS_bucket_files_or_filenames-0.4/setup.cfg
--rw-r--r--   0 preyaaatri   (501) staff       (20)      465 2024-03-31 20:32:01.000000 GCS_bucket_files_or_filenames-0.4/setup.py
+drwxr-xr-x   0 preyaaatri   (501) staff       (20)        0 2024-05-13 03:00:14.349738 GCS_bucket_files_or_filenames-0.6/
+drwxr-xr-x   0 preyaaatri   (501) staff       (20)        0 2024-05-13 03:00:14.348790 GCS_bucket_files_or_filenames-0.6/GCS_bucket_files_or_filenames/
+-rw-r--r--   0 preyaaatri   (501) staff       (20)       34 2024-03-28 02:25:21.000000 GCS_bucket_files_or_filenames-0.6/GCS_bucket_files_or_filenames/__init__.py
+-rw-r--r--   0 preyaaatri   (501) staff       (20)     1746 2024-02-20 17:18:40.000000 GCS_bucket_files_or_filenames-0.6/GCS_bucket_files_or_filenames/main.py
+drwxr-xr-x   0 preyaaatri   (501) staff       (20)        0 2024-05-13 03:00:14.349470 GCS_bucket_files_or_filenames-0.6/GCS_bucket_files_or_filenames.egg-info/
+-rw-r--r--   0 preyaaatri   (501) staff       (20)     2052 2024-05-13 03:00:14.000000 GCS_bucket_files_or_filenames-0.6/GCS_bucket_files_or_filenames.egg-info/PKG-INFO
+-rw-r--r--   0 preyaaatri   (501) staff       (20)      366 2024-05-13 03:00:14.000000 GCS_bucket_files_or_filenames-0.6/GCS_bucket_files_or_filenames.egg-info/SOURCES.txt
+-rw-r--r--   0 preyaaatri   (501) staff       (20)        1 2024-05-13 03:00:14.000000 GCS_bucket_files_or_filenames-0.6/GCS_bucket_files_or_filenames.egg-info/dependency_links.txt
+-rw-r--r--   0 preyaaatri   (501) staff       (20)       96 2024-05-13 03:00:14.000000 GCS_bucket_files_or_filenames-0.6/GCS_bucket_files_or_filenames.egg-info/entry_points.txt
+-rw-r--r--   0 preyaaatri   (501) staff       (20)       30 2024-05-13 03:00:14.000000 GCS_bucket_files_or_filenames-0.6/GCS_bucket_files_or_filenames.egg-info/top_level.txt
+-rw-r--r--   0 preyaaatri   (501) staff       (20)     2052 2024-05-13 03:00:14.349625 GCS_bucket_files_or_filenames-0.6/PKG-INFO
+-rw-r--r--   0 preyaaatri   (501) staff       (20)     1939 2024-02-20 20:18:04.000000 GCS_bucket_files_or_filenames-0.6/README.md
+-rw-r--r--   0 preyaaatri   (501) staff       (20)       38 2024-05-13 03:00:14.349772 GCS_bucket_files_or_filenames-0.6/setup.cfg
+-rw-r--r--   0 preyaaatri   (501) staff       (20)      465 2024-05-13 02:59:54.000000 GCS_bucket_files_or_filenames-0.6/setup.py
```

### Comparing `GCS_bucket_files_or_filenames-0.4/GCS_bucket_files_or_filenames/main.py` & `GCS_bucket_files_or_filenames-0.6/GCS_bucket_files_or_filenames/main.py`

 * *Files identical despite different names*

### Comparing `GCS_bucket_files_or_filenames-0.4/GCS_bucket_files_or_filenames.egg-info/PKG-INFO` & `GCS_bucket_files_or_filenames-0.6/GCS_bucket_files_or_filenames.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GCS-bucket-files-or-filenames
-Version: 0.4
+Version: 0.6
 Description-Content-Type: text/markdown
 
 This document explains the usage of the Python function files_in_bucket, which can be used to list files within a specific folder in a Google Cloud Storage bucket.
 
 Parameters:
 
 1. bucket_name (str): The name of the Google Cloud Storage bucket.
```

### Comparing `GCS_bucket_files_or_filenames-0.4/PKG-INFO` & `GCS_bucket_files_or_filenames-0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GCS_bucket_files_or_filenames
-Version: 0.4
+Version: 0.6
 Description-Content-Type: text/markdown
 
 This document explains the usage of the Python function files_in_bucket, which can be used to list files within a specific folder in a Google Cloud Storage bucket.
 
 Parameters:
 
 1. bucket_name (str): The name of the Google Cloud Storage bucket.
```

### Comparing `GCS_bucket_files_or_filenames-0.4/README.md` & `GCS_bucket_files_or_filenames-0.6/README.md`

 * *Files identical despite different names*

