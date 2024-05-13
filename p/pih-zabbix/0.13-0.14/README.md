# Comparing `tmp/pih-zabbix-0.13.tar.gz` & `tmp/pih-zabbix-0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-zabbix-0.13.tar", last modified: Wed Apr 10 02:33:41 2024, max compression
+gzip compressed data, was "pih-zabbix-0.14.tar", last modified: Mon May 13 03:55:01 2024, max compression
```

## Comparing `pih-zabbix-0.13.tar` & `pih-zabbix-0.14.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 02:33:41.559977 pih-zabbix-0.13/
--rw-rw-rw-   0        0        0      323 2024-04-10 02:33:41.544354 pih-zabbix-0.13/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-10 02:33:41.277707 pih-zabbix-0.13/ZabbixService/
--rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-zabbix-0.13/ZabbixService/__init__.py
--rw-rw-rw-   0        0        0      146 2024-03-06 10:34:07.000000 pih-zabbix-0.13/ZabbixService/__main__.py
--rw-rw-rw-   0        0        0      653 2024-04-10 01:15:07.000000 pih-zabbix-0.13/ZabbixService/const.py
--rw-rw-rw-   0        0        0     3225 2024-04-09 23:32:53.000000 pih-zabbix-0.13/ZabbixService/service.py
-drwxrwxrwx   0        0        0        0 2024-04-10 02:33:41.513104 pih-zabbix-0.13/pih_zabbix.egg-info/
--rw-rw-rw-   0        0        0      323 2024-04-10 02:33:40.000000 pih-zabbix-0.13/pih_zabbix.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2024-04-10 02:33:41.000000 pih-zabbix-0.13/pih_zabbix.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 02:33:40.000000 pih-zabbix-0.13/pih_zabbix.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2024-04-10 02:33:41.000000 pih-zabbix-0.13/pih_zabbix.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       27 2024-04-10 02:33:41.000000 pih-zabbix-0.13/pih_zabbix.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-10 02:33:41.000000 pih-zabbix-0.13/pih_zabbix.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-10 02:33:41.575601 pih-zabbix-0.13/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-13 03:55:01.245687 pih-zabbix-0.14/
+-rw-rw-rw-   0        0        0      323 2024-05-13 03:55:01.184039 pih-zabbix-0.14/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-13 03:55:00.792146 pih-zabbix-0.14/ZabbixService/
+-rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-zabbix-0.14/ZabbixService/__init__.py
+-rw-rw-rw-   0        0        0      146 2024-03-06 10:34:07.000000 pih-zabbix-0.14/ZabbixService/__main__.py
+-rw-rw-rw-   0        0        0      722 2024-05-13 03:54:40.000000 pih-zabbix-0.14/ZabbixService/const.py
+-rw-rw-rw-   0        0        0     3225 2024-04-09 23:32:53.000000 pih-zabbix-0.14/ZabbixService/service.py
+drwxrwxrwx   0        0        0        0 2024-05-13 03:55:01.121564 pih-zabbix-0.14/pih_zabbix.egg-info/
+-rw-rw-rw-   0        0        0      323 2024-05-13 03:55:00.000000 pih-zabbix-0.14/pih_zabbix.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      305 2024-05-13 03:55:00.000000 pih-zabbix-0.14/pih_zabbix.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 03:55:00.000000 pih-zabbix-0.14/pih_zabbix.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-05-13 03:55:00.000000 pih-zabbix-0.14/pih_zabbix.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       27 2024-05-13 03:55:00.000000 pih-zabbix-0.14/pih_zabbix.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-13 03:55:00.000000 pih-zabbix-0.14/pih_zabbix.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 03:55:01.260687 pih-zabbix-0.14/setup.cfg
```

### Comparing `pih-zabbix-0.13/ZabbixService/const.py` & `pih-zabbix-0.14/ZabbixService/const.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,26 +3,27 @@
 from pih import A
 from pih.collections.service import ServiceDescription
 
 NAME: str = "Zabbix"
 
 HOST = A.CT_H.WS255
 
-VERSION: str = "0.13"
+VERSION: str = "0.14"
 
 PACKAGES: tuple[str, ...] = ("pyzabbix", "zabbix_utils")
 
 SD: ServiceDescription = ServiceDescription(
     name=NAME,
     description="Zabbix service",
     host=HOST.NAME,
     use_standalone=True,
     packages=PACKAGES,
     standalone_name="zabbix",
     version=VERSION,
 )
 
 ZABBIX_SERVER_HOST: str = A.CT_H.SERVICES.NAME
+ZABBIX_SERVER_WEB_INTERFACE_PORT_FOR_EXTERNAL_ACCESS: int = 58080
 ZABBIX_SERVER_WEB_INTERFACE_PORT: int = 8080
 ZABBIX_SERVER_PORT: int = 10051
 ZABBIX_SERVER_LOGIN: str = "Admin"
-ZABBIX_SERVER_PASSWORD: str = "zabbix"
+ZABBIX_SERVER_PASSWORD: str = "(ZaPIH!)"
```

### Comparing `pih-zabbix-0.13/ZabbixService/service.py` & `pih-zabbix-0.14/ZabbixService/service.py`

 * *Files identical despite different names*

