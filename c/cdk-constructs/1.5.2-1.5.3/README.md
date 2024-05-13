# Comparing `tmp/cdk-constructs-1.5.2.tar.gz` & `tmp/cdk-constructs-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-constructs-1.5.2.tar", last modified: Mon May 13 16:34:04 2024, max compression
+gzip compressed data, was "cdk-constructs-1.5.3.tar", last modified: Mon May 13 18:47:49 2024, max compression
```

## Comparing `cdk-constructs-1.5.2.tar` & `cdk-constructs-1.5.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:34:04.684748 cdk-constructs-1.5.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-13 16:33:53.000000 cdk-constructs-1.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-13 16:33:53.000000 cdk-constructs-1.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-05-13 16:34:04.684748 cdk-constructs-1.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-05-13 16:33:53.000000 cdk-constructs-1.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-13 16:33:53.000000 cdk-constructs-1.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 16:34:04.684748 cdk-constructs-1.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-13 16:33:53.000000 cdk-constructs-1.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:34:04.684748 cdk-constructs-1.5.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:34:04.684748 cdk-constructs-1.5.2/src/cdk-constructs/
--rw-r--r--   0 runner    (1001) docker     (127)     6459 2024-05-13 16:33:53.000000 cdk-constructs-1.5.2/src/cdk-constructs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:34:04.684748 cdk-constructs-1.5.2/src/cdk-constructs/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-13 16:33:53.000000 cdk-constructs-1.5.2/src/cdk-constructs/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33590 2024-05-13 16:33:53.000000 cdk-constructs-1.5.2/src/cdk-constructs/_jsii/cdk-constructs@1.5.2.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 16:33:53.000000 cdk-constructs-1.5.2/src/cdk-constructs/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:34:04.684748 cdk-constructs-1.5.2/src/cdk_constructs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-05-13 16:34:04.000000 cdk-constructs-1.5.2/src/cdk_constructs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-13 16:34:04.000000 cdk-constructs-1.5.2/src/cdk_constructs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 16:34:04.000000 cdk-constructs-1.5.2/src/cdk_constructs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-13 16:34:04.000000 cdk-constructs-1.5.2/src/cdk_constructs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-13 16:34:04.000000 cdk-constructs-1.5.2/src/cdk_constructs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:49.621497 cdk-constructs-1.5.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-13 18:47:34.000000 cdk-constructs-1.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-13 18:47:34.000000 cdk-constructs-1.5.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-05-13 18:47:49.621497 cdk-constructs-1.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-05-13 18:47:34.000000 cdk-constructs-1.5.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-13 18:47:34.000000 cdk-constructs-1.5.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 18:47:49.621497 cdk-constructs-1.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-13 18:47:34.000000 cdk-constructs-1.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:49.621497 cdk-constructs-1.5.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:49.621497 cdk-constructs-1.5.3/src/cdk-constructs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6459 2024-05-13 18:47:34.000000 cdk-constructs-1.5.3/src/cdk-constructs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:49.621497 cdk-constructs-1.5.3/src/cdk-constructs/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-13 18:47:34.000000 cdk-constructs-1.5.3/src/cdk-constructs/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33590 2024-05-13 18:47:34.000000 cdk-constructs-1.5.3/src/cdk-constructs/_jsii/cdk-constructs@1.5.3.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 18:47:34.000000 cdk-constructs-1.5.3/src/cdk-constructs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:49.621497 cdk-constructs-1.5.3/src/cdk_constructs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-05-13 18:47:49.000000 cdk-constructs-1.5.3/src/cdk_constructs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-13 18:47:49.000000 cdk-constructs-1.5.3/src/cdk_constructs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 18:47:49.000000 cdk-constructs-1.5.3/src/cdk_constructs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-13 18:47:49.000000 cdk-constructs-1.5.3/src/cdk_constructs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-13 18:47:49.000000 cdk-constructs-1.5.3/src/cdk_constructs.egg-info/top_level.txt
```

### Comparing `cdk-constructs-1.5.2/LICENSE` & `cdk-constructs-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-constructs-1.5.2/PKG-INFO` & `cdk-constructs-1.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-constructs
-Version: 1.5.2
+Version: 1.5.3
 Summary: A CDK construct library
 Home-page: https://github.com/tm-lcarvalho/cdk-constructs.git
 Author: tm-lcarvalho<lucio.carvalho@toumoro.com>
 License: GPL-3.0-or-later
 Project-URL: Source, https://github.com/tm-lcarvalho/cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-constructs-1.5.2/README.md` & `cdk-constructs-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `cdk-constructs-1.5.2/setup.py` & `cdk-constructs-1.5.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-constructs",
-    "version": "1.5.2",
+    "version": "1.5.3",
     "description": "A CDK construct library",
     "license": "GPL-3.0-or-later",
     "url": "https://github.com/tm-lcarvalho/cdk-constructs.git",
     "long_description_content_type": "text/markdown",
     "author": "tm-lcarvalho<lucio.carvalho@toumoro.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk-constructs",
         "cdk-constructs._jsii"
     ],
     "package_data": {
         "cdk-constructs._jsii": [
-            "cdk-constructs@1.5.2.jsii.tgz"
+            "cdk-constructs@1.5.3.jsii.tgz"
         ],
         "cdk-constructs": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `cdk-constructs-1.5.2/src/cdk-constructs/__init__.py` & `cdk-constructs-1.5.3/src/cdk-constructs/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-constructs-1.5.2/src/cdk_constructs.egg-info/PKG-INFO` & `cdk-constructs-1.5.3/src/cdk_constructs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-constructs
-Version: 1.5.2
+Version: 1.5.3
 Summary: A CDK construct library
 Home-page: https://github.com/tm-lcarvalho/cdk-constructs.git
 Author: tm-lcarvalho<lucio.carvalho@toumoro.com>
 License: GPL-3.0-or-later
 Project-URL: Source, https://github.com/tm-lcarvalho/cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

