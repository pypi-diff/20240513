# Comparing `tmp/core_module_fancy_tree_registry_app-2.8.0.tar.gz` & `tmp/core_module_fancy_tree_registry_app-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_module_fancy_tree_registry_app-2.8.0.tar", last modified: Tue Mar 12 19:04:41 2024, max compression
+gzip compressed data, was "core_module_fancy_tree_registry_app-2.9.0.tar", last modified: Mon May 13 16:09:47 2024, max compression
```

## Comparing `core_module_fancy_tree_registry_app-2.8.0.tar` & `core_module_fancy_tree_registry_app-2.9.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:41.575877 core_module_fancy_tree_registry_app-2.8.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2024-03-12 19:04:39.000000 core_module_fancy_tree_registry_app-2.8.0/LICENSE.md
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      203 2024-03-12 19:04:39.000000 core_module_fancy_tree_registry_app-2.8.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1154 2024-03-12 19:04:41.568790 core_module_fancy_tree_registry_app-2.8.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      654 2024-03-12 19:04:39.000000 core_module_fancy_tree_registry_app-2.8.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:41.322478 core_module_fancy_tree_registry_app-2.8.0/core_module_fancy_tree_registry_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:39.000000 core_module_fancy_tree_registry_app-2.8.0/core_module_fancy_tree_registry_app/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:41.146667 core_module_fancy_tree_registry_app-2.8.0/core_module_fancy_tree_registry_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:41.151984 core_module_fancy_tree_registry_app-2.8.0/core_module_fancy_tree_registry_app/static/core_module_fancy_tree_registry_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:41.440973 core_module_fancy_tree_registry_app-2.8.0/core_module_fancy_tree_registry_app/static/core_module_fancy_tree_registry_app/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      605 2024-03-12 19:04:39.000000 core_module_fancy_tree_registry_app-2.8.0/core_module_fancy_tree_registry_app/static/core_module_fancy_tree_registry_app/js/fancy_tree.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:41.164169 core_module_fancy_tree_registry_app-2.8.0/core_module_fancy_tree_registry_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:41.459574 core_module_fancy_tree_registry_app-2.8.0/core_module_fancy_tree_registry_app/templates/core_module_fancy_tree_registry_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       89 2024-03-12 19:04:39.000000 core_module_fancy_tree_registry_app-2.8.0/core_module_fancy_tree_registry_app/templates/core_module_fancy_tree_registry_app/fancy_tree.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      316 2024-03-12 19:04:39.000000 core_module_fancy_tree_registry_app-2.8.0/core_module_fancy_tree_registry_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:41.509660 core_module_fancy_tree_registry_app-2.8.0/core_module_fancy_tree_registry_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:39.000000 core_module_fancy_tree_registry_app-2.8.0/core_module_fancy_tree_registry_app/views/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1087 2024-03-12 19:04:39.000000 core_module_fancy_tree_registry_app-2.8.0/core_module_fancy_tree_registry_app/views/forms.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6987 2024-03-12 19:04:39.000000 core_module_fancy_tree_registry_app-2.8.0/core_module_fancy_tree_registry_app/views/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:41.422670 core_module_fancy_tree_registry_app-2.8.0/core_module_fancy_tree_registry_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1154 2024-03-12 19:04:40.000000 core_module_fancy_tree_registry_app-2.8.0/core_module_fancy_tree_registry_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      873 2024-03-12 19:04:40.000000 core_module_fancy_tree_registry_app-2.8.0/core_module_fancy_tree_registry_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2024-03-12 19:04:40.000000 core_module_fancy_tree_registry_app-2.8.0/core_module_fancy_tree_registry_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       60 2024-03-12 19:04:40.000000 core_module_fancy_tree_registry_app-2.8.0/core_module_fancy_tree_registry_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       42 2024-03-12 19:04:40.000000 core_module_fancy_tree_registry_app-2.8.0/core_module_fancy_tree_registry_app.egg-info/top_level.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2024-03-12 19:04:39.000000 core_module_fancy_tree_registry_app-2.8.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       53 2024-03-12 19:04:39.000000 core_module_fancy_tree_registry_app-2.8.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        7 2024-03-12 19:04:39.000000 core_module_fancy_tree_registry_app-2.8.0/requirements.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2024-03-12 19:04:41.583533 core_module_fancy_tree_registry_app-2.8.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1104 2024-03-12 19:04:39.000000 core_module_fancy_tree_registry_app-2.8.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:41.556195 core_module_fancy_tree_registry_app-2.8.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:39.000000 core_module_fancy_tree_registry_app-2.8.0/tests/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      119 2024-03-12 19:04:39.000000 core_module_fancy_tree_registry_app-2.8.0/tests/test_settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:47.047954 core_module_fancy_tree_registry_app-2.9.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2024-05-13 16:09:44.000000 core_module_fancy_tree_registry_app-2.9.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      203 2024-05-13 16:09:44.000000 core_module_fancy_tree_registry_app-2.9.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1154 2024-05-13 16:09:47.041654 core_module_fancy_tree_registry_app-2.9.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      654 2024-05-13 16:09:44.000000 core_module_fancy_tree_registry_app-2.9.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:46.787807 core_module_fancy_tree_registry_app-2.9.0/core_module_fancy_tree_registry_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:44.000000 core_module_fancy_tree_registry_app-2.9.0/core_module_fancy_tree_registry_app/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:46.544405 core_module_fancy_tree_registry_app-2.9.0/core_module_fancy_tree_registry_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:46.549057 core_module_fancy_tree_registry_app-2.9.0/core_module_fancy_tree_registry_app/static/core_module_fancy_tree_registry_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:46.897970 core_module_fancy_tree_registry_app-2.9.0/core_module_fancy_tree_registry_app/static/core_module_fancy_tree_registry_app/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      605 2024-05-13 16:09:44.000000 core_module_fancy_tree_registry_app-2.9.0/core_module_fancy_tree_registry_app/static/core_module_fancy_tree_registry_app/js/fancy_tree.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:46.561435 core_module_fancy_tree_registry_app-2.9.0/core_module_fancy_tree_registry_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:46.914427 core_module_fancy_tree_registry_app-2.9.0/core_module_fancy_tree_registry_app/templates/core_module_fancy_tree_registry_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       89 2024-05-13 16:09:44.000000 core_module_fancy_tree_registry_app-2.9.0/core_module_fancy_tree_registry_app/templates/core_module_fancy_tree_registry_app/fancy_tree.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      316 2024-05-13 16:09:44.000000 core_module_fancy_tree_registry_app-2.9.0/core_module_fancy_tree_registry_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:46.967026 core_module_fancy_tree_registry_app-2.9.0/core_module_fancy_tree_registry_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:44.000000 core_module_fancy_tree_registry_app-2.9.0/core_module_fancy_tree_registry_app/views/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1087 2024-05-13 16:09:44.000000 core_module_fancy_tree_registry_app-2.9.0/core_module_fancy_tree_registry_app/views/forms.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6987 2024-05-13 16:09:44.000000 core_module_fancy_tree_registry_app-2.9.0/core_module_fancy_tree_registry_app/views/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:46.877507 core_module_fancy_tree_registry_app-2.9.0/core_module_fancy_tree_registry_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1154 2024-05-13 16:09:46.000000 core_module_fancy_tree_registry_app-2.9.0/core_module_fancy_tree_registry_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      873 2024-05-13 16:09:46.000000 core_module_fancy_tree_registry_app-2.9.0/core_module_fancy_tree_registry_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2024-05-13 16:09:46.000000 core_module_fancy_tree_registry_app-2.9.0/core_module_fancy_tree_registry_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       60 2024-05-13 16:09:46.000000 core_module_fancy_tree_registry_app-2.9.0/core_module_fancy_tree_registry_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       42 2024-05-13 16:09:46.000000 core_module_fancy_tree_registry_app-2.9.0/core_module_fancy_tree_registry_app.egg-info/top_level.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2024-05-13 16:09:44.000000 core_module_fancy_tree_registry_app-2.9.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       53 2024-05-13 16:09:44.000000 core_module_fancy_tree_registry_app-2.9.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        7 2024-05-13 16:09:44.000000 core_module_fancy_tree_registry_app-2.9.0/requirements.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2024-05-13 16:09:47.051064 core_module_fancy_tree_registry_app-2.9.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1104 2024-05-13 16:09:44.000000 core_module_fancy_tree_registry_app-2.9.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:47.001628 core_module_fancy_tree_registry_app-2.9.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:44.000000 core_module_fancy_tree_registry_app-2.9.0/tests/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      119 2024-05-13 16:09:44.000000 core_module_fancy_tree_registry_app-2.9.0/tests/test_settings.py
```

### Comparing `core_module_fancy_tree_registry_app-2.8.0/LICENSE.md` & `core_module_fancy_tree_registry_app-2.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `core_module_fancy_tree_registry_app-2.8.0/PKG-INFO` & `core_module_fancy_tree_registry_app-2.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_module_fancy_tree_registry_app
-Version: 2.8.0
+Version: 2.9.0
 Summary: Fancy Tree module for the parser core project
 Home-page: https://github.com/usnistgov/core_module_fancy_tree_registry_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: core_module_fancy_tree_registry_app
         ===================================
```

### Comparing `core_module_fancy_tree_registry_app-2.8.0/README.rst` & `core_module_fancy_tree_registry_app-2.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_module_fancy_tree_registry_app-2.8.0/core_module_fancy_tree_registry_app/static/core_module_fancy_tree_registry_app/js/fancy_tree.js` & `core_module_fancy_tree_registry_app-2.9.0/core_module_fancy_tree_registry_app/static/core_module_fancy_tree_registry_app/js/fancy_tree.js`

 * *Files identical despite different names*

### Comparing `core_module_fancy_tree_registry_app-2.8.0/core_module_fancy_tree_registry_app/views/forms.py` & `core_module_fancy_tree_registry_app-2.9.0/core_module_fancy_tree_registry_app/views/forms.py`

 * *Files identical despite different names*

### Comparing `core_module_fancy_tree_registry_app-2.8.0/core_module_fancy_tree_registry_app/views/views.py` & `core_module_fancy_tree_registry_app-2.9.0/core_module_fancy_tree_registry_app/views/views.py`

 * *Files identical despite different names*

### Comparing `core_module_fancy_tree_registry_app-2.8.0/core_module_fancy_tree_registry_app.egg-info/PKG-INFO` & `core_module_fancy_tree_registry_app-2.9.0/core_module_fancy_tree_registry_app.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-module-fancy-tree-registry-app
-Version: 2.8.0
+Version: 2.9.0
 Summary: Fancy Tree module for the parser core project
 Home-page: https://github.com/usnistgov/core_module_fancy_tree_registry_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: core_module_fancy_tree_registry_app
         ===================================
```

### Comparing `core_module_fancy_tree_registry_app-2.8.0/core_module_fancy_tree_registry_app.egg-info/SOURCES.txt` & `core_module_fancy_tree_registry_app-2.9.0/core_module_fancy_tree_registry_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `core_module_fancy_tree_registry_app-2.8.0/setup.py` & `core_module_fancy_tree_registry_app-2.9.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_module_fancy_tree_registry_app",
-    version="2.8.0",
+    version="2.9.0",
     description="Fancy Tree module for the parser core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_module_fancy_tree_registry_app",
     packages=find_packages(),
     include_package_data=True,
```

