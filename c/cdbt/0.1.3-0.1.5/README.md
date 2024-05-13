# Comparing `tmp/cdbt-0.1.3.tar.gz` & `tmp/cdbt-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdbt-0.1.3.tar", last modified: Sun May 12 03:33:48 2024, max compression
+gzip compressed data, was "cdbt-0.1.5.tar", last modified: Sun May 12 23:48:01 2024, max compression
```

## Comparing `cdbt-0.1.3.tar` & `cdbt-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,19 @@
-drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-12 03:33:48.088286 cdbt-0.1.3/
--rw-r--r--   0 craiglathrop   (501) staff       (20)      385 2024-05-12 03:33:48.087844 cdbt-0.1.3/PKG-INFO
-drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-12 03:33:48.081805 cdbt-0.1.3/cdbt/
--rw-r--r--   0 craiglathrop   (501) staff       (20)        0 2024-05-11 20:22:05.000000 cdbt-0.1.3/cdbt/__init__.py
--rw-r--r--   0 craiglathrop   (501) staff       (20)     9791 2024-05-12 03:22:50.000000 cdbt-0.1.3/cdbt/main.py
--rw-r--r--   0 craiglathrop   (501) staff       (20)     6642 2024-05-11 23:20:14.000000 cdbt-0.1.3/cdbt/main_backup.py
-drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-12 03:33:48.087452 cdbt-0.1.3/cdbt.egg-info/
--rw-r--r--   0 craiglathrop   (501) staff       (20)      385 2024-05-12 03:33:48.000000 cdbt-0.1.3/cdbt.egg-info/PKG-INFO
--rw-r--r--   0 craiglathrop   (501) staff       (20)      228 2024-05-12 03:33:48.000000 cdbt-0.1.3/cdbt.egg-info/SOURCES.txt
--rw-r--r--   0 craiglathrop   (501) staff       (20)        1 2024-05-12 03:33:48.000000 cdbt-0.1.3/cdbt.egg-info/dependency_links.txt
--rw-r--r--   0 craiglathrop   (501) staff       (20)       40 2024-05-12 03:33:48.000000 cdbt-0.1.3/cdbt.egg-info/entry_points.txt
--rw-r--r--   0 craiglathrop   (501) staff       (20)        6 2024-05-12 03:33:48.000000 cdbt-0.1.3/cdbt.egg-info/requires.txt
--rw-r--r--   0 craiglathrop   (501) staff       (20)        5 2024-05-12 03:33:48.000000 cdbt-0.1.3/cdbt.egg-info/top_level.txt
--rw-r--r--   0 craiglathrop   (501) staff       (20)       38 2024-05-12 03:33:48.088362 cdbt-0.1.3/setup.cfg
--rwxrwx---   0 craiglathrop   (501) staff       (20)      635 2024-05-12 03:08:36.000000 cdbt-0.1.3/setup.py
+drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-12 23:48:01.558055 cdbt-0.1.5/
+-rw-r--r--   0 craiglathrop   (501) staff       (20)      391 2024-05-12 23:48:01.557484 cdbt-0.1.5/PKG-INFO
+-rw-r--r--   0 craiglathrop   (501) staff       (20)     3396 2024-05-12 23:47:32.000000 cdbt-0.1.5/README.md
+drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-12 23:48:01.541266 cdbt-0.1.5/cdbt/
+-rw-r--r--   0 craiglathrop   (501) staff       (20)        0 2024-05-11 20:22:05.000000 cdbt-0.1.5/cdbt/__init__.py
+-rw-r--r--   0 craiglathrop   (501) staff       (20)     2992 2024-05-12 23:33:23.000000 cdbt-0.1.5/cdbt/cmdline.py
+-rw-r--r--   0 craiglathrop   (501) staff       (20)    11636 2024-05-12 23:33:23.000000 cdbt-0.1.5/cdbt/main.py
+-rw-r--r--   0 craiglathrop   (501) staff       (20)     6642 2024-05-11 23:20:14.000000 cdbt-0.1.5/cdbt/main_backup.py
+drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-12 23:48:01.556707 cdbt-0.1.5/cdbt.egg-info/
+-rw-r--r--   0 craiglathrop   (501) staff       (20)      391 2024-05-12 23:48:01.000000 cdbt-0.1.5/cdbt.egg-info/PKG-INFO
+-rw-r--r--   0 craiglathrop   (501) staff       (20)      273 2024-05-12 23:48:01.000000 cdbt-0.1.5/cdbt.egg-info/SOURCES.txt
+-rw-r--r--   0 craiglathrop   (501) staff       (20)        1 2024-05-12 23:48:01.000000 cdbt-0.1.5/cdbt.egg-info/dependency_links.txt
+-rw-r--r--   0 craiglathrop   (501) staff       (20)       43 2024-05-12 23:48:01.000000 cdbt-0.1.5/cdbt.egg-info/entry_points.txt
+-rw-r--r--   0 craiglathrop   (501) staff       (20)        6 2024-05-12 23:48:01.000000 cdbt-0.1.5/cdbt.egg-info/requires.txt
+-rw-r--r--   0 craiglathrop   (501) staff       (20)        5 2024-05-12 23:48:01.000000 cdbt-0.1.5/cdbt.egg-info/top_level.txt
+-rw-r--r--   0 craiglathrop   (501) staff       (20)       38 2024-05-12 23:48:01.558144 cdbt-0.1.5/setup.cfg
+-rwxrwx---   0 craiglathrop   (501) staff       (20)      644 2024-05-12 19:23:35.000000 cdbt-0.1.5/setup.py
+drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-12 23:48:01.555573 cdbt-0.1.5/tests/
+-rw-r--r--   0 craiglathrop   (501) staff       (20)     6733 2024-05-12 23:31:04.000000 cdbt-0.1.5/tests/test_main.py
```

### Comparing `cdbt-0.1.3/cdbt/main_backup.py` & `cdbt-0.1.5/cdbt/main_backup.py`

 * *Files identical despite different names*

### Comparing `cdbt-0.1.3/setup.py` & `cdbt-0.1.5/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cdbt',
-    version='0.1.3',
+    version='0.1.5',
     description='A CLI tool to manage dbt builds with state handling and manifest management',
     author='Craig Lathrop',
-    author_email='craiglathrop218@gmail.com',
+    author_email='development@coldborecapital.com',
     packages=find_packages(),
     install_requires=[
         'click',
     ],
     entry_points={
         'console_scripts': [
-            'cdbt=cdbt.main:cdbt',
+            'cdbt=cdbt.cmdline:cdbt',
         ],
     },
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
```

