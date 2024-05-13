# Comparing `tmp/pgcopyinsert-0.1.0.tar.gz` & `tmp/pgcopyinsert-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgcopyinsert-0.1.0.tar", last modified: Fri May 10 18:47:35 2024, max compression
+gzip compressed data, was "pgcopyinsert-0.1.1.tar", last modified: Mon May 13 12:05:39 2024, max compression
```

## Comparing `pgcopyinsert-0.1.0.tar` & `pgcopyinsert-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2024-05-10 18:47:35.000000 pgcopyinsert-0.1.0/
--rw-rw-r--   0 odosmatthews   (501) staff       (20)     1068 2024-04-04 19:22:24.000000 pgcopyinsert-0.1.0/LICENSE
--rw-r--r--   0 odosmatthews   (501) staff       (20)     1025 2024-05-10 18:47:35.000000 pgcopyinsert-0.1.0/PKG-INFO
--rw-rw-r--   0 odosmatthews   (501) staff       (20)     3799 2024-05-10 18:46:44.000000 pgcopyinsert-0.1.0/README.md
--rw-rw-r--   0 odosmatthews   (501) staff       (20)     1013 2024-05-10 18:47:35.000000 pgcopyinsert-0.1.0/setup.cfg
--rw-rw-r--   0 odosmatthews   (501) staff       (20)       68 2024-04-04 19:22:25.000000 pgcopyinsert-0.1.0/setup.py
-drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2024-05-10 18:47:35.000000 pgcopyinsert-0.1.0/src/
-drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2024-05-10 18:47:35.000000 pgcopyinsert-0.1.0/src/pgcopyinsert/
--rw-rw-r--   0 odosmatthews   (501) staff       (20)      260 2024-05-10 18:39:51.000000 pgcopyinsert-0.1.0/src/pgcopyinsert/__init__.py
--rw-rw-r--   0 odosmatthews   (501) staff       (20)      219 2024-05-08 17:17:01.000000 pgcopyinsert-0.1.0/src/pgcopyinsert/drivers.py
--rw-rw-r--   0 odosmatthews   (501) staff       (20)      857 2024-05-10 17:21:10.000000 pgcopyinsert-0.1.0/src/pgcopyinsert/insert.py
--rw-rw-r--   0 odosmatthews   (501) staff       (20)      520 2024-05-08 13:13:58.000000 pgcopyinsert-0.1.0/src/pgcopyinsert/names.py
--rw-rw-r--   0 odosmatthews   (501) staff       (20)      645 2024-05-08 17:13:13.000000 pgcopyinsert-0.1.0/src/pgcopyinsert/temp.py
-drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2024-05-10 18:47:35.000000 pgcopyinsert-0.1.0/src/pgcopyinsert.egg-info/
--rw-r--r--   0 odosmatthews   (501) staff       (20)     1025 2024-05-10 18:47:35.000000 pgcopyinsert-0.1.0/src/pgcopyinsert.egg-info/PKG-INFO
--rw-rw-r--   0 odosmatthews   (501) staff       (20)      493 2024-05-10 18:47:35.000000 pgcopyinsert-0.1.0/src/pgcopyinsert.egg-info/SOURCES.txt
--rw-rw-r--   0 odosmatthews   (501) staff       (20)        1 2024-05-10 18:47:35.000000 pgcopyinsert-0.1.0/src/pgcopyinsert.egg-info/dependency_links.txt
--rw-rw-r--   0 odosmatthews   (501) staff       (20)        1 2024-04-09 14:12:13.000000 pgcopyinsert-0.1.0/src/pgcopyinsert.egg-info/not-zip-safe
--rw-rw-r--   0 odosmatthews   (501) staff       (20)      134 2024-05-10 18:47:35.000000 pgcopyinsert-0.1.0/src/pgcopyinsert.egg-info/requires.txt
--rw-rw-r--   0 odosmatthews   (501) staff       (20)       13 2024-05-10 18:47:35.000000 pgcopyinsert-0.1.0/src/pgcopyinsert.egg-info/top_level.txt
-drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2024-05-10 18:47:35.000000 pgcopyinsert-0.1.0/tests/
--rw-rw-r--   0 odosmatthews   (501) staff       (20)     6488 2024-04-08 18:32:29.000000 pgcopyinsert-0.1.0/tests/test_copy.py
--rw-rw-r--   0 odosmatthews   (501) staff       (20)      642 2024-04-08 18:32:29.000000 pgcopyinsert-0.1.0/tests/test_copyinsert.py
--rw-rw-r--   0 odosmatthews   (501) staff       (20)     1820 2024-04-08 18:32:29.000000 pgcopyinsert-0.1.0/tests/test_insert.py
--rw-rw-r--   0 odosmatthews   (501) staff       (20)      785 2024-04-08 18:32:29.000000 pgcopyinsert-0.1.0/tests/test_temp.py
+drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2024-05-13 12:05:39.000000 pgcopyinsert-0.1.1/
+-rw-rw-r--   0 odosmatthews   (501) staff       (20)     1068 2024-04-04 19:22:24.000000 pgcopyinsert-0.1.1/LICENSE
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     1025 2024-05-13 12:05:39.000000 pgcopyinsert-0.1.1/PKG-INFO
+-rw-rw-r--   0 odosmatthews   (501) staff       (20)     3799 2024-05-10 18:46:44.000000 pgcopyinsert-0.1.1/README.md
+-rw-rw-r--   0 odosmatthews   (501) staff       (20)     1013 2024-05-13 12:05:39.000000 pgcopyinsert-0.1.1/setup.cfg
+-rw-rw-r--   0 odosmatthews   (501) staff       (20)       68 2024-04-04 19:22:25.000000 pgcopyinsert-0.1.1/setup.py
+drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2024-05-13 12:05:39.000000 pgcopyinsert-0.1.1/src/
+drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2024-05-13 12:05:39.000000 pgcopyinsert-0.1.1/src/pgcopyinsert/
+-rw-rw-r--   0 odosmatthews   (501) staff       (20)      260 2024-05-10 18:39:51.000000 pgcopyinsert-0.1.1/src/pgcopyinsert/__init__.py
+-rw-rw-r--   0 odosmatthews   (501) staff       (20)      219 2024-05-08 17:17:01.000000 pgcopyinsert-0.1.1/src/pgcopyinsert/drivers.py
+-rw-rw-r--   0 odosmatthews   (501) staff       (20)      857 2024-05-10 17:21:10.000000 pgcopyinsert-0.1.1/src/pgcopyinsert/insert.py
+-rw-rw-r--   0 odosmatthews   (501) staff       (20)      520 2024-05-08 13:13:58.000000 pgcopyinsert-0.1.1/src/pgcopyinsert/names.py
+-rw-rw-r--   0 odosmatthews   (501) staff       (20)      645 2024-05-08 17:13:13.000000 pgcopyinsert-0.1.1/src/pgcopyinsert/temp.py
+drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2024-05-13 12:05:39.000000 pgcopyinsert-0.1.1/src/pgcopyinsert.egg-info/
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     1025 2024-05-13 12:05:39.000000 pgcopyinsert-0.1.1/src/pgcopyinsert.egg-info/PKG-INFO
+-rw-rw-r--   0 odosmatthews   (501) staff       (20)      493 2024-05-13 12:05:39.000000 pgcopyinsert-0.1.1/src/pgcopyinsert.egg-info/SOURCES.txt
+-rw-rw-r--   0 odosmatthews   (501) staff       (20)        1 2024-05-13 12:05:39.000000 pgcopyinsert-0.1.1/src/pgcopyinsert.egg-info/dependency_links.txt
+-rw-rw-r--   0 odosmatthews   (501) staff       (20)        1 2024-04-09 14:12:13.000000 pgcopyinsert-0.1.1/src/pgcopyinsert.egg-info/not-zip-safe
+-rw-rw-r--   0 odosmatthews   (501) staff       (20)      134 2024-05-13 12:05:39.000000 pgcopyinsert-0.1.1/src/pgcopyinsert.egg-info/requires.txt
+-rw-rw-r--   0 odosmatthews   (501) staff       (20)       13 2024-05-13 12:05:39.000000 pgcopyinsert-0.1.1/src/pgcopyinsert.egg-info/top_level.txt
+drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2024-05-13 12:05:39.000000 pgcopyinsert-0.1.1/tests/
+-rw-rw-r--   0 odosmatthews   (501) staff       (20)     6488 2024-04-08 18:32:29.000000 pgcopyinsert-0.1.1/tests/test_copy.py
+-rw-rw-r--   0 odosmatthews   (501) staff       (20)      642 2024-04-08 18:32:29.000000 pgcopyinsert-0.1.1/tests/test_copyinsert.py
+-rw-rw-r--   0 odosmatthews   (501) staff       (20)     1820 2024-04-08 18:32:29.000000 pgcopyinsert-0.1.1/tests/test_insert.py
+-rw-rw-r--   0 odosmatthews   (501) staff       (20)      785 2024-04-08 18:32:29.000000 pgcopyinsert-0.1.1/tests/test_temp.py
```

### Comparing `pgcopyinsert-0.1.0/LICENSE` & `pgcopyinsert-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pgcopyinsert-0.1.0/PKG-INFO` & `pgcopyinsert-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgcopyinsert
-Version: 0.1.0
+Version: 0.1.1
 Summary: Functions for faster PostgreSQL bulk inserts by copying to temp table then inserting from temp table.
 Author: Odos Matthews
 License: MIT
 Platform: unix
 Platform: linux
 Platform: osx
 Platform: cygwin
```

### Comparing `pgcopyinsert-0.1.0/README.md` & `pgcopyinsert-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pgcopyinsert-0.1.0/setup.cfg` & `pgcopyinsert-0.1.1/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pgcopyinsert
-version = 0.1.0
+version = 0.1.1
 description = Functions for faster PostgreSQL bulk inserts by copying to temp table then inserting from temp table.
 author = Odos Matthews
 license = MIT
 license_file = LICENSE
 platforms = unix, linux, osx, cygwin, win32
 classifiers = 
 	Programming Language :: Python :: 3
```

### Comparing `pgcopyinsert-0.1.0/src/pgcopyinsert/insert.py` & `pgcopyinsert-0.1.1/src/pgcopyinsert/insert.py`

 * *Files identical despite different names*

### Comparing `pgcopyinsert-0.1.0/src/pgcopyinsert/names.py` & `pgcopyinsert-0.1.1/src/pgcopyinsert/names.py`

 * *Files identical despite different names*

### Comparing `pgcopyinsert-0.1.0/src/pgcopyinsert/temp.py` & `pgcopyinsert-0.1.1/src/pgcopyinsert/temp.py`

 * *Files identical despite different names*

### Comparing `pgcopyinsert-0.1.0/src/pgcopyinsert.egg-info/PKG-INFO` & `pgcopyinsert-0.1.1/src/pgcopyinsert.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgcopyinsert
-Version: 0.1.0
+Version: 0.1.1
 Summary: Functions for faster PostgreSQL bulk inserts by copying to temp table then inserting from temp table.
 Author: Odos Matthews
 License: MIT
 Platform: unix
 Platform: linux
 Platform: osx
 Platform: cygwin
```

### Comparing `pgcopyinsert-0.1.0/tests/test_copy.py` & `pgcopyinsert-0.1.1/tests/test_copy.py`

 * *Files identical despite different names*

### Comparing `pgcopyinsert-0.1.0/tests/test_copyinsert.py` & `pgcopyinsert-0.1.1/tests/test_copyinsert.py`

 * *Files identical despite different names*

### Comparing `pgcopyinsert-0.1.0/tests/test_insert.py` & `pgcopyinsert-0.1.1/tests/test_insert.py`

 * *Files identical despite different names*

### Comparing `pgcopyinsert-0.1.0/tests/test_temp.py` & `pgcopyinsert-0.1.1/tests/test_temp.py`

 * *Files identical despite different names*

