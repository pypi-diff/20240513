# Comparing `tmp/lprocess-0.0.6.tar.gz` & `tmp/lprocess-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lprocess-0.0.6.tar", last modified: Sat May 11 11:47:21 2024, max compression
+gzip compressed data, was "lprocess-0.0.7.tar", last modified: Mon May 13 15:45:12 2024, max compression
```

## Comparing `lprocess-0.0.6.tar` & `lprocess-0.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 lordpatil  (1000) lordpatil  (1000)        0 2024-05-11 11:47:21.320251 lprocess-0.0.6/
--rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)      505 2024-05-11 11:47:21.320251 lprocess-0.0.6/PKG-INFO
-drwxrwxr-x   0 lordpatil  (1000) lordpatil  (1000)        0 2024-05-11 11:47:21.316251 lprocess-0.0.6/lprocess/
--rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)      810 2024-05-11 11:28:18.000000 lprocess-0.0.6/lprocess/EDA.py
--rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)       21 2024-05-11 11:47:06.000000 lprocess-0.0.6/lprocess/__init__.py
-drwxrwxr-x   0 lordpatil  (1000) lordpatil  (1000)        0 2024-05-11 11:47:21.316251 lprocess-0.0.6/lprocess.egg-info/
--rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)      505 2024-05-11 11:47:21.000000 lprocess-0.0.6/lprocess.egg-info/PKG-INFO
--rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)      204 2024-05-11 11:47:21.000000 lprocess-0.0.6/lprocess.egg-info/SOURCES.txt
--rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)        1 2024-05-11 11:47:21.000000 lprocess-0.0.6/lprocess.egg-info/dependency_links.txt
--rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)       24 2024-05-11 11:47:21.000000 lprocess-0.0.6/lprocess.egg-info/requires.txt
--rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)        9 2024-05-11 11:47:21.000000 lprocess-0.0.6/lprocess.egg-info/top_level.txt
--rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)       38 2024-05-11 11:47:21.320251 lprocess-0.0.6/setup.cfg
--rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)      703 2024-05-11 11:47:15.000000 lprocess-0.0.6/setup.py
+drwxrwxr-x   0 lordpatil  (1000) lordpatil  (1000)        0 2024-05-13 15:45:12.792983 lprocess-0.0.7/
+-rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)      505 2024-05-13 15:45:12.792983 lprocess-0.0.7/PKG-INFO
+drwxrwxr-x   0 lordpatil  (1000) lordpatil  (1000)        0 2024-05-13 15:45:12.792983 lprocess-0.0.7/lprocess/
+-rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)     2114 2024-05-13 15:37:37.000000 lprocess-0.0.7/lprocess/EDA.py
+-rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)       21 2024-05-11 11:47:06.000000 lprocess-0.0.7/lprocess/__init__.py
+drwxrwxr-x   0 lordpatil  (1000) lordpatil  (1000)        0 2024-05-13 15:45:12.792983 lprocess-0.0.7/lprocess.egg-info/
+-rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)      505 2024-05-13 15:45:12.000000 lprocess-0.0.7/lprocess.egg-info/PKG-INFO
+-rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)      204 2024-05-13 15:45:12.000000 lprocess-0.0.7/lprocess.egg-info/SOURCES.txt
+-rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)        1 2024-05-13 15:45:12.000000 lprocess-0.0.7/lprocess.egg-info/dependency_links.txt
+-rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)       24 2024-05-13 15:45:12.000000 lprocess-0.0.7/lprocess.egg-info/requires.txt
+-rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)        9 2024-05-13 15:45:12.000000 lprocess-0.0.7/lprocess.egg-info/top_level.txt
+-rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)       38 2024-05-13 15:45:12.792983 lprocess-0.0.7/setup.cfg
+-rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)      703 2024-05-13 15:44:38.000000 lprocess-0.0.7/setup.py
```

### Comparing `lprocess-0.0.6/setup.py` & `lprocess-0.0.7/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 
-VERSION = '0.0.6'
+VERSION = '0.0.7'
 DESCRIPTION = 'Data Preprocessing library'
 
 
 # Setting up
 setup(
     name="lprocess",
     version=VERSION,
```

