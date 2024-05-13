# Comparing `tmp/molcompview-0.1.1.tar.gz` & `tmp/molcompview-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molcompview-0.1.1.tar", last modified: Fri May 10 21:29:56 2024, max compression
+gzip compressed data, was "molcompview-0.1.5.tar", last modified: Mon May 13 08:37:32 2024, max compression
```

## Comparing `molcompview-0.1.1.tar` & `molcompview-0.1.5.tar`

### file list

```diff
@@ -1,19 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:29:56.595163 molcompview-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-10 21:29:47.000000 molcompview-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-05-10 21:29:56.595163 molcompview-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-05-10 21:29:47.000000 molcompview-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:29:56.591163 molcompview-0.1.1/molcompview/
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-10 21:29:47.000000 molcompview-0.1.1/molcompview/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12165 2024-05-10 21:29:47.000000 molcompview-0.1.1/molcompview/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-05-10 21:29:47.000000 molcompview-0.1.1/molcompview/components.py
--rw-r--r--   0 runner    (1001) docker     (127)     6066 2024-05-10 21:29:47.000000 molcompview-0.1.1/molcompview/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7699 2024-05-10 21:29:47.000000 molcompview-0.1.1/molcompview/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:29:56.595163 molcompview-0.1.1/molcompview.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-05-10 21:29:56.000000 molcompview-0.1.1/molcompview.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-10 21:29:56.000000 molcompview-0.1.1/molcompview.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 21:29:56.000000 molcompview-0.1.1/molcompview.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-10 21:29:56.000000 molcompview-0.1.1/molcompview.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-10 21:29:56.000000 molcompview-0.1.1/molcompview.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-10 21:29:56.000000 molcompview-0.1.1/molcompview.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 21:29:56.595163 molcompview-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-10 21:29:47.000000 molcompview-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:37:32.793287 molcompview-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-13 08:37:28.000000 molcompview-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-05-13 08:37:32.793287 molcompview-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-05-13 08:37:28.000000 molcompview-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:37:32.789287 molcompview-0.1.5/molcompview/
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-13 08:37:28.000000 molcompview-0.1.5/molcompview/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12165 2024-05-13 08:37:28.000000 molcompview-0.1.5/molcompview/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-05-13 08:37:28.000000 molcompview-0.1.5/molcompview/components.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:37:32.789287 molcompview-0.1.5/molcompview/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:37:32.793287 molcompview-0.1.5/molcompview/data/endocrine-receptor/
+-rw-r--r--   0 runner    (1001) docker     (127)    64156 2024-05-13 08:37:28.000000 molcompview-0.1.5/molcompview/data/endocrine-receptor/endocrine.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     6066 2024-05-13 08:37:28.000000 molcompview-0.1.5/molcompview/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7699 2024-05-13 08:37:28.000000 molcompview-0.1.5/molcompview/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:37:32.793287 molcompview-0.1.5/molcompview.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-05-13 08:37:32.000000 molcompview-0.1.5/molcompview.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-13 08:37:32.000000 molcompview-0.1.5/molcompview.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 08:37:32.000000 molcompview-0.1.5/molcompview.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-13 08:37:32.000000 molcompview-0.1.5/molcompview.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 08:37:32.000000 molcompview-0.1.5/molcompview.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-13 08:37:32.000000 molcompview-0.1.5/molcompview.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-13 08:37:32.000000 molcompview-0.1.5/molcompview.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 08:37:32.793287 molcompview-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-13 08:37:28.000000 molcompview-0.1.5/setup.py
```

### Comparing `molcompview-0.1.1/LICENSE` & `molcompview-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `molcompview-0.1.1/PKG-INFO` & `molcompview-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molcompview
-Version: 0.1.1
+Version: 0.1.5
 Summary: MolCompass Visualization Tool: Visualize your Chemical Space
 Home-page: https://github.com/sergsb/molcompview
 Author: Sergey Sosnin
 Author-email: sergey.sosnin@univie.ac.at
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `molcompview-0.1.1/README.md` & `molcompview-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `molcompview-0.1.1/molcompview/actions.py` & `molcompview-0.1.5/molcompview/actions.py`

 * *Files identical despite different names*

### Comparing `molcompview-0.1.1/molcompview/components.py` & `molcompview-0.1.5/molcompview/components.py`

 * *Files identical despite different names*

### Comparing `molcompview-0.1.1/molcompview/functions.py` & `molcompview-0.1.5/molcompview/functions.py`

 * *Files identical despite different names*

### Comparing `molcompview-0.1.1/molcompview/main.py` & `molcompview-0.1.5/molcompview/main.py`

 * *Files identical despite different names*

### Comparing `molcompview-0.1.1/molcompview.egg-info/PKG-INFO` & `molcompview-0.1.5/molcompview.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molcompview
-Version: 0.1.1
+Version: 0.1.5
 Summary: MolCompass Visualization Tool: Visualize your Chemical Space
 Home-page: https://github.com/sergsb/molcompview
 Author: Sergey Sosnin
 Author-email: sergey.sosnin@univie.ac.at
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `molcompview-0.1.1/setup.py` & `molcompview-0.1.5/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 from setuptools import setup,find_packages
 
 setup(
     python_requires='>=3.6',  # Your supported Python ranges
     name = "molcompview",
-    version = "0.1.1",
-    include_package_data=False,
-    packages=find_packages(),
-    install_requires=[
+    version = "0.1.5",
+    include_package_data=True,
+    package_data={
+      'molcompview': ['data/endocrine-receptor/*'],
+   },
+   zip_safe=False, 
+   packages=find_packages(),
+   install_requires=[
         'molcomplib',
         'rdkit',
         'appdata',  
         'numpy',
         'pandas',
         'scipy',
         'scikit-learn',
```

