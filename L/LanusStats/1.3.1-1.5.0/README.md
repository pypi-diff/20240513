# Comparing `tmp/LanusStats-1.3.1.tar.gz` & `tmp/LanusStats-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LanusStats-1.3.1.tar", last modified: Wed May  1 19:40:58 2024, max compression
+gzip compressed data, was "LanusStats-1.5.0.tar", last modified: Mon May 13 02:41:27 2024, max compression
```

## Comparing `LanusStats-1.3.1.tar` & `LanusStats-1.5.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 19:40:58.081485 LanusStats-1.3.1/
-drwxrwxrwx   0        0        0        0 2024-05-01 19:40:58.056334 LanusStats-1.3.1/LanusStats/
--rw-rw-rw-   0        0        0      222 2024-04-07 03:06:19.000000 LanusStats-1.3.1/LanusStats/__init__.py
--rw-rw-rw-   0        0        0     1189 2024-05-01 19:28:29.000000 LanusStats-1.3.1/LanusStats/config.py
--rw-rw-rw-   0        0        0     1731 2024-05-01 19:28:29.000000 LanusStats-1.3.1/LanusStats/exceptions.py
--rw-rw-rw-   0        0        0    14960 2024-05-01 19:28:29.000000 LanusStats-1.3.1/LanusStats/fbref.py
--rw-rw-rw-   0        0        0    11603 2024-05-01 19:28:29.000000 LanusStats-1.3.1/LanusStats/fotmob.py
--rw-rw-rw-   0        0        0    16880 2024-05-01 19:28:29.000000 LanusStats-1.3.1/LanusStats/functions.py
--rw-rw-rw-   0        0        0      303 2024-05-01 19:28:29.000000 LanusStats-1.3.1/LanusStats/sofascore.py
--rw-rw-rw-   0        0        0     9558 2024-05-01 19:28:29.000000 LanusStats-1.3.1/LanusStats/threesixfivescores.py
--rw-rw-rw-   0        0        0    17372 2024-05-01 19:28:29.000000 LanusStats-1.3.1/LanusStats/visualizations.py
-drwxrwxrwx   0        0        0        0 2024-05-01 19:40:58.077799 LanusStats-1.3.1/LanusStats.egg-info/
--rw-rw-rw-   0        0        0     8177 2024-05-01 19:40:57.000000 LanusStats-1.3.1/LanusStats.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      407 2024-05-01 19:40:57.000000 LanusStats-1.3.1/LanusStats.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 19:40:57.000000 LanusStats-1.3.1/LanusStats.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-05-01 19:40:57.000000 LanusStats-1.3.1/LanusStats.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-01 19:40:57.000000 LanusStats-1.3.1/LanusStats.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     8177 2024-05-01 19:40:58.080481 LanusStats-1.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     7795 2024-05-01 19:28:29.000000 LanusStats-1.3.1/README.md
--rw-rw-rw-   0        0        0       42 2024-05-01 19:40:58.082577 LanusStats-1.3.1/setup.cfg
--rw-rw-rw-   0        0        0     1012 2024-05-01 19:40:48.000000 LanusStats-1.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 02:41:27.042312 LanusStats-1.5.0/
+drwxrwxrwx   0        0        0        0 2024-05-13 02:41:27.021291 LanusStats-1.5.0/LanusStats/
+-rw-rw-rw-   0        0        0      222 2024-04-07 03:06:19.000000 LanusStats-1.5.0/LanusStats/__init__.py
+-rw-rw-rw-   0        0        0     1189 2024-05-13 02:39:37.000000 LanusStats-1.5.0/LanusStats/config.py
+-rw-rw-rw-   0        0        0     1731 2024-05-13 02:39:37.000000 LanusStats-1.5.0/LanusStats/exceptions.py
+-rw-rw-rw-   0        0        0    14960 2024-05-13 02:39:37.000000 LanusStats-1.5.0/LanusStats/fbref.py
+-rw-rw-rw-   0        0        0    11603 2024-05-13 02:39:37.000000 LanusStats-1.5.0/LanusStats/fotmob.py
+-rw-rw-rw-   0        0        0    18878 2024-05-13 02:39:49.000000 LanusStats-1.5.0/LanusStats/functions.py
+-rw-rw-rw-   0        0        0    14834 2024-05-13 02:40:55.000000 LanusStats-1.5.0/LanusStats/sofascore.py
+-rw-rw-rw-   0        0        0     9558 2024-05-13 02:39:37.000000 LanusStats-1.5.0/LanusStats/threesixfivescores.py
+-rw-rw-rw-   0        0        0    17372 2024-05-13 02:39:37.000000 LanusStats-1.5.0/LanusStats/visualizations.py
+drwxrwxrwx   0        0        0        0 2024-05-13 02:41:27.036798 LanusStats-1.5.0/LanusStats.egg-info/
+-rw-rw-rw-   0        0        0     8177 2024-05-13 02:41:26.000000 LanusStats-1.5.0/LanusStats.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      407 2024-05-13 02:41:26.000000 LanusStats-1.5.0/LanusStats.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 02:41:26.000000 LanusStats-1.5.0/LanusStats.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-05-13 02:41:26.000000 LanusStats-1.5.0/LanusStats.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-13 02:41:26.000000 LanusStats-1.5.0/LanusStats.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     8177 2024-05-13 02:41:27.041307 LanusStats-1.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7795 2024-05-13 02:39:37.000000 LanusStats-1.5.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-13 02:41:27.042312 LanusStats-1.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     1014 2024-05-13 02:39:49.000000 LanusStats-1.5.0/setup.py
```

### Comparing `LanusStats-1.3.1/LanusStats/config.py` & `LanusStats-1.5.0/LanusStats/config.py`

 * *Files identical despite different names*

### Comparing `LanusStats-1.3.1/LanusStats/exceptions.py` & `LanusStats-1.5.0/LanusStats/exceptions.py`

 * *Files identical despite different names*

### Comparing `LanusStats-1.3.1/LanusStats/fbref.py` & `LanusStats-1.5.0/LanusStats/fbref.py`

 * *Files identical despite different names*

### Comparing `LanusStats-1.3.1/LanusStats/fotmob.py` & `LanusStats-1.5.0/LanusStats/fotmob.py`

 * *Files identical despite different names*

### Comparing `LanusStats-1.3.1/LanusStats/functions.py` & `LanusStats-1.5.0/LanusStats/functions.py`

 * *Files 6% similar despite different names*

```diff
@@ -184,14 +184,15 @@
                     "16/17": 12117,
                     "17/18": 13950,
                     "18/19": 18113,
                     "19/20": 24239,
                     "2021": 37231,
                     "2022": 41884,
                     "2023": 47647,
+                    "2024": 57478
                 },
             },
             "Argentina Copa de la Liga Profesional": {
                 "id": 13475,
                 "seasons": {
                     "2019": 23108,
                     "2020": 34618,
@@ -209,27 +210,28 @@
             },
             "Brasileirão Série A": {
                 "id": 325,
                 "seasons": {
                     "20/21": 27591,
                     "2021": 36166,
                     "2022": 40557,
-                    "2023": 48982
+                    "2023": 48982,
+                    "2024": 58766
                 },
             },
             "Bolivia Division Profesional": {
                 "id": 16736,
                 "seasons": {
-                    "2023": 48353
+                    "2023": 48353, "2024": 58156
                 },
             },
             "Chile Primera Division": {
                 "id": 11653,
                 "seasons": {
-                    "2023": 48017
+                    "2023": 48017, "2024": 57883
                 }
             },
             "Colombia Primera A Apertura": {
                 "id": 11539,
                 "seasons": {
                     "2022": 40320,
                     "2023": 48283,
@@ -243,15 +245,16 @@
                     "2023": 52847
                 },
             },
             "Ecuador LigaPro": {
                 "id": 240,
                 "seasons": {
                     "2022": 40503,
-                    "2023": 48720
+                    "2023": 48720,
+                    "2024": 58043
                 },
             },
             "Mexico LigaMX Apertura": {
                 "id": 11621,
                 "seasons": {
                     "2022": 42017,
                     "2023": 52052
@@ -272,15 +275,15 @@
                     "2023": 48078,
                     "2024": 57741
                 },
             },
             "Uruguay Primera Division": {
                 "id": 278,
                 "seasons": {
-                    "2023": 48634,
+                    "2023": 48634, "2024": 58264
                 },
             },
             "Venezuela Primera Division": {
                 "id": 231,
                 "seasons": {
                     "2023": 48742,
                     "2024": 57694
@@ -353,15 +356,22 @@
             "Copa Sudamericana": {
                 "id": 480,
                 "seasons": {
                     "2018": 15809, "2019": 19990, "2020": 26788, 
                     "2021": 35645, "2022": 40175, "2023": 47968, 
                     "2024": 57297,
                 }
-            }, 
+            },
+            "MLS": {
+                "id": 242,
+                "seasons": {
+                    "2021": 35964, "2022": 40071, "2023": 47955, 
+                    "2024": 57317,
+                }
+            }
         },
         '365Scores': {
             'Argentina Copa de la Liga': {
                 'id': 7214,
                 'seasons': None
             },
             'Primera Division Argentina': {
@@ -388,30 +398,73 @@
         'Fotmob': {
             'Premier League': {
                 'id': 47,
                 'seasons': {
                     '2023/2024': 20720, '2022/2023': 17664, '2021/2022': 16390, '2020/2021': 15382  
                 }
             },
+            'Bundesliga': {
+                'id': 54,
+                'seasons': {
+                    '2023/2024': 20946, '2022/2023': 17801, '2021/2022': 16494, '2020/2021': 15481  
+                }
+            },
+            'La Liga': {
+                'id': 87,
+                'seasons': {
+                    '2023/2024': 21053, '2022/2023': 17852, '2021/2022': 16520, '2020/2021': 15585
+                }
+            },
+            'Serie A': {
+                'id': 55,
+                'seasons': {
+                    '2023/2024': 20956, '2022/2023': 17866, '2021/2022': 16621, '2020/2021': 15604
+                }
+            },
+            'Ligue 1': {
+                'id': 53,
+                'seasons': {
+                    '2023/2024': 20868, '2022/2023': 17810, '2021/2022': 16499, '2020/2021': 15293
+                }
+            },
             'Argentina Copa de la Liga': {
                 'id': 10007,
                 'seasons': {
                     '2024': 22636, '2023': 18412, '2022': 17683, '2021': 16512, '2017/2020': 14230
                 }
             },
             'Argentina Primera Division': {
                 'id': 112,
                 'seasons': {
-                    '2024': 22636, '2023': 19058, '2022': 17301, '2021/2022': 16057, '2020/2021': 15756
+                    '2024': 22635, '2023': 19058, '2022': 17301, '2021/2022': 16057, '2020/2021': 15756
                 }
             },
-            'La Liga': {
-                'id': 87,
+            'Primera Division Colombia': {
+                'id': 274,
                 'seasons': {
-                    '2023/2024': 21053, '2022/2023': 17852, '2021/2022': 16520, '2020/2021': 15585
+                    '2024-Apertura': 22613, '2023-Clausura': "18664-Clausura", '2023-Apertura': "18664-Clausura",
+                    '2022-Clausura': "17283-Clausura", "2022-Apertura": "17283-Apertura"
+                }
+            },
+            'Primera Division Chile': {
+                'id': 273,
+                'seasons': {
+                    '2024': 22749, '2023': 18600, '2022': 17370, "2021": 16185
+                }
+            },
+            'Brasileirao': {
+                'id': 268,
+                'seasons': {
+                    '2024': 22978, '2023': 18982, '2022': 17409, "2021": 16201
+                }
+            },
+            'Primera Division Peru': {
+                'id': 131,
+                'seasons': {
+                    '2024': 22698, '2023': 18625, '2022': 17172, "2021": 16143
                 }
             }
         }
     }
     
     #Exceptions or cases of error
     if season != None and type(season) != str:
```

### Comparing `LanusStats-1.3.1/LanusStats/threesixfivescores.py` & `LanusStats-1.5.0/LanusStats/threesixfivescores.py`

 * *Files identical despite different names*

### Comparing `LanusStats-1.3.1/LanusStats/visualizations.py` & `LanusStats-1.5.0/LanusStats/visualizations.py`

 * *Files identical despite different names*

### Comparing `LanusStats-1.3.1/LanusStats.egg-info/PKG-INFO` & `LanusStats-1.5.0/LanusStats.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LanusStats
-Version: 1.3.1
+Version: 1.5.0
 Summary: Python library for scraping football data and visualize it / Libreria de Python para scrapear data de fútbol y visualizarla
 Home-page: https://github.com/federicorabanos
 Author: Federico Rábanos
 Author-email: lanusstats@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `LanusStats-1.3.1/PKG-INFO` & `LanusStats-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LanusStats
-Version: 1.3.1
+Version: 1.5.0
 Summary: Python library for scraping football data and visualize it / Libreria de Python para scrapear data de fútbol y visualizarla
 Home-page: https://github.com/federicorabanos
 Author: Federico Rábanos
 Author-email: lanusstats@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `LanusStats-1.3.1/README.md` & `LanusStats-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `LanusStats-1.3.1/setup.py` & `LanusStats-1.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '1.3.1'
+
+VERSION = '1.5.0'
 PACKAGE_NAME = 'LanusStats'
 AUTHOR = 'Federico Rábanos'
 AUTHOR_EMAIL = 'lanusstats@gmail.com'
 URL = 'https://github.com/federicorabanos'
 
 LICENSE = 'MIT'
 DESCRIPTION = 'Python library for scraping football data and visualize it / Libreria de Python para scrapear data de fútbol y visualizarla'
```

