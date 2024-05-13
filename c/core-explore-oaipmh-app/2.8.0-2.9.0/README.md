# Comparing `tmp/core_explore_oaipmh_app-2.8.0.tar.gz` & `tmp/core_explore_oaipmh_app-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_explore_oaipmh_app-2.8.0.tar", last modified: Tue Mar 12 19:00:22 2024, max compression
+gzip compressed data, was "core_explore_oaipmh_app-2.9.0.tar", last modified: Mon May 13 16:05:59 2024, max compression
```

## Comparing `core_explore_oaipmh_app-2.8.0.tar` & `core_explore_oaipmh_app-2.9.0.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:22.521803 core_explore_oaipmh_app-2.8.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2024-03-12 19:00:17.000000 core_explore_oaipmh_app-2.8.0/LICENSE.md
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      154 2024-03-12 19:00:17.000000 core_explore_oaipmh_app-2.8.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1428 2024-03-12 19:00:22.515541 core_explore_oaipmh_app-2.8.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      855 2024-03-12 19:00:17.000000 core_explore_oaipmh_app-2.8.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:21.511010 core_explore_oaipmh_app-2.8.0/core_explore_oaipmh_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:17.000000 core_explore_oaipmh_app-2.8.0/core_explore_oaipmh_app/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:21.625999 core_explore_oaipmh_app-2.8.0/core_explore_oaipmh_app/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:17.000000 core_explore_oaipmh_app-2.8.0/core_explore_oaipmh_app/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:21.666215 core_explore_oaipmh_app-2.8.0/core_explore_oaipmh_app/components/query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:17.000000 core_explore_oaipmh_app-2.8.0/core_explore_oaipmh_app/components/query/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1713 2024-03-12 19:00:17.000000 core_explore_oaipmh_app-2.8.0/core_explore_oaipmh_app/components/query/api.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:21.853020 core_explore_oaipmh_app-2.8.0/core_explore_oaipmh_app/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:18.000000 core_explore_oaipmh_app-2.8.0/core_explore_oaipmh_app/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:21.892910 core_explore_oaipmh_app-2.8.0/core_explore_oaipmh_app/rest/query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:18.000000 core_explore_oaipmh_app-2.8.0/core_explore_oaipmh_app/rest/query/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6525 2024-03-12 19:00:18.000000 core_explore_oaipmh_app-2.8.0/core_explore_oaipmh_app/rest/query/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:21.930499 core_explore_oaipmh_app-2.8.0/core_explore_oaipmh_app/rest/result/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:18.000000 core_explore_oaipmh_app-2.8.0/core_explore_oaipmh_app/rest/result/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1747 2024-03-12 19:00:18.000000 core_explore_oaipmh_app-2.8.0/core_explore_oaipmh_app/rest/result/views.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      313 2024-03-12 19:00:18.000000 core_explore_oaipmh_app-2.8.0/core_explore_oaipmh_app/rest/urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      333 2024-03-12 19:00:18.000000 core_explore_oaipmh_app-2.8.0/core_explore_oaipmh_app/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:21.239020 core_explore_oaipmh_app-2.8.0/core_explore_oaipmh_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:21.243610 core_explore_oaipmh_app-2.8.0/core_explore_oaipmh_app/static/core_explore_oaipmh_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:21.248202 core_explore_oaipmh_app-2.8.0/core_explore_oaipmh_app/static/core_explore_oaipmh_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:21.258992 core_explore_oaipmh_app-2.8.0/core_explore_oaipmh_app/static/core_explore_oaipmh_app/user/js/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:21.947689 core_explore_oaipmh_app-2.8.0/core_explore_oaipmh_app/static/core_explore_oaipmh_app/user/js/data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      127 2024-03-12 19:00:18.000000 core_explore_oaipmh_app-2.8.0/core_explore_oaipmh_app/static/core_explore_oaipmh_app/user/js/data/change_display.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:21.965772 core_explore_oaipmh_app-2.8.0/core_explore_oaipmh_app/static/core_explore_oaipmh_app/user/js/data_sources/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2332 2024-03-12 19:00:18.000000 core_explore_oaipmh_app-2.8.0/core_explore_oaipmh_app/static/core_explore_oaipmh_app/user/js/data_sources/list.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:21.275252 core_explore_oaipmh_app-2.8.0/core_explore_oaipmh_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:21.279687 core_explore_oaipmh_app-2.8.0/core_explore_oaipmh_app/templates/core_explore_oaipmh_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:21.284533 core_explore_oaipmh_app-2.8.0/core_explore_oaipmh_app/templates/core_explore_oaipmh_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:22.013181 core_explore_oaipmh_app-2.8.0/core_explore_oaipmh_app/templates/core_explore_oaipmh_app/user/data_sources/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      673 2024-03-12 19:00:18.000000 core_explore_oaipmh_app-2.8.0/core_explore_oaipmh_app/templates/core_explore_oaipmh_app/user/data_sources/list-content.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1279 2024-03-12 19:00:18.000000 core_explore_oaipmh_app-2.8.0/core_explore_oaipmh_app/templates/core_explore_oaipmh_app/user/data_sources/list.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      934 2024-03-12 19:00:18.000000 core_explore_oaipmh_app-2.8.0/core_explore_oaipmh_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:22.036623 core_explore_oaipmh_app-2.8.0/core_explore_oaipmh_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:18.000000 core_explore_oaipmh_app-2.8.0/core_explore_oaipmh_app/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:22.099649 core_explore_oaipmh_app-2.8.0/core_explore_oaipmh_app/views/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:18.000000 core_explore_oaipmh_app-2.8.0/core_explore_oaipmh_app/views/user/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5958 2024-03-12 19:00:18.000000 core_explore_oaipmh_app-2.8.0/core_explore_oaipmh_app/views/user/ajax.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1938 2024-03-12 19:00:18.000000 core_explore_oaipmh_app-2.8.0/core_explore_oaipmh_app/views/user/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:21.605822 core_explore_oaipmh_app-2.8.0/core_explore_oaipmh_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1428 2024-03-12 19:00:20.000000 core_explore_oaipmh_app-2.8.0/core_explore_oaipmh_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1868 2024-03-12 19:00:21.000000 core_explore_oaipmh_app-2.8.0/core_explore_oaipmh_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2024-03-12 19:00:20.000000 core_explore_oaipmh_app-2.8.0/core_explore_oaipmh_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      147 2024-03-12 19:00:20.000000 core_explore_oaipmh_app-2.8.0/core_explore_oaipmh_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       30 2024-03-12 19:00:20.000000 core_explore_oaipmh_app-2.8.0/core_explore_oaipmh_app.egg-info/top_level.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2024-03-12 19:00:18.000000 core_explore_oaipmh_app-2.8.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      115 2024-03-12 19:00:18.000000 core_explore_oaipmh_app-2.8.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2024-03-12 19:00:22.525366 core_explore_oaipmh_app-2.8.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1079 2024-03-12 19:00:18.000000 core_explore_oaipmh_app-2.8.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:22.162428 core_explore_oaipmh_app-2.8.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:18.000000 core_explore_oaipmh_app-2.8.0/tests/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:22.211352 core_explore_oaipmh_app-2.8.0/tests/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:18.000000 core_explore_oaipmh_app-2.8.0/tests/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6073 2024-03-12 19:00:18.000000 core_explore_oaipmh_app-2.8.0/tests/fixtures/fixtures.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:22.232730 core_explore_oaipmh_app-2.8.0/tests/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:18.000000 core_explore_oaipmh_app-2.8.0/tests/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:22.277975 core_explore_oaipmh_app-2.8.0/tests/rest/query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:18.000000 core_explore_oaipmh_app-2.8.0/tests/rest/query/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7300 2024-03-12 19:00:18.000000 core_explore_oaipmh_app-2.8.0/tests/rest/query/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:22.324934 core_explore_oaipmh_app-2.8.0/tests/rest/result/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:18.000000 core_explore_oaipmh_app-2.8.0/tests/rest/result/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2845 2024-03-12 19:00:18.000000 core_explore_oaipmh_app-2.8.0/tests/rest/result/tests_permissions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2093 2024-03-12 19:00:18.000000 core_explore_oaipmh_app-2.8.0/tests/test_settings.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      316 2024-03-12 19:00:18.000000 core_explore_oaipmh_app-2.8.0/tests/test_urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:22.351619 core_explore_oaipmh_app-2.8.0/tests/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:19.000000 core_explore_oaipmh_app-2.8.0/tests/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:22.378785 core_explore_oaipmh_app-2.8.0/tests/views/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:19.000000 core_explore_oaipmh_app-2.8.0/tests/views/user/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:22.448973 core_explore_oaipmh_app-2.8.0/tests/views/user/ajax/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:19.000000 core_explore_oaipmh_app-2.8.0/tests/views/user/ajax/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2219 2024-03-12 19:00:19.000000 core_explore_oaipmh_app-2.8.0/tests/views/user/ajax/tests_permissions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14034 2024-03-12 19:00:19.000000 core_explore_oaipmh_app-2.8.0/tests/views/user/ajax/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:22.495051 core_explore_oaipmh_app-2.8.0/tests/views/user/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:19.000000 core_explore_oaipmh_app-2.8.0/tests/views/user/views/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5472 2024-03-12 19:00:19.000000 core_explore_oaipmh_app-2.8.0/tests/views/user/views/tests_permissions.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:59.370896 core_explore_oaipmh_app-2.9.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2024-05-13 16:05:54.000000 core_explore_oaipmh_app-2.9.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      154 2024-05-13 16:05:54.000000 core_explore_oaipmh_app-2.9.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1428 2024-05-13 16:05:59.364209 core_explore_oaipmh_app-2.9.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      855 2024-05-13 16:05:54.000000 core_explore_oaipmh_app-2.9.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:58.201242 core_explore_oaipmh_app-2.9.0/core_explore_oaipmh_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:54.000000 core_explore_oaipmh_app-2.9.0/core_explore_oaipmh_app/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:58.345029 core_explore_oaipmh_app-2.9.0/core_explore_oaipmh_app/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:54.000000 core_explore_oaipmh_app-2.9.0/core_explore_oaipmh_app/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:58.388428 core_explore_oaipmh_app-2.9.0/core_explore_oaipmh_app/components/query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:54.000000 core_explore_oaipmh_app-2.9.0/core_explore_oaipmh_app/components/query/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1713 2024-05-13 16:05:54.000000 core_explore_oaipmh_app-2.9.0/core_explore_oaipmh_app/components/query/api.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:58.435088 core_explore_oaipmh_app-2.9.0/core_explore_oaipmh_app/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:54.000000 core_explore_oaipmh_app-2.9.0/core_explore_oaipmh_app/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:58.475906 core_explore_oaipmh_app-2.9.0/core_explore_oaipmh_app/rest/query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:54.000000 core_explore_oaipmh_app-2.9.0/core_explore_oaipmh_app/rest/query/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6525 2024-05-13 16:05:54.000000 core_explore_oaipmh_app-2.9.0/core_explore_oaipmh_app/rest/query/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:58.528211 core_explore_oaipmh_app-2.9.0/core_explore_oaipmh_app/rest/result/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:54.000000 core_explore_oaipmh_app-2.9.0/core_explore_oaipmh_app/rest/result/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1747 2024-05-13 16:05:54.000000 core_explore_oaipmh_app-2.9.0/core_explore_oaipmh_app/rest/result/views.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      313 2024-05-13 16:05:54.000000 core_explore_oaipmh_app-2.9.0/core_explore_oaipmh_app/rest/urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      333 2024-05-13 16:05:54.000000 core_explore_oaipmh_app-2.9.0/core_explore_oaipmh_app/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:57.907060 core_explore_oaipmh_app-2.9.0/core_explore_oaipmh_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:57.911116 core_explore_oaipmh_app-2.9.0/core_explore_oaipmh_app/static/core_explore_oaipmh_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:57.915207 core_explore_oaipmh_app-2.9.0/core_explore_oaipmh_app/static/core_explore_oaipmh_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:57.934559 core_explore_oaipmh_app-2.9.0/core_explore_oaipmh_app/static/core_explore_oaipmh_app/user/js/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:58.551053 core_explore_oaipmh_app-2.9.0/core_explore_oaipmh_app/static/core_explore_oaipmh_app/user/js/data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      127 2024-05-13 16:05:54.000000 core_explore_oaipmh_app-2.9.0/core_explore_oaipmh_app/static/core_explore_oaipmh_app/user/js/data/change_display.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:58.570333 core_explore_oaipmh_app-2.9.0/core_explore_oaipmh_app/static/core_explore_oaipmh_app/user/js/data_sources/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2332 2024-05-13 16:05:54.000000 core_explore_oaipmh_app-2.9.0/core_explore_oaipmh_app/static/core_explore_oaipmh_app/user/js/data_sources/list.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:57.953275 core_explore_oaipmh_app-2.9.0/core_explore_oaipmh_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:57.957268 core_explore_oaipmh_app-2.9.0/core_explore_oaipmh_app/templates/core_explore_oaipmh_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:57.961637 core_explore_oaipmh_app-2.9.0/core_explore_oaipmh_app/templates/core_explore_oaipmh_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:58.612812 core_explore_oaipmh_app-2.9.0/core_explore_oaipmh_app/templates/core_explore_oaipmh_app/user/data_sources/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      673 2024-05-13 16:05:54.000000 core_explore_oaipmh_app-2.9.0/core_explore_oaipmh_app/templates/core_explore_oaipmh_app/user/data_sources/list-content.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1279 2024-05-13 16:05:54.000000 core_explore_oaipmh_app-2.9.0/core_explore_oaipmh_app/templates/core_explore_oaipmh_app/user/data_sources/list.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      934 2024-05-13 16:05:54.000000 core_explore_oaipmh_app-2.9.0/core_explore_oaipmh_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:58.634667 core_explore_oaipmh_app-2.9.0/core_explore_oaipmh_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:54.000000 core_explore_oaipmh_app-2.9.0/core_explore_oaipmh_app/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:58.727119 core_explore_oaipmh_app-2.9.0/core_explore_oaipmh_app/views/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:54.000000 core_explore_oaipmh_app-2.9.0/core_explore_oaipmh_app/views/user/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5958 2024-05-13 16:05:54.000000 core_explore_oaipmh_app-2.9.0/core_explore_oaipmh_app/views/user/ajax.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1938 2024-05-13 16:05:55.000000 core_explore_oaipmh_app-2.9.0/core_explore_oaipmh_app/views/user/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:58.311742 core_explore_oaipmh_app-2.9.0/core_explore_oaipmh_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1428 2024-05-13 16:05:57.000000 core_explore_oaipmh_app-2.9.0/core_explore_oaipmh_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1868 2024-05-13 16:05:57.000000 core_explore_oaipmh_app-2.9.0/core_explore_oaipmh_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2024-05-13 16:05:57.000000 core_explore_oaipmh_app-2.9.0/core_explore_oaipmh_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      147 2024-05-13 16:05:57.000000 core_explore_oaipmh_app-2.9.0/core_explore_oaipmh_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       30 2024-05-13 16:05:57.000000 core_explore_oaipmh_app-2.9.0/core_explore_oaipmh_app.egg-info/top_level.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2024-05-13 16:05:55.000000 core_explore_oaipmh_app-2.9.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      115 2024-05-13 16:05:55.000000 core_explore_oaipmh_app-2.9.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2024-05-13 16:05:59.373657 core_explore_oaipmh_app-2.9.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1079 2024-05-13 16:05:55.000000 core_explore_oaipmh_app-2.9.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:58.788702 core_explore_oaipmh_app-2.9.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:55.000000 core_explore_oaipmh_app-2.9.0/tests/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:58.830458 core_explore_oaipmh_app-2.9.0/tests/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:55.000000 core_explore_oaipmh_app-2.9.0/tests/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6073 2024-05-13 16:05:55.000000 core_explore_oaipmh_app-2.9.0/tests/fixtures/fixtures.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:58.848817 core_explore_oaipmh_app-2.9.0/tests/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:55.000000 core_explore_oaipmh_app-2.9.0/tests/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:59.134724 core_explore_oaipmh_app-2.9.0/tests/rest/query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:55.000000 core_explore_oaipmh_app-2.9.0/tests/rest/query/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7300 2024-05-13 16:05:55.000000 core_explore_oaipmh_app-2.9.0/tests/rest/query/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:59.178617 core_explore_oaipmh_app-2.9.0/tests/rest/result/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:55.000000 core_explore_oaipmh_app-2.9.0/tests/rest/result/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2845 2024-05-13 16:05:55.000000 core_explore_oaipmh_app-2.9.0/tests/rest/result/tests_permissions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2093 2024-05-13 16:05:55.000000 core_explore_oaipmh_app-2.9.0/tests/test_settings.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      316 2024-05-13 16:05:55.000000 core_explore_oaipmh_app-2.9.0/tests/test_urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:59.199225 core_explore_oaipmh_app-2.9.0/tests/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:55.000000 core_explore_oaipmh_app-2.9.0/tests/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:59.223996 core_explore_oaipmh_app-2.9.0/tests/views/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:55.000000 core_explore_oaipmh_app-2.9.0/tests/views/user/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:59.296031 core_explore_oaipmh_app-2.9.0/tests/views/user/ajax/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:55.000000 core_explore_oaipmh_app-2.9.0/tests/views/user/ajax/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2219 2024-05-13 16:05:55.000000 core_explore_oaipmh_app-2.9.0/tests/views/user/ajax/tests_permissions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14034 2024-05-13 16:05:55.000000 core_explore_oaipmh_app-2.9.0/tests/views/user/ajax/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:59.342831 core_explore_oaipmh_app-2.9.0/tests/views/user/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:55.000000 core_explore_oaipmh_app-2.9.0/tests/views/user/views/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5472 2024-05-13 16:05:55.000000 core_explore_oaipmh_app-2.9.0/tests/views/user/views/tests_permissions.py
```

### Comparing `core_explore_oaipmh_app-2.8.0/LICENSE.md` & `core_explore_oaipmh_app-2.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `core_explore_oaipmh_app-2.8.0/PKG-INFO` & `core_explore_oaipmh_app-2.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_explore_oaipmh_app
-Version: 2.8.0
+Version: 2.9.0
 Summary: OAI-PMH exploration functions for curator core project
 Home-page: https://github.com/usnistgov/core_explore_oaipmh_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: =======================
         Core Explore Oaipmh App
```

### Comparing `core_explore_oaipmh_app-2.8.0/README.rst` & `core_explore_oaipmh_app-2.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_explore_oaipmh_app-2.8.0/core_explore_oaipmh_app/components/query/api.py` & `core_explore_oaipmh_app-2.9.0/core_explore_oaipmh_app/components/query/api.py`

 * *Files identical despite different names*

### Comparing `core_explore_oaipmh_app-2.8.0/core_explore_oaipmh_app/rest/query/views.py` & `core_explore_oaipmh_app-2.9.0/core_explore_oaipmh_app/rest/query/views.py`

 * *Files identical despite different names*

### Comparing `core_explore_oaipmh_app-2.8.0/core_explore_oaipmh_app/rest/result/views.py` & `core_explore_oaipmh_app-2.9.0/core_explore_oaipmh_app/rest/result/views.py`

 * *Files identical despite different names*

### Comparing `core_explore_oaipmh_app-2.8.0/core_explore_oaipmh_app/static/core_explore_oaipmh_app/user/js/data_sources/list.js` & `core_explore_oaipmh_app-2.9.0/core_explore_oaipmh_app/static/core_explore_oaipmh_app/user/js/data_sources/list.js`

 * *Files identical despite different names*

### Comparing `core_explore_oaipmh_app-2.8.0/core_explore_oaipmh_app/templates/core_explore_oaipmh_app/user/data_sources/list-content.html` & `core_explore_oaipmh_app-2.9.0/core_explore_oaipmh_app/templates/core_explore_oaipmh_app/user/data_sources/list-content.html`

 * *Files identical despite different names*

### Comparing `core_explore_oaipmh_app-2.8.0/core_explore_oaipmh_app/templates/core_explore_oaipmh_app/user/data_sources/list.html` & `core_explore_oaipmh_app-2.9.0/core_explore_oaipmh_app/templates/core_explore_oaipmh_app/user/data_sources/list.html`

 * *Files identical despite different names*

### Comparing `core_explore_oaipmh_app-2.8.0/core_explore_oaipmh_app/urls.py` & `core_explore_oaipmh_app-2.9.0/core_explore_oaipmh_app/urls.py`

 * *Files identical despite different names*

### Comparing `core_explore_oaipmh_app-2.8.0/core_explore_oaipmh_app/views/user/ajax.py` & `core_explore_oaipmh_app-2.9.0/core_explore_oaipmh_app/views/user/ajax.py`

 * *Files identical despite different names*

### Comparing `core_explore_oaipmh_app-2.8.0/core_explore_oaipmh_app/views/user/views.py` & `core_explore_oaipmh_app-2.9.0/core_explore_oaipmh_app/views/user/views.py`

 * *Files identical despite different names*

### Comparing `core_explore_oaipmh_app-2.8.0/core_explore_oaipmh_app.egg-info/PKG-INFO` & `core_explore_oaipmh_app-2.9.0/core_explore_oaipmh_app.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-explore-oaipmh-app
-Version: 2.8.0
+Version: 2.9.0
 Summary: OAI-PMH exploration functions for curator core project
 Home-page: https://github.com/usnistgov/core_explore_oaipmh_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: =======================
         Core Explore Oaipmh App
```

### Comparing `core_explore_oaipmh_app-2.8.0/core_explore_oaipmh_app.egg-info/SOURCES.txt` & `core_explore_oaipmh_app-2.9.0/core_explore_oaipmh_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `core_explore_oaipmh_app-2.8.0/setup.py` & `core_explore_oaipmh_app-2.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_explore_oaipmh_app",
-    version="2.8.0",
+    version="2.9.0",
     description="OAI-PMH exploration functions for curator core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_explore_oaipmh_app",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `core_explore_oaipmh_app-2.8.0/tests/fixtures/fixtures.py` & `core_explore_oaipmh_app-2.9.0/tests/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_explore_oaipmh_app-2.8.0/tests/rest/query/tests_unit.py` & `core_explore_oaipmh_app-2.9.0/tests/rest/query/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_explore_oaipmh_app-2.8.0/tests/rest/result/tests_permissions.py` & `core_explore_oaipmh_app-2.9.0/tests/rest/result/tests_permissions.py`

 * *Files identical despite different names*

### Comparing `core_explore_oaipmh_app-2.8.0/tests/test_settings.py` & `core_explore_oaipmh_app-2.9.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `core_explore_oaipmh_app-2.8.0/tests/views/user/ajax/tests_permissions.py` & `core_explore_oaipmh_app-2.9.0/tests/views/user/ajax/tests_permissions.py`

 * *Files identical despite different names*

### Comparing `core_explore_oaipmh_app-2.8.0/tests/views/user/ajax/tests_unit.py` & `core_explore_oaipmh_app-2.9.0/tests/views/user/ajax/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_explore_oaipmh_app-2.8.0/tests/views/user/views/tests_permissions.py` & `core_explore_oaipmh_app-2.9.0/tests/views/user/views/tests_permissions.py`

 * *Files identical despite different names*

