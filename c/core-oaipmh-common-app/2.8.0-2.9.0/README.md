# Comparing `tmp/core_oaipmh_common_app-2.8.0.tar.gz` & `tmp/core_oaipmh_common_app-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_oaipmh_common_app-2.8.0.tar", last modified: Tue Mar 12 19:05:43 2024, max compression
+gzip compressed data, was "core_oaipmh_common_app-2.9.0.tar", last modified: Mon May 13 16:10:45 2024, max compression
```

## Comparing `core_oaipmh_common_app-2.8.0.tar` & `core_oaipmh_common_app-2.9.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:43.128771 core_oaipmh_common_app-2.8.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2024-03-12 19:05:39.000000 core_oaipmh_common_app-2.8.0/LICENSE.md
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      177 2024-03-12 19:05:39.000000 core_oaipmh_common_app-2.8.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1089 2024-03-12 19:05:43.123291 core_oaipmh_common_app-2.8.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      593 2024-03-12 19:05:39.000000 core_oaipmh_common_app-2.8.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:42.568555 core_oaipmh_common_app-2.8.0/core_oaipmh_common_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:39.000000 core_oaipmh_common_app-2.8.0/core_oaipmh_common_app/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:42.718883 core_oaipmh_common_app-2.8.0/core_oaipmh_common_app/commons/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:39.000000 core_oaipmh_common_app-2.8.0/core_oaipmh_common_app/commons/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1643 2024-03-12 19:05:39.000000 core_oaipmh_common_app-2.8.0/core_oaipmh_common_app/commons/exceptions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      798 2024-03-12 19:05:39.000000 core_oaipmh_common_app-2.8.0/core_oaipmh_common_app/commons/messages.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:42.737993 core_oaipmh_common_app-2.8.0/core_oaipmh_common_app/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:39.000000 core_oaipmh_common_app-2.8.0/core_oaipmh_common_app/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:42.818951 core_oaipmh_common_app-2.8.0/core_oaipmh_common_app/components/oai_metadata_format/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:39.000000 core_oaipmh_common_app-2.8.0/core_oaipmh_common_app/components/oai_metadata_format/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1094 2024-03-12 19:05:39.000000 core_oaipmh_common_app-2.8.0/core_oaipmh_common_app/components/oai_metadata_format/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2908 2024-03-12 19:05:39.000000 core_oaipmh_common_app-2.8.0/core_oaipmh_common_app/components/oai_metadata_format/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:42.873860 core_oaipmh_common_app-2.8.0/core_oaipmh_common_app/components/oai_set/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:39.000000 core_oaipmh_common_app-2.8.0/core_oaipmh_common_app/components/oai_set/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      795 2024-03-12 19:05:39.000000 core_oaipmh_common_app-2.8.0/core_oaipmh_common_app/components/oai_set/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2033 2024-03-12 19:05:39.000000 core_oaipmh_common_app-2.8.0/core_oaipmh_common_app/components/oai_set/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:42.891197 core_oaipmh_common_app-2.8.0/core_oaipmh_common_app/migrations/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:39.000000 core_oaipmh_common_app-2.8.0/core_oaipmh_common_app/migrations/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:42.928790 core_oaipmh_common_app-2.8.0/core_oaipmh_common_app/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      865 2024-03-12 19:05:39.000000 core_oaipmh_common_app-2.8.0/core_oaipmh_common_app/utils/UTCdatetime.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:39.000000 core_oaipmh_common_app-2.8.0/core_oaipmh_common_app/utils/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:42.661890 core_oaipmh_common_app-2.8.0/core_oaipmh_common_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1089 2024-03-12 19:05:42.000000 core_oaipmh_common_app-2.8.0/core_oaipmh_common_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1372 2024-03-12 19:05:42.000000 core_oaipmh_common_app-2.8.0/core_oaipmh_common_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2024-03-12 19:05:42.000000 core_oaipmh_common_app-2.8.0/core_oaipmh_common_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       63 2024-03-12 19:05:42.000000 core_oaipmh_common_app-2.8.0/core_oaipmh_common_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       29 2024-03-12 19:05:42.000000 core_oaipmh_common_app-2.8.0/core_oaipmh_common_app.egg-info/top_level.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2024-03-12 19:05:40.000000 core_oaipmh_common_app-2.8.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       21 2024-03-12 19:05:40.000000 core_oaipmh_common_app-2.8.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       42 2024-03-12 19:05:40.000000 core_oaipmh_common_app-2.8.0/requirements.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2024-03-12 19:05:43.130983 core_oaipmh_common_app-2.8.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1420 2024-03-12 19:05:40.000000 core_oaipmh_common_app-2.8.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:42.964869 core_oaipmh_common_app-2.8.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:40.000000 core_oaipmh_common_app-2.8.0/tests/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:42.979002 core_oaipmh_common_app-2.8.0/tests/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:40.000000 core_oaipmh_common_app-2.8.0/tests/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:43.019948 core_oaipmh_common_app-2.8.0/tests/components/oai_metadata_format/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:40.000000 core_oaipmh_common_app-2.8.0/tests/components/oai_metadata_format/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6179 2024-03-12 19:05:40.000000 core_oaipmh_common_app-2.8.0/tests/components/oai_metadata_format/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:43.037099 core_oaipmh_common_app-2.8.0/tests/components/oai_set/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:40.000000 core_oaipmh_common_app-2.8.0/tests/components/oai_set/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:43.076157 core_oaipmh_common_app-2.8.0/tests/components/oai_set/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:40.000000 core_oaipmh_common_app-2.8.0/tests/components/oai_set/tests/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4771 2024-03-12 19:05:40.000000 core_oaipmh_common_app-2.8.0/tests/components/oai_set/tests/tests_unit.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1510 2024-03-12 19:05:40.000000 core_oaipmh_common_app-2.8.0/tests/test_settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:43.111750 core_oaipmh_common_app-2.8.0/tests/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:40.000000 core_oaipmh_common_app-2.8.0/tests/utils/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1389 2024-03-12 19:05:40.000000 core_oaipmh_common_app-2.8.0/tests/utils/tests_iso8601_operation.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:45.066708 core_oaipmh_common_app-2.9.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2024-05-13 16:10:41.000000 core_oaipmh_common_app-2.9.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      177 2024-05-13 16:10:41.000000 core_oaipmh_common_app-2.9.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1089 2024-05-13 16:10:45.061050 core_oaipmh_common_app-2.9.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      593 2024-05-13 16:10:41.000000 core_oaipmh_common_app-2.9.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:44.450480 core_oaipmh_common_app-2.9.0/core_oaipmh_common_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:41.000000 core_oaipmh_common_app-2.9.0/core_oaipmh_common_app/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:44.613470 core_oaipmh_common_app-2.9.0/core_oaipmh_common_app/commons/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:41.000000 core_oaipmh_common_app-2.9.0/core_oaipmh_common_app/commons/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1643 2024-05-13 16:10:41.000000 core_oaipmh_common_app-2.9.0/core_oaipmh_common_app/commons/exceptions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      798 2024-05-13 16:10:41.000000 core_oaipmh_common_app-2.9.0/core_oaipmh_common_app/commons/messages.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:44.634831 core_oaipmh_common_app-2.9.0/core_oaipmh_common_app/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:41.000000 core_oaipmh_common_app-2.9.0/core_oaipmh_common_app/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:44.711600 core_oaipmh_common_app-2.9.0/core_oaipmh_common_app/components/oai_metadata_format/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:41.000000 core_oaipmh_common_app-2.9.0/core_oaipmh_common_app/components/oai_metadata_format/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1094 2024-05-13 16:10:41.000000 core_oaipmh_common_app-2.9.0/core_oaipmh_common_app/components/oai_metadata_format/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2908 2024-05-13 16:10:41.000000 core_oaipmh_common_app-2.9.0/core_oaipmh_common_app/components/oai_metadata_format/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:44.771483 core_oaipmh_common_app-2.9.0/core_oaipmh_common_app/components/oai_set/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:41.000000 core_oaipmh_common_app-2.9.0/core_oaipmh_common_app/components/oai_set/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      795 2024-05-13 16:10:41.000000 core_oaipmh_common_app-2.9.0/core_oaipmh_common_app/components/oai_set/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2033 2024-05-13 16:10:41.000000 core_oaipmh_common_app-2.9.0/core_oaipmh_common_app/components/oai_set/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:44.790948 core_oaipmh_common_app-2.9.0/core_oaipmh_common_app/migrations/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:41.000000 core_oaipmh_common_app-2.9.0/core_oaipmh_common_app/migrations/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:44.842981 core_oaipmh_common_app-2.9.0/core_oaipmh_common_app/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      865 2024-05-13 16:10:41.000000 core_oaipmh_common_app-2.9.0/core_oaipmh_common_app/utils/UTCdatetime.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:41.000000 core_oaipmh_common_app-2.9.0/core_oaipmh_common_app/utils/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:44.550989 core_oaipmh_common_app-2.9.0/core_oaipmh_common_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1089 2024-05-13 16:10:43.000000 core_oaipmh_common_app-2.9.0/core_oaipmh_common_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1372 2024-05-13 16:10:44.000000 core_oaipmh_common_app-2.9.0/core_oaipmh_common_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2024-05-13 16:10:43.000000 core_oaipmh_common_app-2.9.0/core_oaipmh_common_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       63 2024-05-13 16:10:43.000000 core_oaipmh_common_app-2.9.0/core_oaipmh_common_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       29 2024-05-13 16:10:43.000000 core_oaipmh_common_app-2.9.0/core_oaipmh_common_app.egg-info/top_level.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2024-05-13 16:10:42.000000 core_oaipmh_common_app-2.9.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       21 2024-05-13 16:10:42.000000 core_oaipmh_common_app-2.9.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       42 2024-05-13 16:10:42.000000 core_oaipmh_common_app-2.9.0/requirements.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2024-05-13 16:10:45.069223 core_oaipmh_common_app-2.9.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1420 2024-05-13 16:10:42.000000 core_oaipmh_common_app-2.9.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:44.883154 core_oaipmh_common_app-2.9.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:42.000000 core_oaipmh_common_app-2.9.0/tests/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:44.913518 core_oaipmh_common_app-2.9.0/tests/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:42.000000 core_oaipmh_common_app-2.9.0/tests/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:44.955799 core_oaipmh_common_app-2.9.0/tests/components/oai_metadata_format/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:42.000000 core_oaipmh_common_app-2.9.0/tests/components/oai_metadata_format/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6179 2024-05-13 16:10:42.000000 core_oaipmh_common_app-2.9.0/tests/components/oai_metadata_format/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:44.970654 core_oaipmh_common_app-2.9.0/tests/components/oai_set/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:42.000000 core_oaipmh_common_app-2.9.0/tests/components/oai_set/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:45.008546 core_oaipmh_common_app-2.9.0/tests/components/oai_set/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:42.000000 core_oaipmh_common_app-2.9.0/tests/components/oai_set/tests/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4771 2024-05-13 16:10:42.000000 core_oaipmh_common_app-2.9.0/tests/components/oai_set/tests/tests_unit.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1510 2024-05-13 16:10:42.000000 core_oaipmh_common_app-2.9.0/tests/test_settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:45.050173 core_oaipmh_common_app-2.9.0/tests/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:42.000000 core_oaipmh_common_app-2.9.0/tests/utils/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1389 2024-05-13 16:10:42.000000 core_oaipmh_common_app-2.9.0/tests/utils/tests_iso8601_operation.py
```

### Comparing `core_oaipmh_common_app-2.8.0/LICENSE.md` & `core_oaipmh_common_app-2.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `core_oaipmh_common_app-2.8.0/PKG-INFO` & `core_oaipmh_common_app-2.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_oaipmh_common_app
-Version: 2.8.0
+Version: 2.9.0
 Summary: Base OAI-PMH functions for the curator core project
 Home-page: https://github.com/usnistgov/core_oaipmh_common_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: ======================
         Core Oaipmh Common App
```

### Comparing `core_oaipmh_common_app-2.8.0/README.rst` & `core_oaipmh_common_app-2.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_oaipmh_common_app-2.8.0/core_oaipmh_common_app/commons/exceptions.py` & `core_oaipmh_common_app-2.9.0/core_oaipmh_common_app/commons/exceptions.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_common_app-2.8.0/core_oaipmh_common_app/commons/messages.py` & `core_oaipmh_common_app-2.9.0/core_oaipmh_common_app/commons/messages.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_common_app-2.8.0/core_oaipmh_common_app/components/oai_metadata_format/api.py` & `core_oaipmh_common_app-2.9.0/core_oaipmh_common_app/components/oai_metadata_format/api.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_common_app-2.8.0/core_oaipmh_common_app/components/oai_metadata_format/models.py` & `core_oaipmh_common_app-2.9.0/core_oaipmh_common_app/components/oai_metadata_format/models.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_common_app-2.8.0/core_oaipmh_common_app/components/oai_set/api.py` & `core_oaipmh_common_app-2.9.0/core_oaipmh_common_app/components/oai_set/api.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_common_app-2.8.0/core_oaipmh_common_app/components/oai_set/models.py` & `core_oaipmh_common_app-2.9.0/core_oaipmh_common_app/components/oai_set/models.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_common_app-2.8.0/core_oaipmh_common_app/utils/UTCdatetime.py` & `core_oaipmh_common_app-2.9.0/core_oaipmh_common_app/utils/UTCdatetime.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_common_app-2.8.0/core_oaipmh_common_app.egg-info/PKG-INFO` & `core_oaipmh_common_app-2.9.0/core_oaipmh_common_app.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-oaipmh-common-app
-Version: 2.8.0
+Version: 2.9.0
 Summary: Base OAI-PMH functions for the curator core project
 Home-page: https://github.com/usnistgov/core_oaipmh_common_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: ======================
         Core Oaipmh Common App
```

### Comparing `core_oaipmh_common_app-2.8.0/core_oaipmh_common_app.egg-info/SOURCES.txt` & `core_oaipmh_common_app-2.9.0/core_oaipmh_common_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `core_oaipmh_common_app-2.8.0/setup.py` & `core_oaipmh_common_app-2.9.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_oaipmh_common_app",
-    version="2.8.0",
+    version="2.9.0",
     description="Base OAI-PMH functions for the curator core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_oaipmh_common_app",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `core_oaipmh_common_app-2.8.0/tests/components/oai_metadata_format/tests_unit.py` & `core_oaipmh_common_app-2.9.0/tests/components/oai_metadata_format/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_common_app-2.8.0/tests/components/oai_set/tests/tests_unit.py` & `core_oaipmh_common_app-2.9.0/tests/components/oai_set/tests/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_common_app-2.8.0/tests/test_settings.py` & `core_oaipmh_common_app-2.9.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_common_app-2.8.0/tests/utils/tests_iso8601_operation.py` & `core_oaipmh_common_app-2.9.0/tests/utils/tests_iso8601_operation.py`

 * *Files identical despite different names*

