# Comparing `tmp/pih-plb-0.22.tar.gz` & `tmp/pih-plb-0.22.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-plb-0.22.tar", last modified: Wed May  8 02:56:26 2024, max compression
+gzip compressed data, was "pih-plb-0.22.1.tar", last modified: Mon May 13 02:35:52 2024, max compression
```

## Comparing `pih-plb-0.22.tar` & `pih-plb-0.22.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 02:56:26.815874 pih-plb-0.22/
--rw-rw-rw-   0        0        0      293 2024-05-08 02:56:26.784624 pih-plb-0.22/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-08 02:56:26.357579 pih-plb-0.22/PolibaseService/
--rw-rw-rw-   0        0        0        0 2023-10-13 06:33:11.000000 pih-plb-0.22/PolibaseService/__init__.py
--rw-rw-rw-   0        0        0      150 2024-02-14 23:40:07.000000 pih-plb-0.22/PolibaseService/__main__.py
--rw-rw-rw-   0        0        0    45820 2024-05-08 02:28:38.000000 pih-plb-0.22/PolibaseService/api.py
--rw-rw-rw-   0        0        0     3694 2024-05-08 02:53:02.000000 pih-plb-0.22/PolibaseService/const.py
--rw-rw-rw-   0        0        0    14990 2024-05-08 02:40:04.000000 pih-plb-0.22/PolibaseService/service.py
-drwxrwxrwx   0        0        0        0 2024-05-08 02:56:26.737753 pih-plb-0.22/pih_plb.egg-info/
--rw-rw-rw-   0        0        0      293 2024-05-08 02:56:25.000000 pih-plb-0.22/pih_plb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      318 2024-05-08 02:56:26.000000 pih-plb-0.22/pih_plb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 02:56:25.000000 pih-plb-0.22/pih_plb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2024-05-08 02:56:25.000000 pih-plb-0.22/pih_plb.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2024-05-08 02:56:25.000000 pih-plb-0.22/pih_plb.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-08 02:56:25.000000 pih-plb-0.22/pih_plb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-08 02:56:26.831506 pih-plb-0.22/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-13 02:35:52.852900 pih-plb-0.22.1/
+-rw-rw-rw-   0        0        0      295 2024-05-13 02:35:52.820628 pih-plb-0.22.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-13 02:35:52.382051 pih-plb-0.22.1/PolibaseService/
+-rw-rw-rw-   0        0        0        0 2023-10-13 06:33:11.000000 pih-plb-0.22.1/PolibaseService/__init__.py
+-rw-rw-rw-   0        0        0      150 2024-02-14 23:40:07.000000 pih-plb-0.22.1/PolibaseService/__main__.py
+-rw-rw-rw-   0        0        0    45820 2024-05-08 02:28:38.000000 pih-plb-0.22.1/PolibaseService/api.py
+-rw-rw-rw-   0        0        0     3696 2024-05-08 03:54:41.000000 pih-plb-0.22.1/PolibaseService/const.py
+-rw-rw-rw-   0        0        0    14991 2024-05-08 03:54:34.000000 pih-plb-0.22.1/PolibaseService/service.py
+drwxrwxrwx   0        0        0        0 2024-05-13 02:35:52.789395 pih-plb-0.22.1/pih_plb.egg-info/
+-rw-rw-rw-   0        0        0      295 2024-05-13 02:35:51.000000 pih-plb-0.22.1/pih_plb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      318 2024-05-13 02:35:52.000000 pih-plb-0.22.1/pih_plb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 02:35:51.000000 pih-plb-0.22.1/pih_plb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2024-05-13 02:35:51.000000 pih-plb-0.22.1/pih_plb.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2024-05-13 02:35:51.000000 pih-plb-0.22.1/pih_plb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-13 02:35:51.000000 pih-plb-0.22.1/pih_plb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 02:35:52.852900 pih-plb-0.22.1/setup.cfg
```

### Comparing `pih-plb-0.22/PolibaseService/api.py` & `pih-plb-0.22.1/PolibaseService/api.py`

 * *Files identical despite different names*

### Comparing `pih-plb-0.22/PolibaseService/const.py` & `pih-plb-0.22.1/PolibaseService/const.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pih import A
 from pih.tools import j
 from pih.consts import CONST
 from pih.collections.service import ServiceDescription
 
 NAME: str = "Polibase"
 
-VERSION: str = "0.22"
+VERSION: str = "0.22.1"
 
 HOST = A.CT_H.POLIBASE
 
 PACKAGES: tuple[str, ...] = ("oracledb",)
 
 SD: ServiceDescription = ServiceDescription(
     name=NAME,
```

### Comparing `pih-plb-0.22/PolibaseService/service.py` & `pih-plb-0.22.1/PolibaseService/service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import ipih
 
 from pih import A
 from PolibaseService.const import *
 
 SC = A.CT_SC
-ISOLATED: bool = True
+ISOLATED: bool = False
 DEBUG: bool = False
 
 def start(as_standalone: bool = False) -> None:
 
     if A.U.for_service(SD, as_standalone=as_standalone):
 
         from pih.collections import (
```

