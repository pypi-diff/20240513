# Comparing `tmp/itwingsdatacollector-0.1.tar.gz` & `tmp/itwingsdatacollector-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "itwingsdatacollector-0.1.tar", last modified: Fri May 10 14:10:03 2024, max compression
+gzip compressed data, was "itwingsdatacollector-0.2.tar", last modified: Mon May 13 09:01:50 2024, max compression
```

## Comparing `itwingsdatacollector-0.1.tar` & `itwingsdatacollector-0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 14:10:03.757351 itwingsdatacollector-0.1/
--rw-rw-rw-   0        0        0        0 2021-07-31 02:25:56.000000 itwingsdatacollector-0.1/LICENSE
--rw-rw-rw-   0        0        0      452 2024-05-10 14:10:03.756350 itwingsdatacollector-0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-02 11:00:34.000000 itwingsdatacollector-0.1/README.md
--rw-rw-rw-   0        0        0      103 2021-07-31 02:25:56.000000 itwingsdatacollector-0.1/pyproject.toml
--rw-rw-rw-   0        0        0      592 2024-05-10 14:10:03.766345 itwingsdatacollector-0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-10 14:10:03.654192 itwingsdatacollector-0.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-10 14:10:03.720951 itwingsdatacollector-0.1/src/datacollector/
--rw-rw-rw-   0        0        0     8641 2024-05-10 08:26:03.000000 itwingsdatacollector-0.1/src/datacollector/WebInsightCollector.py
--rw-rw-rw-   0        0        0        0 2024-05-02 06:46:40.000000 itwingsdatacollector-0.1/src/datacollector/__init__.py
--rw-rw-rw-   0        0        0      691 2024-05-10 08:26:07.000000 itwingsdatacollector-0.1/src/datacollector/config.py
--rw-rw-rw-   0        0        0     4368 2024-05-10 14:00:49.000000 itwingsdatacollector-0.1/src/datacollector/google_analytics.py
--rw-rw-rw-   0        0        0     3237 2024-05-10 14:00:52.000000 itwingsdatacollector-0.1/src/datacollector/pagespeed.py
--rw-rw-rw-   0        0        0     2016 2024-05-10 06:50:06.000000 itwingsdatacollector-0.1/src/datacollector/raw_data_to_csv.py
--rw-rw-rw-   0        0        0     1235 2024-05-10 13:59:59.000000 itwingsdatacollector-0.1/src/datacollector/screaming_frog.py
-drwxrwxrwx   0        0        0        0 2024-05-10 14:10:03.755350 itwingsdatacollector-0.1/src/itwingsdatacollector.egg-info/
--rw-rw-rw-   0        0        0      452 2024-05-10 14:10:03.000000 itwingsdatacollector-0.1/src/itwingsdatacollector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      475 2024-05-10 14:10:03.000000 itwingsdatacollector-0.1/src/itwingsdatacollector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 14:10:03.000000 itwingsdatacollector-0.1/src/itwingsdatacollector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-05-10 14:10:03.000000 itwingsdatacollector-0.1/src/itwingsdatacollector.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-13 09:01:49.993109 itwingsdatacollector-0.2/
+-rw-rw-rw-   0        0        0        0 2021-07-31 02:25:56.000000 itwingsdatacollector-0.2/LICENSE
+-rw-rw-rw-   0        0        0      452 2024-05-13 09:01:49.992109 itwingsdatacollector-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-02 11:00:34.000000 itwingsdatacollector-0.2/README.md
+-rw-rw-rw-   0        0        0      103 2021-07-31 02:25:56.000000 itwingsdatacollector-0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      592 2024-05-13 09:01:49.999111 itwingsdatacollector-0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-13 09:01:49.863327 itwingsdatacollector-0.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-13 09:01:49.926290 itwingsdatacollector-0.2/src/datacollector/
+-rw-rw-rw-   0        0        0        0 2024-05-02 06:46:40.000000 itwingsdatacollector-0.2/src/datacollector/__init__.py
+-rw-rw-rw-   0        0        0      691 2024-05-10 08:26:07.000000 itwingsdatacollector-0.2/src/datacollector/config.py
+-rw-rw-rw-   0        0        0     4368 2024-05-10 14:00:49.000000 itwingsdatacollector-0.2/src/datacollector/google_analytics.py
+-rw-rw-rw-   0        0        0     2251 2024-05-13 08:59:32.000000 itwingsdatacollector-0.2/src/datacollector/pagespeed.py
+-rw-rw-rw-   0        0        0     2016 2024-05-10 06:50:06.000000 itwingsdatacollector-0.2/src/datacollector/raw_data_to_csv.py
+-rw-rw-rw-   0        0        0     1235 2024-05-10 13:59:59.000000 itwingsdatacollector-0.2/src/datacollector/screaming_frog.py
+-rw-rw-rw-   0        0        0     4195 2024-05-13 08:44:10.000000 itwingsdatacollector-0.2/src/datacollector/semrush_api.py
+drwxrwxrwx   0        0        0        0 2024-05-13 09:01:49.991111 itwingsdatacollector-0.2/src/itwingsdatacollector.egg-info/
+-rw-rw-rw-   0        0        0      452 2024-05-13 09:01:49.000000 itwingsdatacollector-0.2/src/itwingsdatacollector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      467 2024-05-13 09:01:49.000000 itwingsdatacollector-0.2/src/itwingsdatacollector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 09:01:49.000000 itwingsdatacollector-0.2/src/itwingsdatacollector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-13 09:01:49.000000 itwingsdatacollector-0.2/src/itwingsdatacollector.egg-info/top_level.txt
```

### Comparing `itwingsdatacollector-0.1/setup.cfg` & `itwingsdatacollector-0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2069 7477 696e 6773 6461 7461 636f   = itwingsdataco
 00000020: 6c6c 6563 746f 720d 0a76 6572 7369 6f6e  llector..version
-00000030: 203d 2030 2e31 0d0a 6175 7468 6f72 203d   = 0.1..author =
+00000030: 203d 2030 2e32 0d0a 6175 7468 6f72 203d   = 0.2..author =
 00000040: 204d 6179 616e 6b0d 0a61 7574 686f 725f   Mayank..author_
 00000050: 656d 6169 6c20 3d20 6d61 7961 6e6b 7469  email = mayankti
 00000060: 6d62 6164 6961 4067 6d61 696c 2e63 6f6d  mbadia@gmail.com
 00000070: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description = 
 00000080: 2749 5420 5769 6e67 7320 4461 7461 2043  'IT Wings Data C
 00000090: 6f6c 6c65 6374 6f72 3a20 4120 746f 6f6c  ollector: A tool
 000000a0: 2066 6f72 2063 6f6c 6c65 6374 696e 6720   for collecting
```

### Comparing `itwingsdatacollector-0.1/src/datacollector/config.py` & `itwingsdatacollector-0.2/src/datacollector/config.py`

 * *Files identical despite different names*

### Comparing `itwingsdatacollector-0.1/src/datacollector/google_analytics.py` & `itwingsdatacollector-0.2/src/datacollector/google_analytics.py`

 * *Files identical despite different names*

### Comparing `itwingsdatacollector-0.1/src/datacollector/raw_data_to_csv.py` & `itwingsdatacollector-0.2/src/datacollector/raw_data_to_csv.py`

 * *Files identical despite different names*

### Comparing `itwingsdatacollector-0.1/src/datacollector/screaming_frog.py` & `itwingsdatacollector-0.2/src/datacollector/screaming_frog.py`

 * *Files identical despite different names*

