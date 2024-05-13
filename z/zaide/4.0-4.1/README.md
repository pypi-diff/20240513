# Comparing `tmp/zaide-4.0.tar.gz` & `tmp/zaide-4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zaide-4.0.tar", last modified: Tue Apr 23 01:18:44 2024, max compression
+gzip compressed data, was "zaide-4.1.tar", last modified: Mon May 13 06:13:14 2024, max compression
```

## Comparing `zaide-4.0.tar` & `zaide-4.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 01:18:44.297787 zaide-4.0/
--rw-rw-rw-   0        0        0        0 2024-01-08 03:59:35.000000 zaide-4.0/LICENSE
--rw-rw-rw-   0        0        0      227 2024-04-23 01:18:44.287740 zaide-4.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-01-12 03:39:56.000000 zaide-4.0/README.rst
--rw-rw-rw-   0        0        0       42 2024-04-23 01:18:44.297787 zaide-4.0/setup.cfg
--rw-rw-rw-   0        0        0     1029 2024-01-12 13:15:01.000000 zaide-4.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-23 01:18:44.248067 zaide-4.0/zaide/
--rw-rw-rw-   0        0        0    14133 2024-03-01 12:23:13.000000 zaide-4.0/zaide/__cls_aide_base__.py
--rw-rw-rw-   0        0        0     6364 2024-03-28 08:54:50.000000 zaide-4.0/zaide/__cls_aide_rst__.py
--rw-rw-rw-   0        0        0     6260 2024-03-08 06:14:19.000000 zaide-4.0/zaide/__cls_aide_rst_files__.py
--rw-rw-rw-   0        0        0      237 2024-02-28 12:06:08.000000 zaide-4.0/zaide/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 01:18:44.282704 zaide-4.0/zaide.egg-info/
--rw-rw-rw-   0        0        0      227 2024-04-23 01:18:43.000000 zaide-4.0/zaide.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2024-04-23 01:18:43.000000 zaide-4.0/zaide.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 01:18:43.000000 zaide-4.0/zaide.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-04-23 01:18:43.000000 zaide-4.0/zaide.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-13 06:13:14.624960 zaide-4.1/
+-rw-rw-rw-   0        0        0        0 2024-01-08 03:59:35.000000 zaide-4.1/LICENSE
+-rw-rw-rw-   0        0        0      227 2024-05-13 06:13:14.619960 zaide-4.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-01-12 03:39:56.000000 zaide-4.1/README.rst
+-rw-rw-rw-   0        0        0       42 2024-05-13 06:13:14.625959 zaide-4.1/setup.cfg
+-rw-rw-rw-   0        0        0     1029 2024-01-12 13:15:01.000000 zaide-4.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 06:13:14.581994 zaide-4.1/zaide/
+-rw-rw-rw-   0        0        0    14133 2024-03-01 12:23:13.000000 zaide-4.1/zaide/__cls_aide_base__.py
+-rw-rw-rw-   0        0        0     6364 2024-03-28 08:54:50.000000 zaide-4.1/zaide/__cls_aide_rst__.py
+-rw-rw-rw-   0        0        0     6260 2024-03-08 06:14:19.000000 zaide-4.1/zaide/__cls_aide_rst_files__.py
+-rw-rw-rw-   0        0        0      237 2024-02-28 12:06:08.000000 zaide-4.1/zaide/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 06:13:14.616959 zaide-4.1/zaide.egg-info/
+-rw-rw-rw-   0        0        0      227 2024-05-13 06:13:13.000000 zaide-4.1/zaide.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2024-05-13 06:13:14.000000 zaide-4.1/zaide.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 06:13:14.000000 zaide-4.1/zaide.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-13 06:13:14.000000 zaide-4.1/zaide.egg-info/top_level.txt
```

### Comparing `zaide-4.0/setup.py` & `zaide-4.1/setup.py`

 * *Files identical despite different names*

### Comparing `zaide-4.0/zaide/__cls_aide_base__.py` & `zaide-4.1/zaide/__cls_aide_base__.py`

 * *Files identical despite different names*

### Comparing `zaide-4.0/zaide/__cls_aide_rst__.py` & `zaide-4.1/zaide/__cls_aide_rst__.py`

 * *Files identical despite different names*

### Comparing `zaide-4.0/zaide/__cls_aide_rst_files__.py` & `zaide-4.1/zaide/__cls_aide_rst_files__.py`

 * *Files identical despite different names*

