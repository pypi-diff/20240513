# Comparing `tmp/lib_version_remla24_team02-0.0.1.tar.gz` & `tmp/lib_version_remla24_team02-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib_version_remla24_team02-0.0.1.tar", last modified: Sun May 12 14:10:53 2024, max compression
+gzip compressed data, was "lib_version_remla24_team02-0.0.2.tar", last modified: Sun May 12 14:58:43 2024, max compression
```

## Comparing `lib_version_remla24_team02-0.0.1.tar` & `lib_version_remla24_team02-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 14:10:53.579668 lib_version_remla24_team02-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-12 14:10:45.000000 lib_version_remla24_team02-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-12 14:10:53.579668 lib_version_remla24_team02-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-12 14:10:45.000000 lib_version_remla24_team02-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 14:10:53.575668 lib_version_remla24_team02-0.0.1/lib_version_remla24_team02/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 14:10:45.000000 lib_version_remla24_team02-0.0.1/lib_version_remla24_team02/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-12 14:10:45.000000 lib_version_remla24_team02-0.0.1/lib_version_remla24_team02/version_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 14:10:53.579668 lib_version_remla24_team02-0.0.1/lib_version_remla24_team02.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-12 14:10:53.000000 lib_version_remla24_team02-0.0.1/lib_version_remla24_team02.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-12 14:10:53.000000 lib_version_remla24_team02-0.0.1/lib_version_remla24_team02.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 14:10:53.000000 lib_version_remla24_team02-0.0.1/lib_version_remla24_team02.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-12 14:10:53.000000 lib_version_remla24_team02-0.0.1/lib_version_remla24_team02.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 14:10:53.579668 lib_version_remla24_team02-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-12 14:10:53.000000 lib_version_remla24_team02-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 14:58:43.115169 lib_version_remla24_team02-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-12 14:58:31.000000 lib_version_remla24_team02-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-12 14:58:43.115169 lib_version_remla24_team02-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-12 14:58:31.000000 lib_version_remla24_team02-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 14:58:43.115169 lib_version_remla24_team02-0.0.2/lib_version_remla24_team02/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-12 14:58:31.000000 lib_version_remla24_team02-0.0.2/lib_version_remla24_team02/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-12 14:58:31.000000 lib_version_remla24_team02-0.0.2/lib_version_remla24_team02/version_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 14:58:43.115169 lib_version_remla24_team02-0.0.2/lib_version_remla24_team02.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-12 14:58:43.000000 lib_version_remla24_team02-0.0.2/lib_version_remla24_team02.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-12 14:58:43.000000 lib_version_remla24_team02-0.0.2/lib_version_remla24_team02.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 14:58:43.000000 lib_version_remla24_team02-0.0.2/lib_version_remla24_team02.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-12 14:58:43.000000 lib_version_remla24_team02-0.0.2/lib_version_remla24_team02.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 14:58:43.115169 lib_version_remla24_team02-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-12 14:58:42.000000 lib_version_remla24_team02-0.0.2/setup.py
```

### Comparing `lib_version_remla24_team02-0.0.1/LICENSE` & `lib_version_remla24_team02-0.0.2/LICENSE`

 * *Files identical despite different names*

