# Comparing `tmp/core_module_text_area_app-2.8.0.tar.gz` & `tmp/core_module_text_area_app-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_module_text_area_app-2.8.0.tar", last modified: Tue Mar 12 19:05:32 2024, max compression
+gzip compressed data, was "core_module_text_area_app-2.9.0.tar", last modified: Mon May 13 16:10:35 2024, max compression
```

## Comparing `core_module_text_area_app-2.8.0.tar` & `core_module_text_area_app-2.9.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:32.437215 core_module_text_area_app-2.8.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2024-03-12 19:05:30.000000 core_module_text_area_app-2.8.0/LICENSE.md
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      183 2024-03-12 19:05:30.000000 core_module_text_area_app-2.8.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1052 2024-03-12 19:05:32.430396 core_module_text_area_app-2.8.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      573 2024-03-12 19:05:30.000000 core_module_text_area_app-2.8.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:32.176885 core_module_text_area_app-2.8.0/core_module_text_area_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:30.000000 core_module_text_area_app-2.8.0/core_module_text_area_app/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      587 2024-03-12 19:05:30.000000 core_module_text_area_app-2.8.0/core_module_text_area_app/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:31.979917 core_module_text_area_app-2.8.0/core_module_text_area_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:32.329292 core_module_text_area_app-2.8.0/core_module_text_area_app/templates/core_module_text_area_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      195 2024-03-12 19:05:30.000000 core_module_text_area_app-2.8.0/core_module_text_area_app/templates/core_module_text_area_app/predefined_entities_warning.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      288 2024-03-12 19:05:30.000000 core_module_text_area_app-2.8.0/core_module_text_area_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:32.364973 core_module_text_area_app-2.8.0/core_module_text_area_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:30.000000 core_module_text_area_app-2.8.0/core_module_text_area_app/views/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1851 2024-03-12 19:05:30.000000 core_module_text_area_app-2.8.0/core_module_text_area_app/views/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:32.309025 core_module_text_area_app-2.8.0/core_module_text_area_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1052 2024-03-12 19:05:31.000000 core_module_text_area_app-2.8.0/core_module_text_area_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      696 2024-03-12 19:05:31.000000 core_module_text_area_app-2.8.0/core_module_text_area_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2024-03-12 19:05:31.000000 core_module_text_area_app-2.8.0/core_module_text_area_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       30 2024-03-12 19:05:31.000000 core_module_text_area_app-2.8.0/core_module_text_area_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       32 2024-03-12 19:05:31.000000 core_module_text_area_app-2.8.0/core_module_text_area_app.egg-info/top_level.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2024-03-12 19:05:30.000000 core_module_text_area_app-2.8.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       23 2024-03-12 19:05:30.000000 core_module_text_area_app-2.8.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        7 2024-03-12 19:05:30.000000 core_module_text_area_app-2.8.0/requirements.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2024-03-12 19:05:32.439834 core_module_text_area_app-2.8.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1073 2024-03-12 19:05:30.000000 core_module_text_area_app-2.8.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:32.415905 core_module_text_area_app-2.8.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:30.000000 core_module_text_area_app-2.8.0/tests/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1312 2024-03-12 19:05:30.000000 core_module_text_area_app-2.8.0/tests/test_settings.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2836 2024-03-12 19:05:30.000000 core_module_text_area_app-2.8.0/tests/test_unit_views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:35.258043 core_module_text_area_app-2.9.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2024-05-13 16:10:33.000000 core_module_text_area_app-2.9.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      183 2024-05-13 16:10:33.000000 core_module_text_area_app-2.9.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1052 2024-05-13 16:10:35.251132 core_module_text_area_app-2.9.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      573 2024-05-13 16:10:33.000000 core_module_text_area_app-2.9.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:35.005609 core_module_text_area_app-2.9.0/core_module_text_area_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:33.000000 core_module_text_area_app-2.9.0/core_module_text_area_app/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      587 2024-05-13 16:10:33.000000 core_module_text_area_app-2.9.0/core_module_text_area_app/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:34.812228 core_module_text_area_app-2.9.0/core_module_text_area_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:35.121564 core_module_text_area_app-2.9.0/core_module_text_area_app/templates/core_module_text_area_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      195 2024-05-13 16:10:33.000000 core_module_text_area_app-2.9.0/core_module_text_area_app/templates/core_module_text_area_app/predefined_entities_warning.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      288 2024-05-13 16:10:33.000000 core_module_text_area_app-2.9.0/core_module_text_area_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:35.178731 core_module_text_area_app-2.9.0/core_module_text_area_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:33.000000 core_module_text_area_app-2.9.0/core_module_text_area_app/views/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1851 2024-05-13 16:10:33.000000 core_module_text_area_app-2.9.0/core_module_text_area_app/views/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:35.100766 core_module_text_area_app-2.9.0/core_module_text_area_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1052 2024-05-13 16:10:34.000000 core_module_text_area_app-2.9.0/core_module_text_area_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      696 2024-05-13 16:10:34.000000 core_module_text_area_app-2.9.0/core_module_text_area_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2024-05-13 16:10:34.000000 core_module_text_area_app-2.9.0/core_module_text_area_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       30 2024-05-13 16:10:34.000000 core_module_text_area_app-2.9.0/core_module_text_area_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       32 2024-05-13 16:10:34.000000 core_module_text_area_app-2.9.0/core_module_text_area_app.egg-info/top_level.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2024-05-13 16:10:33.000000 core_module_text_area_app-2.9.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       23 2024-05-13 16:10:33.000000 core_module_text_area_app-2.9.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        7 2024-05-13 16:10:33.000000 core_module_text_area_app-2.9.0/requirements.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2024-05-13 16:10:35.261266 core_module_text_area_app-2.9.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1073 2024-05-13 16:10:33.000000 core_module_text_area_app-2.9.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:35.237528 core_module_text_area_app-2.9.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:33.000000 core_module_text_area_app-2.9.0/tests/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1312 2024-05-13 16:10:33.000000 core_module_text_area_app-2.9.0/tests/test_settings.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2836 2024-05-13 16:10:33.000000 core_module_text_area_app-2.9.0/tests/test_unit_views.py
```

### Comparing `core_module_text_area_app-2.8.0/LICENSE.md` & `core_module_text_area_app-2.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `core_module_text_area_app-2.8.0/PKG-INFO` & `core_module_text_area_app-2.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_module_text_area_app
-Version: 2.8.0
+Version: 2.9.0
 Summary: Text Area module for the parser core project
 Home-page: https://github.com/usnistgov/core_module_text_area_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: core_module_text_area_app
         =========================
```

### Comparing `core_module_text_area_app-2.8.0/README.rst` & `core_module_text_area_app-2.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_module_text_area_app-2.8.0/core_module_text_area_app/settings.py` & `core_module_text_area_app-2.9.0/core_module_text_area_app/settings.py`

 * *Files identical despite different names*

### Comparing `core_module_text_area_app-2.8.0/core_module_text_area_app/views/views.py` & `core_module_text_area_app-2.9.0/core_module_text_area_app/views/views.py`

 * *Files identical despite different names*

### Comparing `core_module_text_area_app-2.8.0/core_module_text_area_app.egg-info/PKG-INFO` & `core_module_text_area_app-2.9.0/core_module_text_area_app.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-module-text-area-app
-Version: 2.8.0
+Version: 2.9.0
 Summary: Text Area module for the parser core project
 Home-page: https://github.com/usnistgov/core_module_text_area_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: core_module_text_area_app
         =========================
```

### Comparing `core_module_text_area_app-2.8.0/core_module_text_area_app.egg-info/SOURCES.txt` & `core_module_text_area_app-2.9.0/core_module_text_area_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `core_module_text_area_app-2.8.0/setup.py` & `core_module_text_area_app-2.9.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_module_text_area_app",
-    version="2.8.0",
+    version="2.9.0",
     description="Text Area module for the parser core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_module_text_area_app",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `core_module_text_area_app-2.8.0/tests/test_settings.py` & `core_module_text_area_app-2.9.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `core_module_text_area_app-2.8.0/tests/test_unit_views.py` & `core_module_text_area_app-2.9.0/tests/test_unit_views.py`

 * *Files identical despite different names*

