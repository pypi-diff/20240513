# Comparing `tmp/TSCC-0.0.2.tar.gz` & `tmp/tscc-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TSCC-0.0.2.tar", last modified: Fri Mar 22 15:10:10 2024, max compression
+gzip compressed data, was "tscc-0.0.3.tar", last modified: Mon May 13 12:11:29 2024, max compression
```

## Comparing `TSCC-0.0.2.tar` & `tscc-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-03-22 15:10:10.558850 TSCC-0.0.2/
--rw-rw-rw-   0        0        0     1091 2024-01-24 11:16:11.000000 TSCC-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      802 2024-03-22 15:10:10.558850 TSCC-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      174 2024-01-24 11:15:13.000000 TSCC-0.0.2/README.md
--rw-rw-rw-   0        0        0      610 2024-03-22 15:09:46.000000 TSCC-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-22 15:10:10.558850 TSCC-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-22 15:10:10.546365 TSCC-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2024-03-22 15:10:10.553220 TSCC-0.0.2/src/TSCC/
--rw-rw-rw-   0        0        0        0 2024-01-24 11:10:49.000000 TSCC-0.0.2/src/TSCC/__init__.py
--rw-rw-rw-   0        0        0       43 2024-01-24 11:11:30.000000 TSCC-0.0.2/src/TSCC/example.py
-drwxrwxrwx   0        0        0        0 2024-03-22 15:10:10.558850 TSCC-0.0.2/src/TSCC.egg-info/
--rw-rw-rw-   0        0        0      802 2024-03-22 15:10:10.000000 TSCC-0.0.2/src/TSCC.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      201 2024-03-22 15:10:10.000000 TSCC-0.0.2/src/TSCC.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-22 15:10:10.000000 TSCC-0.0.2/src/TSCC.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-03-22 15:10:10.000000 TSCC-0.0.2/src/TSCC.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-13 12:11:29.753092 tscc-0.0.3/
+-rw-rw-rw-   0        0        0     1091 2024-01-24 11:16:11.000000 tscc-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      784 2024-05-13 12:11:29.751875 tscc-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      332 2024-05-13 12:08:52.000000 tscc-0.0.3/README.md
+-rw-rw-rw-   0        0        0      475 2024-05-13 12:10:02.000000 tscc-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-13 12:11:29.753595 tscc-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-13 12:11:29.733821 tscc-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2024-05-13 12:11:29.745457 tscc-0.0.3/src/TSCC/
+-rw-rw-rw-   0        0        0        0 2024-01-24 11:10:49.000000 tscc-0.0.3/src/TSCC/__init__.py
+-rw-rw-rw-   0        0        0       43 2024-01-24 11:11:30.000000 tscc-0.0.3/src/TSCC/example.py
+drwxrwxrwx   0        0        0        0 2024-05-13 12:11:29.751875 tscc-0.0.3/src/TSCC.egg-info/
+-rw-rw-rw-   0        0        0      784 2024-05-13 12:11:29.000000 tscc-0.0.3/src/TSCC.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      201 2024-05-13 12:11:29.000000 tscc-0.0.3/src/TSCC.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 12:11:29.000000 tscc-0.0.3/src/TSCC.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-13 12:11:29.000000 tscc-0.0.3/src/TSCC.egg-info/top_level.txt
```

### Comparing `TSCC-0.0.2/LICENSE` & `tscc-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `TSCC-0.0.2/PKG-INFO` & `tscc-0.0.3/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: TSCC
-Version: 0.0.2
-Summary: Our python package 'Time Series check & correct' can be used to enhance data quality for sensor data in the water field. The release will be in Q3 2024 or earlier.
+Version: 0.0.3
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/pypa/TSCC
 Project-URL: Issues, https://github.com/pypa/TSCC/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Example Package
+# Time Series check & correct
+
+Our python package 'Time Series check & correct' can be used to enhance data quality
+for sensor data in the water field. The release will be in Q3 2024 or earlier and the package was developed
+by the Institute for Hydraulic Engineering and Water Management at the University of Duisburg-Essen.
 
-This is a simple example package. You can use
-[GitHub-flavored Markdown](https://guides.github.com/features/mastering-markdown/)
-to write your content.
```

### Comparing `TSCC-0.0.2/src/TSCC.egg-info/PKG-INFO` & `tscc-0.0.3/src/TSCC.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: TSCC
-Version: 0.0.2
-Summary: Our python package 'Time Series check & correct' can be used to enhance data quality for sensor data in the water field. The release will be in Q3 2024 or earlier.
+Version: 0.0.3
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/pypa/TSCC
 Project-URL: Issues, https://github.com/pypa/TSCC/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Example Package
+# Time Series check & correct
+
+Our python package 'Time Series check & correct' can be used to enhance data quality
+for sensor data in the water field. The release will be in Q3 2024 or earlier and the package was developed
+by the Institute for Hydraulic Engineering and Water Management at the University of Duisburg-Essen.
 
-This is a simple example package. You can use
-[GitHub-flavored Markdown](https://guides.github.com/features/mastering-markdown/)
-to write your content.
```

