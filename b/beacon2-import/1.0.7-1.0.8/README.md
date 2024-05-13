# Comparing `tmp/beacon2-import-1.0.7.tar.gz` & `tmp/beacon2-import-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/beacon2-import-1.0.7.tar", last modified: Wed May  1 11:38:58 2024, max compression
+gzip compressed data, was "dist/beacon2-import-1.0.8.tar", last modified: Mon May 13 13:26:14 2024, max compression
```

## Comparing `beacon2-import-1.0.7.tar` & `beacon2-import-1.0.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 khaled    (1000) khaled    (1000)        0 2024-05-01 11:38:58.000000 beacon2-import-1.0.7/
-drwxrwxr-x   0 khaled    (1000) khaled    (1000)        0 2024-05-01 11:38:58.000000 beacon2-import-1.0.7/beacon2_import.egg-info/
--rw-rw-r--   0 khaled    (1000) khaled    (1000)       36 2024-05-01 11:38:58.000000 beacon2-import-1.0.7/beacon2_import.egg-info/top_level.txt
--rw-rw-r--   0 khaled    (1000) khaled    (1000)      425 2024-05-01 11:38:58.000000 beacon2-import-1.0.7/beacon2_import.egg-info/SOURCES.txt
--rw-r--r--   0 khaled    (1000) khaled    (1000)      258 2024-05-01 11:38:58.000000 beacon2-import-1.0.7/beacon2_import.egg-info/PKG-INFO
--rw-rw-r--   0 khaled    (1000) khaled    (1000)       61 2024-05-01 11:38:58.000000 beacon2-import-1.0.7/beacon2_import.egg-info/dependency_links.txt
--rw-rw-r--   0 khaled    (1000) khaled    (1000)       47 2024-05-01 11:38:58.000000 beacon2-import-1.0.7/beacon2_import.egg-info/requires.txt
--rw-rw-r--   0 khaled    (1000) khaled    (1000)      141 2024-05-01 11:38:58.000000 beacon2-import-1.0.7/beacon2_import.egg-info/entry_points.txt
--rw-rw-r--   0 khaled    (1000) khaled    (1000)      258 2024-05-01 11:38:58.000000 beacon2-import-1.0.7/PKG-INFO
--rw-rw-r--   0 khaled    (1000) khaled    (1000)     5439 2024-04-08 12:17:34.000000 beacon2-import-1.0.7/utils.py
-drwxrwxr-x   0 khaled    (1000) khaled    (1000)        0 2024-05-01 11:38:58.000000 beacon2-import-1.0.7/beacon2_import/
--rw-rw-r--   0 khaled    (1000) khaled    (1000)     5439 2024-04-08 11:27:46.000000 beacon2-import-1.0.7/beacon2_import/utils.py
--rw-rw-r--   0 khaled    (1000) khaled    (1000)    16574 2024-05-01 11:30:19.000000 beacon2-import-1.0.7/beacon2_import/beacon2_import.py
--rw-rw-r--   0 khaled    (1000) khaled    (1000)        0 2024-04-08 11:28:20.000000 beacon2-import-1.0.7/beacon2_import/__init__.py
--rw-rw-r--   0 khaled    (1000) khaled    (1000)       38 2024-05-01 11:38:58.000000 beacon2-import-1.0.7/setup.cfg
--rw-rw-r--   0 khaled    (1000) khaled    (1000)      234 2024-04-08 12:42:00.000000 beacon2-import-1.0.7/README.md
--rw-rw-r--   0 khaled    (1000) khaled    (1000)      807 2024-05-01 11:36:53.000000 beacon2-import-1.0.7/setup.py
-drwxrwxr-x   0 khaled    (1000) khaled    (1000)        0 2024-05-01 11:38:58.000000 beacon2-import-1.0.7/beacon2_search/
--rw-rw-r--   0 khaled    (1000) khaled    (1000)     5439 2024-04-08 11:27:52.000000 beacon2-import-1.0.7/beacon2_search/utils.py
--rw-rw-r--   0 khaled    (1000) khaled    (1000)    13150 2024-04-08 11:19:47.000000 beacon2-import-1.0.7/beacon2_search/beacon2_search.py
--rw-rw-r--   0 khaled    (1000) khaled    (1000)        0 2024-04-08 11:28:15.000000 beacon2-import-1.0.7/beacon2_search/__init__.py
+drwxrwxr-x   0 khaled    (1000) khaled    (1000)        0 2024-05-13 13:26:14.000000 beacon2-import-1.0.8/
+drwxrwxr-x   0 khaled    (1000) khaled    (1000)        0 2024-05-13 13:26:14.000000 beacon2-import-1.0.8/beacon2_import.egg-info/
+-rw-rw-r--   0 khaled    (1000) khaled    (1000)       36 2024-05-13 13:26:14.000000 beacon2-import-1.0.8/beacon2_import.egg-info/top_level.txt
+-rw-rw-r--   0 khaled    (1000) khaled    (1000)      425 2024-05-13 13:26:14.000000 beacon2-import-1.0.8/beacon2_import.egg-info/SOURCES.txt
+-rw-r--r--   0 khaled    (1000) khaled    (1000)      258 2024-05-13 13:26:14.000000 beacon2-import-1.0.8/beacon2_import.egg-info/PKG-INFO
+-rw-rw-r--   0 khaled    (1000) khaled    (1000)       61 2024-05-13 13:26:14.000000 beacon2-import-1.0.8/beacon2_import.egg-info/dependency_links.txt
+-rw-rw-r--   0 khaled    (1000) khaled    (1000)       47 2024-05-13 13:26:14.000000 beacon2-import-1.0.8/beacon2_import.egg-info/requires.txt
+-rw-rw-r--   0 khaled    (1000) khaled    (1000)      141 2024-05-13 13:26:14.000000 beacon2-import-1.0.8/beacon2_import.egg-info/entry_points.txt
+-rw-rw-r--   0 khaled    (1000) khaled    (1000)      258 2024-05-13 13:26:14.000000 beacon2-import-1.0.8/PKG-INFO
+-rw-rw-r--   0 khaled    (1000) khaled    (1000)     5439 2024-04-08 12:17:34.000000 beacon2-import-1.0.8/utils.py
+drwxrwxr-x   0 khaled    (1000) khaled    (1000)        0 2024-05-13 13:26:14.000000 beacon2-import-1.0.8/beacon2_import/
+-rw-rw-r--   0 khaled    (1000) khaled    (1000)     5439 2024-04-08 11:27:46.000000 beacon2-import-1.0.8/beacon2_import/utils.py
+-rw-rw-r--   0 khaled    (1000) khaled    (1000)    16574 2024-05-01 11:30:19.000000 beacon2-import-1.0.8/beacon2_import/beacon2_import.py
+-rw-rw-r--   0 khaled    (1000) khaled    (1000)        0 2024-04-08 11:28:20.000000 beacon2-import-1.0.8/beacon2_import/__init__.py
+-rw-rw-r--   0 khaled    (1000) khaled    (1000)       38 2024-05-13 13:26:14.000000 beacon2-import-1.0.8/setup.cfg
+-rw-rw-r--   0 khaled    (1000) khaled    (1000)      234 2024-04-08 12:42:00.000000 beacon2-import-1.0.8/README.md
+-rw-rw-r--   0 khaled    (1000) khaled    (1000)      807 2024-05-13 13:23:54.000000 beacon2-import-1.0.8/setup.py
+drwxrwxr-x   0 khaled    (1000) khaled    (1000)        0 2024-05-13 13:26:14.000000 beacon2-import-1.0.8/beacon2_search/
+-rw-rw-r--   0 khaled    (1000) khaled    (1000)     5439 2024-04-08 11:27:52.000000 beacon2-import-1.0.8/beacon2_search/utils.py
+-rw-rw-r--   0 khaled    (1000) khaled    (1000)    13157 2024-05-13 13:19:45.000000 beacon2-import-1.0.8/beacon2_search/beacon2_search.py
+-rw-rw-r--   0 khaled    (1000) khaled    (1000)        0 2024-04-08 11:28:15.000000 beacon2-import-1.0.8/beacon2_search/__init__.py
```

### Comparing `beacon2-import-1.0.7/utils.py` & `beacon2-import-1.0.8/utils.py`

 * *Files identical despite different names*

### Comparing `beacon2-import-1.0.7/beacon2_import/utils.py` & `beacon2-import-1.0.8/beacon2_import/utils.py`

 * *Files identical despite different names*

### Comparing `beacon2-import-1.0.7/beacon2_import/beacon2_import.py` & `beacon2-import-1.0.8/beacon2_import/beacon2_import.py`

 * *Files identical despite different names*

### Comparing `beacon2-import-1.0.7/setup.py` & `beacon2-import-1.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='beacon2-import',
-    version='1.0.7',
+    version='1.0.8',
     author='Khaled Jumah',
     author_email='khalled.jooma@yahoo.com',
     description='Seamlessly import and query genomic variant data from a beacon',
     license = 'CC-BY-NC-4.0',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
```

### Comparing `beacon2-import-1.0.7/beacon2_search/utils.py` & `beacon2-import-1.0.8/beacon2_search/utils.py`

 * *Files identical despite different names*

### Comparing `beacon2-import-1.0.7/beacon2_search/beacon2_search.py` & `beacon2-import-1.0.8/beacon2_search/beacon2_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,15 +191,15 @@
             for arg in required_args:
                 if not getattr(args, arg):
                     print(f"Missing value -> {arg}. Use -h or --help for usage details.")
                     parsers[args.command].print_help()
                     sys.exit(1)
         
         query = {
-            "referenceName": args.geneId,
+            "referenceName": args.referenceName,
             "start": {"$gte": args.start_minimum, "$lte": args.start_maximum},
             "end": {"$gte": args.end_minimum, "$lte": args.end_maximum},
             "variantType": args.variantType
         }
     # Connect to MongoDB collection
     advanced_required_args = ['database_auth_source', 'database_user', 'database_password']
     if any(getattr(args, arg)  != "" for arg in advanced_required_args):
```

