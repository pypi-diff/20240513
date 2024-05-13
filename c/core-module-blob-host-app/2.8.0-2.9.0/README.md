# Comparing `tmp/core_module_blob_host_app-2.8.0.tar.gz` & `tmp/core_module_blob_host_app-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_module_blob_host_app-2.8.0.tar", last modified: Tue Mar 12 19:04:05 2024, max compression
+gzip compressed data, was "core_module_blob_host_app-2.9.0.tar", last modified: Mon May 13 16:09:12 2024, max compression
```

## Comparing `core_module_blob_host_app-2.8.0.tar` & `core_module_blob_host_app-2.9.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:05.619392 core_module_blob_host_app-2.8.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2024-03-12 19:04:03.000000 core_module_blob_host_app-2.8.0/LICENSE.md
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      183 2024-03-12 19:04:03.000000 core_module_blob_host_app-2.8.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1052 2024-03-12 19:04:05.613092 core_module_blob_host_app-2.8.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      573 2024-03-12 19:04:03.000000 core_module_blob_host_app-2.8.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:05.331326 core_module_blob_host_app-2.8.0/core_module_blob_host_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:03.000000 core_module_blob_host_app-2.8.0/core_module_blob_host_app/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      621 2024-03-12 19:04:03.000000 core_module_blob_host_app-2.8.0/core_module_blob_host_app/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:05.154431 core_module_blob_host_app-2.8.0/core_module_blob_host_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:05.158048 core_module_blob_host_app-2.8.0/core_module_blob_host_app/static/core_module_blob_host_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:05.426223 core_module_blob_host_app-2.8.0/core_module_blob_host_app/static/core_module_blob_host_app/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      347 2024-03-12 19:04:03.000000 core_module_blob_host_app-2.8.0/core_module_blob_host_app/static/core_module_blob_host_app/js/blob_host.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:05.177022 core_module_blob_host_app-2.8.0/core_module_blob_host_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:05.453512 core_module_blob_host_app-2.8.0/core_module_blob_host_app/templates/core_module_blob_host_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      156 2024-03-12 19:04:03.000000 core_module_blob_host_app-2.8.0/core_module_blob_host_app/templates/core_module_blob_host_app/blob_host.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      533 2024-03-12 19:04:03.000000 core_module_blob_host_app-2.8.0/core_module_blob_host_app/templates/core_module_blob_host_app/blob_host_display.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      288 2024-03-12 19:04:03.000000 core_module_blob_host_app-2.8.0/core_module_blob_host_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:05.499508 core_module_blob_host_app-2.8.0/core_module_blob_host_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:03.000000 core_module_blob_host_app-2.8.0/core_module_blob_host_app/views/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      152 2024-03-12 19:04:03.000000 core_module_blob_host_app-2.8.0/core_module_blob_host_app/views/forms.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5796 2024-03-12 19:04:03.000000 core_module_blob_host_app-2.8.0/core_module_blob_host_app/views/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:05.409433 core_module_blob_host_app-2.8.0/core_module_blob_host_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1052 2024-03-12 19:04:04.000000 core_module_blob_host_app-2.8.0/core_module_blob_host_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      940 2024-03-12 19:04:05.000000 core_module_blob_host_app-2.8.0/core_module_blob_host_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2024-03-12 19:04:04.000000 core_module_blob_host_app-2.8.0/core_module_blob_host_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       51 2024-03-12 19:04:04.000000 core_module_blob_host_app-2.8.0/core_module_blob_host_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       32 2024-03-12 19:04:04.000000 core_module_blob_host_app-2.8.0/core_module_blob_host_app.egg-info/top_level.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2024-03-12 19:04:03.000000 core_module_blob_host_app-2.8.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       44 2024-03-12 19:04:03.000000 core_module_blob_host_app-2.8.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        7 2024-03-12 19:04:03.000000 core_module_blob_host_app-2.8.0/requirements.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2024-03-12 19:04:05.621820 core_module_blob_host_app-2.8.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1073 2024-03-12 19:04:03.000000 core_module_blob_host_app-2.8.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:05.533352 core_module_blob_host_app-2.8.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:03.000000 core_module_blob_host_app-2.8.0/tests/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1849 2024-03-12 19:04:03.000000 core_module_blob_host_app-2.8.0/tests/test_settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:05.559339 core_module_blob_host_app-2.8.0/tests/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:03.000000 core_module_blob_host_app-2.8.0/tests/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:05.600023 core_module_blob_host_app-2.8.0/tests/views/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:04:03.000000 core_module_blob_host_app-2.8.0/tests/views/views/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6574 2024-03-12 19:04:03.000000 core_module_blob_host_app-2.8.0/tests/views/views/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:11.991838 core_module_blob_host_app-2.9.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2024-05-13 16:09:09.000000 core_module_blob_host_app-2.9.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      183 2024-05-13 16:09:09.000000 core_module_blob_host_app-2.9.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1052 2024-05-13 16:09:11.984833 core_module_blob_host_app-2.9.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      573 2024-05-13 16:09:09.000000 core_module_blob_host_app-2.9.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:11.654225 core_module_blob_host_app-2.9.0/core_module_blob_host_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:09.000000 core_module_blob_host_app-2.9.0/core_module_blob_host_app/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      621 2024-05-13 16:09:09.000000 core_module_blob_host_app-2.9.0/core_module_blob_host_app/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:11.429375 core_module_blob_host_app-2.9.0/core_module_blob_host_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:11.433650 core_module_blob_host_app-2.9.0/core_module_blob_host_app/static/core_module_blob_host_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:11.775663 core_module_blob_host_app-2.9.0/core_module_blob_host_app/static/core_module_blob_host_app/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      347 2024-05-13 16:09:09.000000 core_module_blob_host_app-2.9.0/core_module_blob_host_app/static/core_module_blob_host_app/js/blob_host.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:11.445297 core_module_blob_host_app-2.9.0/core_module_blob_host_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:11.808725 core_module_blob_host_app-2.9.0/core_module_blob_host_app/templates/core_module_blob_host_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      156 2024-05-13 16:09:09.000000 core_module_blob_host_app-2.9.0/core_module_blob_host_app/templates/core_module_blob_host_app/blob_host.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      533 2024-05-13 16:09:09.000000 core_module_blob_host_app-2.9.0/core_module_blob_host_app/templates/core_module_blob_host_app/blob_host_display.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      288 2024-05-13 16:09:09.000000 core_module_blob_host_app-2.9.0/core_module_blob_host_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:11.861755 core_module_blob_host_app-2.9.0/core_module_blob_host_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:09.000000 core_module_blob_host_app-2.9.0/core_module_blob_host_app/views/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      152 2024-05-13 16:09:09.000000 core_module_blob_host_app-2.9.0/core_module_blob_host_app/views/forms.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5796 2024-05-13 16:09:09.000000 core_module_blob_host_app-2.9.0/core_module_blob_host_app/views/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:11.754678 core_module_blob_host_app-2.9.0/core_module_blob_host_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1052 2024-05-13 16:09:10.000000 core_module_blob_host_app-2.9.0/core_module_blob_host_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      940 2024-05-13 16:09:11.000000 core_module_blob_host_app-2.9.0/core_module_blob_host_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2024-05-13 16:09:11.000000 core_module_blob_host_app-2.9.0/core_module_blob_host_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       51 2024-05-13 16:09:11.000000 core_module_blob_host_app-2.9.0/core_module_blob_host_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       32 2024-05-13 16:09:11.000000 core_module_blob_host_app-2.9.0/core_module_blob_host_app.egg-info/top_level.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2024-05-13 16:09:09.000000 core_module_blob_host_app-2.9.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       44 2024-05-13 16:09:09.000000 core_module_blob_host_app-2.9.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        7 2024-05-13 16:09:09.000000 core_module_blob_host_app-2.9.0/requirements.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2024-05-13 16:09:11.994786 core_module_blob_host_app-2.9.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1073 2024-05-13 16:09:09.000000 core_module_blob_host_app-2.9.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:11.898618 core_module_blob_host_app-2.9.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:09.000000 core_module_blob_host_app-2.9.0/tests/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1849 2024-05-13 16:09:09.000000 core_module_blob_host_app-2.9.0/tests/test_settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:11.914674 core_module_blob_host_app-2.9.0/tests/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:09.000000 core_module_blob_host_app-2.9.0/tests/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:11.957810 core_module_blob_host_app-2.9.0/tests/views/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:09:09.000000 core_module_blob_host_app-2.9.0/tests/views/views/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6574 2024-05-13 16:09:09.000000 core_module_blob_host_app-2.9.0/tests/views/views/tests_unit.py
```

### Comparing `core_module_blob_host_app-2.8.0/LICENSE.md` & `core_module_blob_host_app-2.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `core_module_blob_host_app-2.8.0/PKG-INFO` & `core_module_blob_host_app-2.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_module_blob_host_app
-Version: 2.8.0
+Version: 2.9.0
 Summary: Blob Host module for the parser core project
 Home-page: https://github.com/usnistgov/core_module_blob_host_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: core_module_blob_host_app
         =========================
```

### Comparing `core_module_blob_host_app-2.8.0/README.rst` & `core_module_blob_host_app-2.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_module_blob_host_app-2.8.0/core_module_blob_host_app/settings.py` & `core_module_blob_host_app-2.9.0/core_module_blob_host_app/settings.py`

 * *Files identical despite different names*

### Comparing `core_module_blob_host_app-2.8.0/core_module_blob_host_app/templates/core_module_blob_host_app/blob_host_display.html` & `core_module_blob_host_app-2.9.0/core_module_blob_host_app/templates/core_module_blob_host_app/blob_host_display.html`

 * *Files identical despite different names*

### Comparing `core_module_blob_host_app-2.8.0/core_module_blob_host_app/views/views.py` & `core_module_blob_host_app-2.9.0/core_module_blob_host_app/views/views.py`

 * *Files identical despite different names*

### Comparing `core_module_blob_host_app-2.8.0/core_module_blob_host_app.egg-info/PKG-INFO` & `core_module_blob_host_app-2.9.0/core_module_blob_host_app.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-module-blob-host-app
-Version: 2.8.0
+Version: 2.9.0
 Summary: Blob Host module for the parser core project
 Home-page: https://github.com/usnistgov/core_module_blob_host_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: core_module_blob_host_app
         =========================
```

### Comparing `core_module_blob_host_app-2.8.0/core_module_blob_host_app.egg-info/SOURCES.txt` & `core_module_blob_host_app-2.9.0/core_module_blob_host_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `core_module_blob_host_app-2.8.0/setup.py` & `core_module_blob_host_app-2.9.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_module_blob_host_app",
-    version="2.8.0",
+    version="2.9.0",
     description="Blob Host module for the parser core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_module_blob_host_app",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `core_module_blob_host_app-2.8.0/tests/test_settings.py` & `core_module_blob_host_app-2.9.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `core_module_blob_host_app-2.8.0/tests/views/views/tests_unit.py` & `core_module_blob_host_app-2.9.0/tests/views/views/tests_unit.py`

 * *Files identical despite different names*

