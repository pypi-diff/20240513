# Comparing `tmp/core_module_advanced_blob_host_app-2.8.0.tar.gz` & `tmp/core_module_advanced_blob_host_app-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_module_advanced_blob_host_app-2.8.0.tar", last modified: Tue Mar 12 19:03:57 2024, max compression
+gzip compressed data, was "core_module_advanced_blob_host_app-2.9.0.tar", last modified: Mon May 13 16:09:03 2024, max compression
```

## Comparing `core_module_advanced_blob_host_app-2.8.0.tar` & `core_module_advanced_blob_host_app-2.9.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:57.387974 core_module_advanced_blob_host_app-2.8.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2024-03-12 19:03:54.000000 core_module_advanced_blob_host_app-2.8.0/LICENSE.md
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      201 2024-03-12 19:03:54.000000 core_module_advanced_blob_host_app-2.8.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1160 2024-03-12 19:03:57.380964 core_module_advanced_blob_host_app-2.8.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      654 2024-03-12 19:03:54.000000 core_module_advanced_blob_host_app-2.8.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:57.141284 core_module_advanced_blob_host_app-2.8.0/core_module_advanced_blob_host_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:55.000000 core_module_advanced_blob_host_app-2.8.0/core_module_advanced_blob_host_app/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      437 2024-03-12 19:03:55.000000 core_module_advanced_blob_host_app-2.8.0/core_module_advanced_blob_host_app/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:56.935489 core_module_advanced_blob_host_app-2.8.0/core_module_advanced_blob_host_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:56.946572 core_module_advanced_blob_host_app-2.8.0/core_module_advanced_blob_host_app/static/core_module_advanced_blob_host_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:57.254252 core_module_advanced_blob_host_app-2.8.0/core_module_advanced_blob_host_app/static/core_module_advanced_blob_host_app/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      616 2024-03-12 19:03:55.000000 core_module_advanced_blob_host_app-2.8.0/core_module_advanced_blob_host_app/static/core_module_advanced_blob_host_app/css/advanced_blob_host.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:57.271515 core_module_advanced_blob_host_app-2.8.0/core_module_advanced_blob_host_app/static/core_module_advanced_blob_host_app/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      387 2024-03-12 19:03:55.000000 core_module_advanced_blob_host_app-2.8.0/core_module_advanced_blob_host_app/static/core_module_advanced_blob_host_app/js/advanced_blob_host.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:56.959573 core_module_advanced_blob_host_app-2.8.0/core_module_advanced_blob_host_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:57.289810 core_module_advanced_blob_host_app-2.8.0/core_module_advanced_blob_host_app/templates/core_module_advanced_blob_host_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      807 2024-03-12 19:03:55.000000 core_module_advanced_blob_host_app-2.8.0/core_module_advanced_blob_host_app/templates/core_module_advanced_blob_host_app/advanced_blob_host.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      349 2024-03-12 19:03:55.000000 core_module_advanced_blob_host_app-2.8.0/core_module_advanced_blob_host_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:57.329228 core_module_advanced_blob_host_app-2.8.0/core_module_advanced_blob_host_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:55.000000 core_module_advanced_blob_host_app-2.8.0/core_module_advanced_blob_host_app/views/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3032 2024-03-12 19:03:55.000000 core_module_advanced_blob_host_app-2.8.0/core_module_advanced_blob_host_app/views/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:57.232946 core_module_advanced_blob_host_app-2.8.0/core_module_advanced_blob_host_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1160 2024-03-12 19:03:56.000000 core_module_advanced_blob_host_app-2.8.0/core_module_advanced_blob_host_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      976 2024-03-12 19:03:56.000000 core_module_advanced_blob_host_app-2.8.0/core_module_advanced_blob_host_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2024-03-12 19:03:56.000000 core_module_advanced_blob_host_app-2.8.0/core_module_advanced_blob_host_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      124 2024-03-12 19:03:56.000000 core_module_advanced_blob_host_app-2.8.0/core_module_advanced_blob_host_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       41 2024-03-12 19:03:56.000000 core_module_advanced_blob_host_app-2.8.0/core_module_advanced_blob_host_app.egg-info/top_level.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2024-03-12 19:03:55.000000 core_module_advanced_blob_host_app-2.8.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      117 2024-03-12 19:03:55.000000 core_module_advanced_blob_host_app-2.8.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        7 2024-03-12 19:03:55.000000 core_module_advanced_blob_host_app-2.8.0/requirements.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2024-03-12 19:03:57.390510 core_module_advanced_blob_host_app-2.8.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1104 2024-03-12 19:03:55.000000 core_module_advanced_blob_host_app-2.8.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:57.367182 core_module_advanced_blob_host_app-2.8.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:55.000000 core_module_advanced_blob_host_app-2.8.0/tests/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      119 2024-03-12 19:03:55.000000 core_module_advanced_blob_host_app-2.8.0/tests/test_settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:03.497676 core_module_advanced_blob_host_app-2.9.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2024-05-13 16:08:56.000000 core_module_advanced_blob_host_app-2.9.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      201 2024-05-13 16:08:56.000000 core_module_advanced_blob_host_app-2.9.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1160 2024-05-13 16:09:03.491003 core_module_advanced_blob_host_app-2.9.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      654 2024-05-13 16:08:56.000000 core_module_advanced_blob_host_app-2.9.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:03.237227 core_module_advanced_blob_host_app-2.9.0/core_module_advanced_blob_host_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:56.000000 core_module_advanced_blob_host_app-2.9.0/core_module_advanced_blob_host_app/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      437 2024-05-13 16:08:56.000000 core_module_advanced_blob_host_app-2.9.0/core_module_advanced_blob_host_app/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:02.736841 core_module_advanced_blob_host_app-2.9.0/core_module_advanced_blob_host_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:02.774673 core_module_advanced_blob_host_app-2.9.0/core_module_advanced_blob_host_app/static/core_module_advanced_blob_host_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:03.353897 core_module_advanced_blob_host_app-2.9.0/core_module_advanced_blob_host_app/static/core_module_advanced_blob_host_app/css/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      616 2024-05-13 16:08:56.000000 core_module_advanced_blob_host_app-2.9.0/core_module_advanced_blob_host_app/static/core_module_advanced_blob_host_app/css/advanced_blob_host.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:03.368632 core_module_advanced_blob_host_app-2.9.0/core_module_advanced_blob_host_app/static/core_module_advanced_blob_host_app/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      387 2024-05-13 16:08:56.000000 core_module_advanced_blob_host_app-2.9.0/core_module_advanced_blob_host_app/static/core_module_advanced_blob_host_app/js/advanced_blob_host.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:02.787814 core_module_advanced_blob_host_app-2.9.0/core_module_advanced_blob_host_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:03.386510 core_module_advanced_blob_host_app-2.9.0/core_module_advanced_blob_host_app/templates/core_module_advanced_blob_host_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      807 2024-05-13 16:08:56.000000 core_module_advanced_blob_host_app-2.9.0/core_module_advanced_blob_host_app/templates/core_module_advanced_blob_host_app/advanced_blob_host.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      349 2024-05-13 16:08:56.000000 core_module_advanced_blob_host_app-2.9.0/core_module_advanced_blob_host_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:03.428994 core_module_advanced_blob_host_app-2.9.0/core_module_advanced_blob_host_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:56.000000 core_module_advanced_blob_host_app-2.9.0/core_module_advanced_blob_host_app/views/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3032 2024-05-13 16:08:56.000000 core_module_advanced_blob_host_app-2.9.0/core_module_advanced_blob_host_app/views/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:03.331599 core_module_advanced_blob_host_app-2.9.0/core_module_advanced_blob_host_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1160 2024-05-13 16:09:00.000000 core_module_advanced_blob_host_app-2.9.0/core_module_advanced_blob_host_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      976 2024-05-13 16:09:02.000000 core_module_advanced_blob_host_app-2.9.0/core_module_advanced_blob_host_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2024-05-13 16:09:00.000000 core_module_advanced_blob_host_app-2.9.0/core_module_advanced_blob_host_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      124 2024-05-13 16:09:00.000000 core_module_advanced_blob_host_app-2.9.0/core_module_advanced_blob_host_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       41 2024-05-13 16:09:00.000000 core_module_advanced_blob_host_app-2.9.0/core_module_advanced_blob_host_app.egg-info/top_level.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2024-05-13 16:08:56.000000 core_module_advanced_blob_host_app-2.9.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      117 2024-05-13 16:08:56.000000 core_module_advanced_blob_host_app-2.9.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        7 2024-05-13 16:08:56.000000 core_module_advanced_blob_host_app-2.9.0/requirements.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2024-05-13 16:09:03.500409 core_module_advanced_blob_host_app-2.9.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1104 2024-05-13 16:08:56.000000 core_module_advanced_blob_host_app-2.9.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:03.468392 core_module_advanced_blob_host_app-2.9.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:56.000000 core_module_advanced_blob_host_app-2.9.0/tests/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      119 2024-05-13 16:08:56.000000 core_module_advanced_blob_host_app-2.9.0/tests/test_settings.py
```

### Comparing `core_module_advanced_blob_host_app-2.8.0/LICENSE.md` & `core_module_advanced_blob_host_app-2.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `core_module_advanced_blob_host_app-2.8.0/PKG-INFO` & `core_module_advanced_blob_host_app-2.9.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_module_advanced_blob_host_app
-Version: 2.8.0
+Version: 2.9.0
 Summary: Advanced Blob Host module for the parser core project
 Home-page: https://github.com/usnistgov/core_module_advanced_blob_host_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: core_module_advanced_blob_host_app
         ==================================
```

### Comparing `core_module_advanced_blob_host_app-2.8.0/README.rst` & `core_module_advanced_blob_host_app-2.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_module_advanced_blob_host_app-2.8.0/core_module_advanced_blob_host_app/static/core_module_advanced_blob_host_app/css/advanced_blob_host.css` & `core_module_advanced_blob_host_app-2.9.0/core_module_advanced_blob_host_app/static/core_module_advanced_blob_host_app/css/advanced_blob_host.css`

 * *Files identical despite different names*

### Comparing `core_module_advanced_blob_host_app-2.8.0/core_module_advanced_blob_host_app/templates/core_module_advanced_blob_host_app/advanced_blob_host.html` & `core_module_advanced_blob_host_app-2.9.0/core_module_advanced_blob_host_app/templates/core_module_advanced_blob_host_app/advanced_blob_host.html`

 * *Files identical despite different names*

### Comparing `core_module_advanced_blob_host_app-2.8.0/core_module_advanced_blob_host_app/views/views.py` & `core_module_advanced_blob_host_app-2.9.0/core_module_advanced_blob_host_app/views/views.py`

 * *Files identical despite different names*

### Comparing `core_module_advanced_blob_host_app-2.8.0/core_module_advanced_blob_host_app.egg-info/PKG-INFO` & `core_module_advanced_blob_host_app-2.9.0/core_module_advanced_blob_host_app.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-module-advanced-blob-host-app
-Version: 2.8.0
+Version: 2.9.0
 Summary: Advanced Blob Host module for the parser core project
 Home-page: https://github.com/usnistgov/core_module_advanced_blob_host_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: core_module_advanced_blob_host_app
         ==================================
```

### Comparing `core_module_advanced_blob_host_app-2.8.0/core_module_advanced_blob_host_app.egg-info/SOURCES.txt` & `core_module_advanced_blob_host_app-2.9.0/core_module_advanced_blob_host_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `core_module_advanced_blob_host_app-2.8.0/setup.py` & `core_module_advanced_blob_host_app-2.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_module_advanced_blob_host_app",
-    version="2.8.0",
+    version="2.9.0",
     description="Advanced Blob Host module for the parser core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_module_advanced_blob_host_app",
     packages=find_packages(),
     include_package_data=True,
```

