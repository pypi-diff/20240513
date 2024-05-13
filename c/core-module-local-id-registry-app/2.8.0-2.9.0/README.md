# Comparing `tmp/core_module_local_id_registry_app-2.8.0.tar.gz` & `tmp/core_module_local_id_registry_app-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_module_local_id_registry_app-2.8.0.tar", last modified: Tue Mar 12 19:04:50 2024, max compression
+gzip compressed data, was "core_module_local_id_registry_app-2.9.0.tar", last modified: Mon May 13 16:09:55 2024, max compression
```

## Comparing `core_module_local_id_registry_app-2.8.0.tar` & `core_module_local_id_registry_app-2.9.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:50.871198 core_module_local_id_registry_app-2.8.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2024-03-12 19:04:48.000000 core_module_local_id_registry_app-2.8.0/LICENSE.md
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      199 2024-03-12 19:04:48.000000 core_module_local_id_registry_app-2.8.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1091 2024-03-12 19:04:50.862813 core_module_local_id_registry_app-2.8.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      616 2024-03-12 19:04:48.000000 core_module_local_id_registry_app-2.8.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:50.490649 core_module_local_id_registry_app-2.8.0/core_module_local_id_registry_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:48.000000 core_module_local_id_registry_app-2.8.0/core_module_local_id_registry_app/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      600 2024-03-12 19:04:48.000000 core_module_local_id_registry_app-2.8.0/core_module_local_id_registry_app/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:50.269646 core_module_local_id_registry_app-2.8.0/core_module_local_id_registry_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:50.279758 core_module_local_id_registry_app-2.8.0/core_module_local_id_registry_app/static/core_module_local_id_registry_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:50.609390 core_module_local_id_registry_app-2.8.0/core_module_local_id_registry_app/static/core_module_local_id_registry_app/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      537 2024-03-12 19:04:48.000000 core_module_local_id_registry_app-2.8.0/core_module_local_id_registry_app/static/core_module_local_id_registry_app/css/module_local_id.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:50.627135 core_module_local_id_registry_app-2.8.0/core_module_local_id_registry_app/static/core_module_local_id_registry_app/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      778 2024-03-12 19:04:48.000000 core_module_local_id_registry_app-2.8.0/core_module_local_id_registry_app/static/core_module_local_id_registry_app/js/module_local_id.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:50.289929 core_module_local_id_registry_app-2.8.0/core_module_local_id_registry_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:50.659709 core_module_local_id_registry_app-2.8.0/core_module_local_id_registry_app/templates/core_module_local_id_registry_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       89 2024-03-12 19:04:48.000000 core_module_local_id_registry_app-2.8.0/core_module_local_id_registry_app/templates/core_module_local_id_registry_app/pid_display_box.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      383 2024-03-12 19:04:48.000000 core_module_local_id_registry_app-2.8.0/core_module_local_id_registry_app/templates/core_module_local_id_registry_app/pid_edit_input.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      334 2024-03-12 19:04:48.000000 core_module_local_id_registry_app-2.8.0/core_module_local_id_registry_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:50.701884 core_module_local_id_registry_app-2.8.0/core_module_local_id_registry_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:48.000000 core_module_local_id_registry_app-2.8.0/core_module_local_id_registry_app/views/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9381 2024-03-12 19:04:48.000000 core_module_local_id_registry_app-2.8.0/core_module_local_id_registry_app/views/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:50.585248 core_module_local_id_registry_app-2.8.0/core_module_local_id_registry_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1091 2024-03-12 19:04:49.000000 core_module_local_id_registry_app-2.8.0/core_module_local_id_registry_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1212 2024-03-12 19:04:50.000000 core_module_local_id_registry_app-2.8.0/core_module_local_id_registry_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2024-03-12 19:04:49.000000 core_module_local_id_registry_app-2.8.0/core_module_local_id_registry_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      104 2024-03-12 19:04:49.000000 core_module_local_id_registry_app-2.8.0/core_module_local_id_registry_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       40 2024-03-12 19:04:49.000000 core_module_local_id_registry_app-2.8.0/core_module_local_id_registry_app.egg-info/top_level.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2024-03-12 19:04:48.000000 core_module_local_id_registry_app-2.8.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       97 2024-03-12 19:04:48.000000 core_module_local_id_registry_app-2.8.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        7 2024-03-12 19:04:48.000000 core_module_local_id_registry_app-2.8.0/requirements.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2024-03-12 19:04:50.874384 core_module_local_id_registry_app-2.8.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1081 2024-03-12 19:04:48.000000 core_module_local_id_registry_app-2.8.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:50.739663 core_module_local_id_registry_app-2.8.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:48.000000 core_module_local_id_registry_app-2.8.0/tests/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      969 2024-03-12 19:04:48.000000 core_module_local_id_registry_app-2.8.0/tests/test_settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:50.758026 core_module_local_id_registry_app-2.8.0/tests/views/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:50.843655 core_module_local_id_registry_app-2.8.0/tests/views/LocalIdRegistryModule/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:48.000000 core_module_local_id_registry_app-2.8.0/tests/views/LocalIdRegistryModule/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1918 2024-03-12 19:04:48.000000 core_module_local_id_registry_app-2.8.0/tests/views/LocalIdRegistryModule/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    38419 2024-03-12 19:04:48.000000 core_module_local_id_registry_app-2.8.0/tests/views/LocalIdRegistryModule/test_unit.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:48.000000 core_module_local_id_registry_app-2.8.0/tests/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:55.503486 core_module_local_id_registry_app-2.9.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2024-05-13 16:09:52.000000 core_module_local_id_registry_app-2.9.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      199 2024-05-13 16:09:52.000000 core_module_local_id_registry_app-2.9.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1091 2024-05-13 16:09:55.497425 core_module_local_id_registry_app-2.9.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      616 2024-05-13 16:09:52.000000 core_module_local_id_registry_app-2.9.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:55.122368 core_module_local_id_registry_app-2.9.0/core_module_local_id_registry_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:52.000000 core_module_local_id_registry_app-2.9.0/core_module_local_id_registry_app/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      600 2024-05-13 16:09:52.000000 core_module_local_id_registry_app-2.9.0/core_module_local_id_registry_app/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:54.903256 core_module_local_id_registry_app-2.9.0/core_module_local_id_registry_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:54.913612 core_module_local_id_registry_app-2.9.0/core_module_local_id_registry_app/static/core_module_local_id_registry_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:55.250669 core_module_local_id_registry_app-2.9.0/core_module_local_id_registry_app/static/core_module_local_id_registry_app/css/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      537 2024-05-13 16:09:52.000000 core_module_local_id_registry_app-2.9.0/core_module_local_id_registry_app/static/core_module_local_id_registry_app/css/module_local_id.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:55.268936 core_module_local_id_registry_app-2.9.0/core_module_local_id_registry_app/static/core_module_local_id_registry_app/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      778 2024-05-13 16:09:52.000000 core_module_local_id_registry_app-2.9.0/core_module_local_id_registry_app/static/core_module_local_id_registry_app/js/module_local_id.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:54.925010 core_module_local_id_registry_app-2.9.0/core_module_local_id_registry_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:55.306542 core_module_local_id_registry_app-2.9.0/core_module_local_id_registry_app/templates/core_module_local_id_registry_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       89 2024-05-13 16:09:53.000000 core_module_local_id_registry_app-2.9.0/core_module_local_id_registry_app/templates/core_module_local_id_registry_app/pid_display_box.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      383 2024-05-13 16:09:53.000000 core_module_local_id_registry_app-2.9.0/core_module_local_id_registry_app/templates/core_module_local_id_registry_app/pid_edit_input.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      334 2024-05-13 16:09:53.000000 core_module_local_id_registry_app-2.9.0/core_module_local_id_registry_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:55.354079 core_module_local_id_registry_app-2.9.0/core_module_local_id_registry_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:53.000000 core_module_local_id_registry_app-2.9.0/core_module_local_id_registry_app/views/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9381 2024-05-13 16:09:53.000000 core_module_local_id_registry_app-2.9.0/core_module_local_id_registry_app/views/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:55.222274 core_module_local_id_registry_app-2.9.0/core_module_local_id_registry_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1091 2024-05-13 16:09:54.000000 core_module_local_id_registry_app-2.9.0/core_module_local_id_registry_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1212 2024-05-13 16:09:54.000000 core_module_local_id_registry_app-2.9.0/core_module_local_id_registry_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2024-05-13 16:09:54.000000 core_module_local_id_registry_app-2.9.0/core_module_local_id_registry_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      104 2024-05-13 16:09:54.000000 core_module_local_id_registry_app-2.9.0/core_module_local_id_registry_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       40 2024-05-13 16:09:54.000000 core_module_local_id_registry_app-2.9.0/core_module_local_id_registry_app.egg-info/top_level.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2024-05-13 16:09:53.000000 core_module_local_id_registry_app-2.9.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       97 2024-05-13 16:09:53.000000 core_module_local_id_registry_app-2.9.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        7 2024-05-13 16:09:53.000000 core_module_local_id_registry_app-2.9.0/requirements.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2024-05-13 16:09:55.505850 core_module_local_id_registry_app-2.9.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1081 2024-05-13 16:09:53.000000 core_module_local_id_registry_app-2.9.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:55.409602 core_module_local_id_registry_app-2.9.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:53.000000 core_module_local_id_registry_app-2.9.0/tests/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      969 2024-05-13 16:09:53.000000 core_module_local_id_registry_app-2.9.0/tests/test_settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:55.428017 core_module_local_id_registry_app-2.9.0/tests/views/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:55.484264 core_module_local_id_registry_app-2.9.0/tests/views/LocalIdRegistryModule/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:53.000000 core_module_local_id_registry_app-2.9.0/tests/views/LocalIdRegistryModule/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1918 2024-05-13 16:09:53.000000 core_module_local_id_registry_app-2.9.0/tests/views/LocalIdRegistryModule/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    38419 2024-05-13 16:09:53.000000 core_module_local_id_registry_app-2.9.0/tests/views/LocalIdRegistryModule/test_unit.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:53.000000 core_module_local_id_registry_app-2.9.0/tests/views/__init__.py
```

### Comparing `core_module_local_id_registry_app-2.8.0/LICENSE.md` & `core_module_local_id_registry_app-2.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `core_module_local_id_registry_app-2.8.0/PKG-INFO` & `core_module_local_id_registry_app-2.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_module_local_id_registry_app
-Version: 2.8.0
+Version: 2.9.0
 Summary: Local id registry module
 Home-page: https://github.com/usnistgov/core_module_local_id_registry_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: core_module_local_id_registry_app
         =================================
```

### Comparing `core_module_local_id_registry_app-2.8.0/README.rst` & `core_module_local_id_registry_app-2.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_module_local_id_registry_app-2.8.0/core_module_local_id_registry_app/settings.py` & `core_module_local_id_registry_app-2.9.0/core_module_local_id_registry_app/settings.py`

 * *Files identical despite different names*

### Comparing `core_module_local_id_registry_app-2.8.0/core_module_local_id_registry_app/static/core_module_local_id_registry_app/css/module_local_id.css` & `core_module_local_id_registry_app-2.9.0/core_module_local_id_registry_app/static/core_module_local_id_registry_app/css/module_local_id.css`

 * *Files identical despite different names*

### Comparing `core_module_local_id_registry_app-2.8.0/core_module_local_id_registry_app/static/core_module_local_id_registry_app/js/module_local_id.js` & `core_module_local_id_registry_app-2.9.0/core_module_local_id_registry_app/static/core_module_local_id_registry_app/js/module_local_id.js`

 * *Files identical despite different names*

### Comparing `core_module_local_id_registry_app-2.8.0/core_module_local_id_registry_app/views/views.py` & `core_module_local_id_registry_app-2.9.0/core_module_local_id_registry_app/views/views.py`

 * *Files identical despite different names*

### Comparing `core_module_local_id_registry_app-2.8.0/core_module_local_id_registry_app.egg-info/PKG-INFO` & `core_module_local_id_registry_app-2.9.0/core_module_local_id_registry_app.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-module-local-id-registry-app
-Version: 2.8.0
+Version: 2.9.0
 Summary: Local id registry module
 Home-page: https://github.com/usnistgov/core_module_local_id_registry_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: core_module_local_id_registry_app
         =================================
```

### Comparing `core_module_local_id_registry_app-2.8.0/core_module_local_id_registry_app.egg-info/SOURCES.txt` & `core_module_local_id_registry_app-2.9.0/core_module_local_id_registry_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `core_module_local_id_registry_app-2.8.0/setup.py` & `core_module_local_id_registry_app-2.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_module_local_id_registry_app",
-    version="2.8.0",
+    version="2.9.0",
     description="Local id registry module",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_module_local_id_registry_app",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `core_module_local_id_registry_app-2.8.0/tests/test_settings.py` & `core_module_local_id_registry_app-2.9.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `core_module_local_id_registry_app-2.8.0/tests/views/LocalIdRegistryModule/fixtures.py` & `core_module_local_id_registry_app-2.9.0/tests/views/LocalIdRegistryModule/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_module_local_id_registry_app-2.8.0/tests/views/LocalIdRegistryModule/test_unit.py` & `core_module_local_id_registry_app-2.9.0/tests/views/LocalIdRegistryModule/test_unit.py`

 * *Files identical despite different names*

