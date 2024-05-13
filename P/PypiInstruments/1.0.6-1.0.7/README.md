# Comparing `tmp/PypiInstruments-1.0.6.tar.gz` & `tmp/PypiInstruments-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PypiInstruments-1.0.6.tar", last modified: Thu May  9 04:59:18 2024, max compression
+gzip compressed data, was "PypiInstruments-1.0.7.tar", last modified: Mon May 13 03:22:55 2024, max compression
```

## Comparing `PypiInstruments-1.0.6.tar` & `PypiInstruments-1.0.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 04:59:18.117360 PypiInstruments-1.0.6/
--rw-rw-rw-   0        0        0       83 2024-05-09 04:59:18.115598 PypiInstruments-1.0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-09 04:59:18.017112 PypiInstruments-1.0.6/PypiInstruments.egg-info/
--rw-rw-rw-   0        0        0       83 2024-05-09 04:59:17.000000 PypiInstruments-1.0.6/PypiInstruments.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      436 2024-05-09 04:59:17.000000 PypiInstruments-1.0.6/PypiInstruments.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 04:59:17.000000 PypiInstruments-1.0.6/PypiInstruments.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-06 10:18:59.000000 PypiInstruments-1.0.6/PypiInstruments.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       16 2024-05-09 04:59:17.000000 PypiInstruments-1.0.6/PypiInstruments.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-09 04:59:18.098987 PypiInstruments-1.0.6/instruments/
--rw-rw-rw-   0        0        0     2120 2024-05-09 03:56:02.000000 PypiInstruments-1.0.6/instruments/DP821A.py
--rw-rw-rw-   0        0        0     3815 2024-05-09 03:56:02.000000 PypiInstruments-1.0.6/instruments/Multimemter.py
--rw-rw-rw-   0        0        0      982 2024-05-09 03:56:02.000000 PypiInstruments-1.0.6/instruments/SMU_Examples.py
--rw-rw-rw-   0        0        0        2 2024-05-08 01:30:53.000000 PypiInstruments-1.0.6/instruments/__init__.py
--rw-rw-rw-   0        0        0      297 2024-04-28 10:28:19.000000 PypiInstruments-1.0.6/instruments/device_scan.py
--rw-rw-rw-   0        0        0      740 2024-04-29 02:13:11.000000 PypiInstruments-1.0.6/instruments/instruments_name.py
--rw-rw-rw-   0        0        0    11485 2024-05-09 03:56:02.000000 PypiInstruments-1.0.6/instruments/smu_keithley_2450.py
-drwxrwxrwx   0        0        0        0 2024-05-09 04:59:18.114155 PypiInstruments-1.0.6/one/
--rw-rw-rw-   0        0        0        0 2024-05-06 09:46:19.000000 PypiInstruments-1.0.6/one/__init__.py
--rw-rw-rw-   0        0        0      104 2024-05-04 13:35:48.000000 PypiInstruments-1.0.6/one/hello.py
--rw-rw-rw-   0        0        0        0 2024-05-04 13:27:19.000000 PypiInstruments-1.0.6/one/main.py
--rw-rw-rw-   0        0        0       42 2024-05-09 04:59:18.117360 PypiInstruments-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0      273 2024-05-09 03:56:02.000000 PypiInstruments-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 03:22:55.816334 PypiInstruments-1.0.7/
+-rw-rw-rw-   0        0        0       83 2024-05-13 03:22:55.815330 PypiInstruments-1.0.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-13 03:22:55.711899 PypiInstruments-1.0.7/PypiInstruments.egg-info/
+-rw-rw-rw-   0        0        0       83 2024-05-13 03:22:55.000000 PypiInstruments-1.0.7/PypiInstruments.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      436 2024-05-13 03:22:55.000000 PypiInstruments-1.0.7/PypiInstruments.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 03:22:55.000000 PypiInstruments-1.0.7/PypiInstruments.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-06 10:18:59.000000 PypiInstruments-1.0.7/PypiInstruments.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       16 2024-05-13 03:22:55.000000 PypiInstruments-1.0.7/PypiInstruments.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-13 03:22:55.795984 PypiInstruments-1.0.7/instruments/
+-rw-rw-rw-   0        0        0     2120 2024-05-09 03:56:02.000000 PypiInstruments-1.0.7/instruments/DP821A.py
+-rw-rw-rw-   0        0        0     3815 2024-05-09 03:56:02.000000 PypiInstruments-1.0.7/instruments/Multimemter.py
+-rw-rw-rw-   0        0        0      982 2024-05-09 03:56:02.000000 PypiInstruments-1.0.7/instruments/SMU_Examples.py
+-rw-rw-rw-   0        0        0      201 2024-05-13 03:22:46.000000 PypiInstruments-1.0.7/instruments/__init__.py
+-rw-rw-rw-   0        0        0      297 2024-04-28 10:28:19.000000 PypiInstruments-1.0.7/instruments/device_scan.py
+-rw-rw-rw-   0        0        0      740 2024-04-29 02:13:11.000000 PypiInstruments-1.0.7/instruments/instruments_name.py
+-rw-rw-rw-   0        0        0    11485 2024-05-09 03:56:02.000000 PypiInstruments-1.0.7/instruments/smu_keithley_2450.py
+drwxrwxrwx   0        0        0        0 2024-05-13 03:22:55.814827 PypiInstruments-1.0.7/one/
+-rw-rw-rw-   0        0        0        0 2024-05-06 09:46:19.000000 PypiInstruments-1.0.7/one/__init__.py
+-rw-rw-rw-   0        0        0      104 2024-05-04 13:35:48.000000 PypiInstruments-1.0.7/one/hello.py
+-rw-rw-rw-   0        0        0        0 2024-05-04 13:27:19.000000 PypiInstruments-1.0.7/one/main.py
+-rw-rw-rw-   0        0        0       42 2024-05-13 03:22:55.816334 PypiInstruments-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      273 2024-05-13 03:22:50.000000 PypiInstruments-1.0.7/setup.py
```

### Comparing `PypiInstruments-1.0.6/instruments/DP821A.py` & `PypiInstruments-1.0.7/instruments/DP821A.py`

 * *Files identical despite different names*

### Comparing `PypiInstruments-1.0.6/instruments/Multimemter.py` & `PypiInstruments-1.0.7/instruments/Multimemter.py`

 * *Files identical despite different names*

### Comparing `PypiInstruments-1.0.6/instruments/SMU_Examples.py` & `PypiInstruments-1.0.7/instruments/SMU_Examples.py`

 * *Files identical despite different names*

### Comparing `PypiInstruments-1.0.6/instruments/instruments_name.py` & `PypiInstruments-1.0.7/instruments/instruments_name.py`

 * *Files identical despite different names*

### Comparing `PypiInstruments-1.0.6/instruments/smu_keithley_2450.py` & `PypiInstruments-1.0.7/instruments/smu_keithley_2450.py`

 * *Files identical despite different names*

