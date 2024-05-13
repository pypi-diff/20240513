# Comparing `tmp/cdk-vpc-toumoro-projen-1.4.6.tar.gz` & `tmp/cdk-vpc-toumoro-projen-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-vpc-toumoro-projen-1.4.6.tar", last modified: Thu May  9 14:44:13 2024, max compression
+gzip compressed data, was "cdk-vpc-toumoro-projen-1.5.0.tar", last modified: Mon May 13 15:28:59 2024, max compression
```

## Comparing `cdk-vpc-toumoro-projen-1.4.6.tar` & `cdk-vpc-toumoro-projen-1.5.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:44:13.086614 cdk-vpc-toumoro-projen-1.4.6/
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-09 14:44:02.000000 cdk-vpc-toumoro-projen-1.4.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-09 14:44:02.000000 cdk-vpc-toumoro-projen-1.4.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-09 14:44:13.086614 cdk-vpc-toumoro-projen-1.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-09 14:44:02.000000 cdk-vpc-toumoro-projen-1.4.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-09 14:44:02.000000 cdk-vpc-toumoro-projen-1.4.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 14:44:13.086614 cdk-vpc-toumoro-projen-1.4.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-05-09 14:44:02.000000 cdk-vpc-toumoro-projen-1.4.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:44:13.086614 cdk-vpc-toumoro-projen-1.4.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:44:13.086614 cdk-vpc-toumoro-projen-1.4.6/src/cdk-vpc-toumoro-projen/
--rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-05-09 14:44:02.000000 cdk-vpc-toumoro-projen-1.4.6/src/cdk-vpc-toumoro-projen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:44:13.086614 cdk-vpc-toumoro-projen-1.4.6/src/cdk-vpc-toumoro-projen/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-09 14:44:02.000000 cdk-vpc-toumoro-projen-1.4.6/src/cdk-vpc-toumoro-projen/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30898 2024-05-09 14:44:02.000000 cdk-vpc-toumoro-projen-1.4.6/src/cdk-vpc-toumoro-projen/_jsii/cdk-vpc-toumoro-projen@1.4.6.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 14:44:02.000000 cdk-vpc-toumoro-projen-1.4.6/src/cdk-vpc-toumoro-projen/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:44:13.086614 cdk-vpc-toumoro-projen-1.4.6/src/cdk_vpc_toumoro_projen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-09 14:44:13.000000 cdk-vpc-toumoro-projen-1.4.6/src/cdk_vpc_toumoro_projen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-09 14:44:13.000000 cdk-vpc-toumoro-projen-1.4.6/src/cdk_vpc_toumoro_projen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 14:44:13.000000 cdk-vpc-toumoro-projen-1.4.6/src/cdk_vpc_toumoro_projen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-09 14:44:13.000000 cdk-vpc-toumoro-projen-1.4.6/src/cdk_vpc_toumoro_projen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-09 14:44:13.000000 cdk-vpc-toumoro-projen-1.4.6/src/cdk_vpc_toumoro_projen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:28:59.203225 cdk-vpc-toumoro-projen-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-13 15:28:49.000000 cdk-vpc-toumoro-projen-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-13 15:28:49.000000 cdk-vpc-toumoro-projen-1.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-05-13 15:28:59.203225 cdk-vpc-toumoro-projen-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-05-13 15:28:49.000000 cdk-vpc-toumoro-projen-1.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-13 15:28:49.000000 cdk-vpc-toumoro-projen-1.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 15:28:59.203225 cdk-vpc-toumoro-projen-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-05-13 15:28:49.000000 cdk-vpc-toumoro-projen-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:28:59.199226 cdk-vpc-toumoro-projen-1.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:28:59.199226 cdk-vpc-toumoro-projen-1.5.0/src/cdk-vpc-toumoro-projen/
+-rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-05-13 15:28:49.000000 cdk-vpc-toumoro-projen-1.5.0/src/cdk-vpc-toumoro-projen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:28:59.199226 cdk-vpc-toumoro-projen-1.5.0/src/cdk-vpc-toumoro-projen/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-13 15:28:49.000000 cdk-vpc-toumoro-projen-1.5.0/src/cdk-vpc-toumoro-projen/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32914 2024-05-13 15:28:49.000000 cdk-vpc-toumoro-projen-1.5.0/src/cdk-vpc-toumoro-projen/_jsii/cdk-vpc-toumoro-projen@1.5.0.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 15:28:49.000000 cdk-vpc-toumoro-projen-1.5.0/src/cdk-vpc-toumoro-projen/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:28:59.199226 cdk-vpc-toumoro-projen-1.5.0/src/cdk_vpc_toumoro_projen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-05-13 15:28:59.000000 cdk-vpc-toumoro-projen-1.5.0/src/cdk_vpc_toumoro_projen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-13 15:28:59.000000 cdk-vpc-toumoro-projen-1.5.0/src/cdk_vpc_toumoro_projen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 15:28:59.000000 cdk-vpc-toumoro-projen-1.5.0/src/cdk_vpc_toumoro_projen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-13 15:28:59.000000 cdk-vpc-toumoro-projen-1.5.0/src/cdk_vpc_toumoro_projen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-13 15:28:59.000000 cdk-vpc-toumoro-projen-1.5.0/src/cdk_vpc_toumoro_projen.egg-info/top_level.txt
```

### Comparing `cdk-vpc-toumoro-projen-1.4.6/LICENSE` & `cdk-vpc-toumoro-projen-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-vpc-toumoro-projen-1.4.6/setup.py` & `cdk-vpc-toumoro-projen-1.5.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-vpc-toumoro-projen",
-    "version": "1.4.6",
+    "version": "1.5.0",
     "description": "A CDK construct library to create a VPC with public and private subnets.",
     "license": "GPL-3.0-or-later",
     "url": "https://github.com/tm-lcarvalho/cdk-vpc-toumoro-projen.git",
     "long_description_content_type": "text/markdown",
     "author": "tm-lcarvalho<lucio.carvalho@toumoro.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk-vpc-toumoro-projen",
         "cdk-vpc-toumoro-projen._jsii"
     ],
     "package_data": {
         "cdk-vpc-toumoro-projen._jsii": [
-            "cdk-vpc-toumoro-projen@1.4.6.jsii.tgz"
+            "cdk-vpc-toumoro-projen@1.5.0.jsii.tgz"
         ],
         "cdk-vpc-toumoro-projen": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

