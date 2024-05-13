# Comparing `tmp/lib_version_urlphishing-1.0.1.tar.gz` & `tmp/lib_version_urlphishing-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib_version_urlphishing-1.0.1.tar", last modified: Mon May 13 00:11:45 2024, max compression
+gzip compressed data, was "lib_version_urlphishing-1.0.3.tar", last modified: Mon May 13 00:49:58 2024, max compression
```

## Comparing `lib_version_urlphishing-1.0.1.tar` & `lib_version_urlphishing-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 00:11:45.182547 lib_version_urlphishing-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-13 00:11:33.000000 lib_version_urlphishing-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-13 00:11:45.182547 lib_version_urlphishing-1.0.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 00:11:45.182547 lib_version_urlphishing-1.0.1/lib-version/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 00:11:33.000000 lib_version_urlphishing-1.0.1/lib-version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-13 00:11:33.000000 lib_version_urlphishing-1.0.1/lib-version/version.py
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-13 00:11:33.000000 lib_version_urlphishing-1.0.1/lib-version/version_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 00:11:45.182547 lib_version_urlphishing-1.0.1/lib_version_URLPhishing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-13 00:11:45.000000 lib_version_urlphishing-1.0.1/lib_version_URLPhishing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-13 00:11:45.000000 lib_version_urlphishing-1.0.1/lib_version_URLPhishing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 00:11:45.000000 lib_version_urlphishing-1.0.1/lib_version_URLPhishing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-13 00:11:45.000000 lib_version_urlphishing-1.0.1/lib_version_URLPhishing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 00:11:45.182547 lib_version_urlphishing-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-13 00:11:33.000000 lib_version_urlphishing-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 00:49:58.226074 lib_version_urlphishing-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-13 00:49:44.000000 lib_version_urlphishing-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-13 00:49:58.226074 lib_version_urlphishing-1.0.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 00:49:58.222074 lib_version_urlphishing-1.0.3/lib_version_URLPhishing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 00:49:44.000000 lib_version_urlphishing-1.0.3/lib_version_URLPhishing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-13 00:49:44.000000 lib_version_urlphishing-1.0.3/lib_version_URLPhishing/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-13 00:49:44.000000 lib_version_urlphishing-1.0.3/lib_version_URLPhishing/version_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 00:49:58.226074 lib_version_urlphishing-1.0.3/lib_version_URLPhishing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-13 00:49:58.000000 lib_version_urlphishing-1.0.3/lib_version_URLPhishing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-13 00:49:58.000000 lib_version_urlphishing-1.0.3/lib_version_URLPhishing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 00:49:58.000000 lib_version_urlphishing-1.0.3/lib_version_URLPhishing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-13 00:49:58.000000 lib_version_urlphishing-1.0.3/lib_version_URLPhishing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 00:49:58.226074 lib_version_urlphishing-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-13 00:49:44.000000 lib_version_urlphishing-1.0.3/setup.py
```

### Comparing `lib_version_urlphishing-1.0.1/setup.py` & `lib_version_urlphishing-1.0.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 import os
 
 # Get the directory where setup.py is located
 here = os.path.abspath(os.path.dirname(__file__))
 
 # Use it to build the path to version.py
-version_file = os.path.join(here, 'lib-version', 'version.py')
+version_file = os.path.join(here, 'lib_version_URLPhishing', 'version.py')
 
 # Safely read the version from version.py
 version = {}
 with open(version_file, 'r') as file:
     exec(file.read(), version)
 
 setup(
```

