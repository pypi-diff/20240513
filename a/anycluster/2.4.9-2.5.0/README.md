# Comparing `tmp/anycluster-2.4.9.tar.gz` & `tmp/anycluster-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anycluster-2.4.9.tar", last modified: Thu Apr 25 08:01:44 2024, max compression
+gzip compressed data, was "anycluster-2.5.0.tar", last modified: Mon May 13 07:18:11 2024, max compression
```

## Comparing `anycluster-2.4.9.tar` & `anycluster-2.5.0.tar`

### file list

```diff
@@ -1,54 +1,65 @@
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-25 08:01:44.769286 anycluster-2.4.9/
--rw-r--r--   0 tom       (1000) tom       (1000)     1078 2023-01-20 06:49:37.000000 anycluster-2.4.9/LICENSE
--rw-r--r--   0 tom       (1000) tom       (1000)      219 2023-04-22 19:21:48.000000 anycluster-2.4.9/MANIFEST.in
--rw-r--r--   0 tom       (1000) tom       (1000)     2342 2024-04-25 08:01:44.769286 anycluster-2.4.9/PKG-INFO
--rw-r--r--   0 tom       (1000) tom       (1000)     1668 2023-04-22 19:37:42.000000 anycluster-2.4.9/README.md
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-25 08:01:44.765953 anycluster-2.4.9/anycluster/
--rw-r--r--   0 tom       (1000) tom       (1000)     1594 2023-04-19 10:28:26.000000 anycluster-2.4.9/anycluster/ClusterCache.py
--rw-r--r--   0 tom       (1000) tom       (1000)     7237 2023-10-17 06:13:56.000000 anycluster-2.4.9/anycluster/FilterComposer.py
--rw-r--r--   0 tom       (1000) tom       (1000)    41927 2024-04-25 07:18:05.000000 anycluster-2.4.9/anycluster/MapClusterer.py
--rw-r--r--   0 tom       (1000) tom       (1000)    10605 2023-03-06 13:41:59.000000 anycluster-2.4.9/anycluster/MapTools.py
--rw-r--r--   0 tom       (1000) tom       (1000)      112 2023-04-19 10:38:36.000000 anycluster-2.4.9/anycluster/__init__.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-25 08:01:44.769286 anycluster-2.4.9/anycluster/api/
--rw-r--r--   0 tom       (1000) tom       (1000)     3180 2023-03-21 14:03:34.000000 anycluster-2.4.9/anycluster/api/json_schemas.py
--rw-r--r--   0 tom       (1000) tom       (1000)     5396 2024-04-25 07:14:35.000000 anycluster-2.4.9/anycluster/api/serializers.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-25 08:01:44.769286 anycluster-2.4.9/anycluster/api/tests/
--rw-r--r--   0 tom       (1000) tom       (1000)     3519 2023-06-13 06:32:18.000000 anycluster-2.4.9/anycluster/api/tests/test_serializers.py
--rw-r--r--   0 tom       (1000) tom       (1000)    15654 2023-10-17 05:32:09.000000 anycluster-2.4.9/anycluster/api/tests/test_views.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1165 2023-05-26 08:37:19.000000 anycluster-2.4.9/anycluster/api/urls.py
--rw-r--r--   0 tom       (1000) tom       (1000)    10705 2024-04-25 07:52:20.000000 anycluster-2.4.9/anycluster/api/views.py
--rw-r--r--   0 tom       (1000) tom       (1000)       95 2023-03-02 07:01:38.000000 anycluster-2.4.9/anycluster/apps.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1142 2023-01-20 06:49:37.000000 anycluster-2.4.9/anycluster/clusters.py
--rw-r--r--   0 tom       (1000) tom       (1000)      602 2023-10-20 10:21:42.000000 anycluster-2.4.9/anycluster/definitions.py
--rw-r--r--   0 tom       (1000) tom       (1000)    16529 2023-01-20 06:49:37.000000 anycluster-2.4.9/anycluster/globalmaptiles.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-25 08:01:44.765953 anycluster-2.4.9/anycluster/static/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-25 08:01:44.765953 anycluster-2.4.9/anycluster/static/anycluster/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-25 08:01:44.769286 anycluster-2.4.9/anycluster/static/anycluster/images/
--rw-r--r--   0 tom       (1000) tom       (1000)     1445 2023-01-20 06:49:37.000000 anycluster-2.4.9/anycluster/static/anycluster/images/10.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1912 2023-01-20 06:49:37.000000 anycluster-2.4.9/anycluster/static/anycluster/images/100.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2093 2023-01-20 06:49:37.000000 anycluster-2.4.9/anycluster/static/anycluster/images/1000.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2811 2023-01-20 06:49:37.000000 anycluster-2.4.9/anycluster/static/anycluster/images/10000.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1409 2023-01-20 06:49:37.000000 anycluster-2.4.9/anycluster/static/anycluster/images/10000_empty.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1262 2023-01-20 06:49:37.000000 anycluster-2.4.9/anycluster/static/anycluster/images/1000_empty.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1034 2023-01-20 06:49:37.000000 anycluster-2.4.9/anycluster/static/anycluster/images/100_empty.png
--rw-r--r--   0 tom       (1000) tom       (1000)      784 2023-01-20 06:49:37.000000 anycluster-2.4.9/anycluster/static/anycluster/images/10_empty.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1253 2023-01-20 06:49:37.000000 anycluster-2.4.9/anycluster/static/anycluster/images/5.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1974 2023-01-20 06:49:37.000000 anycluster-2.4.9/anycluster/static/anycluster/images/50.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1023 2023-01-20 06:49:37.000000 anycluster-2.4.9/anycluster/static/anycluster/images/50_empty.png
--rw-r--r--   0 tom       (1000) tom       (1000)      749 2023-01-20 06:49:37.000000 anycluster-2.4.9/anycluster/static/anycluster/images/5_empty.png
--rwxr-xr-x   0 tom       (1000) tom       (1000)     1158 2023-01-20 06:49:37.000000 anycluster-2.4.9/anycluster/static/anycluster/images/pin_unknown.png
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-25 08:01:44.769286 anycluster-2.4.9/anycluster/tests/
--rw-r--r--   0 tom       (1000) tom       (1000)     2901 2023-10-16 11:02:25.000000 anycluster-2.4.9/anycluster/tests/common.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2412 2023-10-16 11:00:30.000000 anycluster-2.4.9/anycluster/tests/mixins.py
--rw-r--r--   0 tom       (1000) tom       (1000)     6963 2023-04-19 10:47:33.000000 anycluster-2.4.9/anycluster/tests/test_ClusterCache.py
--rw-r--r--   0 tom       (1000) tom       (1000)     9985 2023-10-16 10:29:51.000000 anycluster-2.4.9/anycluster/tests/test_FilterComposer.py
--rw-r--r--   0 tom       (1000) tom       (1000)    32345 2023-10-20 14:21:31.000000 anycluster-2.4.9/anycluster/tests/test_MapClusterer.py
--rw-r--r--   0 tom       (1000) tom       (1000)      223 2023-06-06 12:24:50.000000 anycluster-2.4.9/anycluster/utils.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-25 08:01:44.769286 anycluster-2.4.9/anycluster.egg-info/
--rw-r--r--   0 tom       (1000) tom       (1000)     2342 2024-04-25 08:01:44.000000 anycluster-2.4.9/anycluster.egg-info/PKG-INFO
--rw-r--r--   0 tom       (1000) tom       (1000)     1421 2024-04-25 08:01:44.000000 anycluster-2.4.9/anycluster.egg-info/SOURCES.txt
--rw-r--r--   0 tom       (1000) tom       (1000)        1 2024-04-25 08:01:44.000000 anycluster-2.4.9/anycluster.egg-info/dependency_links.txt
--rw-r--r--   0 tom       (1000) tom       (1000)       40 2024-04-25 08:01:44.000000 anycluster-2.4.9/anycluster.egg-info/requires.txt
--rw-r--r--   0 tom       (1000) tom       (1000)       11 2024-04-25 08:01:44.000000 anycluster-2.4.9/anycluster.egg-info/top_level.txt
--rw-r--r--   0 tom       (1000) tom       (1000)       38 2024-04-25 08:01:44.769286 anycluster-2.4.9/setup.cfg
--rw-r--r--   0 tom       (1000) tom       (1000)      989 2024-04-25 07:57:46.000000 anycluster-2.4.9/setup.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-05-13 07:18:11.428828 anycluster-2.5.0/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1078 2023-01-20 06:49:37.000000 anycluster-2.5.0/LICENSE
+-rw-r--r--   0 tom       (1000) tom       (1000)      219 2023-04-22 19:21:48.000000 anycluster-2.5.0/MANIFEST.in
+-rw-r--r--   0 tom       (1000) tom       (1000)     2342 2024-05-13 07:18:11.428828 anycluster-2.5.0/PKG-INFO
+-rw-r--r--   0 tom       (1000) tom       (1000)     1668 2023-04-22 19:37:42.000000 anycluster-2.5.0/README.md
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-05-13 07:18:11.422161 anycluster-2.5.0/anycluster/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1594 2023-04-19 10:28:26.000000 anycluster-2.5.0/anycluster/ClusterCache.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     7237 2023-10-17 06:13:56.000000 anycluster-2.5.0/anycluster/FilterComposer.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    42145 2024-05-13 07:11:04.000000 anycluster-2.5.0/anycluster/MapClusterer.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    10605 2023-03-06 13:41:59.000000 anycluster-2.5.0/anycluster/MapTools.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      112 2023-04-19 10:38:36.000000 anycluster-2.5.0/anycluster/__init__.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-05-13 07:18:11.422161 anycluster-2.5.0/anycluster/api/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-05-13 07:18:11.425495 anycluster-2.5.0/anycluster/api/__pycache__/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1976 2024-05-13 06:57:46.000000 anycluster-2.5.0/anycluster/api/__pycache__/json_schemas.cpython-311.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     8297 2024-05-13 06:57:46.000000 anycluster-2.5.0/anycluster/api/__pycache__/serializers.cpython-311.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     2017 2024-05-13 06:57:47.000000 anycluster-2.5.0/anycluster/api/__pycache__/urls.cpython-311.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)    15109 2024-05-13 07:14:55.000000 anycluster-2.5.0/anycluster/api/__pycache__/views.cpython-311.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     3180 2023-03-21 14:03:34.000000 anycluster-2.5.0/anycluster/api/json_schemas.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     5396 2024-04-25 07:14:35.000000 anycluster-2.5.0/anycluster/api/serializers.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-05-13 07:18:11.425495 anycluster-2.5.0/anycluster/api/tests/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-05-13 07:18:11.425495 anycluster-2.5.0/anycluster/api/tests/__pycache__/
+-rw-r--r--   0 tom       (1000) tom       (1000)     5354 2024-05-13 06:57:57.000000 anycluster-2.5.0/anycluster/api/tests/__pycache__/test_serializers.cpython-311.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)    22918 2024-05-13 07:14:55.000000 anycluster-2.5.0/anycluster/api/tests/__pycache__/test_views.cpython-311.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     3517 2024-05-13 06:59:13.000000 anycluster-2.5.0/anycluster/api/tests/test_serializers.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    18233 2024-05-13 07:14:39.000000 anycluster-2.5.0/anycluster/api/tests/test_views.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1165 2023-05-26 08:37:19.000000 anycluster-2.5.0/anycluster/api/urls.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    10865 2024-05-13 07:15:08.000000 anycluster-2.5.0/anycluster/api/views.py
+-rw-r--r--   0 tom       (1000) tom       (1000)       95 2023-03-02 07:01:38.000000 anycluster-2.5.0/anycluster/apps.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1142 2023-01-20 06:49:37.000000 anycluster-2.5.0/anycluster/clusters.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      602 2023-10-20 10:21:42.000000 anycluster-2.5.0/anycluster/definitions.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    16529 2023-01-20 06:49:37.000000 anycluster-2.5.0/anycluster/globalmaptiles.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-05-13 07:18:11.422161 anycluster-2.5.0/anycluster/static/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-05-13 07:18:11.422161 anycluster-2.5.0/anycluster/static/anycluster/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-05-13 07:18:11.425495 anycluster-2.5.0/anycluster/static/anycluster/images/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1445 2023-01-20 06:49:37.000000 anycluster-2.5.0/anycluster/static/anycluster/images/10.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1912 2023-01-20 06:49:37.000000 anycluster-2.5.0/anycluster/static/anycluster/images/100.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2093 2023-01-20 06:49:37.000000 anycluster-2.5.0/anycluster/static/anycluster/images/1000.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2811 2023-01-20 06:49:37.000000 anycluster-2.5.0/anycluster/static/anycluster/images/10000.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1409 2023-01-20 06:49:37.000000 anycluster-2.5.0/anycluster/static/anycluster/images/10000_empty.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1262 2023-01-20 06:49:37.000000 anycluster-2.5.0/anycluster/static/anycluster/images/1000_empty.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1034 2023-01-20 06:49:37.000000 anycluster-2.5.0/anycluster/static/anycluster/images/100_empty.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      784 2023-01-20 06:49:37.000000 anycluster-2.5.0/anycluster/static/anycluster/images/10_empty.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1253 2023-01-20 06:49:37.000000 anycluster-2.5.0/anycluster/static/anycluster/images/5.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1974 2023-01-20 06:49:37.000000 anycluster-2.5.0/anycluster/static/anycluster/images/50.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1023 2023-01-20 06:49:37.000000 anycluster-2.5.0/anycluster/static/anycluster/images/50_empty.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      749 2023-01-20 06:49:37.000000 anycluster-2.5.0/anycluster/static/anycluster/images/5_empty.png
+-rwxr-xr-x   0 tom       (1000) tom       (1000)     1158 2023-01-20 06:49:37.000000 anycluster-2.5.0/anycluster/static/anycluster/images/pin_unknown.png
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-05-13 07:18:11.425495 anycluster-2.5.0/anycluster/tests/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-05-13 07:18:11.425495 anycluster-2.5.0/anycluster/tests/__pycache__/
+-rw-r--r--   0 tom       (1000) tom       (1000)     2040 2024-05-13 06:57:46.000000 anycluster-2.5.0/anycluster/tests/__pycache__/common.cpython-311.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     5160 2024-05-13 06:57:46.000000 anycluster-2.5.0/anycluster/tests/__pycache__/mixins.cpython-311.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     2901 2023-10-16 11:02:25.000000 anycluster-2.5.0/anycluster/tests/common.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     2412 2023-10-16 11:00:30.000000 anycluster-2.5.0/anycluster/tests/mixins.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     6963 2023-04-19 10:47:33.000000 anycluster-2.5.0/anycluster/tests/test_ClusterCache.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     9985 2023-10-16 10:29:51.000000 anycluster-2.5.0/anycluster/tests/test_FilterComposer.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    32345 2023-10-20 14:21:31.000000 anycluster-2.5.0/anycluster/tests/test_MapClusterer.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      223 2023-06-06 12:24:50.000000 anycluster-2.5.0/anycluster/utils.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-05-13 07:18:11.425495 anycluster-2.5.0/anycluster.egg-info/
+-rw-r--r--   0 tom       (1000) tom       (1000)     2342 2024-05-13 07:18:11.000000 anycluster-2.5.0/anycluster.egg-info/PKG-INFO
+-rw-r--r--   0 tom       (1000) tom       (1000)     1859 2024-05-13 07:18:11.000000 anycluster-2.5.0/anycluster.egg-info/SOURCES.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)        1 2024-05-13 07:18:11.000000 anycluster-2.5.0/anycluster.egg-info/dependency_links.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)       40 2024-05-13 07:18:11.000000 anycluster-2.5.0/anycluster.egg-info/requires.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)       11 2024-05-13 07:18:11.000000 anycluster-2.5.0/anycluster.egg-info/top_level.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)       38 2024-05-13 07:18:11.428828 anycluster-2.5.0/setup.cfg
+-rw-r--r--   0 tom       (1000) tom       (1000)      989 2024-05-13 07:17:45.000000 anycluster-2.5.0/setup.py
```

### Comparing `anycluster-2.4.9/LICENSE` & `anycluster-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `anycluster-2.4.9/PKG-INFO` & `anycluster-2.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anycluster
-Version: 2.4.9
+Version: 2.5.0
 Summary: anycluster provides Server-Side clustering of map markers for Geodjango
 Home-page: https://github.com/biodiv/anycluster
 Author: Thomas Uher
 Author-email: thomas.uher@sisol-systems.com
 License: The MIT License
 Keywords: django,cluster,kmeans,grid,server-side clustering
 Platform: OS Independent
```

### Comparing `anycluster-2.4.9/README.md` & `anycluster-2.5.0/README.md`

 * *Files identical despite different names*

### Comparing `anycluster-2.4.9/anycluster/ClusterCache.py` & `anycluster-2.5.0/anycluster/ClusterCache.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.4.9/anycluster/FilterComposer.py` & `anycluster-2.5.0/anycluster/FilterComposer.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.4.9/anycluster/MapClusterer.py` & `anycluster-2.5.0/anycluster/MapClusterer.py`

 * *Files 1% similar despite different names*

```diff
@@ -688,31 +688,36 @@
 
         gis_fields_str.rstrip(',')
 
         return gis_fields_str
 
 
     # return all IDs of the pins contained by a kmeans cluster
-    def get_kmeans_cluster_content(self, geometry_type, ids, x, y, filters, zoom, input_srid=4326):
+    def get_kmeans_cluster_content(self, geometry_type, ids, x, y, filters, zoom, geojson=None, input_srid=4326):
 
         cluster = Point(x, y, srid=input_srid)
 
         # request lnglat point
         cell_geos = self.maptools.getCellForPointAsGeos(cluster, zoom, self.grid_size, self.db_srid)
 
         cluster.transform(self.db_srid)
 
         query_geometry = None
         k = BASE_K
+        
+        cluster_geometries = self.cluster_cache.geometries
 
-        if not self.cluster_cache.geometries:
-            raise ValueError('[MapClusterer]: No cached geometries found')
+        if not cluster_geometries:
+            if not geojson:
+                raise ValueError('[MapClusterer]: No cached geometries found, no geojson submitted')
+            
+            cluster_geometries = self.get_cluster_geometries(geojson, geometry_type, zoom)
 
 
-        for geometry in self.cluster_cache.geometries:
+        for geometry in cluster_geometries:
 
             geos = GEOSGeometry(geometry)
             # cached geometries are always srid==self.db_srid
             # bug: geos.srid is set to 4326 here, which is wrong
             # it is impossible to instantiate with GEOSGeometry(geometry, srid=3857), which throws an error
 
             #if geos.srid != self.db_srid:
```

### Comparing `anycluster-2.4.9/anycluster/MapTools.py` & `anycluster-2.5.0/anycluster/MapTools.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.4.9/anycluster/api/json_schemas.py` & `anycluster-2.5.0/anycluster/api/json_schemas.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.4.9/anycluster/api/serializers.py` & `anycluster-2.5.0/anycluster/api/serializers.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.4.9/anycluster/api/tests/test_serializers.py` & `anycluster-2.5.0/anycluster/api/tests/test_serializers.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,9 +126,8 @@
                         'operator': '=',
                     }
                 ]
             }
         }
 
         nested_value = serializer.validate_modulations(nested_modulation)
-        self.assertEqual(nested_value, nested_modulation)
-
+        self.assertEqual(nested_value, nested_modulation)
```

### Comparing `anycluster-2.4.9/anycluster/api/tests/test_views.py` & `anycluster-2.5.0/anycluster/api/tests/test_views.py`

 * *Files 9% similar despite different names*

```diff
@@ -247,16 +247,16 @@
                     is_left_join = False
                     for filter in filters:
                         if '__' in filter['column']:
                             is_left_join = True
                             break
 
                     if is_left_join == True:
-                        print(kmeans_response.data)
-                        print(filters)
+                        #print(kmeans_response.data)
+                        #print(filters)
                         continue
 
                 cluster = kmeans_response.data[0]
 
                 # raw test
                 cluster_cache = ClusterCache(geometry_type, ZOOM, CLUSTER_TYPE_KMEANS, filters)
                 cluster_cache.load_geometries(kmeans_request.session['anycluster_cache'])
@@ -298,14 +298,89 @@
                 request = factory.post(url, post_data, format='json')
                 request.session = kmeans_request.session
 
                 view = GetClusterContent.as_view()
                 response = view(request, **url_kwargs)
 
                 self.assertEqual(response.status_code, status.HTTP_200_OK)
+                
+    def test_post_with_geojson(self):
+        
+        filter_lists = self.get_test_filters()
+
+        for geometry_type in GEOMETRY_TYPES:
+
+            for filters in filter_lists:
+        
+                url_kwargs = {
+                    'zoom': ZOOM,
+                    'grid_size': GRID_SIZE,
+                }
+
+                kmeans_url = reverse('kmeans_cluster', kwargs=url_kwargs)
+
+                kmeans_post_data = {
+                    'geojson' : GEOJSON_RECTANGLE,
+                    'filters': filters,
+                    'geometry_type': geometry_type,
+                }
+                
+                factory = APIRequestFactory()
+                kmeans_request = factory.post(kmeans_url, kmeans_post_data, format='json')
+                kmeans_request.session = {}
+
+                kmeans_view = KmeansCluster.as_view()
+
+                kmeans_response = kmeans_view(kmeans_request, **url_kwargs)
+                
+                if geometry_type == GEOMETRY_TYPE_AREA:
+                    self.assertEqual(len(kmeans_request.session['anycluster_cache']['geometries']), 1)
+
+                # for left join, the data has to be changed to yield a result
+                if len(kmeans_response.data) == 0:
+                    is_left_join = False
+                    for filter in filters:
+                        if '__' in filter['column']:
+                            is_left_join = True
+                            break
+
+                    if is_left_join == True:
+                        #print(kmeans_response.data)
+                        #print(filters)
+                        continue
+
+                cluster = kmeans_response.data[0]
+
+
+                ids = cluster['ids']
+                x = cluster['center']['x']
+                y = cluster['center']['y']
+
+                # view test
+                print('requesting content for cluster ids: {}'.format(ids) )
+
+                url = reverse('get_kmeans_cluster_content', kwargs=url_kwargs)
+
+                post_data = {
+                    'geometry_type': geometry_type,
+                    'geojson': GEOJSON_RECTANGLE,
+                    'ids': ids,
+                    'x': x,
+                    'y': y,
+                    'filters': filters,
+                }
+
+                request = factory.post(url, post_data, format='json')
+                request.session = {}
+
+                view = GetClusterContent.as_view()
+                response = view(request, **url_kwargs)
+
+                self.assertEqual(response.status_code, status.HTTP_200_OK)
+        
 
 
 class TestGetAreaContent(WithGIS, WithFilters, APITestCase):
 
     def test_post(self):
 
         url_kwargs = {
```

### Comparing `anycluster-2.4.9/anycluster/api/urls.py` & `anycluster-2.5.0/anycluster/api/urls.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.4.9/anycluster/api/views.py` & `anycluster-2.5.0/anycluster/api/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -156,17 +156,19 @@
         serializer = ClusterContentRequestSerializer(data=request.data)
 
         if serializer.is_valid():
 
             # awlays use tha latest cache
             cache = request.session.get(self.cache_name, {})
             cached_geometries = cache.get('geometries', [])
+            geojson = serializer.validated_data.get('geojson', None)
 
             if not cached_geometries:
-                raise ValueError('[GetClusterContent]: No cached geometries found')
+                if not geojson:
+                    raise ValueError('[GetClusterContent]: No cached geometries found, and no geojson submitted')
 
             geometry_type = serializer.validated_data['geometry_type']
             output_srid = self.parse_srid(serializer.validated_data['output_srid'])
             input_srid = self.parse_srid(serializer.validated_data['input_srid'])
 
             filters = serializer.validated_data['filters']
 
@@ -176,18 +178,18 @@
             ids = serializer.validated_data['ids']
             x = serializer.validated_data['x']
             y = serializer.validated_data['y']
 
             zoom = kwargs['zoom']
 
             cluster_content = map_clusterer.get_kmeans_cluster_content(geometry_type, ids, x, y, filters, zoom,
-                input_srid=input_srid)
+                geojson=geojson, input_srid=input_srid)
 
             data = self.serialize_gis_model_list(map_clusterer, cluster_content)
-
+            
             return Response(data)
 
         return Response(serializer.errors, status=status.HTTP_400_BAD_REQUEST)
 
 
 
 '''
```

### Comparing `anycluster-2.4.9/anycluster/clusters.py` & `anycluster-2.5.0/anycluster/clusters.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.4.9/anycluster/definitions.py` & `anycluster-2.5.0/anycluster/definitions.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.4.9/anycluster/globalmaptiles.py` & `anycluster-2.5.0/anycluster/globalmaptiles.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.4.9/anycluster/static/anycluster/images/10.png` & `anycluster-2.5.0/anycluster/static/anycluster/images/10.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.4.9/anycluster/static/anycluster/images/100.png` & `anycluster-2.5.0/anycluster/static/anycluster/images/100.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.4.9/anycluster/static/anycluster/images/1000.png` & `anycluster-2.5.0/anycluster/static/anycluster/images/1000.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.4.9/anycluster/static/anycluster/images/10000.png` & `anycluster-2.5.0/anycluster/static/anycluster/images/10000.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.4.9/anycluster/static/anycluster/images/10000_empty.png` & `anycluster-2.5.0/anycluster/static/anycluster/images/10000_empty.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.4.9/anycluster/static/anycluster/images/1000_empty.png` & `anycluster-2.5.0/anycluster/static/anycluster/images/1000_empty.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.4.9/anycluster/static/anycluster/images/100_empty.png` & `anycluster-2.5.0/anycluster/static/anycluster/images/100_empty.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.4.9/anycluster/static/anycluster/images/10_empty.png` & `anycluster-2.5.0/anycluster/static/anycluster/images/10_empty.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.4.9/anycluster/static/anycluster/images/5.png` & `anycluster-2.5.0/anycluster/static/anycluster/images/5.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.4.9/anycluster/static/anycluster/images/50.png` & `anycluster-2.5.0/anycluster/static/anycluster/images/50.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.4.9/anycluster/static/anycluster/images/50_empty.png` & `anycluster-2.5.0/anycluster/static/anycluster/images/50_empty.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.4.9/anycluster/static/anycluster/images/5_empty.png` & `anycluster-2.5.0/anycluster/static/anycluster/images/5_empty.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.4.9/anycluster/static/anycluster/images/pin_unknown.png` & `anycluster-2.5.0/anycluster/static/anycluster/images/pin_unknown.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.4.9/anycluster/tests/common.py` & `anycluster-2.5.0/anycluster/tests/common.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.4.9/anycluster/tests/mixins.py` & `anycluster-2.5.0/anycluster/tests/mixins.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.4.9/anycluster/tests/test_ClusterCache.py` & `anycluster-2.5.0/anycluster/tests/test_ClusterCache.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.4.9/anycluster/tests/test_FilterComposer.py` & `anycluster-2.5.0/anycluster/tests/test_FilterComposer.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.4.9/anycluster/tests/test_MapClusterer.py` & `anycluster-2.5.0/anycluster/tests/test_MapClusterer.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.4.9/anycluster.egg-info/PKG-INFO` & `anycluster-2.5.0/anycluster.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anycluster
-Version: 2.4.9
+Version: 2.5.0
 Summary: anycluster provides Server-Side clustering of map markers for Geodjango
 Home-page: https://github.com/biodiv/anycluster
 Author: Thomas Uher
 Author-email: thomas.uher@sisol-systems.com
 License: The MIT License
 Keywords: django,cluster,kmeans,grid,server-side clustering
 Platform: OS Independent
```

### Comparing `anycluster-2.4.9/setup.py` & `anycluster-2.5.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     'psycopg2',
     'djangorestframework',
     'jsonschema',
 ]
 
 setup(
     name="anycluster",
-    version='2.4.9',
+    version='2.5.0',
     description='anycluster provides Server-Side clustering of map markers for Geodjango',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='The MIT License',
     platforms=['OS Independent'],
     keywords='django, cluster, kmeans, grid, server-side clustering',
     author='Thomas Uher',
```

