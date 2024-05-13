# Comparing `tmp/core_module_excel_uploader_app-2.8.0.tar.gz` & `tmp/core_module_excel_uploader_app-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_module_excel_uploader_app-2.8.0.tar", last modified: Tue Mar 12 19:04:32 2024, max compression
+gzip compressed data, was "core_module_excel_uploader_app-2.9.0.tar", last modified: Mon May 13 16:09:39 2024, max compression
```

## Comparing `core_module_excel_uploader_app-2.8.0.tar` & `core_module_excel_uploader_app-2.9.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:32.875246 core_module_excel_uploader_app-2.8.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2024-03-12 19:04:30.000000 core_module_excel_uploader_app-2.8.0/LICENSE.md
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      193 2024-03-12 19:04:30.000000 core_module_excel_uploader_app-2.8.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1160 2024-03-12 19:04:32.866923 core_module_excel_uploader_app-2.8.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      666 2024-03-12 19:04:30.000000 core_module_excel_uploader_app-2.8.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:32.538223 core_module_excel_uploader_app-2.8.0/core_module_excel_uploader_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:30.000000 core_module_excel_uploader_app-2.8.0/core_module_excel_uploader_app/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:32.324116 core_module_excel_uploader_app-2.8.0/core_module_excel_uploader_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:32.339767 core_module_excel_uploader_app-2.8.0/core_module_excel_uploader_app/static/core_module_excel_uploader_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:32.656145 core_module_excel_uploader_app-2.8.0/core_module_excel_uploader_app/static/core_module_excel_uploader_app/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      426 2024-03-12 19:04:30.000000 core_module_excel_uploader_app-2.8.0/core_module_excel_uploader_app/static/core_module_excel_uploader_app/css/excel_uploader.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:32.674203 core_module_excel_uploader_app-2.8.0/core_module_excel_uploader_app/static/core_module_excel_uploader_app/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      310 2024-03-12 19:04:30.000000 core_module_excel_uploader_app-2.8.0/core_module_excel_uploader_app/static/core_module_excel_uploader_app/js/excel_uploader.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:32.691885 core_module_excel_uploader_app-2.8.0/core_module_excel_uploader_app/static/core_module_excel_uploader_app/xls/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    25600 2024-03-12 19:04:30.000000 core_module_excel_uploader_app-2.8.0/core_module_excel_uploader_app/static/core_module_excel_uploader_app/xls/data.xls
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:32.350161 core_module_excel_uploader_app-2.8.0/core_module_excel_uploader_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:32.707811 core_module_excel_uploader_app-2.8.0/core_module_excel_uploader_app/templates/core_module_excel_uploader_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      161 2024-03-12 19:04:30.000000 core_module_excel_uploader_app-2.8.0/core_module_excel_uploader_app/templates/core_module_excel_uploader_app/excel_uploader.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      318 2024-03-12 19:04:30.000000 core_module_excel_uploader_app-2.8.0/core_module_excel_uploader_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:32.764263 core_module_excel_uploader_app-2.8.0/core_module_excel_uploader_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:30.000000 core_module_excel_uploader_app-2.8.0/core_module_excel_uploader_app/views/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      178 2024-03-12 19:04:30.000000 core_module_excel_uploader_app-2.8.0/core_module_excel_uploader_app/views/forms.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7537 2024-03-12 19:04:30.000000 core_module_excel_uploader_app-2.8.0/core_module_excel_uploader_app/views/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:32.634653 core_module_excel_uploader_app-2.8.0/core_module_excel_uploader_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1160 2024-03-12 19:04:31.000000 core_module_excel_uploader_app-2.8.0/core_module_excel_uploader_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1071 2024-03-12 19:04:32.000000 core_module_excel_uploader_app-2.8.0/core_module_excel_uploader_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2024-03-12 19:04:31.000000 core_module_excel_uploader_app-2.8.0/core_module_excel_uploader_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       42 2024-03-12 19:04:31.000000 core_module_excel_uploader_app-2.8.0/core_module_excel_uploader_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       37 2024-03-12 19:04:31.000000 core_module_excel_uploader_app-2.8.0/core_module_excel_uploader_app.egg-info/top_level.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2024-03-12 19:04:30.000000 core_module_excel_uploader_app-2.8.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       23 2024-03-12 19:04:30.000000 core_module_excel_uploader_app-2.8.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       19 2024-03-12 19:04:30.000000 core_module_excel_uploader_app-2.8.0/requirements.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2024-03-12 19:04:32.878538 core_module_excel_uploader_app-2.8.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1093 2024-03-12 19:04:30.000000 core_module_excel_uploader_app-2.8.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:32.800212 core_module_excel_uploader_app-2.8.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:30.000000 core_module_excel_uploader_app-2.8.0/tests/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1642 2024-03-12 19:04:30.000000 core_module_excel_uploader_app-2.8.0/tests/test_settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:32.815385 core_module_excel_uploader_app-2.8.0/tests/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:30.000000 core_module_excel_uploader_app-2.8.0/tests/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:32.852248 core_module_excel_uploader_app-2.8.0/tests/views/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:30.000000 core_module_excel_uploader_app-2.8.0/tests/views/views/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1550 2024-03-12 19:04:30.000000 core_module_excel_uploader_app-2.8.0/tests/views/views/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:38.988806 core_module_excel_uploader_app-2.9.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2024-05-13 16:09:36.000000 core_module_excel_uploader_app-2.9.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      193 2024-05-13 16:09:36.000000 core_module_excel_uploader_app-2.9.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1160 2024-05-13 16:09:38.983447 core_module_excel_uploader_app-2.9.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      666 2024-05-13 16:09:36.000000 core_module_excel_uploader_app-2.9.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:38.646863 core_module_excel_uploader_app-2.9.0/core_module_excel_uploader_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:36.000000 core_module_excel_uploader_app-2.9.0/core_module_excel_uploader_app/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:38.428377 core_module_excel_uploader_app-2.9.0/core_module_excel_uploader_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:38.447754 core_module_excel_uploader_app-2.9.0/core_module_excel_uploader_app/static/core_module_excel_uploader_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:38.775190 core_module_excel_uploader_app-2.9.0/core_module_excel_uploader_app/static/core_module_excel_uploader_app/css/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      426 2024-05-13 16:09:36.000000 core_module_excel_uploader_app-2.9.0/core_module_excel_uploader_app/static/core_module_excel_uploader_app/css/excel_uploader.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:38.790806 core_module_excel_uploader_app-2.9.0/core_module_excel_uploader_app/static/core_module_excel_uploader_app/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      310 2024-05-13 16:09:36.000000 core_module_excel_uploader_app-2.9.0/core_module_excel_uploader_app/static/core_module_excel_uploader_app/js/excel_uploader.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:38.806096 core_module_excel_uploader_app-2.9.0/core_module_excel_uploader_app/static/core_module_excel_uploader_app/xls/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    25600 2024-05-13 16:09:36.000000 core_module_excel_uploader_app-2.9.0/core_module_excel_uploader_app/static/core_module_excel_uploader_app/xls/data.xls
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:38.460828 core_module_excel_uploader_app-2.9.0/core_module_excel_uploader_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:38.822700 core_module_excel_uploader_app-2.9.0/core_module_excel_uploader_app/templates/core_module_excel_uploader_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      161 2024-05-13 16:09:36.000000 core_module_excel_uploader_app-2.9.0/core_module_excel_uploader_app/templates/core_module_excel_uploader_app/excel_uploader.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      318 2024-05-13 16:09:36.000000 core_module_excel_uploader_app-2.9.0/core_module_excel_uploader_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:38.872821 core_module_excel_uploader_app-2.9.0/core_module_excel_uploader_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:36.000000 core_module_excel_uploader_app-2.9.0/core_module_excel_uploader_app/views/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      178 2024-05-13 16:09:36.000000 core_module_excel_uploader_app-2.9.0/core_module_excel_uploader_app/views/forms.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7537 2024-05-13 16:09:36.000000 core_module_excel_uploader_app-2.9.0/core_module_excel_uploader_app/views/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:38.754591 core_module_excel_uploader_app-2.9.0/core_module_excel_uploader_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1160 2024-05-13 16:09:38.000000 core_module_excel_uploader_app-2.9.0/core_module_excel_uploader_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1071 2024-05-13 16:09:38.000000 core_module_excel_uploader_app-2.9.0/core_module_excel_uploader_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2024-05-13 16:09:38.000000 core_module_excel_uploader_app-2.9.0/core_module_excel_uploader_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       42 2024-05-13 16:09:38.000000 core_module_excel_uploader_app-2.9.0/core_module_excel_uploader_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       37 2024-05-13 16:09:38.000000 core_module_excel_uploader_app-2.9.0/core_module_excel_uploader_app.egg-info/top_level.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2024-05-13 16:09:36.000000 core_module_excel_uploader_app-2.9.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       23 2024-05-13 16:09:36.000000 core_module_excel_uploader_app-2.9.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       19 2024-05-13 16:09:36.000000 core_module_excel_uploader_app-2.9.0/requirements.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2024-05-13 16:09:38.990991 core_module_excel_uploader_app-2.9.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1093 2024-05-13 16:09:36.000000 core_module_excel_uploader_app-2.9.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:38.913011 core_module_excel_uploader_app-2.9.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:36.000000 core_module_excel_uploader_app-2.9.0/tests/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1642 2024-05-13 16:09:36.000000 core_module_excel_uploader_app-2.9.0/tests/test_settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:38.928789 core_module_excel_uploader_app-2.9.0/tests/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:36.000000 core_module_excel_uploader_app-2.9.0/tests/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:38.971755 core_module_excel_uploader_app-2.9.0/tests/views/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:36.000000 core_module_excel_uploader_app-2.9.0/tests/views/views/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1550 2024-05-13 16:09:36.000000 core_module_excel_uploader_app-2.9.0/tests/views/views/tests_unit.py
```

### Comparing `core_module_excel_uploader_app-2.8.0/LICENSE.md` & `core_module_excel_uploader_app-2.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `core_module_excel_uploader_app-2.8.0/PKG-INFO` & `core_module_excel_uploader_app-2.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_module_excel_uploader_app
-Version: 2.8.0
+Version: 2.9.0
 Summary: Excel Uploader module for the parser core project
 Home-page: https://github.com/usnistgov/core_module_excel_uploader_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: core_module_excel_uploader_app
         ==============================
```

### Comparing `core_module_excel_uploader_app-2.8.0/README.rst` & `core_module_excel_uploader_app-2.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_module_excel_uploader_app-2.8.0/core_module_excel_uploader_app/static/core_module_excel_uploader_app/xls/data.xls` & `core_module_excel_uploader_app-2.9.0/core_module_excel_uploader_app/static/core_module_excel_uploader_app/xls/data.xls`

 * *Files identical despite different names*

### Comparing `core_module_excel_uploader_app-2.8.0/core_module_excel_uploader_app/views/views.py` & `core_module_excel_uploader_app-2.9.0/core_module_excel_uploader_app/views/views.py`

 * *Files identical despite different names*

### Comparing `core_module_excel_uploader_app-2.8.0/core_module_excel_uploader_app.egg-info/PKG-INFO` & `core_module_excel_uploader_app-2.9.0/core_module_excel_uploader_app.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-module-excel-uploader-app
-Version: 2.8.0
+Version: 2.9.0
 Summary: Excel Uploader module for the parser core project
 Home-page: https://github.com/usnistgov/core_module_excel_uploader_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: core_module_excel_uploader_app
         ==============================
```

### Comparing `core_module_excel_uploader_app-2.8.0/core_module_excel_uploader_app.egg-info/SOURCES.txt` & `core_module_excel_uploader_app-2.9.0/core_module_excel_uploader_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `core_module_excel_uploader_app-2.8.0/setup.py` & `core_module_excel_uploader_app-2.9.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_module_excel_uploader_app",
-    version="2.8.0",
+    version="2.9.0",
     description="Excel Uploader module for the parser core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_module_excel_uploader_app",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `core_module_excel_uploader_app-2.8.0/tests/test_settings.py` & `core_module_excel_uploader_app-2.9.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `core_module_excel_uploader_app-2.8.0/tests/views/views/tests_unit.py` & `core_module_excel_uploader_app-2.9.0/tests/views/views/tests_unit.py`

 * *Files identical despite different names*

