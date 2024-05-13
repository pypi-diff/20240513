# Comparing `tmp/core_module_chemical_composition_simple_app-2.8.0.tar.gz` & `tmp/core_module_chemical_composition_simple_app-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_module_chemical_composition_simple_app-2.8.0.tar", last modified: Tue Mar 12 19:04:24 2024, max compression
+gzip compressed data, was "core_module_chemical_composition_simple_app-2.9.0.tar", last modified: Mon May 13 16:09:28 2024, max compression
```

## Comparing `core_module_chemical_composition_simple_app-2.8.0.tar` & `core_module_chemical_composition_simple_app-2.9.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:24.428020 core_module_chemical_composition_simple_app-2.8.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2024-03-12 19:04:22.000000 core_module_chemical_composition_simple_app-2.8.0/LICENSE.md
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      189 2024-03-12 19:04:22.000000 core_module_chemical_composition_simple_app-2.8.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1277 2024-03-12 19:04:24.421557 core_module_chemical_composition_simple_app-2.8.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      736 2024-03-12 19:04:22.000000 core_module_chemical_composition_simple_app-2.8.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:24.241113 core_module_chemical_composition_simple_app-2.8.0/core_module_chemical_composition_simple_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:22.000000 core_module_chemical_composition_simple_app-2.8.0/core_module_chemical_composition_simple_app/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:24.066238 core_module_chemical_composition_simple_app-2.8.0/core_module_chemical_composition_simple_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:24.070715 core_module_chemical_composition_simple_app-2.8.0/core_module_chemical_composition_simple_app/static/core_module_chemical_composition_simple_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:24.350532 core_module_chemical_composition_simple_app-2.8.0/core_module_chemical_composition_simple_app/static/core_module_chemical_composition_simple_app/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1374 2024-03-12 19:04:22.000000 core_module_chemical_composition_simple_app-2.8.0/core_module_chemical_composition_simple_app/static/core_module_chemical_composition_simple_app/js/chemical_element_composition_simple.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      392 2024-03-12 19:04:22.000000 core_module_chemical_composition_simple_app-2.8.0/core_module_chemical_composition_simple_app/urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3023 2024-03-12 19:04:22.000000 core_module_chemical_composition_simple_app-2.8.0/core_module_chemical_composition_simple_app/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:24.330824 core_module_chemical_composition_simple_app-2.8.0/core_module_chemical_composition_simple_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1277 2024-03-12 19:04:23.000000 core_module_chemical_composition_simple_app-2.8.0/core_module_chemical_composition_simple_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      747 2024-03-12 19:04:23.000000 core_module_chemical_composition_simple_app-2.8.0/core_module_chemical_composition_simple_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2024-03-12 19:04:23.000000 core_module_chemical_composition_simple_app-2.8.0/core_module_chemical_composition_simple_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        7 2024-03-12 19:04:23.000000 core_module_chemical_composition_simple_app-2.8.0/core_module_chemical_composition_simple_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       50 2024-03-12 19:04:23.000000 core_module_chemical_composition_simple_app-2.8.0/core_module_chemical_composition_simple_app.egg-info/top_level.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2024-03-12 19:04:22.000000 core_module_chemical_composition_simple_app-2.8.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        7 2024-03-12 19:04:22.000000 core_module_chemical_composition_simple_app-2.8.0/requirements.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2024-03-12 19:04:24.430586 core_module_chemical_composition_simple_app-2.8.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      990 2024-03-12 19:04:22.000000 core_module_chemical_composition_simple_app-2.8.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:24.388329 core_module_chemical_composition_simple_app-2.8.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:22.000000 core_module_chemical_composition_simple_app-2.8.0/tests/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      120 2024-03-12 19:04:22.000000 core_module_chemical_composition_simple_app-2.8.0/tests/test_settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:28.956942 core_module_chemical_composition_simple_app-2.9.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2024-05-13 16:09:26.000000 core_module_chemical_composition_simple_app-2.9.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      189 2024-05-13 16:09:26.000000 core_module_chemical_composition_simple_app-2.9.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1277 2024-05-13 16:09:28.950153 core_module_chemical_composition_simple_app-2.9.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      736 2024-05-13 16:09:26.000000 core_module_chemical_composition_simple_app-2.9.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:28.739640 core_module_chemical_composition_simple_app-2.9.0/core_module_chemical_composition_simple_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:26.000000 core_module_chemical_composition_simple_app-2.9.0/core_module_chemical_composition_simple_app/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:28.555398 core_module_chemical_composition_simple_app-2.9.0/core_module_chemical_composition_simple_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:28.569517 core_module_chemical_composition_simple_app-2.9.0/core_module_chemical_composition_simple_app/static/core_module_chemical_composition_simple_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:28.894956 core_module_chemical_composition_simple_app-2.9.0/core_module_chemical_composition_simple_app/static/core_module_chemical_composition_simple_app/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1374 2024-05-13 16:09:26.000000 core_module_chemical_composition_simple_app-2.9.0/core_module_chemical_composition_simple_app/static/core_module_chemical_composition_simple_app/js/chemical_element_composition_simple.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      392 2024-05-13 16:09:26.000000 core_module_chemical_composition_simple_app-2.9.0/core_module_chemical_composition_simple_app/urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3023 2024-05-13 16:09:26.000000 core_module_chemical_composition_simple_app-2.9.0/core_module_chemical_composition_simple_app/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:28.874588 core_module_chemical_composition_simple_app-2.9.0/core_module_chemical_composition_simple_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1277 2024-05-13 16:09:28.000000 core_module_chemical_composition_simple_app-2.9.0/core_module_chemical_composition_simple_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      747 2024-05-13 16:09:28.000000 core_module_chemical_composition_simple_app-2.9.0/core_module_chemical_composition_simple_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2024-05-13 16:09:28.000000 core_module_chemical_composition_simple_app-2.9.0/core_module_chemical_composition_simple_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        7 2024-05-13 16:09:28.000000 core_module_chemical_composition_simple_app-2.9.0/core_module_chemical_composition_simple_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       50 2024-05-13 16:09:28.000000 core_module_chemical_composition_simple_app-2.9.0/core_module_chemical_composition_simple_app.egg-info/top_level.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2024-05-13 16:09:26.000000 core_module_chemical_composition_simple_app-2.9.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        7 2024-05-13 16:09:26.000000 core_module_chemical_composition_simple_app-2.9.0/requirements.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2024-05-13 16:09:28.959511 core_module_chemical_composition_simple_app-2.9.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      990 2024-05-13 16:09:26.000000 core_module_chemical_composition_simple_app-2.9.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:28.929765 core_module_chemical_composition_simple_app-2.9.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:26.000000 core_module_chemical_composition_simple_app-2.9.0/tests/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      120 2024-05-13 16:09:26.000000 core_module_chemical_composition_simple_app-2.9.0/tests/test_settings.py
```

### Comparing `core_module_chemical_composition_simple_app-2.8.0/LICENSE.md` & `core_module_chemical_composition_simple_app-2.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `core_module_chemical_composition_simple_app-2.8.0/PKG-INFO` & `core_module_chemical_composition_simple_app-2.9.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_module_chemical_composition_simple_app
-Version: 2.8.0
+Version: 2.9.0
 Summary: Chemical composition simple module for the parser core project
 Home-page: https://github.com/usnistgov/core_module_chemical_composition_simple_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: core_module_chemical_composition_simple_app
         ===========================================
```

### Comparing `core_module_chemical_composition_simple_app-2.8.0/README.rst` & `core_module_chemical_composition_simple_app-2.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_module_chemical_composition_simple_app-2.8.0/core_module_chemical_composition_simple_app/static/core_module_chemical_composition_simple_app/js/chemical_element_composition_simple.js` & `core_module_chemical_composition_simple_app-2.9.0/core_module_chemical_composition_simple_app/static/core_module_chemical_composition_simple_app/js/chemical_element_composition_simple.js`

 * *Files identical despite different names*

### Comparing `core_module_chemical_composition_simple_app-2.8.0/core_module_chemical_composition_simple_app/views.py` & `core_module_chemical_composition_simple_app-2.9.0/core_module_chemical_composition_simple_app/views.py`

 * *Files identical despite different names*

### Comparing `core_module_chemical_composition_simple_app-2.8.0/core_module_chemical_composition_simple_app.egg-info/PKG-INFO` & `core_module_chemical_composition_simple_app-2.9.0/core_module_chemical_composition_simple_app.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-module-chemical-composition-simple-app
-Version: 2.8.0
+Version: 2.9.0
 Summary: Chemical composition simple module for the parser core project
 Home-page: https://github.com/usnistgov/core_module_chemical_composition_simple_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: core_module_chemical_composition_simple_app
         ===========================================
```

### Comparing `core_module_chemical_composition_simple_app-2.8.0/core_module_chemical_composition_simple_app.egg-info/SOURCES.txt` & `core_module_chemical_composition_simple_app-2.9.0/core_module_chemical_composition_simple_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `core_module_chemical_composition_simple_app-2.8.0/setup.py` & `core_module_chemical_composition_simple_app-2.9.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_module_chemical_composition_simple_app",
-    version="2.8.0",
+    version="2.9.0",
     description="Chemical composition simple module for the parser core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_module_chemical_composition_simple_app",
     packages=find_packages(),
     include_package_data=True,
```

