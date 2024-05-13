# Comparing `tmp/pandas_geojson-2.2.0.tar.gz` & `tmp/pandas_geojson-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandas_geojson-2.2.0.tar", last modified: Wed May  1 06:21:51 2024, max compression
+gzip compressed data, was "pandas_geojson-2.2.1.tar", last modified: Mon May 13 15:52:06 2024, max compression
```

## Comparing `pandas_geojson-2.2.0.tar` & `pandas_geojson-2.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 06:21:51.087011 pandas_geojson-2.2.0/
--rw-rw-rw-   0        0        0     1097 2024-03-18 19:56:01.000000 pandas_geojson-2.2.0/LICENSE
--rw-rw-rw-   0        0        0    16534 2024-05-01 06:21:51.083990 pandas_geojson-2.2.0/PKG-INFO
--rw-rw-rw-   0        0        0    16124 2024-05-01 06:11:36.000000 pandas_geojson-2.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-01 06:21:51.053930 pandas_geojson-2.2.0/pandas_geojson/
--rw-rw-rw-   0        0        0      491 2024-05-01 06:11:36.000000 pandas_geojson-2.2.0/pandas_geojson/__init__.py
--rw-rw-rw-   0        0        0    10815 2024-05-01 06:11:36.000000 pandas_geojson-2.2.0/pandas_geojson/core.py
--rw-rw-rw-   0        0        0     1333 2024-05-01 06:12:26.000000 pandas_geojson-2.2.0/pandas_geojson/io.py
-drwxrwxrwx   0        0        0        0 2024-05-01 06:21:51.082481 pandas_geojson-2.2.0/pandas_geojson.egg-info/
--rw-rw-rw-   0        0        0    16534 2024-05-01 06:21:51.000000 pandas_geojson-2.2.0/pandas_geojson.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2024-05-01 06:21:51.000000 pandas_geojson-2.2.0/pandas_geojson.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 06:21:51.000000 pandas_geojson-2.2.0/pandas_geojson.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-05-01 06:21:51.000000 pandas_geojson-2.2.0/pandas_geojson.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-01 06:21:51.088014 pandas_geojson-2.2.0/setup.cfg
--rw-rw-rw-   0        0        0      815 2024-05-01 06:11:36.000000 pandas_geojson-2.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 15:52:06.480268 pandas_geojson-2.2.1/
+-rw-rw-rw-   0        0        0     1097 2024-05-13 15:39:26.000000 pandas_geojson-2.2.1/LICENSE
+-rw-rw-rw-   0        0        0    16477 2024-05-13 15:52:06.479267 pandas_geojson-2.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0    16082 2024-05-13 15:51:58.000000 pandas_geojson-2.2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 15:52:06.457310 pandas_geojson-2.2.1/pandas_geojson/
+-rw-rw-rw-   0        0        0      491 2024-05-13 15:41:25.000000 pandas_geojson-2.2.1/pandas_geojson/__init__.py
+-rw-rw-rw-   0        0        0    10815 2024-05-13 15:39:26.000000 pandas_geojson-2.2.1/pandas_geojson/core.py
+-rw-rw-rw-   0        0        0      645 2024-05-13 15:39:26.000000 pandas_geojson-2.2.1/pandas_geojson/io.py
+drwxrwxrwx   0        0        0        0 2024-05-13 15:52:06.476834 pandas_geojson-2.2.1/pandas_geojson.egg-info/
+-rw-rw-rw-   0        0        0    16477 2024-05-13 15:52:06.000000 pandas_geojson-2.2.1/pandas_geojson.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2024-05-13 15:52:06.000000 pandas_geojson-2.2.1/pandas_geojson.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 15:52:06.000000 pandas_geojson-2.2.1/pandas_geojson.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-13 15:52:06.000000 pandas_geojson-2.2.1/pandas_geojson.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 15:52:06.481281 pandas_geojson-2.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      800 2024-05-13 15:41:24.000000 pandas_geojson-2.2.1/setup.py
```

### Comparing `pandas_geojson-2.2.0/LICENSE` & `pandas_geojson-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pandas_geojson-2.2.0/PKG-INFO` & `pandas_geojson-2.2.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: pandas_geojson
-Version: 2.2.0
-Summary: Convert Pandas Dataframe to GeoJSON
-Home-page: https://github.com/jrasband-dev/pandas-geojson
-Author: Jayden Rasband
-Author-email: jayden.rasband@gmail.com
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ![](https://raw.githubusercontent.com/jrasband-dev/pandas-geojson/master/static/pandasgeojson.png)
 
 ---
 ![PyPI - Version](https://img.shields.io/pypi/v/pandas-geojson)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/pandas-geojson)
 ![PyPI - License](https://img.shields.io/pypi/l/pandas-geojson)
 ![Libraries.io SourceRank](https://img.shields.io/librariesio/sourcerank/pypi/pandas-geojson)
@@ -602,16 +589,7 @@
                 }
             }
         ]
     }
 
 
 
-
-```python
-
-```
-
-
-```python
-
-```
```

### Comparing `pandas_geojson-2.2.0/README.md` & `pandas_geojson-2.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: pandas_geojson
+Version: 2.2.1
+Summary: Manage GeoJSON Files
+Home-page: https://github.com/jrasband-dev/pandas-geojson
+Author: Jayden Rasband
+Author-email: jayden.rasband@gmail.com
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ![](https://raw.githubusercontent.com/jrasband-dev/pandas-geojson/master/static/pandasgeojson.png)
 
 ---
 ![PyPI - Version](https://img.shields.io/pypi/v/pandas-geojson)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/pandas-geojson)
 ![PyPI - License](https://img.shields.io/pypi/l/pandas-geojson)
 ![Libraries.io SourceRank](https://img.shields.io/librariesio/sourcerank/pypi/pandas-geojson)
@@ -589,16 +602,7 @@
                 }
             }
         ]
     }
 
 
 
-
-```python
-
-```
-
-
-```python
-
-```
```

### Comparing `pandas_geojson-2.2.0/pandas_geojson/core.py` & `pandas_geojson-2.2.1/pandas_geojson/core.py`

 * *Files identical despite different names*

### Comparing `pandas_geojson-2.2.0/pandas_geojson.egg-info/PKG-INFO` & `pandas_geojson-2.2.1/pandas_geojson.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pandas_geojson
-Version: 2.2.0
-Summary: Convert Pandas Dataframe to GeoJSON
+Version: 2.2.1
+Summary: Manage GeoJSON Files
 Home-page: https://github.com/jrasband-dev/pandas-geojson
 Author: Jayden Rasband
 Author-email: jayden.rasband@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
@@ -602,16 +602,7 @@
                 }
             }
         ]
     }
 
 
 
-
-```python
-
-```
-
-
-```python
-
-```
```

### Comparing `pandas_geojson-2.2.0/setup.py` & `pandas_geojson-2.2.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="pandas_geojson",
-    version="2.2.0",
-    description="Convert Pandas Dataframe to GeoJSON",
+    version="2.2.1",
+    description="Manage GeoJSON Files",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/jrasband-dev/pandas-geojson",
     author="Jayden Rasband",
     author_email="jayden.rasband@gmail.com",
     license="MIT",
     classifiers=[
```

