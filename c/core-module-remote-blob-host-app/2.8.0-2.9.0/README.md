# Comparing `tmp/core_module_remote_blob_host_app-2.8.0.tar.gz` & `tmp/core_module_remote_blob_host_app-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_module_remote_blob_host_app-2.8.0.tar", last modified: Tue Mar 12 19:05:15 2024, max compression
+gzip compressed data, was "core_module_remote_blob_host_app-2.9.0.tar", last modified: Mon May 13 16:10:19 2024, max compression
```

## Comparing `core_module_remote_blob_host_app-2.8.0.tar` & `core_module_remote_blob_host_app-2.9.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:15.817958 core_module_remote_blob_host_app-2.8.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2024-03-12 19:05:13.000000 core_module_remote_blob_host_app-2.8.0/LICENSE.md
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      197 2024-03-12 19:05:13.000000 core_module_remote_blob_host_app-2.8.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1136 2024-03-12 19:05:15.812064 core_module_remote_blob_host_app-2.8.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      636 2024-03-12 19:05:13.000000 core_module_remote_blob_host_app-2.8.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:15.618132 core_module_remote_blob_host_app-2.8.0/core_module_remote_blob_host_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:13.000000 core_module_remote_blob_host_app-2.8.0/core_module_remote_blob_host_app/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      435 2024-03-12 19:05:13.000000 core_module_remote_blob_host_app-2.8.0/core_module_remote_blob_host_app/settings.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      328 2024-03-12 19:05:13.000000 core_module_remote_blob_host_app-2.8.0/core_module_remote_blob_host_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:15.764496 core_module_remote_blob_host_app-2.8.0/core_module_remote_blob_host_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:13.000000 core_module_remote_blob_host_app-2.8.0/core_module_remote_blob_host_app/views/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      157 2024-03-12 19:05:13.000000 core_module_remote_blob_host_app-2.8.0/core_module_remote_blob_host_app/views/forms.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1903 2024-03-12 19:05:13.000000 core_module_remote_blob_host_app-2.8.0/core_module_remote_blob_host_app/views/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:15.708855 core_module_remote_blob_host_app-2.8.0/core_module_remote_blob_host_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1136 2024-03-12 19:05:15.000000 core_module_remote_blob_host_app-2.8.0/core_module_remote_blob_host_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      694 2024-03-12 19:05:15.000000 core_module_remote_blob_host_app-2.8.0/core_module_remote_blob_host_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2024-03-12 19:05:15.000000 core_module_remote_blob_host_app-2.8.0/core_module_remote_blob_host_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       84 2024-03-12 19:05:15.000000 core_module_remote_blob_host_app-2.8.0/core_module_remote_blob_host_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       39 2024-03-12 19:05:15.000000 core_module_remote_blob_host_app-2.8.0/core_module_remote_blob_host_app.egg-info/top_level.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2024-03-12 19:05:13.000000 core_module_remote_blob_host_app-2.8.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2024-03-12 19:05:13.000000 core_module_remote_blob_host_app-2.8.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        7 2024-03-12 19:05:13.000000 core_module_remote_blob_host_app-2.8.0/requirements.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2024-03-12 19:05:15.820031 core_module_remote_blob_host_app-2.8.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1101 2024-03-12 19:05:13.000000 core_module_remote_blob_host_app-2.8.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:15.799364 core_module_remote_blob_host_app-2.8.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:13.000000 core_module_remote_blob_host_app-2.8.0/tests/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      119 2024-03-12 19:05:13.000000 core_module_remote_blob_host_app-2.8.0/tests/test_settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:19.899100 core_module_remote_blob_host_app-2.9.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2024-05-13 16:10:17.000000 core_module_remote_blob_host_app-2.9.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      197 2024-05-13 16:10:17.000000 core_module_remote_blob_host_app-2.9.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1136 2024-05-13 16:10:19.893326 core_module_remote_blob_host_app-2.9.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      636 2024-05-13 16:10:17.000000 core_module_remote_blob_host_app-2.9.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:19.684598 core_module_remote_blob_host_app-2.9.0/core_module_remote_blob_host_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:17.000000 core_module_remote_blob_host_app-2.9.0/core_module_remote_blob_host_app/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      435 2024-05-13 16:10:17.000000 core_module_remote_blob_host_app-2.9.0/core_module_remote_blob_host_app/settings.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      328 2024-05-13 16:10:17.000000 core_module_remote_blob_host_app-2.9.0/core_module_remote_blob_host_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:19.823679 core_module_remote_blob_host_app-2.9.0/core_module_remote_blob_host_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:17.000000 core_module_remote_blob_host_app-2.9.0/core_module_remote_blob_host_app/views/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      157 2024-05-13 16:10:17.000000 core_module_remote_blob_host_app-2.9.0/core_module_remote_blob_host_app/views/forms.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1903 2024-05-13 16:10:17.000000 core_module_remote_blob_host_app-2.9.0/core_module_remote_blob_host_app/views/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:19.766196 core_module_remote_blob_host_app-2.9.0/core_module_remote_blob_host_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1136 2024-05-13 16:10:19.000000 core_module_remote_blob_host_app-2.9.0/core_module_remote_blob_host_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      694 2024-05-13 16:10:19.000000 core_module_remote_blob_host_app-2.9.0/core_module_remote_blob_host_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2024-05-13 16:10:19.000000 core_module_remote_blob_host_app-2.9.0/core_module_remote_blob_host_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       84 2024-05-13 16:10:19.000000 core_module_remote_blob_host_app-2.9.0/core_module_remote_blob_host_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       39 2024-05-13 16:10:19.000000 core_module_remote_blob_host_app-2.9.0/core_module_remote_blob_host_app.egg-info/top_level.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2024-05-13 16:10:17.000000 core_module_remote_blob_host_app-2.9.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2024-05-13 16:10:17.000000 core_module_remote_blob_host_app-2.9.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        7 2024-05-13 16:10:17.000000 core_module_remote_blob_host_app-2.9.0/requirements.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2024-05-13 16:10:19.901261 core_module_remote_blob_host_app-2.9.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1101 2024-05-13 16:10:18.000000 core_module_remote_blob_host_app-2.9.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:19.866808 core_module_remote_blob_host_app-2.9.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:18.000000 core_module_remote_blob_host_app-2.9.0/tests/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      119 2024-05-13 16:10:18.000000 core_module_remote_blob_host_app-2.9.0/tests/test_settings.py
```

### Comparing `core_module_remote_blob_host_app-2.8.0/LICENSE.md` & `core_module_remote_blob_host_app-2.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `core_module_remote_blob_host_app-2.8.0/PKG-INFO` & `core_module_remote_blob_host_app-2.9.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_module_remote_blob_host_app
-Version: 2.8.0
+Version: 2.9.0
 Summary: Remote Blob Host module for the parser core project
 Home-page: https://github.com/usnistgov/core_module_remote_blob_host_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: core_module_remote_blob_host_app
         ================================
```

### Comparing `core_module_remote_blob_host_app-2.8.0/README.rst` & `core_module_remote_blob_host_app-2.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_module_remote_blob_host_app-2.8.0/core_module_remote_blob_host_app/views/views.py` & `core_module_remote_blob_host_app-2.9.0/core_module_remote_blob_host_app/views/views.py`

 * *Files identical despite different names*

### Comparing `core_module_remote_blob_host_app-2.8.0/core_module_remote_blob_host_app.egg-info/PKG-INFO` & `core_module_remote_blob_host_app-2.9.0/core_module_remote_blob_host_app.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-module-remote-blob-host-app
-Version: 2.8.0
+Version: 2.9.0
 Summary: Remote Blob Host module for the parser core project
 Home-page: https://github.com/usnistgov/core_module_remote_blob_host_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: core_module_remote_blob_host_app
         ================================
```

### Comparing `core_module_remote_blob_host_app-2.8.0/core_module_remote_blob_host_app.egg-info/SOURCES.txt` & `core_module_remote_blob_host_app-2.9.0/core_module_remote_blob_host_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `core_module_remote_blob_host_app-2.8.0/setup.py` & `core_module_remote_blob_host_app-2.9.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_module_remote_blob_host_app",
-    version="2.8.0",
+    version="2.9.0",
     description="Remote Blob Host module for the parser core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_module_remote_blob_host_app",
     packages=find_packages(),
     include_package_data=True,
```

