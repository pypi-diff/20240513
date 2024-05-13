# Comparing `tmp/core_file_preview_app-2.8.0.tar.gz` & `tmp/core_file_preview_app-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_file_preview_app-2.8.0.tar", last modified: Tue Mar 12 19:01:26 2024, max compression
+gzip compressed data, was "core_file_preview_app-2.9.0.tar", last modified: Mon May 13 16:07:02 2024, max compression
```

## Comparing `core_file_preview_app-2.8.0.tar` & `core_file_preview_app-2.9.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:26.203075 core_file_preview_app-2.8.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2024-03-12 19:01:20.000000 core_file_preview_app-2.8.0/LICENSE.md
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      175 2024-03-12 19:01:20.000000 core_file_preview_app-2.8.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1117 2024-03-12 19:01:26.197233 core_file_preview_app-2.8.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      617 2024-03-12 19:01:20.000000 core_file_preview_app-2.8.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:24.392071 core_file_preview_app-2.8.0/core_file_preview_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:20.000000 core_file_preview_app-2.8.0/core_file_preview_app/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:22.174728 core_file_preview_app-2.8.0/core_file_preview_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:22.178636 core_file_preview_app-2.8.0/core_file_preview_app/static/core_file_preview_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:22.187857 core_file_preview_app-2.8.0/core_file_preview_app/static/core_file_preview_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:25.439999 core_file_preview_app-2.8.0/core_file_preview_app/static/core_file_preview_app/user/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      432 2024-03-12 19:01:20.000000 core_file_preview_app-2.8.0/core_file_preview_app/static/core_file_preview_app/user/css/file_preview.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:26.029126 core_file_preview_app-2.8.0/core_file_preview_app/static/core_file_preview_app/user/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5773 2024-03-12 19:01:20.000000 core_file_preview_app-2.8.0/core_file_preview_app/static/core_file_preview_app/user/js/file_preview.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       75 2024-03-12 19:01:20.000000 core_file_preview_app-2.8.0/core_file_preview_app/static/core_file_preview_app/user/js/file_preview.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:22.201619 core_file_preview_app-2.8.0/core_file_preview_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:22.205848 core_file_preview_app-2.8.0/core_file_preview_app/templates/core_file_preview_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:26.059761 core_file_preview_app-2.8.0/core_file_preview_app/templates/core_file_preview_app/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      717 2024-03-12 19:01:20.000000 core_file_preview_app-2.8.0/core_file_preview_app/templates/core_file_preview_app/user/file_preview_modal.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      295 2024-03-12 19:01:20.000000 core_file_preview_app-2.8.0/core_file_preview_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:26.082110 core_file_preview_app-2.8.0/core_file_preview_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:20.000000 core_file_preview_app-2.8.0/core_file_preview_app/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:26.129858 core_file_preview_app-2.8.0/core_file_preview_app/views/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:20.000000 core_file_preview_app-2.8.0/core_file_preview_app/views/user/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2735 2024-03-12 19:01:20.000000 core_file_preview_app-2.8.0/core_file_preview_app/views/user/ajax.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:25.403485 core_file_preview_app-2.8.0/core_file_preview_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1117 2024-03-12 19:01:21.000000 core_file_preview_app-2.8.0/core_file_preview_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      865 2024-03-12 19:01:22.000000 core_file_preview_app-2.8.0/core_file_preview_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2024-03-12 19:01:21.000000 core_file_preview_app-2.8.0/core_file_preview_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       67 2024-03-12 19:01:21.000000 core_file_preview_app-2.8.0/core_file_preview_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       28 2024-03-12 19:01:21.000000 core_file_preview_app-2.8.0/core_file_preview_app.egg-info/top_level.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2024-03-12 19:01:20.000000 core_file_preview_app-2.8.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       21 2024-03-12 19:01:20.000000 core_file_preview_app-2.8.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       46 2024-03-12 19:01:20.000000 core_file_preview_app-2.8.0/requirements.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2024-03-12 19:01:26.205615 core_file_preview_app-2.8.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1411 2024-03-12 19:01:20.000000 core_file_preview_app-2.8.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:26.181686 core_file_preview_app-2.8.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:20.000000 core_file_preview_app-2.8.0/tests/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      259 2024-03-12 19:01:20.000000 core_file_preview_app-2.8.0/tests/test_settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:02.715541 core_file_preview_app-2.9.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2024-05-13 16:07:00.000000 core_file_preview_app-2.9.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      175 2024-05-13 16:07:00.000000 core_file_preview_app-2.9.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1117 2024-05-13 16:07:02.708601 core_file_preview_app-2.9.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      617 2024-05-13 16:07:00.000000 core_file_preview_app-2.9.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:02.351760 core_file_preview_app-2.9.0/core_file_preview_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:00.000000 core_file_preview_app-2.9.0/core_file_preview_app/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:02.146348 core_file_preview_app-2.9.0/core_file_preview_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:02.151061 core_file_preview_app-2.9.0/core_file_preview_app/static/core_file_preview_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:02.161819 core_file_preview_app-2.9.0/core_file_preview_app/static/core_file_preview_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:02.505246 core_file_preview_app-2.9.0/core_file_preview_app/static/core_file_preview_app/user/css/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      432 2024-05-13 16:07:00.000000 core_file_preview_app-2.9.0/core_file_preview_app/static/core_file_preview_app/user/css/file_preview.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:02.540532 core_file_preview_app-2.9.0/core_file_preview_app/static/core_file_preview_app/user/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5773 2024-05-13 16:07:00.000000 core_file_preview_app-2.9.0/core_file_preview_app/static/core_file_preview_app/user/js/file_preview.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       75 2024-05-13 16:07:00.000000 core_file_preview_app-2.9.0/core_file_preview_app/static/core_file_preview_app/user/js/file_preview.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:02.176497 core_file_preview_app-2.9.0/core_file_preview_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:02.181034 core_file_preview_app-2.9.0/core_file_preview_app/templates/core_file_preview_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:02.595085 core_file_preview_app-2.9.0/core_file_preview_app/templates/core_file_preview_app/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      717 2024-05-13 16:07:00.000000 core_file_preview_app-2.9.0/core_file_preview_app/templates/core_file_preview_app/user/file_preview_modal.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      295 2024-05-13 16:07:00.000000 core_file_preview_app-2.9.0/core_file_preview_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:02.610052 core_file_preview_app-2.9.0/core_file_preview_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:00.000000 core_file_preview_app-2.9.0/core_file_preview_app/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:02.656818 core_file_preview_app-2.9.0/core_file_preview_app/views/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:00.000000 core_file_preview_app-2.9.0/core_file_preview_app/views/user/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2735 2024-05-13 16:07:00.000000 core_file_preview_app-2.9.0/core_file_preview_app/views/user/ajax.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:02.486360 core_file_preview_app-2.9.0/core_file_preview_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1117 2024-05-13 16:07:01.000000 core_file_preview_app-2.9.0/core_file_preview_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      865 2024-05-13 16:07:02.000000 core_file_preview_app-2.9.0/core_file_preview_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2024-05-13 16:07:01.000000 core_file_preview_app-2.9.0/core_file_preview_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       67 2024-05-13 16:07:01.000000 core_file_preview_app-2.9.0/core_file_preview_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       28 2024-05-13 16:07:01.000000 core_file_preview_app-2.9.0/core_file_preview_app.egg-info/top_level.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2024-05-13 16:07:00.000000 core_file_preview_app-2.9.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       21 2024-05-13 16:07:00.000000 core_file_preview_app-2.9.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       46 2024-05-13 16:07:00.000000 core_file_preview_app-2.9.0/requirements.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2024-05-13 16:07:02.717957 core_file_preview_app-2.9.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1411 2024-05-13 16:07:00.000000 core_file_preview_app-2.9.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:02.694608 core_file_preview_app-2.9.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:00.000000 core_file_preview_app-2.9.0/tests/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      259 2024-05-13 16:07:00.000000 core_file_preview_app-2.9.0/tests/test_settings.py
```

### Comparing `core_file_preview_app-2.8.0/LICENSE.md` & `core_file_preview_app-2.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `core_file_preview_app-2.8.0/PKG-INFO` & `core_file_preview_app-2.9.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_file_preview_app
-Version: 2.8.0
+Version: 2.9.0
 Summary: File preview functionalities for the curator core project
 Home-page: https://github.com/usnistgov/core_main_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: =====================
         Core File Preview App
```

### Comparing `core_file_preview_app-2.8.0/README.rst` & `core_file_preview_app-2.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_file_preview_app-2.8.0/core_file_preview_app/static/core_file_preview_app/user/js/file_preview.js` & `core_file_preview_app-2.9.0/core_file_preview_app/static/core_file_preview_app/user/js/file_preview.js`

 * *Files identical despite different names*

### Comparing `core_file_preview_app-2.8.0/core_file_preview_app/templates/core_file_preview_app/user/file_preview_modal.html` & `core_file_preview_app-2.9.0/core_file_preview_app/templates/core_file_preview_app/user/file_preview_modal.html`

 * *Files identical despite different names*

### Comparing `core_file_preview_app-2.8.0/core_file_preview_app/views/user/ajax.py` & `core_file_preview_app-2.9.0/core_file_preview_app/views/user/ajax.py`

 * *Files identical despite different names*

### Comparing `core_file_preview_app-2.8.0/core_file_preview_app.egg-info/PKG-INFO` & `core_file_preview_app-2.9.0/core_file_preview_app.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-file-preview-app
-Version: 2.8.0
+Version: 2.9.0
 Summary: File preview functionalities for the curator core project
 Home-page: https://github.com/usnistgov/core_main_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: =====================
         Core File Preview App
```

### Comparing `core_file_preview_app-2.8.0/core_file_preview_app.egg-info/SOURCES.txt` & `core_file_preview_app-2.9.0/core_file_preview_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `core_file_preview_app-2.8.0/setup.py` & `core_file_preview_app-2.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_file_preview_app",
-    version="2.8.0",
+    version="2.9.0",
     description="File preview functionalities for the curator core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_main_app",
     packages=find_packages(),
     include_package_data=True,
```

