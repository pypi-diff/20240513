# Comparing `tmp/core_module_periodic_table_app-2.8.0.tar.gz` & `tmp/core_module_periodic_table_app-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_module_periodic_table_app-2.8.0.tar", last modified: Tue Mar 12 19:04:58 2024, max compression
+gzip compressed data, was "core_module_periodic_table_app-2.9.0.tar", last modified: Mon May 13 16:10:03 2024, max compression
```

## Comparing `core_module_periodic_table_app-2.8.0.tar` & `core_module_periodic_table_app-2.9.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:58.556719 core_module_periodic_table_app-2.8.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2024-03-12 19:04:56.000000 core_module_periodic_table_app-2.8.0/LICENSE.md
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      193 2024-03-12 19:04:56.000000 core_module_periodic_table_app-2.8.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1112 2024-03-12 19:04:58.551417 core_module_periodic_table_app-2.8.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      618 2024-03-12 19:04:56.000000 core_module_periodic_table_app-2.8.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:58.330631 core_module_periodic_table_app-2.8.0/core_module_periodic_table_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:56.000000 core_module_periodic_table_app-2.8.0/core_module_periodic_table_app/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:58.132888 core_module_periodic_table_app-2.8.0/core_module_periodic_table_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:58.143440 core_module_periodic_table_app-2.8.0/core_module_periodic_table_app/static/core_module_periodic_table_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:58.442232 core_module_periodic_table_app-2.8.0/core_module_periodic_table_app/static/core_module_periodic_table_app/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1416 2024-03-12 19:04:56.000000 core_module_periodic_table_app-2.8.0/core_module_periodic_table_app/static/core_module_periodic_table_app/css/periodic.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:58.457756 core_module_periodic_table_app-2.8.0/core_module_periodic_table_app/static/core_module_periodic_table_app/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1075 2024-03-12 19:04:56.000000 core_module_periodic_table_app-2.8.0/core_module_periodic_table_app/static/core_module_periodic_table_app/js/periodic.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:58.156567 core_module_periodic_table_app-2.8.0/core_module_periodic_table_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:58.489974 core_module_periodic_table_app-2.8.0/core_module_periodic_table_app/templates/core_module_periodic_table_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10866 2024-03-12 19:04:56.000000 core_module_periodic_table_app-2.8.0/core_module_periodic_table_app/templates/core_module_periodic_table_app/periodic.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      146 2024-03-12 19:04:56.000000 core_module_periodic_table_app-2.8.0/core_module_periodic_table_app/templates/core_module_periodic_table_app/periodic_simple.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      312 2024-03-12 19:04:56.000000 core_module_periodic_table_app-2.8.0/core_module_periodic_table_app/urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1731 2024-03-12 19:04:56.000000 core_module_periodic_table_app-2.8.0/core_module_periodic_table_app/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:58.422224 core_module_periodic_table_app-2.8.0/core_module_periodic_table_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1112 2024-03-12 19:04:57.000000 core_module_periodic_table_app-2.8.0/core_module_periodic_table_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      902 2024-03-12 19:04:58.000000 core_module_periodic_table_app-2.8.0/core_module_periodic_table_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2024-03-12 19:04:57.000000 core_module_periodic_table_app-2.8.0/core_module_periodic_table_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       30 2024-03-12 19:04:57.000000 core_module_periodic_table_app-2.8.0/core_module_periodic_table_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       37 2024-03-12 19:04:57.000000 core_module_periodic_table_app-2.8.0/core_module_periodic_table_app.egg-info/top_level.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2024-03-12 19:04:56.000000 core_module_periodic_table_app-2.8.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       23 2024-03-12 19:04:56.000000 core_module_periodic_table_app-2.8.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        7 2024-03-12 19:04:56.000000 core_module_periodic_table_app-2.8.0/requirements.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2024-03-12 19:04:58.558931 core_module_periodic_table_app-2.8.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1093 2024-03-12 19:04:56.000000 core_module_periodic_table_app-2.8.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:58.539221 core_module_periodic_table_app-2.8.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:56.000000 core_module_periodic_table_app-2.8.0/tests/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1262 2024-03-12 19:04:56.000000 core_module_periodic_table_app-2.8.0/tests/test_settings.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4065 2024-03-12 19:04:56.000000 core_module_periodic_table_app-2.8.0/tests/test_unit_views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:03.317081 core_module_periodic_table_app-2.9.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2024-05-13 16:10:01.000000 core_module_periodic_table_app-2.9.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      193 2024-05-13 16:10:01.000000 core_module_periodic_table_app-2.9.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1112 2024-05-13 16:10:03.311423 core_module_periodic_table_app-2.9.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      618 2024-05-13 16:10:01.000000 core_module_periodic_table_app-2.9.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:03.103388 core_module_periodic_table_app-2.9.0/core_module_periodic_table_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:01.000000 core_module_periodic_table_app-2.9.0/core_module_periodic_table_app/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:02.941215 core_module_periodic_table_app-2.9.0/core_module_periodic_table_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:02.949791 core_module_periodic_table_app-2.9.0/core_module_periodic_table_app/static/core_module_periodic_table_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:03.215159 core_module_periodic_table_app-2.9.0/core_module_periodic_table_app/static/core_module_periodic_table_app/css/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1416 2024-05-13 16:10:01.000000 core_module_periodic_table_app-2.9.0/core_module_periodic_table_app/static/core_module_periodic_table_app/css/periodic.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:03.227902 core_module_periodic_table_app-2.9.0/core_module_periodic_table_app/static/core_module_periodic_table_app/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1075 2024-05-13 16:10:01.000000 core_module_periodic_table_app-2.9.0/core_module_periodic_table_app/static/core_module_periodic_table_app/js/periodic.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:02.959455 core_module_periodic_table_app-2.9.0/core_module_periodic_table_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:03.254869 core_module_periodic_table_app-2.9.0/core_module_periodic_table_app/templates/core_module_periodic_table_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10866 2024-05-13 16:10:01.000000 core_module_periodic_table_app-2.9.0/core_module_periodic_table_app/templates/core_module_periodic_table_app/periodic.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      146 2024-05-13 16:10:01.000000 core_module_periodic_table_app-2.9.0/core_module_periodic_table_app/templates/core_module_periodic_table_app/periodic_simple.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      312 2024-05-13 16:10:01.000000 core_module_periodic_table_app-2.9.0/core_module_periodic_table_app/urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1731 2024-05-13 16:10:01.000000 core_module_periodic_table_app-2.9.0/core_module_periodic_table_app/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:03.198183 core_module_periodic_table_app-2.9.0/core_module_periodic_table_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1112 2024-05-13 16:10:02.000000 core_module_periodic_table_app-2.9.0/core_module_periodic_table_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      902 2024-05-13 16:10:02.000000 core_module_periodic_table_app-2.9.0/core_module_periodic_table_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2024-05-13 16:10:02.000000 core_module_periodic_table_app-2.9.0/core_module_periodic_table_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       30 2024-05-13 16:10:02.000000 core_module_periodic_table_app-2.9.0/core_module_periodic_table_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       37 2024-05-13 16:10:02.000000 core_module_periodic_table_app-2.9.0/core_module_periodic_table_app.egg-info/top_level.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2024-05-13 16:10:01.000000 core_module_periodic_table_app-2.9.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       23 2024-05-13 16:10:01.000000 core_module_periodic_table_app-2.9.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        7 2024-05-13 16:10:01.000000 core_module_periodic_table_app-2.9.0/requirements.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2024-05-13 16:10:03.319247 core_module_periodic_table_app-2.9.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1093 2024-05-13 16:10:01.000000 core_module_periodic_table_app-2.9.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:03.300526 core_module_periodic_table_app-2.9.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:01.000000 core_module_periodic_table_app-2.9.0/tests/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1262 2024-05-13 16:10:01.000000 core_module_periodic_table_app-2.9.0/tests/test_settings.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4065 2024-05-13 16:10:01.000000 core_module_periodic_table_app-2.9.0/tests/test_unit_views.py
```

### Comparing `core_module_periodic_table_app-2.8.0/LICENSE.md` & `core_module_periodic_table_app-2.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `core_module_periodic_table_app-2.8.0/PKG-INFO` & `core_module_periodic_table_app-2.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_module_periodic_table_app
-Version: 2.8.0
+Version: 2.9.0
 Summary: Periodic table module for the parser core project
 Home-page: https://github.com/usnistgov/core_module_periodic_table_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: core_module_periodic_table_app
         ==============================
```

### Comparing `core_module_periodic_table_app-2.8.0/README.rst` & `core_module_periodic_table_app-2.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_module_periodic_table_app-2.8.0/core_module_periodic_table_app/static/core_module_periodic_table_app/css/periodic.css` & `core_module_periodic_table_app-2.9.0/core_module_periodic_table_app/static/core_module_periodic_table_app/css/periodic.css`

 * *Files identical despite different names*

### Comparing `core_module_periodic_table_app-2.8.0/core_module_periodic_table_app/static/core_module_periodic_table_app/js/periodic.js` & `core_module_periodic_table_app-2.9.0/core_module_periodic_table_app/static/core_module_periodic_table_app/js/periodic.js`

 * *Files identical despite different names*

### Comparing `core_module_periodic_table_app-2.8.0/core_module_periodic_table_app/templates/core_module_periodic_table_app/periodic.html` & `core_module_periodic_table_app-2.9.0/core_module_periodic_table_app/templates/core_module_periodic_table_app/periodic.html`

 * *Files identical despite different names*

### Comparing `core_module_periodic_table_app-2.8.0/core_module_periodic_table_app/views.py` & `core_module_periodic_table_app-2.9.0/core_module_periodic_table_app/views.py`

 * *Files identical despite different names*

### Comparing `core_module_periodic_table_app-2.8.0/core_module_periodic_table_app.egg-info/PKG-INFO` & `core_module_periodic_table_app-2.9.0/core_module_periodic_table_app.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-module-periodic-table-app
-Version: 2.8.0
+Version: 2.9.0
 Summary: Periodic table module for the parser core project
 Home-page: https://github.com/usnistgov/core_module_periodic_table_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: core_module_periodic_table_app
         ==============================
```

### Comparing `core_module_periodic_table_app-2.8.0/core_module_periodic_table_app.egg-info/SOURCES.txt` & `core_module_periodic_table_app-2.9.0/core_module_periodic_table_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `core_module_periodic_table_app-2.8.0/setup.py` & `core_module_periodic_table_app-2.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_module_periodic_table_app",
-    version="2.8.0",
+    version="2.9.0",
     description="Periodic table module for the parser core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_module_periodic_table_app",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `core_module_periodic_table_app-2.8.0/tests/test_settings.py` & `core_module_periodic_table_app-2.9.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `core_module_periodic_table_app-2.8.0/tests/test_unit_views.py` & `core_module_periodic_table_app-2.9.0/tests/test_unit_views.py`

 * *Files identical despite different names*

