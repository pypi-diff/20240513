# Comparing `tmp/ipih-0.22.tar.gz` & `tmp/ipih-0.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipih-0.22.tar", last modified: Mon May  6 03:57:09 2024, max compression
+gzip compressed data, was "ipih-0.23.tar", last modified: Mon May 13 02:12:55 2024, max compression
```

## Comparing `ipih-0.22.tar` & `ipih-0.23.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 03:57:09.696561 ipih-0.22/
--rw-rw-rw-   0        0        0      472 2024-05-06 03:57:09.649687 ipih-0.22/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-06 03:57:09.288232 ipih-0.22/ipih/
--rw-rw-rw-   0        0        0     1317 2024-05-03 03:11:37.000000 ipih-0.22/ipih/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-06 03:57:09.602813 ipih-0.22/ipih.egg-info/
--rw-rw-rw-   0        0        0      472 2024-05-06 03:57:09.000000 ipih-0.22/ipih.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      155 2024-05-06 03:57:09.000000 ipih-0.22/ipih.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 03:57:09.000000 ipih-0.22/ipih.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       85 2024-05-06 03:57:09.000000 ipih-0.22/ipih.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-05-06 03:57:09.000000 ipih-0.22/ipih.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-06 03:57:09.712194 ipih-0.22/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-13 02:12:55.256033 ipih-0.23/
+-rw-rw-rw-   0        0        0      472 2024-05-13 02:12:55.224789 ipih-0.23/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-13 02:12:54.925236 ipih-0.23/ipih/
+-rw-rw-rw-   0        0        0     1317 2024-05-13 02:11:59.000000 ipih-0.23/ipih/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 02:12:55.193521 ipih-0.23/ipih.egg-info/
+-rw-rw-rw-   0        0        0      472 2024-05-13 02:12:54.000000 ipih-0.23/ipih.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      155 2024-05-13 02:12:54.000000 ipih-0.23/ipih.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 02:12:54.000000 ipih-0.23/ipih.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       85 2024-05-13 02:12:54.000000 ipih-0.23/ipih.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-13 02:12:54.000000 ipih-0.23/ipih.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 02:12:55.271664 ipih-0.23/setup.cfg
```

### Comparing `ipih-0.22/ipih/__init__.py` & `ipih-0.23/ipih/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import sys
 import os
 import importlib.util
 import platform
 
 
 NAME: str = "ipih"
-VERSION: str = "0.22"
+VERSION: str = "0.23"
 
 ROOT_MODULE_NAME: str = "pih"
 FACADE_FOLDER_NAME: str = "facade"
 BUILD_FOLDER_NAME: str = ".build"
 BUILD_FILES_FOLDER_NAME: str = ".files"
 WINDOWS_SHARE_DOMAIN_NAME: str = ROOT_MODULE_NAME
 WINDOWS_SHARE_DOMAIN_ALIAS: str = "fmv"
 
-SERVICE_ADMIN_HOST_NAME: str = "fmvdc1"
+SERVICE_ADMIN_HOST_NAME: str = "ws-735"
 SERVICE_ADMIN_GRPC_PORT: int = 20
 
 
 def get_path(is_linux: bool = False) -> str:
     if is_linux:
         return f"//mnt/{FACADE_FOLDER_NAME}"
     return f"//{WINDOWS_SHARE_DOMAIN_ALIAS}/{FACADE_FOLDER_NAME}"
```

