# Comparing `tmp/core_module_raw_xml_app-2.8.0.tar.gz` & `tmp/core_module_raw_xml_app-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_module_raw_xml_app-2.8.0.tar", last modified: Tue Mar 12 19:05:07 2024, max compression
+gzip compressed data, was "core_module_raw_xml_app-2.9.0.tar", last modified: Mon May 13 16:10:12 2024, max compression
```

## Comparing `core_module_raw_xml_app-2.8.0.tar` & `core_module_raw_xml_app-2.9.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:07.249633 core_module_raw_xml_app-2.8.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2024-03-12 19:05:05.000000 core_module_raw_xml_app-2.8.0/LICENSE.md
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      179 2024-03-12 19:05:05.000000 core_module_raw_xml_app-2.8.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1028 2024-03-12 19:05:07.244655 core_module_raw_xml_app-2.8.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      555 2024-03-12 19:05:05.000000 core_module_raw_xml_app-2.8.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:07.053908 core_module_raw_xml_app-2.8.0/core_module_raw_xml_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:05.000000 core_module_raw_xml_app-2.8.0/core_module_raw_xml_app/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      276 2024-03-12 19:05:05.000000 core_module_raw_xml_app-2.8.0/core_module_raw_xml_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:07.188961 core_module_raw_xml_app-2.8.0/core_module_raw_xml_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:05.000000 core_module_raw_xml_app-2.8.0/core_module_raw_xml_app/views/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2686 2024-03-12 19:05:05.000000 core_module_raw_xml_app-2.8.0/core_module_raw_xml_app/views/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:07.148994 core_module_raw_xml_app-2.8.0/core_module_raw_xml_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1028 2024-03-12 19:05:06.000000 core_module_raw_xml_app-2.8.0/core_module_raw_xml_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      545 2024-03-12 19:05:06.000000 core_module_raw_xml_app-2.8.0/core_module_raw_xml_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2024-03-12 19:05:06.000000 core_module_raw_xml_app-2.8.0/core_module_raw_xml_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       40 2024-03-12 19:05:06.000000 core_module_raw_xml_app-2.8.0/core_module_raw_xml_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       30 2024-03-12 19:05:06.000000 core_module_raw_xml_app-2.8.0/core_module_raw_xml_app.egg-info/top_level.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2024-03-12 19:05:05.000000 core_module_raw_xml_app-2.8.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       33 2024-03-12 19:05:05.000000 core_module_raw_xml_app-2.8.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        7 2024-03-12 19:05:05.000000 core_module_raw_xml_app-2.8.0/requirements.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2024-03-12 19:05:07.251933 core_module_raw_xml_app-2.8.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1065 2024-03-12 19:05:05.000000 core_module_raw_xml_app-2.8.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:07.233782 core_module_raw_xml_app-2.8.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:05.000000 core_module_raw_xml_app-2.8.0/tests/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      120 2024-03-12 19:05:05.000000 core_module_raw_xml_app-2.8.0/tests/test_settings.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       33 2024-03-12 19:05:05.000000 core_module_raw_xml_app-2.8.0/tests/test_unit_views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:12.201518 core_module_raw_xml_app-2.9.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2024-05-13 16:10:08.000000 core_module_raw_xml_app-2.9.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      179 2024-05-13 16:10:08.000000 core_module_raw_xml_app-2.9.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1028 2024-05-13 16:10:12.194769 core_module_raw_xml_app-2.9.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      555 2024-05-13 16:10:08.000000 core_module_raw_xml_app-2.9.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:10.437447 core_module_raw_xml_app-2.9.0/core_module_raw_xml_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:08.000000 core_module_raw_xml_app-2.9.0/core_module_raw_xml_app/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      276 2024-05-13 16:10:08.000000 core_module_raw_xml_app-2.9.0/core_module_raw_xml_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:12.119343 core_module_raw_xml_app-2.9.0/core_module_raw_xml_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:08.000000 core_module_raw_xml_app-2.9.0/core_module_raw_xml_app/views/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2686 2024-05-13 16:10:08.000000 core_module_raw_xml_app-2.9.0/core_module_raw_xml_app/views/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:10.526741 core_module_raw_xml_app-2.9.0/core_module_raw_xml_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1028 2024-05-13 16:10:10.000000 core_module_raw_xml_app-2.9.0/core_module_raw_xml_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      545 2024-05-13 16:10:10.000000 core_module_raw_xml_app-2.9.0/core_module_raw_xml_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2024-05-13 16:10:10.000000 core_module_raw_xml_app-2.9.0/core_module_raw_xml_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       40 2024-05-13 16:10:10.000000 core_module_raw_xml_app-2.9.0/core_module_raw_xml_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       30 2024-05-13 16:10:10.000000 core_module_raw_xml_app-2.9.0/core_module_raw_xml_app.egg-info/top_level.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2024-05-13 16:10:08.000000 core_module_raw_xml_app-2.9.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       33 2024-05-13 16:10:08.000000 core_module_raw_xml_app-2.9.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        7 2024-05-13 16:10:08.000000 core_module_raw_xml_app-2.9.0/requirements.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2024-05-13 16:10:12.204124 core_module_raw_xml_app-2.9.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1065 2024-05-13 16:10:08.000000 core_module_raw_xml_app-2.9.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:12.175579 core_module_raw_xml_app-2.9.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:08.000000 core_module_raw_xml_app-2.9.0/tests/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      120 2024-05-13 16:10:08.000000 core_module_raw_xml_app-2.9.0/tests/test_settings.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       33 2024-05-13 16:10:08.000000 core_module_raw_xml_app-2.9.0/tests/test_unit_views.py
```

### Comparing `core_module_raw_xml_app-2.8.0/LICENSE.md` & `core_module_raw_xml_app-2.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `core_module_raw_xml_app-2.8.0/PKG-INFO` & `core_module_raw_xml_app-2.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_module_raw_xml_app
-Version: 2.8.0
+Version: 2.9.0
 Summary: Raw xml module for the parser core project
 Home-page: https://github.com/usnistgov/core_module_raw_xml_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: core_module_raw_xml_app
         =======================
```

### Comparing `core_module_raw_xml_app-2.8.0/README.rst` & `core_module_raw_xml_app-2.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_module_raw_xml_app-2.8.0/core_module_raw_xml_app/views/views.py` & `core_module_raw_xml_app-2.9.0/core_module_raw_xml_app/views/views.py`

 * *Files identical despite different names*

### Comparing `core_module_raw_xml_app-2.8.0/core_module_raw_xml_app.egg-info/PKG-INFO` & `core_module_raw_xml_app-2.9.0/core_module_raw_xml_app.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-module-raw-xml-app
-Version: 2.8.0
+Version: 2.9.0
 Summary: Raw xml module for the parser core project
 Home-page: https://github.com/usnistgov/core_module_raw_xml_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: core_module_raw_xml_app
         =======================
```

### Comparing `core_module_raw_xml_app-2.8.0/core_module_raw_xml_app.egg-info/SOURCES.txt` & `core_module_raw_xml_app-2.9.0/core_module_raw_xml_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `core_module_raw_xml_app-2.8.0/setup.py` & `core_module_raw_xml_app-2.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_module_raw_xml_app",
-    version="2.8.0",
+    version="2.9.0",
     description="Raw xml module for the parser core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_module_raw_xml_app",
     packages=find_packages(),
     include_package_data=True,
```

