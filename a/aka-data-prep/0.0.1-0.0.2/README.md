# Comparing `tmp/aka_data_prep-0.0.1.tar.gz` & `tmp/aka_data_prep-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aka_data_prep-0.0.1.tar", last modified: Sun May 12 22:20:30 2024, max compression
+gzip compressed data, was "aka_data_prep-0.0.2.tar", last modified: Sun May 12 22:33:19 2024, max compression
```

## Comparing `aka_data_prep-0.0.1.tar` & `aka_data_prep-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 22:20:32.000000 aka_data_prep-0.0.1/
--rw-rw-rw-   0        0        0      190 2024-05-12 22:20:32.000000 aka_data_prep-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-12 11:48:58.000000 aka_data_prep-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-12 22:20:32.000000 aka_data_prep-0.0.1/aka_data_prep/
--rw-rw-rw-   0        0        0       93 2024-05-12 22:14:14.000000 aka_data_prep-0.0.1/aka_data_prep/__init__.py
--rw-rw-rw-   0        0        0    15276 2024-05-12 22:12:26.000000 aka_data_prep-0.0.1/aka_data_prep/aka_data_prep.py
-drwxrwxrwx   0        0        0        0 2024-05-12 22:20:32.000000 aka_data_prep-0.0.1/aka_data_prep.egg-info/
--rw-rw-rw-   0        0        0      190 2024-05-12 22:20:30.000000 aka_data_prep-0.0.1/aka_data_prep.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      259 2024-05-12 22:20:30.000000 aka_data_prep-0.0.1/aka_data_prep.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 22:20:30.000000 aka_data_prep-0.0.1/aka_data_prep.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2024-05-12 22:20:30.000000 aka_data_prep-0.0.1/aka_data_prep.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-12 22:20:30.000000 aka_data_prep-0.0.1/aka_data_prep.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-12 22:20:32.000000 aka_data_prep-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      465 2024-05-12 22:18:24.000000 aka_data_prep-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 22:33:20.000000 aka_data_prep-0.0.2/
+-rw-rw-rw-   0        0        0      190 2024-05-12 22:33:20.000000 aka_data_prep-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-12 11:48:58.000000 aka_data_prep-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-12 22:33:20.000000 aka_data_prep-0.0.2/aka_data_prep/
+-rw-rw-rw-   0        0        0       93 2024-05-12 22:14:14.000000 aka_data_prep-0.0.2/aka_data_prep/__init__.py
+-rw-rw-rw-   0        0        0    15276 2024-05-12 22:12:26.000000 aka_data_prep-0.0.2/aka_data_prep/aka_data_prep.py
+drwxrwxrwx   0        0        0        0 2024-05-12 22:33:20.000000 aka_data_prep-0.0.2/aka_data_prep.egg-info/
+-rw-rw-rw-   0        0        0      190 2024-05-12 22:33:20.000000 aka_data_prep-0.0.2/aka_data_prep.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2024-05-12 22:33:20.000000 aka_data_prep-0.0.2/aka_data_prep.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 22:33:20.000000 aka_data_prep-0.0.2/aka_data_prep.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-05-12 22:33:20.000000 aka_data_prep-0.0.2/aka_data_prep.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-12 22:33:20.000000 aka_data_prep-0.0.2/aka_data_prep.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-12 22:33:20.000000 aka_data_prep-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      425 2024-05-12 22:33:08.000000 aka_data_prep-0.0.2/setup.py
```

### Comparing `aka_data_prep-0.0.1/aka_data_prep/aka_data_prep.py` & `aka_data_prep-0.0.2/aka_data_prep/aka_data_prep.py`

 * *Files identical despite different names*

