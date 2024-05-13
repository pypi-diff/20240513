# Comparing `tmp/core_module_status_registry_app-2.8.0.tar.gz` & `tmp/core_module_status_registry_app-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_module_status_registry_app-2.8.0.tar", last modified: Tue Mar 12 19:05:24 2024, max compression
+gzip compressed data, was "core_module_status_registry_app-2.9.0.tar", last modified: Mon May 13 16:10:27 2024, max compression
```

## Comparing `core_module_status_registry_app-2.8.0.tar` & `core_module_status_registry_app-2.9.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:24.145217 core_module_status_registry_app-2.8.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2024-03-12 19:05:21.000000 core_module_status_registry_app-2.8.0/LICENSE.md
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      195 2024-03-12 19:05:21.000000 core_module_status_registry_app-2.8.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1067 2024-03-12 19:05:24.138790 core_module_status_registry_app-2.8.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      598 2024-03-12 19:05:21.000000 core_module_status_registry_app-2.8.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:23.825987 core_module_status_registry_app-2.8.0/core_module_status_registry_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:21.000000 core_module_status_registry_app-2.8.0/core_module_status_registry_app/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      324 2024-03-12 19:05:21.000000 core_module_status_registry_app-2.8.0/core_module_status_registry_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:24.086061 core_module_status_registry_app-2.8.0/core_module_status_registry_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:21.000000 core_module_status_registry_app-2.8.0/core_module_status_registry_app/views/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1581 2024-03-12 19:05:21.000000 core_module_status_registry_app-2.8.0/core_module_status_registry_app/views/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:23.925037 core_module_status_registry_app-2.8.0/core_module_status_registry_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1067 2024-03-12 19:05:23.000000 core_module_status_registry_app-2.8.0/core_module_status_registry_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      592 2024-03-12 19:05:23.000000 core_module_status_registry_app-2.8.0/core_module_status_registry_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2024-03-12 19:05:23.000000 core_module_status_registry_app-2.8.0/core_module_status_registry_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       60 2024-03-12 19:05:23.000000 core_module_status_registry_app-2.8.0/core_module_status_registry_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2024-03-12 19:05:23.000000 core_module_status_registry_app-2.8.0/core_module_status_registry_app.egg-info/top_level.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2024-03-12 19:05:21.000000 core_module_status_registry_app-2.8.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       53 2024-03-12 19:05:22.000000 core_module_status_registry_app-2.8.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        7 2024-03-12 19:05:22.000000 core_module_status_registry_app-2.8.0/requirements.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2024-03-12 19:05:24.148421 core_module_status_registry_app-2.8.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1069 2024-03-12 19:05:22.000000 core_module_status_registry_app-2.8.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:24.125252 core_module_status_registry_app-2.8.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:22.000000 core_module_status_registry_app-2.8.0/tests/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      119 2024-03-12 19:05:22.000000 core_module_status_registry_app-2.8.0/tests/test_settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:27.902911 core_module_status_registry_app-2.9.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2024-05-13 16:10:25.000000 core_module_status_registry_app-2.9.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      195 2024-05-13 16:10:25.000000 core_module_status_registry_app-2.9.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1067 2024-05-13 16:10:27.896770 core_module_status_registry_app-2.9.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      598 2024-05-13 16:10:25.000000 core_module_status_registry_app-2.9.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:27.663684 core_module_status_registry_app-2.9.0/core_module_status_registry_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:25.000000 core_module_status_registry_app-2.9.0/core_module_status_registry_app/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      324 2024-05-13 16:10:25.000000 core_module_status_registry_app-2.9.0/core_module_status_registry_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:27.828245 core_module_status_registry_app-2.9.0/core_module_status_registry_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:25.000000 core_module_status_registry_app-2.9.0/core_module_status_registry_app/views/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1581 2024-05-13 16:10:25.000000 core_module_status_registry_app-2.9.0/core_module_status_registry_app/views/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:27.774939 core_module_status_registry_app-2.9.0/core_module_status_registry_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1067 2024-05-13 16:10:27.000000 core_module_status_registry_app-2.9.0/core_module_status_registry_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      592 2024-05-13 16:10:27.000000 core_module_status_registry_app-2.9.0/core_module_status_registry_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2024-05-13 16:10:27.000000 core_module_status_registry_app-2.9.0/core_module_status_registry_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       60 2024-05-13 16:10:27.000000 core_module_status_registry_app-2.9.0/core_module_status_registry_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2024-05-13 16:10:27.000000 core_module_status_registry_app-2.9.0/core_module_status_registry_app.egg-info/top_level.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2024-05-13 16:10:25.000000 core_module_status_registry_app-2.9.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       53 2024-05-13 16:10:25.000000 core_module_status_registry_app-2.9.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        7 2024-05-13 16:10:25.000000 core_module_status_registry_app-2.9.0/requirements.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2024-05-13 16:10:27.905041 core_module_status_registry_app-2.9.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1069 2024-05-13 16:10:25.000000 core_module_status_registry_app-2.9.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:27.883506 core_module_status_registry_app-2.9.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:26.000000 core_module_status_registry_app-2.9.0/tests/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      119 2024-05-13 16:10:26.000000 core_module_status_registry_app-2.9.0/tests/test_settings.py
```

### Comparing `core_module_status_registry_app-2.8.0/LICENSE.md` & `core_module_status_registry_app-2.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `core_module_status_registry_app-2.8.0/PKG-INFO` & `core_module_status_registry_app-2.9.0/core_module_status_registry_app.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
-Name: core_module_status_registry_app
-Version: 2.8.0
+Name: core-module-status-registry-app
+Version: 2.9.0
 Summary: Status registry module
 Home-page: https://github.com/usnistgov/core_module_status_registry_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: core_module_status_registry_app
         ===============================
```

### Comparing `core_module_status_registry_app-2.8.0/README.rst` & `core_module_status_registry_app-2.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_module_status_registry_app-2.8.0/core_module_status_registry_app/views/views.py` & `core_module_status_registry_app-2.9.0/core_module_status_registry_app/views/views.py`

 * *Files identical despite different names*

### Comparing `core_module_status_registry_app-2.8.0/core_module_status_registry_app.egg-info/PKG-INFO` & `core_module_status_registry_app-2.9.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
-Name: core-module-status-registry-app
-Version: 2.8.0
+Name: core_module_status_registry_app
+Version: 2.9.0
 Summary: Status registry module
 Home-page: https://github.com/usnistgov/core_module_status_registry_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: core_module_status_registry_app
         ===============================
```

### Comparing `core_module_status_registry_app-2.8.0/core_module_status_registry_app.egg-info/SOURCES.txt` & `core_module_status_registry_app-2.9.0/core_module_status_registry_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `core_module_status_registry_app-2.8.0/setup.py` & `core_module_status_registry_app-2.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_module_status_registry_app",
-    version="2.8.0",
+    version="2.9.0",
     description="Status registry module",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_module_status_registry_app",
     packages=find_packages(),
     include_package_data=True,
```

