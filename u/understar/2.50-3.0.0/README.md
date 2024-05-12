# Comparing `tmp/understar-2.50.tar.gz` & `tmp/understar-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "understar-2.50.tar", last modified: Sun Feb  4 21:31:56 2024, max compression
+gzip compressed data, was "understar-3.0.0.tar", last modified: Sun May 12 22:06:46 2024, max compression
```

## Comparing `understar-2.50.tar` & `understar-3.0.0.tar`

### file list

```diff
@@ -1,38 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-02-04 21:31:56.581492 understar-2.50/
--rw-rw-rw-   0        0        0     1088 2023-11-28 22:26:56.000000 understar-2.50/LICENSE
--rw-rw-rw-   0        0        0     1210 2023-08-10 02:35:08.000000 understar-2.50/LICENSE.md
--rw-rw-rw-   0        0        0      685 2024-02-04 21:31:56.580499 understar-2.50/PKG-INFO
--rw-rw-rw-   0        0        0       74 2023-10-12 16:18:40.000000 understar-2.50/README.md
--rw-rw-rw-   0        0        0       42 2024-02-04 21:31:56.582490 understar-2.50/setup.cfg
--rw-rw-rw-   0        0        0     1290 2024-02-04 21:31:37.000000 understar-2.50/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-04 21:31:56.521653 understar-2.50/understar/
--rw-rw-rw-   0        0        0        6 2024-02-04 21:31:44.000000 understar-2.50/understar/.version
--rw-rw-rw-   0        0        0       25 2023-08-10 02:35:08.000000 understar-2.50/understar/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-04 21:31:56.547583 understar-2.50/understar/system/
--rw-rw-rw-   0        0        0       22 2023-08-10 02:35:08.000000 understar-2.50/understar/system/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-04 21:31:56.549578 understar-2.50/understar/system/app/
--rw-rw-rw-   0        0        0       91 2023-08-10 02:35:08.000000 understar-2.50/understar/system/app/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-04 21:31:56.551573 understar-2.50/understar/system/app/config/
--rw-rw-rw-   0        0        0    20416 2023-08-10 02:35:08.000000 understar-2.50/understar/system/app/config/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-04 21:31:56.558554 understar-2.50/understar/system/app/config/apt/
--rw-rw-rw-   0        0        0       32 2023-08-10 02:35:08.000000 understar-2.50/understar/system/app/config/apt/__init__.py
--rw-rw-rw-   0        0        0     3425 2023-08-10 02:35:08.000000 understar-2.50/understar/system/app/config/apt/install.py
--rw-rw-rw-   0        0        0     1355 2023-08-10 02:35:08.000000 understar-2.50/understar/system/app/config/apt/uninstall.py
-drwxrwxrwx   0        0        0        0 2024-02-04 21:31:56.561587 understar-2.50/understar/system/app/maintenance/
--rw-rw-rw-   0        0        0      924 2023-08-10 02:35:08.000000 understar-2.50/understar/system/app/maintenance/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-04 21:31:56.578529 understar-2.50/understar/system/lib/
--rw-rw-rw-   0        0        0      151 2023-08-10 02:35:08.000000 understar-2.50/understar/system/lib/__init__.py
--rw-rw-rw-   0        0        0     5733 2024-02-04 20:54:15.000000 understar-2.50/understar/system/lib/app.py
--rw-rw-rw-   0        0        0     1032 2023-08-10 02:35:08.000000 understar-2.50/understar/system/lib/com.py
--rw-rw-rw-   0        0        0    12154 2023-08-10 02:35:08.000000 understar-2.50/understar/system/lib/event.py
--rw-rw-rw-   0        0        0     3891 2023-08-10 02:35:08.000000 understar-2.50/understar/system/lib/save.py
--rw-rw-rw-   0        0        0     2805 2023-08-10 02:35:08.000000 understar-2.50/understar/system/lib/store.py
--rw-rw-rw-   0        0        0      176 2023-08-10 02:35:08.000000 understar-2.50/understar/system/lib/types.py
--rw-rw-rw-   0        0        0     5891 2023-09-06 15:07:59.000000 understar-2.50/understar/system/lib/utils.py
--rw-rw-rw-   0        0        0    32739 2023-08-18 06:39:34.000000 understar-2.50/understar/understar.py
-drwxrwxrwx   0        0        0        0 2024-02-04 21:31:56.545620 understar-2.50/understar.egg-info/
--rw-rw-rw-   0        0        0      685 2024-02-04 21:31:56.000000 understar-2.50/understar.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      782 2024-02-04 21:31:56.000000 understar-2.50/understar.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-04 21:31:56.000000 understar-2.50/understar.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2024-02-04 21:31:56.000000 understar-2.50/understar.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-02-04 21:31:56.000000 understar-2.50/understar.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-12 22:06:46.525437 understar-3.0.0/
+-rw-rw-rw-   0        0        0     1143 2024-05-12 21:42:57.000000 understar-3.0.0/LICENSE
+-rw-rw-rw-   0        0        0     1431 2024-05-12 22:06:46.524438 understar-3.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      816 2024-05-12 22:06:36.000000 understar-3.0.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-12 22:06:46.478928 understar-3.0.0/hot_import/
+-rw-rw-rw-   0        0        0       27 2023-12-03 22:42:50.000000 understar-3.0.0/hot_import/__init__.py
+-rw-rw-rw-   0        0        0     7533 2023-12-04 20:00:33.000000 understar-3.0.0/hot_import/hot_import.py
+-rw-rw-rw-   0        0        0       42 2024-05-12 22:06:46.526442 understar-3.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1034 2024-05-12 22:03:10.000000 understar-3.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 22:06:46.482872 understar-3.0.0/test_import/
+-rw-rw-rw-   0        0        0       21 2023-12-03 22:42:50.000000 understar-3.0.0/test_import/__init__.py
+-rw-rw-rw-   0        0        0      502 2024-05-12 21:47:02.000000 understar-3.0.0/test_import/test.py
+drwxrwxrwx   0        0        0        0 2024-05-12 22:06:46.522436 understar-3.0.0/understar.egg-info/
+-rw-rw-rw-   0        0        0     1431 2024-05-12 22:06:46.000000 understar-3.0.0/understar.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2024-05-12 22:06:46.000000 understar-3.0.0/understar.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 22:06:46.000000 understar-3.0.0/understar.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-12 22:06:46.000000 understar-3.0.0/understar.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2024-05-12 22:06:46.000000 understar-3.0.0/understar.egg-info/top_level.txt
```

