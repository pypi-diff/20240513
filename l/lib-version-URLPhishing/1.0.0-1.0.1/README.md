# Comparing `tmp/lib_version_urlphishing-1.0.0.tar.gz` & `tmp/lib_version_urlphishing-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib_version_urlphishing-1.0.0.tar", last modified: Sun May 12 18:55:37 2024, max compression
+gzip compressed data, was "lib_version_urlphishing-1.0.1.tar", last modified: Mon May 13 00:11:45 2024, max compression
```

## Comparing `lib_version_urlphishing-1.0.0.tar` & `lib_version_urlphishing-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 18:55:37.672125 lib_version_urlphishing-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-12 18:55:24.000000 lib_version_urlphishing-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-12 18:55:37.672125 lib_version_urlphishing-1.0.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 18:55:37.672125 lib_version_urlphishing-1.0.0/lib-version/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-12 18:55:24.000000 lib_version_urlphishing-1.0.0/lib-version/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 18:55:37.672125 lib_version_urlphishing-1.0.0/lib_version_URLPhishing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-12 18:55:37.000000 lib_version_urlphishing-1.0.0/lib_version_URLPhishing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-12 18:55:37.000000 lib_version_urlphishing-1.0.0/lib_version_URLPhishing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 18:55:37.000000 lib_version_urlphishing-1.0.0/lib_version_URLPhishing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 18:55:37.000000 lib_version_urlphishing-1.0.0/lib_version_URLPhishing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 18:55:37.672125 lib_version_urlphishing-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-12 18:55:24.000000 lib_version_urlphishing-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 00:11:45.182547 lib_version_urlphishing-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-13 00:11:33.000000 lib_version_urlphishing-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-13 00:11:45.182547 lib_version_urlphishing-1.0.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 00:11:45.182547 lib_version_urlphishing-1.0.1/lib-version/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 00:11:33.000000 lib_version_urlphishing-1.0.1/lib-version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-13 00:11:33.000000 lib_version_urlphishing-1.0.1/lib-version/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-13 00:11:33.000000 lib_version_urlphishing-1.0.1/lib-version/version_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 00:11:45.182547 lib_version_urlphishing-1.0.1/lib_version_URLPhishing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-13 00:11:45.000000 lib_version_urlphishing-1.0.1/lib_version_URLPhishing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-13 00:11:45.000000 lib_version_urlphishing-1.0.1/lib_version_URLPhishing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 00:11:45.000000 lib_version_urlphishing-1.0.1/lib_version_URLPhishing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-13 00:11:45.000000 lib_version_urlphishing-1.0.1/lib_version_URLPhishing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 00:11:45.182547 lib_version_urlphishing-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-13 00:11:33.000000 lib_version_urlphishing-1.0.1/setup.py
```

### Comparing `lib_version_urlphishing-1.0.0/setup.py` & `lib_version_urlphishing-1.0.1/setup.py`

 * *Files identical despite different names*

