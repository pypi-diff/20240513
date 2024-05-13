# Comparing `tmp/gpuhunt-0.0.9rc2.tar.gz` & `tmp/gpuhunt-0.0.9rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpuhunt-0.0.9rc2.tar", last modified: Mon Apr  8 09:26:11 2024, max compression
+gzip compressed data, was "gpuhunt-0.0.9rc3.tar", last modified: Fri Apr 12 10:06:58 2024, max compression
```

## Comparing `gpuhunt-0.0.9rc2.tar` & `gpuhunt-0.0.9rc3.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:26:11.855010 gpuhunt-0.0.9rc2/
--rw-r--r--   0 runner    (1001) docker     (127)    15976 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-04-08 09:26:11.855010 gpuhunt-0.0.9rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 09:26:11.855010 gpuhunt-0.0.9rc2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:26:11.843010 gpuhunt-0.0.9rc2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:26:11.843010 gpuhunt-0.0.9rc2/src/gpuhunt/
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/src/gpuhunt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/src/gpuhunt/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:26:11.847010 gpuhunt-0.0.9rc2/src/gpuhunt/_internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/src/gpuhunt/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9224 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/src/gpuhunt/_internal/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/src/gpuhunt/_internal/constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/src/gpuhunt/_internal/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     5230 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/src/gpuhunt/_internal/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/src/gpuhunt/_internal/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/src/gpuhunt/_internal/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:26:11.847010 gpuhunt-0.0.9rc2/src/gpuhunt/providers/
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/src/gpuhunt/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8194 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/src/gpuhunt/providers/aws.py
--rw-r--r--   0 runner    (1001) docker     (127)    10015 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/src/gpuhunt/providers/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)    14565 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/src/gpuhunt/providers/cudo.py
--rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/src/gpuhunt/providers/datacrunch.py
--rw-r--r--   0 runner    (1001) docker     (127)     9430 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/src/gpuhunt/providers/gcp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/src/gpuhunt/providers/lambdalabs.py
--rw-r--r--   0 runner    (1001) docker     (127)    11796 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/src/gpuhunt/providers/nebius.py
--rw-r--r--   0 runner    (1001) docker     (127)     8308 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/src/gpuhunt/providers/runpod.py
--rw-r--r--   0 runner    (1001) docker     (127)     9566 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/src/gpuhunt/providers/tensordock.py
--rw-r--r--   0 runner    (1001) docker     (127)     6169 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/src/gpuhunt/providers/vastai.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-08 09:26:09.000000 gpuhunt-0.0.9rc2/src/gpuhunt/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:26:11.851010 gpuhunt-0.0.9rc2/src/gpuhunt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-04-08 09:26:11.000000 gpuhunt-0.0.9rc2/src/gpuhunt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-08 09:26:11.000000 gpuhunt-0.0.9rc2/src/gpuhunt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 09:26:11.000000 gpuhunt-0.0.9rc2/src/gpuhunt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-08 09:26:11.000000 gpuhunt-0.0.9rc2/src/gpuhunt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-08 09:26:11.000000 gpuhunt-0.0.9rc2/src/gpuhunt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:26:11.851010 gpuhunt-0.0.9rc2/src/integrity_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/src/integrity_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/src/integrity_tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/src/integrity_tests/test_all.py
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/src/integrity_tests/test_aws.py
--rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/src/integrity_tests/test_azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/src/integrity_tests/test_datacrunch.py
--rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/src/integrity_tests/test_gcp.py
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/src/integrity_tests/test_nebius.py
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/src/integrity_tests/test_runpod.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:26:11.851010 gpuhunt-0.0.9rc2/src/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/src/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:26:11.851010 gpuhunt-0.0.9rc2/src/tests/_internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/src/tests/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/src/tests/_internal/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/src/tests/_internal/test_constraints.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:26:11.851010 gpuhunt-0.0.9rc2/src/tests/providers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/src/tests/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7243 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/src/tests/providers/test_cudo.py
--rw-r--r--   0 runner    (1001) docker     (127)    11443 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/src/tests/providers/test_datacrunch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/src/tests/providers/test_providers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/src/tests/providers/test_tensordock.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-08 09:26:02.000000 gpuhunt-0.0.9rc2/src/tests/providers/test_vastai.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:06:58.579416 gpuhunt-0.0.9rc3/
+-rw-r--r--   0 runner    (1001) docker     (127)    15976 2024-04-12 10:06:47.000000 gpuhunt-0.0.9rc3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-04-12 10:06:58.579416 gpuhunt-0.0.9rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-04-12 10:06:47.000000 gpuhunt-0.0.9rc3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-12 10:06:47.000000 gpuhunt-0.0.9rc3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 10:06:58.579416 gpuhunt-0.0.9rc3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:06:58.567416 gpuhunt-0.0.9rc3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:06:58.567416 gpuhunt-0.0.9rc3/src/gpuhunt/
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-12 10:06:47.000000 gpuhunt-0.0.9rc3/src/gpuhunt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-04-12 10:06:47.000000 gpuhunt-0.0.9rc3/src/gpuhunt/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:06:58.571416 gpuhunt-0.0.9rc3/src/gpuhunt/_internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 10:06:47.000000 gpuhunt-0.0.9rc3/src/gpuhunt/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9224 2024-04-12 10:06:47.000000 gpuhunt-0.0.9rc3/src/gpuhunt/_internal/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-04-12 10:06:47.000000 gpuhunt-0.0.9rc3/src/gpuhunt/_internal/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-12 10:06:47.000000 gpuhunt-0.0.9rc3/src/gpuhunt/_internal/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5230 2024-04-12 10:06:47.000000 gpuhunt-0.0.9rc3/src/gpuhunt/_internal/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-12 10:06:47.000000 gpuhunt-0.0.9rc3/src/gpuhunt/_internal/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-12 10:06:47.000000 gpuhunt-0.0.9rc3/src/gpuhunt/_internal/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:06:58.571416 gpuhunt-0.0.9rc3/src/gpuhunt/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-12 10:06:47.000000 gpuhunt-0.0.9rc3/src/gpuhunt/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8194 2024-04-12 10:06:47.000000 gpuhunt-0.0.9rc3/src/gpuhunt/providers/aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10015 2024-04-12 10:06:47.000000 gpuhunt-0.0.9rc3/src/gpuhunt/providers/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14565 2024-04-12 10:06:47.000000 gpuhunt-0.0.9rc3/src/gpuhunt/providers/cudo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-04-12 10:06:47.000000 gpuhunt-0.0.9rc3/src/gpuhunt/providers/datacrunch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9430 2024-04-12 10:06:47.000000 gpuhunt-0.0.9rc3/src/gpuhunt/providers/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-04-12 10:06:47.000000 gpuhunt-0.0.9rc3/src/gpuhunt/providers/lambdalabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11796 2024-04-12 10:06:47.000000 gpuhunt-0.0.9rc3/src/gpuhunt/providers/nebius.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8516 2024-04-12 10:06:47.000000 gpuhunt-0.0.9rc3/src/gpuhunt/providers/runpod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9566 2024-04-12 10:06:47.000000 gpuhunt-0.0.9rc3/src/gpuhunt/providers/tensordock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6206 2024-04-12 10:06:47.000000 gpuhunt-0.0.9rc3/src/gpuhunt/providers/vastai.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-12 10:06:56.000000 gpuhunt-0.0.9rc3/src/gpuhunt/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:06:58.575416 gpuhunt-0.0.9rc3/src/gpuhunt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-04-12 10:06:58.000000 gpuhunt-0.0.9rc3/src/gpuhunt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-12 10:06:58.000000 gpuhunt-0.0.9rc3/src/gpuhunt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 10:06:58.000000 gpuhunt-0.0.9rc3/src/gpuhunt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-12 10:06:58.000000 gpuhunt-0.0.9rc3/src/gpuhunt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-12 10:06:58.000000 gpuhunt-0.0.9rc3/src/gpuhunt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:06:58.575416 gpuhunt-0.0.9rc3/src/integrity_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 10:06:47.000000 gpuhunt-0.0.9rc3/src/integrity_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-12 10:06:47.000000 gpuhunt-0.0.9rc3/src/integrity_tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-12 10:06:47.000000 gpuhunt-0.0.9rc3/src/integrity_tests/test_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-04-12 10:06:47.000000 gpuhunt-0.0.9rc3/src/integrity_tests/test_aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-04-12 10:06:47.000000 gpuhunt-0.0.9rc3/src/integrity_tests/test_azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-12 10:06:47.000000 gpuhunt-0.0.9rc3/src/integrity_tests/test_datacrunch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-04-12 10:06:47.000000 gpuhunt-0.0.9rc3/src/integrity_tests/test_gcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-12 10:06:47.000000 gpuhunt-0.0.9rc3/src/integrity_tests/test_nebius.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-04-12 10:06:47.000000 gpuhunt-0.0.9rc3/src/integrity_tests/test_runpod.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:06:58.575416 gpuhunt-0.0.9rc3/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 10:06:47.000000 gpuhunt-0.0.9rc3/src/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:06:58.575416 gpuhunt-0.0.9rc3/src/tests/_internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 10:06:47.000000 gpuhunt-0.0.9rc3/src/tests/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-12 10:06:47.000000 gpuhunt-0.0.9rc3/src/tests/_internal/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-04-12 10:06:47.000000 gpuhunt-0.0.9rc3/src/tests/_internal/test_constraints.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:06:58.575416 gpuhunt-0.0.9rc3/src/tests/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 10:06:47.000000 gpuhunt-0.0.9rc3/src/tests/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7243 2024-04-12 10:06:47.000000 gpuhunt-0.0.9rc3/src/tests/providers/test_cudo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11443 2024-04-12 10:06:47.000000 gpuhunt-0.0.9rc3/src/tests/providers/test_datacrunch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-12 10:06:47.000000 gpuhunt-0.0.9rc3/src/tests/providers/test_providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-04-12 10:06:47.000000 gpuhunt-0.0.9rc3/src/tests/providers/test_tensordock.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-12 10:06:47.000000 gpuhunt-0.0.9rc3/src/tests/providers/test_vastai.py
```

### Comparing `gpuhunt-0.0.9rc2/LICENSE` & `gpuhunt-0.0.9rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.9rc2/PKG-INFO` & `gpuhunt-0.0.9rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpuhunt
-Version: 0.0.9rc2
+Version: 0.0.9rc3
 Summary: A catalog of GPU pricing for different cloud providers
 Author: dstack GmbH
 Project-URL: GitHub, https://github.com/dstackai/gpuhunt
 Project-URL: Issues, https://github.com/dstackai/gpuhunt/issues
 Keywords: gpu,cloud,pricing
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `gpuhunt-0.0.9rc2/README.md` & `gpuhunt-0.0.9rc3/README.md`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.9rc2/pyproject.toml` & `gpuhunt-0.0.9rc3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.9rc2/src/gpuhunt/__main__.py` & `gpuhunt-0.0.9rc3/src/gpuhunt/__main__.py`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.9rc2/src/gpuhunt/_internal/catalog.py` & `gpuhunt-0.0.9rc3/src/gpuhunt/_internal/catalog.py`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.9rc2/src/gpuhunt/_internal/constraints.py` & `gpuhunt-0.0.9rc3/src/gpuhunt/_internal/constraints.py`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.9rc2/src/gpuhunt/_internal/default.py` & `gpuhunt-0.0.9rc3/src/gpuhunt/_internal/default.py`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.9rc2/src/gpuhunt/_internal/models.py` & `gpuhunt-0.0.9rc3/src/gpuhunt/_internal/models.py`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.9rc2/src/gpuhunt/_internal/storage.py` & `gpuhunt-0.0.9rc3/src/gpuhunt/_internal/storage.py`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.9rc2/src/gpuhunt/providers/aws.py` & `gpuhunt-0.0.9rc3/src/gpuhunt/providers/aws.py`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.9rc2/src/gpuhunt/providers/azure.py` & `gpuhunt-0.0.9rc3/src/gpuhunt/providers/azure.py`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.9rc2/src/gpuhunt/providers/cudo.py` & `gpuhunt-0.0.9rc3/src/gpuhunt/providers/cudo.py`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.9rc2/src/gpuhunt/providers/datacrunch.py` & `gpuhunt-0.0.9rc3/src/gpuhunt/providers/datacrunch.py`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.9rc2/src/gpuhunt/providers/gcp.py` & `gpuhunt-0.0.9rc3/src/gpuhunt/providers/gcp.py`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.9rc2/src/gpuhunt/providers/lambdalabs.py` & `gpuhunt-0.0.9rc3/src/gpuhunt/providers/lambdalabs.py`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.9rc2/src/gpuhunt/providers/nebius.py` & `gpuhunt-0.0.9rc3/src/gpuhunt/providers/nebius.py`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.9rc2/src/gpuhunt/providers/runpod.py` & `gpuhunt-0.0.9rc3/src/gpuhunt/providers/runpod.py`

 * *Files 12% similar despite different names*

```diff
@@ -198,29 +198,38 @@
                 disk_size=None,
             )
         )
 
     return catalog_items
 
 
-GPU_MAP = {
-    "NVIDIA A100 80GB PCIe": "A100",
-    "NVIDIA A100-SXM4-80GB": "A100",
-    "NVIDIA A40": "A40",
-    "NVIDIA GeForce RTX 4090": "RTX4090",
-    "NVIDIA H100 80GB HBM3": "H100",
-    "NVIDIA L40S": "L40",
-    "NVIDIA L40": "L40",
-    "NVIDIA RTX 4000 Ada Generation": "RTX4000",
-    "NVIDIA RTX 6000 Ada Generation": "RTX6000",
-    "NVIDIA RTX A4000": "RTXA4000",
-    # "NVIDIA RTX A4500": "RTXA4500",
-    "NVIDIA RTX A5000": "RTXA5000",
-    "NVIDIA RTX A6000": "RTXA6000",
-}
+def get_gpu_map():
+    payload_gpus = {"query": "query GpuTypes { gpuTypes { id displayName memoryInGb } }"}
+    gpu_types = make_request(payload_gpus)
+    gpu_map = {
+        item["id"]: get_gpu_name(item["displayName"])
+        for item in gpu_types["data"]["gpuTypes"]
+        if get_gpu_name(item["displayName"]) is not None
+    }
+    return gpu_map
+
+
+def get_gpu_name(name: str) -> Optional[str]:
+    if "V100" in name:
+        return "V100"
+    if name.startswith(("A", "L", "H")):
+        gpu_name, _, _ = name.partition(" ")
+        return gpu_name
+    if name.startswith("RTX"):
+        gpu_name = name.replace(" ", "")
+        return gpu_name
+    return None
+
+
+GPU_MAP = get_gpu_map()
 
 gpu_types_query = """
 query GpuTypes {
   countryCodes
   dataCenters {
     id
     name
```

### Comparing `gpuhunt-0.0.9rc2/src/gpuhunt/providers/tensordock.py` & `gpuhunt-0.0.9rc3/src/gpuhunt/providers/tensordock.py`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.9rc2/src/gpuhunt/providers/vastai.py` & `gpuhunt-0.0.9rc3/src/gpuhunt/providers/vastai.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,39 +35,39 @@
         filters["order"] = [["score", "desc"]]
         resp = requests.post(bundles_url, json=filters)
         resp.raise_for_status()
         data = resp.json()
 
         instance_offers = []
         for offer in data["offers"]:
+            disk_size = query_filter and query_filter.min_disk_size or offer["disk_space"]
             if not self.satisfies_filters(offer, filters):
                 logger.warning("Offer %s does not satisfy filters", offer["id"])
                 continue
             gpu_name = get_gpu_name(offer["gpu_name"])
             gpu_memory = normalize_gpu_memory(gpu_name, offer["gpu_ram"])
             ondemand_offer = RawCatalogItem(
                 instance_name=str(offer["id"]),
                 location=get_location(offer["geolocation"]),
                 # storage_cost is $/gb/month
                 price=round(
-                    offer["dph_base"]
-                    + (query_filter.min_disk_size or 0) * offer["storage_cost"] / 30 / 24,
+                    offer["dph_base"] + disk_size * offer["storage_cost"] / 30 / 24,
                     5,
                 ),
                 cpu=int(offer["cpu_cores_effective"]),
                 memory=float(
                     int(
                         offer["cpu_ram"] * offer["cpu_cores_effective"] / offer["cpu_cores"] / kilo
                     )
                 ),
                 gpu_count=offer["num_gpus"],
                 gpu_name=gpu_name,
                 gpu_memory=float(gpu_memory),
                 spot=False,
-                disk_size=offer["disk_space"],
+                disk_size=disk_size,
             )
             instance_offers.append(ondemand_offer)
 
             spot_offer = copy.deepcopy(ondemand_offer)
             spot_offer.price = round(offer["min_bid"], 5)
             spot_offer.spot = True
             instance_offers.append(spot_offer)
```

### Comparing `gpuhunt-0.0.9rc2/src/gpuhunt.egg-info/PKG-INFO` & `gpuhunt-0.0.9rc3/src/gpuhunt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpuhunt
-Version: 0.0.9rc2
+Version: 0.0.9rc3
 Summary: A catalog of GPU pricing for different cloud providers
 Author: dstack GmbH
 Project-URL: GitHub, https://github.com/dstackai/gpuhunt
 Project-URL: Issues, https://github.com/dstackai/gpuhunt/issues
 Keywords: gpu,cloud,pricing
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `gpuhunt-0.0.9rc2/src/gpuhunt.egg-info/SOURCES.txt` & `gpuhunt-0.0.9rc3/src/gpuhunt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.9rc2/src/integrity_tests/test_aws.py` & `gpuhunt-0.0.9rc3/src/integrity_tests/test_aws.py`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.9rc2/src/integrity_tests/test_azure.py` & `gpuhunt-0.0.9rc3/src/integrity_tests/test_azure.py`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.9rc2/src/integrity_tests/test_datacrunch.py` & `gpuhunt-0.0.9rc3/src/integrity_tests/test_datacrunch.py`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.9rc2/src/integrity_tests/test_gcp.py` & `gpuhunt-0.0.9rc3/src/integrity_tests/test_gcp.py`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.9rc2/src/integrity_tests/test_nebius.py` & `gpuhunt-0.0.9rc3/src/integrity_tests/test_nebius.py`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.9rc2/src/integrity_tests/test_runpod.py` & `gpuhunt-0.0.9rc3/src/integrity_tests/test_runpod.py`

 * *Files 15% similar despite different names*

```diff
@@ -24,14 +24,15 @@
         "CA-MTL-1",
         "CA-MTL-2",
         "EU-NL-1",
         "EU-RO-1",
         "EU-SE-1",
         "EUR-IS-1",
         "EUR-IS-2",
+        "EUR-NO-1",
         "US-OR-1",
     }
     locations = select_row(data_rows, "location")
     assert set(locations) == expected
 
     count = Counter(locations)
     for loc in expected:
@@ -51,10 +52,10 @@
 
 def test_price(data_rows):
     prices = select_row(data_rows, "price")
     assert min(float(p) for p in prices) > 0
 
 
 def test_gpu_present(data_rows):
-    refs = [name for name in GPU_MAP.values()]
-    gpus = select_row(data_rows, "gpu_name")
-    assert set(gpus) == set(refs)
+    refs = set(name for name in GPU_MAP.values())
+    gpus = set(select_row(data_rows, "gpu_name"))
+    assert len(refs & gpus) > 7
```

### Comparing `gpuhunt-0.0.9rc2/src/tests/_internal/test_catalog.py` & `gpuhunt-0.0.9rc3/src/tests/_internal/test_catalog.py`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.9rc2/src/tests/_internal/test_constraints.py` & `gpuhunt-0.0.9rc3/src/tests/_internal/test_constraints.py`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.9rc2/src/tests/providers/test_cudo.py` & `gpuhunt-0.0.9rc3/src/tests/providers/test_cudo.py`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.9rc2/src/tests/providers/test_datacrunch.py` & `gpuhunt-0.0.9rc3/src/tests/providers/test_datacrunch.py`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.9rc2/src/tests/providers/test_providers.py` & `gpuhunt-0.0.9rc3/src/tests/providers/test_providers.py`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.9rc2/src/tests/providers/test_tensordock.py` & `gpuhunt-0.0.9rc3/src/tests/providers/test_tensordock.py`

 * *Files identical despite different names*

