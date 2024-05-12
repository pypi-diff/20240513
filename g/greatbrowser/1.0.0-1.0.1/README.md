# Comparing `tmp/greatbrowser-1.0.0.tar.gz` & `tmp/greatbrowser-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "greatbrowser-1.0.0.tar", last modified: Sun May 12 21:20:46 2024, max compression
+gzip compressed data, was "greatbrowser-1.0.1.tar", last modified: Sun May 12 23:57:30 2024, max compression
```

## Comparing `greatbrowser-1.0.0.tar` & `greatbrowser-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 21:20:46.392625 greatbrowser-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-12 21:20:30.000000 greatbrowser-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-12 21:20:46.392625 greatbrowser-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-12 21:20:30.000000 greatbrowser-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 21:20:46.392625 greatbrowser-1.0.0/greatbrowser/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-12 21:20:30.000000 greatbrowser-1.0.0/greatbrowser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16720 2024-05-12 21:20:30.000000 greatbrowser-1.0.0/greatbrowser/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    13204 2024-05-12 21:20:30.000000 greatbrowser-1.0.0/greatbrowser/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 21:20:46.392625 greatbrowser-1.0.0/greatbrowser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-12 21:20:46.000000 greatbrowser-1.0.0/greatbrowser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-12 21:20:46.000000 greatbrowser-1.0.0/greatbrowser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 21:20:46.000000 greatbrowser-1.0.0/greatbrowser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-12 21:20:46.000000 greatbrowser-1.0.0/greatbrowser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-12 21:20:46.000000 greatbrowser-1.0.0/greatbrowser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 21:20:46.392625 greatbrowser-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-12 21:20:30.000000 greatbrowser-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 23:57:30.073462 greatbrowser-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-12 23:57:17.000000 greatbrowser-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-05-12 23:57:30.073462 greatbrowser-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-05-12 23:57:17.000000 greatbrowser-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 23:57:30.073462 greatbrowser-1.0.1/greatbrowser/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-12 23:57:17.000000 greatbrowser-1.0.1/greatbrowser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16720 2024-05-12 23:57:17.000000 greatbrowser-1.0.1/greatbrowser/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13204 2024-05-12 23:57:17.000000 greatbrowser-1.0.1/greatbrowser/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 23:57:30.073462 greatbrowser-1.0.1/greatbrowser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-05-12 23:57:30.000000 greatbrowser-1.0.1/greatbrowser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-12 23:57:30.000000 greatbrowser-1.0.1/greatbrowser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 23:57:30.000000 greatbrowser-1.0.1/greatbrowser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-12 23:57:30.000000 greatbrowser-1.0.1/greatbrowser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-12 23:57:30.000000 greatbrowser-1.0.1/greatbrowser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 23:57:30.073462 greatbrowser-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-12 23:57:17.000000 greatbrowser-1.0.1/setup.py
```

### Comparing `greatbrowser-1.0.0/LICENSE` & `greatbrowser-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `greatbrowser-1.0.0/README.md` & `greatbrowser-1.0.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# greatbrowser v1.0.0
+# greatbrowser v1.0.1
 A selenium implementation in python for Stanford's GREAT browser, allowing for quick and easy genomic analysis.
 
 This repository can be installed as a module
 
 ```
 pip install greatbrowser
 ```
@@ -12,15 +12,15 @@
 ```
 from greatbrowser import great_analysis, great_global_controls, great_get_options
 ```
 
 A guide demonstrating how these functions may be used is available in the "tests" folder (see: "sample_usage")
 
 The user experience is primarily built around a single function, great_analysis(), with the complementary functions great_get_options() and great_global_controls()
-providing context regarding some of the parameters for this function. The "sample_usage" jupyter file  gives some examples of how the parameters may be tuned.
+providing context regarding some of the parameters for this function.
 
 The current version supports the ability to find gene associations using probe sets as well the ability to download any GREAT-generated table or plot in dataframe form. 
 UCSC genome browser implementation is also supported. Customizability is controlled through parameter tuning, some of which are specific, 
 while others are encapsulated within the "global_settings" dictionary parameter as key options. More specific information is available in the great_analysis() docstring. 
 
 This repository is ideal for individuals attempting to conduct many different analyses using GREAT across many different probe sets. 
 It is fully functional with regards to its ability to modify table output settings,
```

### Comparing `greatbrowser-1.0.0/greatbrowser/functions.py` & `greatbrowser-1.0.1/greatbrowser/functions.py`

 * *Files identical despite different names*

### Comparing `greatbrowser-1.0.0/greatbrowser/main.py` & `greatbrowser-1.0.1/greatbrowser/main.py`

 * *Files identical despite different names*

### Comparing `greatbrowser-1.0.0/setup.py` & `greatbrowser-1.0.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
+VERSION = '1.0.1'
 DESCRIPTION = "Automate Stanford's GREAT browser"
-LONG_DESCRIPTION = "A Selenium implementation in Python for Stanford's GREAT browser, allowing for quick and easy genomic analysis."
+
+from pathlib import Path
+this_directory = Path(__file__).parent
+long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="greatbrowser",
     version=VERSION,
     author="Sam Anderson",
     author_email="sanderson01@wesleyan.edu",
     description=DESCRIPTION,
-    long_description=LONG_DESCRIPTION,
+    long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=[
         'selenium',
         'beautifulsoup4',
         'requests',
         'webdriver_manager',
```

