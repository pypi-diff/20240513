# Comparing `tmp/gcix-0.0.8.tar.gz` & `tmp/gcix-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gcix-0.0.8.tar", last modified: Fri Aug 11 13:25:17 2023, max compression
+gzip compressed data, was "gcix-0.0.9.tar", last modified: Fri Aug 11 16:32:21 2023, max compression
```

## Comparing `gcix-0.0.8.tar` & `gcix-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-11 13:25:17.512868 gcix-0.0.8/
--rw-r--r--   0 root         (0) root         (0)    11358 2023-08-11 13:25:09.000000 gcix-0.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2023-08-11 13:25:09.000000 gcix-0.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8533 2023-08-11 13:25:17.512868 gcix-0.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7612 2023-08-11 13:25:09.000000 gcix-0.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2023-08-11 13:25:09.000000 gcix-0.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-11 13:25:17.512868 gcix-0.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1682 2023-08-11 13:25:09.000000 gcix-0.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-11 13:25:17.505868 gcix-0.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-11 13:25:17.507868 gcix-0.0.8/src/gcix/
--rw-r--r--   0 root         (0) root         (0)   441194 2023-08-11 13:25:09.000000 gcix-0.0.8/src/gcix/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-11 13:25:17.507868 gcix-0.0.8/src/gcix/_jsii/
--rw-r--r--   0 root         (0) root         (0)      337 2023-08-11 13:25:09.000000 gcix-0.0.8/src/gcix/_jsii/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-11 13:25:17.512868 gcix-0.0.8/src/gcix/_jsii/bin/
--rw-r--r--   0 root         (0) root         (0)      256 2023-08-11 13:25:09.000000 gcix-0.0.8/src/gcix/_jsii/bin/cfnwaiter
--rw-r--r--   0 root         (0) root         (0)  1680165 2023-08-11 13:25:09.000000 gcix-0.0.8/src/gcix/_jsii/gcix@v0.0.8.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-11 13:25:09.000000 gcix-0.0.8/src/gcix/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-11 13:25:17.507868 gcix-0.0.8/src/gcix.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8533 2023-08-11 13:25:17.000000 gcix-0.0.8/src/gcix.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      343 2023-08-11 13:25:17.000000 gcix-0.0.8/src/gcix.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-11 13:25:17.000000 gcix-0.0.8/src/gcix.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       57 2023-08-11 13:25:17.000000 gcix-0.0.8/src/gcix.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-08-11 13:25:17.000000 gcix-0.0.8/src/gcix.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-11 16:32:21.554008 gcix-0.0.9/
+-rw-r--r--   0 root         (0) root         (0)    11358 2023-08-11 16:32:14.000000 gcix-0.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2023-08-11 16:32:14.000000 gcix-0.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8533 2023-08-11 16:32:21.553008 gcix-0.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7612 2023-08-11 16:32:14.000000 gcix-0.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      234 2023-08-11 16:32:14.000000 gcix-0.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-11 16:32:21.554008 gcix-0.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1682 2023-08-11 16:32:14.000000 gcix-0.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-11 16:32:21.545008 gcix-0.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-11 16:32:21.547008 gcix-0.0.9/src/gcix/
+-rw-r--r--   0 root         (0) root         (0)   441194 2023-08-11 16:32:14.000000 gcix-0.0.9/src/gcix/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-11 16:32:21.548008 gcix-0.0.9/src/gcix/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      337 2023-08-11 16:32:14.000000 gcix-0.0.9/src/gcix/_jsii/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-11 16:32:21.553008 gcix-0.0.9/src/gcix/_jsii/bin/
+-rw-r--r--   0 root         (0) root         (0)      256 2023-08-11 16:32:14.000000 gcix-0.0.9/src/gcix/_jsii/bin/cfnwaiter
+-rw-r--r--   0 root         (0) root         (0)  1680283 2023-08-11 16:32:14.000000 gcix-0.0.9/src/gcix/_jsii/gcix@v0.0.9.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-11 16:32:14.000000 gcix-0.0.9/src/gcix/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-11 16:32:21.548008 gcix-0.0.9/src/gcix.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8533 2023-08-11 16:32:21.000000 gcix-0.0.9/src/gcix.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      343 2023-08-11 16:32:21.000000 gcix-0.0.9/src/gcix.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-11 16:32:21.000000 gcix-0.0.9/src/gcix.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2023-08-11 16:32:21.000000 gcix-0.0.9/src/gcix.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-08-11 16:32:21.000000 gcix-0.0.9/src/gcix.egg-info/top_level.txt
```

### Comparing `gcix-0.0.8/LICENSE` & `gcix-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gcix-0.0.8/PKG-INFO` & `gcix-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gcix
-Version: 0.0.8
+Version: 0.0.9
 Summary: GitLab CI X Library (X stands for multilanguage)
 Home-page: https://gitlab.com/gcix/gcix.git
 Author: Daniel von Essen<daniel@vonessen.eu>
 License: Apache-2.0
 Project-URL: Source, https://gitlab.com/gcix/gcix.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gcix-0.0.8/README.md` & `gcix-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `gcix-0.0.8/setup.py` & `gcix-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "gcix",
-    "version": "v0.0.8",
+    "version": "v0.0.9",
     "description": "GitLab CI X Library (X stands for multilanguage)",
     "license": "Apache-2.0",
     "url": "https://gitlab.com/gcix/gcix.git",
     "long_description_content_type": "text/markdown",
     "author": "Daniel von Essen<daniel@vonessen.eu>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "gcix",
         "gcix._jsii"
     ],
     "package_data": {
         "gcix._jsii": [
-            "gcix@v0.0.8.jsii.tgz"
+            "gcix@v0.0.9.jsii.tgz"
         ],
         "gcix": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `gcix-0.0.8/src/gcix/__init__.py` & `gcix-0.0.9/src/gcix/__init__.py`

 * *Files identical despite different names*

### Comparing `gcix-0.0.8/src/gcix.egg-info/PKG-INFO` & `gcix-0.0.9/src/gcix.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gcix
-Version: 0.0.8
+Version: 0.0.9
 Summary: GitLab CI X Library (X stands for multilanguage)
 Home-page: https://gitlab.com/gcix/gcix.git
 Author: Daniel von Essen<daniel@vonessen.eu>
 License: Apache-2.0
 Project-URL: Source, https://gitlab.com/gcix/gcix.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

