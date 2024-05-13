# Comparing `tmp/superblocks-types-0.0.2.tar.gz` & `tmp/superblocks-types-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superblocks-types-0.0.2.tar", last modified: Fri May 10 20:51:09 2024, max compression
+gzip compressed data, was "superblocks-types-0.0.3.tar", last modified: Mon May 13 13:59:56 2024, max compression
```

## Comparing `superblocks-types-0.0.2.tar` & `superblocks-types-0.0.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-10 20:51:09.923549 superblocks-types-0.0.2/
--rw-r--r--   0 joeygreco   (501) staff       (20)      694 2024-05-10 20:51:09.923365 superblocks-types-0.0.2/PKG-INFO
--rw-r--r--   0 joeygreco   (501) staff       (20)     2857 2023-10-13 17:42:57.000000 superblocks-types-0.0.2/README.md
--rw-r--r--   0 joeygreco   (501) staff       (20)       38 2024-05-10 20:51:09.923657 superblocks-types-0.0.2/setup.cfg
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-10 20:51:09.923120 superblocks-types-0.0.2/superblocks_types.egg-info/
--rw-r--r--   0 joeygreco   (501) staff       (20)      694 2024-05-10 20:51:09.000000 superblocks-types-0.0.2/superblocks_types.egg-info/PKG-INFO
--rw-r--r--   0 joeygreco   (501) staff       (20)      173 2024-05-10 20:51:09.000000 superblocks-types-0.0.2/superblocks_types.egg-info/SOURCES.txt
--rw-r--r--   0 joeygreco   (501) staff       (20)        1 2024-05-10 20:51:09.000000 superblocks-types-0.0.2/superblocks_types.egg-info/dependency_links.txt
--rw-r--r--   0 joeygreco   (501) staff       (20)        1 2024-05-10 20:51:09.000000 superblocks-types-0.0.2/superblocks_types.egg-info/top_level.txt
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:59:56.271715 superblocks-types-0.0.3/
+-rw-r--r--   0 joeygreco   (501) staff       (20)      699 2024-05-13 13:59:56.271350 superblocks-types-0.0.3/PKG-INFO
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2857 2023-10-13 17:42:57.000000 superblocks-types-0.0.3/README.md
+-rw-r--r--   0 joeygreco   (501) staff       (20)       38 2024-05-13 13:59:56.271800 superblocks-types-0.0.3/setup.cfg
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:59:56.271029 superblocks-types-0.0.3/superblocks_types.egg-info/
+-rw-r--r--   0 joeygreco   (501) staff       (20)      699 2024-05-13 13:59:56.000000 superblocks-types-0.0.3/superblocks_types.egg-info/PKG-INFO
+-rw-r--r--   0 joeygreco   (501) staff       (20)      173 2024-05-13 13:59:56.000000 superblocks-types-0.0.3/superblocks_types.egg-info/SOURCES.txt
+-rw-r--r--   0 joeygreco   (501) staff       (20)        1 2024-05-13 13:59:56.000000 superblocks-types-0.0.3/superblocks_types.egg-info/dependency_links.txt
+-rw-r--r--   0 joeygreco   (501) staff       (20)        1 2024-05-13 13:59:56.000000 superblocks-types-0.0.3/superblocks_types.egg-info/top_level.txt
```

### Comparing `superblocks-types-0.0.2/PKG-INFO` & `superblocks-types-0.0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superblocks-types
-Version: 0.0.2
+Version: 0.0.3
 Summary: The Official Python Types for Superblocks
 Home-page: https://github.com/superblocksteam/types
 Author: Joey Greco
 Author-email: joeyagreco@gmail.com
 License: MIT
 Keywords: superblocks types
 Requires-Python: >=3.10
@@ -29,9 +29,9 @@
 ```sh
 make deps
 ```
 
 Build Package
 
 ```sh
-make pkg-build
+make pypi-pkg-build
 ```
```

### Comparing `superblocks-types-0.0.2/README.md` & `superblocks-types-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.2/superblocks_types.egg-info/PKG-INFO` & `superblocks-types-0.0.3/superblocks_types.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superblocks-types
-Version: 0.0.2
+Version: 0.0.3
 Summary: The Official Python Types for Superblocks
 Home-page: https://github.com/superblocksteam/types
 Author: Joey Greco
 Author-email: joeyagreco@gmail.com
 License: MIT
 Keywords: superblocks types
 Requires-Python: >=3.10
@@ -29,9 +29,9 @@
 ```sh
 make deps
 ```
 
 Build Package
 
 ```sh
-make pkg-build
+make pypi-pkg-build
 ```
```

