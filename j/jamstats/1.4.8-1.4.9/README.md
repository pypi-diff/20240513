# Comparing `tmp/jamstats-1.4.8.tar.gz` & `tmp/jamstats-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jamstats-1.4.8.tar", last modified: Thu Mar  7 15:18:14 2024, max compression
+gzip compressed data, was "jamstats-1.4.9.tar", last modified: Sat Mar  9 04:52:13 2024, max compression
```

## Comparing `jamstats-1.4.8.tar` & `jamstats-1.4.9.tar`

### file list

```diff
@@ -1,47 +1,59 @@
-drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2024-03-07 15:18:14.394754 jamstats-1.4.8/
--rw-r--r--   0 damonmay   (501) staff       (20)    18092 2023-02-20 06:19:34.000000 jamstats-1.4.8/LICENSE
--rw-r--r--   0 damonmay   (501) staff       (20)      797 2024-03-07 15:18:14.393859 jamstats-1.4.8/PKG-INFO
--rw-r--r--   0 damonmay   (501) staff       (20)     8755 2023-10-25 02:29:22.000000 jamstats-1.4.8/README.md
-drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2024-03-07 15:18:14.369272 jamstats-1.4.8/bin/
--rwxr-xr-x   0 damonmay   (501) staff       (20)    11566 2024-02-13 03:42:06.000000 jamstats-1.4.8/bin/jamstats
--rwxr-xr-x   0 damonmay   (501) staff       (20)    10842 2024-02-13 03:42:06.000000 jamstats-1.4.8/bin/jamstats-nogui
--rw-r--r--   0 damonmay   (501) staff       (20)       38 2024-03-07 15:18:14.394894 jamstats-1.4.8/setup.cfg
--rw-r--r--   0 damonmay   (501) staff       (20)     1150 2024-03-07 15:17:56.000000 jamstats-1.4.8/setup.py
--rw-r--r--   0 damonmay   (501) staff       (20)      925 2024-03-07 15:18:03.000000 jamstats-1.4.8/setup_nogui.py
-drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2024-03-07 15:18:14.362987 jamstats-1.4.8/src/
-drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2024-03-07 15:18:14.370404 jamstats-1.4.8/src/jamstats/
--rw-r--r--   0 damonmay   (501) staff       (20)        0 2023-02-20 06:19:34.000000 jamstats-1.4.8/src/jamstats/__init__.py
-drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2024-03-07 15:18:14.376741 jamstats-1.4.8/src/jamstats/data/
--rw-r--r--   0 damonmay   (501) staff       (20)        0 2023-02-20 06:19:34.000000 jamstats-1.4.8/src/jamstats/data/__init__.py
--rw-r--r--   0 damonmay   (501) staff       (20)    13215 2023-11-02 03:23:36.000000 jamstats-1.4.8/src/jamstats/data/game_data.py
--rw-r--r--   0 damonmay   (501) staff       (20)    39185 2024-02-19 22:51:23.000000 jamstats-1.4.8/src/jamstats/data/json_to_pandas.py
-drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2024-03-07 15:18:14.380631 jamstats-1.4.8/src/jamstats/io/
--rw-r--r--   0 damonmay   (501) staff       (20)        0 2023-02-20 06:19:34.000000 jamstats-1.4.8/src/jamstats/io/__init__.py
--rw-r--r--   0 damonmay   (501) staff       (20)     2564 2023-04-25 03:00:12.000000 jamstats-1.4.8/src/jamstats/io/scoreboard_json_io.py
--rw-r--r--   0 damonmay   (501) staff       (20)    10201 2023-04-25 03:00:12.000000 jamstats-1.4.8/src/jamstats/io/scoreboard_server_io.py
--rw-r--r--   0 damonmay   (501) staff       (20)     2216 2023-02-20 06:19:34.000000 jamstats-1.4.8/src/jamstats/io/tsv_io.py
-drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2024-03-07 15:18:14.384937 jamstats-1.4.8/src/jamstats/plots/
--rw-r--r--   0 damonmay   (501) staff       (20)        0 2023-02-20 06:19:34.000000 jamstats-1.4.8/src/jamstats/plots/__init__.py
--rw-r--r--   0 damonmay   (501) staff       (20)    13882 2024-02-19 21:58:39.000000 jamstats-1.4.8/src/jamstats/plots/advanced_plots.py
--rw-r--r--   0 damonmay   (501) staff       (20)    20070 2024-02-19 22:57:33.000000 jamstats-1.4.8/src/jamstats/plots/basic_plots.py
--rw-r--r--   0 damonmay   (501) staff       (20)     3071 2023-11-02 03:23:36.000000 jamstats-1.4.8/src/jamstats/plots/plot_together.py
--rw-r--r--   0 damonmay   (501) staff       (20)     6055 2023-10-25 02:29:22.000000 jamstats-1.4.8/src/jamstats/plots/plot_util.py
-drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2024-03-07 15:18:14.385849 jamstats-1.4.8/src/jamstats/resources/
--rw-r--r--   0 damonmay   (501) staff       (20)        0 2023-02-20 06:19:34.000000 jamstats-1.4.8/src/jamstats/resources/__init__.py
--rw-r--r--   0 damonmay   (501) staff       (20)        6 2024-03-07 15:17:52.000000 jamstats-1.4.8/src/jamstats/resources/jamstats_version.txt
-drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2024-03-07 15:18:14.387862 jamstats-1.4.8/src/jamstats/tables/
--rw-r--r--   0 damonmay   (501) staff       (20)        0 2023-10-25 02:29:22.000000 jamstats-1.4.8/src/jamstats/tables/__init__.py
--rw-r--r--   0 damonmay   (501) staff       (20)    31937 2024-02-19 22:51:28.000000 jamstats-1.4.8/src/jamstats/tables/jamstats_tables.py
--rw-r--r--   0 damonmay   (501) staff       (20)     3094 2024-02-19 21:13:36.000000 jamstats-1.4.8/src/jamstats/tables/table_util.py
-drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2024-03-07 15:18:14.389046 jamstats-1.4.8/src/jamstats/util/
--rw-r--r--   0 damonmay   (501) staff       (20)        0 2023-02-20 06:19:34.000000 jamstats-1.4.8/src/jamstats/util/__init__.py
--rw-r--r--   0 damonmay   (501) staff       (20)     2599 2023-10-25 02:29:22.000000 jamstats-1.4.8/src/jamstats/util/resources.py
-drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2024-03-07 15:18:14.389877 jamstats-1.4.8/src/jamstats/web/
--rw-r--r--   0 damonmay   (501) staff       (20)        0 2023-02-20 06:19:34.000000 jamstats-1.4.8/src/jamstats/web/__init__.py
--rw-r--r--   0 damonmay   (501) staff       (20)    18413 2024-01-31 06:49:44.000000 jamstats-1.4.8/src/jamstats/web/statserver.py
-drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2024-03-07 15:18:14.392176 jamstats-1.4.8/src/jamstats.egg-info/
--rw-r--r--   0 damonmay   (501) staff       (20)      797 2024-03-07 15:18:14.000000 jamstats-1.4.8/src/jamstats.egg-info/PKG-INFO
--rw-r--r--   0 damonmay   (501) staff       (20)      981 2024-03-07 15:18:14.000000 jamstats-1.4.8/src/jamstats.egg-info/SOURCES.txt
--rw-r--r--   0 damonmay   (501) staff       (20)        1 2024-03-07 15:18:14.000000 jamstats-1.4.8/src/jamstats.egg-info/dependency_links.txt
--rw-r--r--   0 damonmay   (501) staff       (20)      233 2024-03-07 15:18:14.000000 jamstats-1.4.8/src/jamstats.egg-info/requires.txt
--rw-r--r--   0 damonmay   (501) staff       (20)        9 2024-03-07 15:18:14.000000 jamstats-1.4.8/src/jamstats.egg-info/top_level.txt
+drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2024-03-09 04:52:13.221128 jamstats-1.4.9/
+-rw-r--r--   0 damonmay   (501) staff       (20)    18092 2023-02-20 06:19:34.000000 jamstats-1.4.9/LICENSE
+-rw-r--r--   0 damonmay   (501) staff       (20)       43 2024-03-09 04:51:06.000000 jamstats-1.4.9/MANIFEST.in
+-rw-r--r--   0 damonmay   (501) staff       (20)      797 2024-03-09 04:52:13.220277 jamstats-1.4.9/PKG-INFO
+-rw-r--r--   0 damonmay   (501) staff       (20)     8755 2023-10-25 02:29:22.000000 jamstats-1.4.9/README.md
+drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2024-03-09 04:52:13.179420 jamstats-1.4.9/bin/
+-rwxr-xr-x   0 damonmay   (501) staff       (20)    11566 2024-02-13 03:42:06.000000 jamstats-1.4.9/bin/jamstats
+-rwxr-xr-x   0 damonmay   (501) staff       (20)    10842 2024-02-13 03:42:06.000000 jamstats-1.4.9/bin/jamstats-nogui
+drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2024-03-09 04:52:13.180376 jamstats-1.4.9/resources/
+-rw-r--r--   0 damonmay   (501) staff       (20)        6 2024-03-09 04:50:00.000000 jamstats-1.4.9/resources/jamstats_version.txt
+-rw-r--r--   0 damonmay   (501) staff       (20)       38 2024-03-09 04:52:13.221249 jamstats-1.4.9/setup.cfg
+-rw-r--r--   0 damonmay   (501) staff       (20)     1150 2024-03-09 04:50:12.000000 jamstats-1.4.9/setup.py
+-rw-r--r--   0 damonmay   (501) staff       (20)      925 2024-03-09 04:50:17.000000 jamstats-1.4.9/setup_nogui.py
+drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2024-03-09 04:52:13.170668 jamstats-1.4.9/src/
+drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2024-03-09 04:52:13.170108 jamstats-1.4.9/src/build/
+drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2024-03-09 04:52:13.180737 jamstats-1.4.9/src/build/jamstats/
+-rw-r--r--   0 damonmay   (501) staff       (20)  5901116 2024-02-13 03:55:11.000000 jamstats-1.4.9/src/build/jamstats/xref-jamstats.html
+drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2024-03-09 04:52:13.197179 jamstats-1.4.9/src/jamstats/
+-rw-r--r--   0 damonmay   (501) staff       (20)        0 2023-02-20 06:19:34.000000 jamstats-1.4.9/src/jamstats/__init__.py
+drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2024-03-09 04:52:13.200716 jamstats-1.4.9/src/jamstats/data/
+-rw-r--r--   0 damonmay   (501) staff       (20)        0 2023-02-20 06:19:34.000000 jamstats-1.4.9/src/jamstats/data/__init__.py
+-rw-r--r--   0 damonmay   (501) staff       (20)    13215 2023-11-02 03:23:36.000000 jamstats-1.4.9/src/jamstats/data/game_data.py
+-rw-r--r--   0 damonmay   (501) staff       (20)    39185 2024-02-19 22:51:23.000000 jamstats-1.4.9/src/jamstats/data/json_to_pandas.py
+drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2024-03-09 04:52:13.203826 jamstats-1.4.9/src/jamstats/io/
+-rw-r--r--   0 damonmay   (501) staff       (20)        0 2023-02-20 06:19:34.000000 jamstats-1.4.9/src/jamstats/io/__init__.py
+-rw-r--r--   0 damonmay   (501) staff       (20)     2564 2023-04-25 03:00:12.000000 jamstats-1.4.9/src/jamstats/io/scoreboard_json_io.py
+-rw-r--r--   0 damonmay   (501) staff       (20)    10201 2023-04-25 03:00:12.000000 jamstats-1.4.9/src/jamstats/io/scoreboard_server_io.py
+-rw-r--r--   0 damonmay   (501) staff       (20)     2216 2023-02-20 06:19:34.000000 jamstats-1.4.9/src/jamstats/io/tsv_io.py
+drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2024-03-09 04:52:13.210262 jamstats-1.4.9/src/jamstats/plots/
+-rw-r--r--   0 damonmay   (501) staff       (20)        0 2023-02-20 06:19:34.000000 jamstats-1.4.9/src/jamstats/plots/__init__.py
+-rw-r--r--   0 damonmay   (501) staff       (20)    13882 2024-02-19 21:58:39.000000 jamstats-1.4.9/src/jamstats/plots/advanced_plots.py
+-rw-r--r--   0 damonmay   (501) staff       (20)    20070 2024-02-19 22:57:33.000000 jamstats-1.4.9/src/jamstats/plots/basic_plots.py
+-rw-r--r--   0 damonmay   (501) staff       (20)     3071 2023-11-02 03:23:36.000000 jamstats-1.4.9/src/jamstats/plots/plot_together.py
+-rw-r--r--   0 damonmay   (501) staff       (20)     6055 2023-10-25 02:29:22.000000 jamstats-1.4.9/src/jamstats/plots/plot_util.py
+drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2024-03-09 04:52:13.211660 jamstats-1.4.9/src/jamstats/resources/
+-rw-r--r--   0 damonmay   (501) staff       (20)        0 2023-02-20 06:19:34.000000 jamstats-1.4.9/src/jamstats/resources/__init__.py
+-rw-r--r--   0 damonmay   (501) staff       (20)        6 2024-03-09 04:50:05.000000 jamstats-1.4.9/src/jamstats/resources/jamstats_version.txt
+drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2024-03-09 04:52:13.213828 jamstats-1.4.9/src/jamstats/tables/
+-rw-r--r--   0 damonmay   (501) staff       (20)        0 2023-10-25 02:29:22.000000 jamstats-1.4.9/src/jamstats/tables/__init__.py
+-rw-r--r--   0 damonmay   (501) staff       (20)    31937 2024-02-19 22:51:28.000000 jamstats-1.4.9/src/jamstats/tables/jamstats_tables.py
+-rw-r--r--   0 damonmay   (501) staff       (20)     3094 2024-02-19 21:13:36.000000 jamstats-1.4.9/src/jamstats/tables/table_util.py
+drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2024-03-09 04:52:13.214447 jamstats-1.4.9/src/jamstats/templates/
+-rw-r--r--   0 damonmay   (501) staff       (20)     5976 2024-01-31 06:42:59.000000 jamstats-1.4.9/src/jamstats/templates/jamstats_gameplots.html
+drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2024-03-09 04:52:13.215331 jamstats-1.4.9/src/jamstats/util/
+-rw-r--r--   0 damonmay   (501) staff       (20)        0 2023-02-20 06:19:34.000000 jamstats-1.4.9/src/jamstats/util/__init__.py
+-rw-r--r--   0 damonmay   (501) staff       (20)     2599 2023-10-25 02:29:22.000000 jamstats-1.4.9/src/jamstats/util/resources.py
+drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2024-03-09 04:52:13.216307 jamstats-1.4.9/src/jamstats/web/
+-rw-r--r--   0 damonmay   (501) staff       (20)        0 2023-02-20 06:19:34.000000 jamstats-1.4.9/src/jamstats/web/__init__.py
+-rw-r--r--   0 damonmay   (501) staff       (20)    18413 2024-01-31 06:49:44.000000 jamstats-1.4.9/src/jamstats/web/statserver.py
+drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2024-03-09 04:52:13.218882 jamstats-1.4.9/src/jamstats.egg-info/
+-rw-r--r--   0 damonmay   (501) staff       (20)      797 2024-03-09 04:52:12.000000 jamstats-1.4.9/src/jamstats.egg-info/PKG-INFO
+-rw-r--r--   0 damonmay   (501) staff       (20)     1184 2024-03-09 04:52:13.000000 jamstats-1.4.9/src/jamstats.egg-info/SOURCES.txt
+-rw-r--r--   0 damonmay   (501) staff       (20)        1 2024-03-09 04:52:12.000000 jamstats-1.4.9/src/jamstats.egg-info/dependency_links.txt
+-rw-r--r--   0 damonmay   (501) staff       (20)      233 2024-03-09 04:52:12.000000 jamstats-1.4.9/src/jamstats.egg-info/requires.txt
+-rw-r--r--   0 damonmay   (501) staff       (20)        9 2024-03-09 04:52:12.000000 jamstats-1.4.9/src/jamstats.egg-info/top_level.txt
+drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2024-03-09 04:52:13.173602 jamstats-1.4.9/webapp/
+drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2024-03-09 04:52:13.217981 jamstats-1.4.9/webapp/templates/
+-rw-r--r--   0 damonmay   (501) staff       (20)     1397 2023-02-20 06:19:34.000000 jamstats-1.4.9/webapp/templates/display_game_plots.html
+-rw-r--r--   0 damonmay   (501) staff       (20)     3177 2023-04-25 03:00:12.000000 jamstats-1.4.9/webapp/templates/upload_game.html
```

### Comparing `jamstats-1.4.8/LICENSE` & `jamstats-1.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `jamstats-1.4.8/PKG-INFO` & `jamstats-1.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jamstats
-Version: 1.4.8
+Version: 1.4.9
 Summary: Data processing, stats and plots on roller derby scoreboard JSON files
 Author: Damon May
 Project-URL: Source, https://github.com/dhmay/jamstats
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 License-File: LICENSE
```

### Comparing `jamstats-1.4.8/README.md` & `jamstats-1.4.9/README.md`

 * *Files identical despite different names*

### Comparing `jamstats-1.4.8/bin/jamstats` & `jamstats-1.4.9/bin/jamstats`

 * *Files identical despite different names*

### Comparing `jamstats-1.4.8/bin/jamstats-nogui` & `jamstats-1.4.9/bin/jamstats-nogui`

 * *Files identical despite different names*

### Comparing `jamstats-1.4.8/setup.py` & `jamstats-1.4.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='jamstats',
-    version='1.4.8',
+    version='1.4.9',
     description='Data processing, stats and plots on roller derby scoreboard JSON files',
     author='Damon May',
     package_dir={"":"src"},
     include_package_data=True,
     packages=find_packages('src', exclude=['test']),
     scripts=['bin/jamstats', 'bin/jamstats-nogui'],
     install_requires=['pandas>=2.2.0', 'seaborn>=0.13.2', 'flask>=3.0.2',
```

### Comparing `jamstats-1.4.8/setup_nogui.py` & `jamstats-1.4.9/setup_nogui.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='jamstats-nogui',
-    version='1.4.8',
+    version='1.4.9',
     description='Data processing, stats and plots on roller derby scoreboard JSON files. No-GUI version.',
     author='Damon May',
     package_dir={"":"src"},
     include_package_data=True,
     packages=['jamstats'],
     scripts=['bin/jamstats-nogui'],
     install_requires=['pandas>=2.2.0', 'seaborn>=0.13.2', 'flask>=3.0.2',
```

### Comparing `jamstats-1.4.8/src/jamstats/data/game_data.py` & `jamstats-1.4.9/src/jamstats/data/game_data.py`

 * *Files identical despite different names*

### Comparing `jamstats-1.4.8/src/jamstats/data/json_to_pandas.py` & `jamstats-1.4.9/src/jamstats/data/json_to_pandas.py`

 * *Files identical despite different names*

### Comparing `jamstats-1.4.8/src/jamstats/io/scoreboard_json_io.py` & `jamstats-1.4.9/src/jamstats/io/scoreboard_json_io.py`

 * *Files identical despite different names*

### Comparing `jamstats-1.4.8/src/jamstats/io/scoreboard_server_io.py` & `jamstats-1.4.9/src/jamstats/io/scoreboard_server_io.py`

 * *Files identical despite different names*

### Comparing `jamstats-1.4.8/src/jamstats/io/tsv_io.py` & `jamstats-1.4.9/src/jamstats/io/tsv_io.py`

 * *Files identical despite different names*

### Comparing `jamstats-1.4.8/src/jamstats/plots/advanced_plots.py` & `jamstats-1.4.9/src/jamstats/plots/advanced_plots.py`

 * *Files identical despite different names*

### Comparing `jamstats-1.4.8/src/jamstats/plots/basic_plots.py` & `jamstats-1.4.9/src/jamstats/plots/basic_plots.py`

 * *Files identical despite different names*

### Comparing `jamstats-1.4.8/src/jamstats/plots/plot_together.py` & `jamstats-1.4.9/src/jamstats/plots/plot_together.py`

 * *Files identical despite different names*

### Comparing `jamstats-1.4.8/src/jamstats/plots/plot_util.py` & `jamstats-1.4.9/src/jamstats/plots/plot_util.py`

 * *Files identical despite different names*

### Comparing `jamstats-1.4.8/src/jamstats/tables/jamstats_tables.py` & `jamstats-1.4.9/src/jamstats/tables/jamstats_tables.py`

 * *Files identical despite different names*

### Comparing `jamstats-1.4.8/src/jamstats/tables/table_util.py` & `jamstats-1.4.9/src/jamstats/tables/table_util.py`

 * *Files identical despite different names*

### Comparing `jamstats-1.4.8/src/jamstats/util/resources.py` & `jamstats-1.4.9/src/jamstats/util/resources.py`

 * *Files identical despite different names*

### Comparing `jamstats-1.4.8/src/jamstats/web/statserver.py` & `jamstats-1.4.9/src/jamstats/web/statserver.py`

 * *Files identical despite different names*

### Comparing `jamstats-1.4.8/src/jamstats.egg-info/PKG-INFO` & `jamstats-1.4.9/src/jamstats.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jamstats
-Version: 1.4.8
+Version: 1.4.9
 Summary: Data processing, stats and plots on roller derby scoreboard JSON files
 Author: Damon May
 Project-URL: Source, https://github.com/dhmay/jamstats
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 License-File: LICENSE
```

