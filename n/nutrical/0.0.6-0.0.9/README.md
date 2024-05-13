# Comparing `tmp/nutrical-0.0.6.tar.gz` & `tmp/nutrical-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nutrical-0.0.6.tar", last modified: Wed May  8 07:27:24 2024, max compression
+gzip compressed data, was "nutrical-0.0.9.tar", last modified: Mon May 13 03:05:45 2024, max compression
```

## Comparing `nutrical-0.0.6.tar` & `nutrical-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 07:27:24.312829 nutrical-0.0.6/
--rw-rw-rw-   0        0        0    16827 2024-05-08 07:27:24.310717 nutrical-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0    12042 2024-05-08 07:25:48.000000 nutrical-0.0.6/README.md
--rw-rw-rw-   0        0        0        2 2024-05-08 07:27:22.000000 nutrical-0.0.6/VERSION
-drwxrwxrwx   0        0        0        0 2024-05-08 07:27:24.305539 nutrical-0.0.6/data/
--rw-rw-rw-   0        0        0     3509 2024-05-02 05:10:03.000000 nutrical-0.0.6/data/TW_FDA_nutrition_items.csv
-drwxrwxrwx   0        0        0        0 2024-05-08 07:27:24.280519 nutrical-0.0.6/nutrical/
--rw-rw-rw-   0        0        0       42 2024-05-03 05:46:07.000000 nutrical-0.0.6/nutrical/__init__.py
--rw-rw-rw-   0        0        0     1499 2024-05-08 03:45:36.000000 nutrical-0.0.6/nutrical/io.py
--rw-rw-rw-   0        0        0     6202 2024-05-08 03:36:52.000000 nutrical-0.0.6/nutrical/nutrical.py
--rw-rw-rw-   0        0        0       95 2024-05-02 07:08:54.000000 nutrical-0.0.6/nutrical/taiwan-fda.py
--rw-rw-rw-   0        0        0     1840 2024-05-05 23:54:15.000000 nutrical-0.0.6/nutrical/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-08 07:27:24.297852 nutrical-0.0.6/nutrical.egg-info/
--rw-rw-rw-   0        0        0    16827 2024-05-08 07:27:24.000000 nutrical-0.0.6/nutrical.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      339 2024-05-08 07:27:24.000000 nutrical-0.0.6/nutrical.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 07:27:24.000000 nutrical-0.0.6/nutrical.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-05-08 07:27:24.000000 nutrical-0.0.6/nutrical.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-08 07:27:24.000000 nutrical-0.0.6/nutrical.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-08 07:27:24.313868 nutrical-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      949 2024-05-03 02:55:53.000000 nutrical-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 03:05:45.371257 nutrical-0.0.9/
+-rw-rw-rw-   0        0        0    16827 2024-05-13 03:05:45.369268 nutrical-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0    12042 2024-05-08 07:25:48.000000 nutrical-0.0.9/README.md
+-rw-rw-rw-   0        0        0        2 2024-05-13 03:05:43.000000 nutrical-0.0.9/VERSION
+drwxrwxrwx   0        0        0        0 2024-05-13 03:05:45.357420 nutrical-0.0.9/data/
+-rw-rw-rw-   0        0        0     3509 2024-05-02 05:10:03.000000 nutrical-0.0.9/data/TW_FDA_nutrition_items.csv
+drwxrwxrwx   0        0        0        0 2024-05-13 03:05:45.288160 nutrical-0.0.9/nutrical/
+-rw-rw-rw-   0        0        0       42 2024-05-03 05:46:07.000000 nutrical-0.0.9/nutrical/__init__.py
+-rw-rw-rw-   0        0        0     1499 2024-05-08 03:45:36.000000 nutrical-0.0.9/nutrical/io.py
+-rw-rw-rw-   0        0        0     6202 2024-05-08 03:36:52.000000 nutrical-0.0.9/nutrical/nutrical.py
+-rw-rw-rw-   0        0        0       95 2024-05-02 07:08:54.000000 nutrical-0.0.9/nutrical/taiwan-fda.py
+-rw-rw-rw-   0        0        0     1840 2024-05-05 23:54:15.000000 nutrical-0.0.9/nutrical/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-13 03:05:45.346366 nutrical-0.0.9/nutrical.egg-info/
+-rw-rw-rw-   0        0        0    16827 2024-05-13 03:05:44.000000 nutrical-0.0.9/nutrical.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      339 2024-05-13 03:05:45.000000 nutrical-0.0.9/nutrical.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 03:05:44.000000 nutrical-0.0.9/nutrical.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-13 03:05:44.000000 nutrical-0.0.9/nutrical.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-13 03:05:44.000000 nutrical-0.0.9/nutrical.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 03:05:45.372725 nutrical-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      949 2024-05-03 02:55:53.000000 nutrical-0.0.9/setup.py
```

### Comparing `nutrical-0.0.6/PKG-INFO` & `nutrical-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nutrical
-Version: 0.0.6
+Version: 0.0.9
 Summary: Nutrition calculation for recipes and ingredients
 Home-page: https://github.com/liao961120/nutrical
 Author: Yongfu Liao
 Author-email: liao961120@gmail.com
 License: UNKNOWN
 Description: Nutritional value calculation for recipes and ingredients
         =========================================================
```

### Comparing `nutrical-0.0.6/README.md` & `nutrical-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `nutrical-0.0.6/data/TW_FDA_nutrition_items.csv` & `nutrical-0.0.9/data/TW_FDA_nutrition_items.csv`

 * *Files identical despite different names*

### Comparing `nutrical-0.0.6/nutrical/io.py` & `nutrical-0.0.9/nutrical/io.py`

 * *Files identical despite different names*

### Comparing `nutrical-0.0.6/nutrical/nutrical.py` & `nutrical-0.0.9/nutrical/nutrical.py`

 * *Files identical despite different names*

### Comparing `nutrical-0.0.6/nutrical/utils.py` & `nutrical-0.0.9/nutrical/utils.py`

 * *Files identical despite different names*

### Comparing `nutrical-0.0.6/nutrical.egg-info/PKG-INFO` & `nutrical-0.0.9/nutrical.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nutrical
-Version: 0.0.6
+Version: 0.0.9
 Summary: Nutrition calculation for recipes and ingredients
 Home-page: https://github.com/liao961120/nutrical
 Author: Yongfu Liao
 Author-email: liao961120@gmail.com
 License: UNKNOWN
 Description: Nutritional value calculation for recipes and ingredients
         =========================================================
```

### Comparing `nutrical-0.0.6/setup.py` & `nutrical-0.0.9/setup.py`

 * *Files identical despite different names*

