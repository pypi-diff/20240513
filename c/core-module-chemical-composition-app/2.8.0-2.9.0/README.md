# Comparing `tmp/core_module_chemical_composition_app-2.8.0.tar.gz` & `tmp/core_module_chemical_composition_app-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_module_chemical_composition_app-2.8.0.tar", last modified: Tue Mar 12 19:04:13 2024, max compression
+gzip compressed data, was "core_module_chemical_composition_app-2.9.0.tar", last modified: Mon May 13 16:09:20 2024, max compression
```

## Comparing `core_module_chemical_composition_app-2.8.0.tar` & `core_module_chemical_composition_app-2.9.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:13.483865 core_module_chemical_composition_app-2.8.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2024-03-12 19:04:11.000000 core_module_chemical_composition_app-2.8.0/LICENSE.md
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      175 2024-03-12 19:04:11.000000 core_module_chemical_composition_app-2.8.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1184 2024-03-12 19:04:13.476760 core_module_chemical_composition_app-2.8.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      672 2024-03-12 19:04:11.000000 core_module_chemical_composition_app-2.8.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:13.207601 core_module_chemical_composition_app-2.8.0/core_module_chemical_composition_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:11.000000 core_module_chemical_composition_app-2.8.0/core_module_chemical_composition_app/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3537 2024-03-12 19:04:11.000000 core_module_chemical_composition_app-2.8.0/core_module_chemical_composition_app/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      435 2024-03-12 19:04:11.000000 core_module_chemical_composition_app-2.8.0/core_module_chemical_composition_app/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:12.968807 core_module_chemical_composition_app-2.8.0/core_module_chemical_composition_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:12.979961 core_module_chemical_composition_app-2.8.0/core_module_chemical_composition_app/static/core_module_chemical_composition_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:13.327217 core_module_chemical_composition_app-2.8.0/core_module_chemical_composition_app/static/core_module_chemical_composition_app/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      372 2024-03-12 19:04:11.000000 core_module_chemical_composition_app-2.8.0/core_module_chemical_composition_app/static/core_module_chemical_composition_app/css/chemical_element_composition.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:13.372071 core_module_chemical_composition_app-2.8.0/core_module_chemical_composition_app/static/core_module_chemical_composition_app/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1492 2024-03-12 19:04:11.000000 core_module_chemical_composition_app-2.8.0/core_module_chemical_composition_app/static/core_module_chemical_composition_app/js/chemical_element_composition.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1389 2024-03-12 19:04:11.000000 core_module_chemical_composition_app-2.8.0/core_module_chemical_composition_app/static/core_module_chemical_composition_app/js/events.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:12.992962 core_module_chemical_composition_app-2.8.0/core_module_chemical_composition_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:13.424714 core_module_chemical_composition_app-2.8.0/core_module_chemical_composition_app/templates/core_module_chemical_composition_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      113 2024-03-12 19:04:11.000000 core_module_chemical_composition_app-2.8.0/core_module_chemical_composition_app/templates/core_module_chemical_composition_app/chemical_composition.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2061 2024-03-12 19:04:11.000000 core_module_chemical_composition_app-2.8.0/core_module_chemical_composition_app/templates/core_module_chemical_composition_app/edit_data.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      832 2024-03-12 19:04:11.000000 core_module_chemical_composition_app-2.8.0/core_module_chemical_composition_app/templates/core_module_chemical_composition_app/render_data.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      352 2024-03-12 19:04:11.000000 core_module_chemical_composition_app-2.8.0/core_module_chemical_composition_app/urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4217 2024-03-12 19:04:11.000000 core_module_chemical_composition_app-2.8.0/core_module_chemical_composition_app/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:13.306109 core_module_chemical_composition_app-2.8.0/core_module_chemical_composition_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1184 2024-03-12 19:04:12.000000 core_module_chemical_composition_app-2.8.0/core_module_chemical_composition_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1285 2024-03-12 19:04:12.000000 core_module_chemical_composition_app-2.8.0/core_module_chemical_composition_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2024-03-12 19:04:12.000000 core_module_chemical_composition_app-2.8.0/core_module_chemical_composition_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        7 2024-03-12 19:04:12.000000 core_module_chemical_composition_app-2.8.0/core_module_chemical_composition_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       43 2024-03-12 19:04:12.000000 core_module_chemical_composition_app-2.8.0/core_module_chemical_composition_app.egg-info/top_level.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2024-03-12 19:04:11.000000 core_module_chemical_composition_app-2.8.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        7 2024-03-12 19:04:11.000000 core_module_chemical_composition_app-2.8.0/requirements.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2024-03-12 19:04:13.486718 core_module_chemical_composition_app-2.8.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      960 2024-03-12 19:04:11.000000 core_module_chemical_composition_app-2.8.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:13.462175 core_module_chemical_composition_app-2.8.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:11.000000 core_module_chemical_composition_app-2.8.0/tests/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      120 2024-03-12 19:04:11.000000 core_module_chemical_composition_app-2.8.0/tests/test_settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:20.751911 core_module_chemical_composition_app-2.9.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2024-05-13 16:09:18.000000 core_module_chemical_composition_app-2.9.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      175 2024-05-13 16:09:18.000000 core_module_chemical_composition_app-2.9.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1184 2024-05-13 16:09:20.745535 core_module_chemical_composition_app-2.9.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      672 2024-05-13 16:09:18.000000 core_module_chemical_composition_app-2.9.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:20.475889 core_module_chemical_composition_app-2.9.0/core_module_chemical_composition_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:18.000000 core_module_chemical_composition_app-2.9.0/core_module_chemical_composition_app/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3537 2024-05-13 16:09:18.000000 core_module_chemical_composition_app-2.9.0/core_module_chemical_composition_app/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      435 2024-05-13 16:09:18.000000 core_module_chemical_composition_app-2.9.0/core_module_chemical_composition_app/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:20.240765 core_module_chemical_composition_app-2.9.0/core_module_chemical_composition_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:20.259987 core_module_chemical_composition_app-2.9.0/core_module_chemical_composition_app/static/core_module_chemical_composition_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:20.600343 core_module_chemical_composition_app-2.9.0/core_module_chemical_composition_app/static/core_module_chemical_composition_app/css/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      372 2024-05-13 16:09:18.000000 core_module_chemical_composition_app-2.9.0/core_module_chemical_composition_app/static/core_module_chemical_composition_app/css/chemical_element_composition.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:20.639163 core_module_chemical_composition_app-2.9.0/core_module_chemical_composition_app/static/core_module_chemical_composition_app/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1492 2024-05-13 16:09:18.000000 core_module_chemical_composition_app-2.9.0/core_module_chemical_composition_app/static/core_module_chemical_composition_app/js/chemical_element_composition.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1389 2024-05-13 16:09:18.000000 core_module_chemical_composition_app-2.9.0/core_module_chemical_composition_app/static/core_module_chemical_composition_app/js/events.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:20.273477 core_module_chemical_composition_app-2.9.0/core_module_chemical_composition_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:20.687861 core_module_chemical_composition_app-2.9.0/core_module_chemical_composition_app/templates/core_module_chemical_composition_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      113 2024-05-13 16:09:18.000000 core_module_chemical_composition_app-2.9.0/core_module_chemical_composition_app/templates/core_module_chemical_composition_app/chemical_composition.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2061 2024-05-13 16:09:18.000000 core_module_chemical_composition_app-2.9.0/core_module_chemical_composition_app/templates/core_module_chemical_composition_app/edit_data.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      832 2024-05-13 16:09:18.000000 core_module_chemical_composition_app-2.9.0/core_module_chemical_composition_app/templates/core_module_chemical_composition_app/render_data.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      352 2024-05-13 16:09:18.000000 core_module_chemical_composition_app-2.9.0/core_module_chemical_composition_app/urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4217 2024-05-13 16:09:18.000000 core_module_chemical_composition_app-2.9.0/core_module_chemical_composition_app/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:20.578744 core_module_chemical_composition_app-2.9.0/core_module_chemical_composition_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1184 2024-05-13 16:09:19.000000 core_module_chemical_composition_app-2.9.0/core_module_chemical_composition_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1285 2024-05-13 16:09:20.000000 core_module_chemical_composition_app-2.9.0/core_module_chemical_composition_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2024-05-13 16:09:19.000000 core_module_chemical_composition_app-2.9.0/core_module_chemical_composition_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        7 2024-05-13 16:09:19.000000 core_module_chemical_composition_app-2.9.0/core_module_chemical_composition_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       43 2024-05-13 16:09:19.000000 core_module_chemical_composition_app-2.9.0/core_module_chemical_composition_app.egg-info/top_level.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2024-05-13 16:09:18.000000 core_module_chemical_composition_app-2.9.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        7 2024-05-13 16:09:18.000000 core_module_chemical_composition_app-2.9.0/requirements.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2024-05-13 16:09:20.754302 core_module_chemical_composition_app-2.9.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      960 2024-05-13 16:09:18.000000 core_module_chemical_composition_app-2.9.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:20.722716 core_module_chemical_composition_app-2.9.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:18.000000 core_module_chemical_composition_app-2.9.0/tests/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      120 2024-05-13 16:09:18.000000 core_module_chemical_composition_app-2.9.0/tests/test_settings.py
```

### Comparing `core_module_chemical_composition_app-2.8.0/LICENSE.md` & `core_module_chemical_composition_app-2.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `core_module_chemical_composition_app-2.8.0/PKG-INFO` & `core_module_chemical_composition_app-2.9.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_module_chemical_composition_app
-Version: 2.8.0
+Version: 2.9.0
 Summary: Chemical composition module for the parser core project
 Home-page: https://github.com/usnistgov/core_module_chemical_composition_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: core_module_chemical_composition_app
         ====================================
```

### Comparing `core_module_chemical_composition_app-2.8.0/README.rst` & `core_module_chemical_composition_app-2.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_module_chemical_composition_app-2.8.0/core_module_chemical_composition_app/api.py` & `core_module_chemical_composition_app-2.9.0/core_module_chemical_composition_app/api.py`

 * *Files identical despite different names*

### Comparing `core_module_chemical_composition_app-2.8.0/core_module_chemical_composition_app/static/core_module_chemical_composition_app/js/chemical_element_composition.js` & `core_module_chemical_composition_app-2.9.0/core_module_chemical_composition_app/static/core_module_chemical_composition_app/js/chemical_element_composition.js`

 * *Files identical despite different names*

### Comparing `core_module_chemical_composition_app-2.8.0/core_module_chemical_composition_app/static/core_module_chemical_composition_app/js/events.js` & `core_module_chemical_composition_app-2.9.0/core_module_chemical_composition_app/static/core_module_chemical_composition_app/js/events.js`

 * *Files identical despite different names*

### Comparing `core_module_chemical_composition_app-2.8.0/core_module_chemical_composition_app/templates/core_module_chemical_composition_app/edit_data.html` & `core_module_chemical_composition_app-2.9.0/core_module_chemical_composition_app/templates/core_module_chemical_composition_app/edit_data.html`

 * *Files identical despite different names*

### Comparing `core_module_chemical_composition_app-2.8.0/core_module_chemical_composition_app/templates/core_module_chemical_composition_app/render_data.html` & `core_module_chemical_composition_app-2.9.0/core_module_chemical_composition_app/templates/core_module_chemical_composition_app/render_data.html`

 * *Files identical despite different names*

### Comparing `core_module_chemical_composition_app-2.8.0/core_module_chemical_composition_app/views.py` & `core_module_chemical_composition_app-2.9.0/core_module_chemical_composition_app/views.py`

 * *Files identical despite different names*

### Comparing `core_module_chemical_composition_app-2.8.0/core_module_chemical_composition_app.egg-info/PKG-INFO` & `core_module_chemical_composition_app-2.9.0/core_module_chemical_composition_app.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-module-chemical-composition-app
-Version: 2.8.0
+Version: 2.9.0
 Summary: Chemical composition module for the parser core project
 Home-page: https://github.com/usnistgov/core_module_chemical_composition_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: core_module_chemical_composition_app
         ====================================
```

### Comparing `core_module_chemical_composition_app-2.8.0/core_module_chemical_composition_app.egg-info/SOURCES.txt` & `core_module_chemical_composition_app-2.9.0/core_module_chemical_composition_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `core_module_chemical_composition_app-2.8.0/setup.py` & `core_module_chemical_composition_app-2.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_module_chemical_composition_app",
-    version="2.8.0",
+    version="2.9.0",
     description="Chemical composition module for the parser core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_module_chemical_composition_app",
     packages=find_packages(),
     include_package_data=True,
```

