# Comparing `tmp/core_curate_registry_app-2.8.0.tar.gz` & `tmp/core_curate_registry_app-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_curate_registry_app-2.8.0.tar", last modified: Tue Mar 12 18:57:56 2024, max compression
+gzip compressed data, was "core_curate_registry_app-2.9.0.tar", last modified: Mon May 13 16:03:22 2024, max compression
```

## Comparing `core_curate_registry_app-2.8.0.tar` & `core_curate_registry_app-2.9.0.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:56.499876 core_curate_registry_app-2.8.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2024-03-12 18:57:48.000000 core_curate_registry_app-2.8.0/LICENSE.md
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      156 2024-03-12 18:57:48.000000 core_curate_registry_app-2.8.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1180 2024-03-12 18:57:56.492506 core_curate_registry_app-2.8.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      644 2024-03-12 18:57:48.000000 core_curate_registry_app-2.8.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:53.826750 core_curate_registry_app-2.8.0/core_curate_registry_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:48.000000 core_curate_registry_app-2.8.0/core_curate_registry_app/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:53.948059 core_curate_registry_app-2.8.0/core_curate_registry_app/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:48.000000 core_curate_registry_app-2.8.0/core_curate_registry_app/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:53.999169 core_curate_registry_app-2.8.0/core_curate_registry_app/components/curate_data_structure/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:48.000000 core_curate_registry_app-2.8.0/core_curate_registry_app/components/curate_data_structure/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      620 2024-03-12 18:57:48.000000 core_curate_registry_app-2.8.0/core_curate_registry_app/components/curate_data_structure/api.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:55.730283 core_curate_registry_app-2.8.0/core_curate_registry_app/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:48.000000 core_curate_registry_app-2.8.0/core_curate_registry_app/rest/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      332 2024-03-12 18:57:48.000000 core_curate_registry_app-2.8.0/core_curate_registry_app/rest/urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      809 2024-03-12 18:57:48.000000 core_curate_registry_app-2.8.0/core_curate_registry_app/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:51.282895 core_curate_registry_app-2.8.0/core_curate_registry_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:51.269994 core_curate_registry_app-2.8.0/core_curate_registry_app/static/core_curate_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:51.273945 core_curate_registry_app-2.8.0/core_curate_registry_app/static/core_curate_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:55.805703 core_curate_registry_app-2.8.0/core_curate_registry_app/static/core_curate_app/user/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       75 2024-03-12 18:57:48.000000 core_curate_registry_app-2.8.0/core_curate_registry_app/static/core_curate_app/user/js/select_template.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2047 2024-03-12 18:57:48.000000 core_curate_registry_app-2.8.0/core_curate_registry_app/static/core_curate_app/user/js/view_data_registry.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      181 2024-03-12 18:57:48.000000 core_curate_registry_app-2.8.0/core_curate_registry_app/static/core_curate_app/user/js/view_data_registry.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:51.286763 core_curate_registry_app-2.8.0/core_curate_registry_app/static/core_curate_registry_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:51.296562 core_curate_registry_app-2.8.0/core_curate_registry_app/static/core_curate_registry_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:55.837064 core_curate_registry_app-2.8.0/core_curate_registry_app/static/core_curate_registry_app/user/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       61 2024-03-12 18:57:48.000000 core_curate_registry_app-2.8.0/core_curate_registry_app/static/core_curate_registry_app/user/css/index.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:55.973147 core_curate_registry_app-2.8.0/core_curate_registry_app/static/core_curate_registry_app/user/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      348 2024-03-12 18:57:48.000000 core_curate_registry_app-2.8.0/core_curate_registry_app/static/core_curate_registry_app/user/js/banner.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1056 2024-03-12 18:57:48.000000 core_curate_registry_app-2.8.0/core_curate_registry_app/static/core_curate_registry_app/user/js/enter_data_registry.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       86 2024-03-12 18:57:48.000000 core_curate_registry_app-2.8.0/core_curate_registry_app/static/core_curate_registry_app/user/js/enter_data_registry.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      945 2024-03-12 18:57:48.000000 core_curate_registry_app-2.8.0/core_curate_registry_app/static/core_curate_registry_app/user/js/role.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      871 2024-03-12 18:57:48.000000 core_curate_registry_app-2.8.0/core_curate_registry_app/static/core_curate_registry_app/user/js/start_curate.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1158 2024-03-12 18:57:48.000000 core_curate_registry_app-2.8.0/core_curate_registry_app/static/core_curate_registry_app/user/js/title.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       45 2024-03-12 18:57:48.000000 core_curate_registry_app-2.8.0/core_curate_registry_app/static/core_curate_registry_app/user/js/title.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:53.620011 core_curate_registry_app-2.8.0/core_curate_registry_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:51.312962 core_curate_registry_app-2.8.0/core_curate_registry_app/templates/core_curate_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:56.001378 core_curate_registry_app-2.8.0/core_curate_registry_app/templates/core_curate_app/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      543 2024-03-12 18:57:48.000000 core_curate_registry_app-2.8.0/core_curate_registry_app/templates/core_curate_app/user/curate_start.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:56.026771 core_curate_registry_app-2.8.0/core_curate_registry_app/templates/core_curate_app/user/data-entry/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2942 2024-03-12 18:57:48.000000 core_curate_registry_app-2.8.0/core_curate_registry_app/templates/core_curate_app/user/data-entry/enter_data.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:56.049398 core_curate_registry_app-2.8.0/core_curate_registry_app/templates/core_curate_app/user/data-entry/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      786 2024-03-12 18:57:48.000000 core_curate_registry_app-2.8.0/core_curate_registry_app/templates/core_curate_app/user/data-entry/modals/xml-valid-registry.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:56.068986 core_curate_registry_app-2.8.0/core_curate_registry_app/templates/core_curate_app/user/data-review/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:56.089796 core_curate_registry_app-2.8.0/core_curate_registry_app/templates/core_curate_app/user/data-review/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1314 2024-03-12 18:57:48.000000 core_curate_registry_app-2.8.0/core_curate_registry_app/templates/core_curate_app/user/data-review/modals/save-form-registry.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1896 2024-03-12 18:57:48.000000 core_curate_registry_app-2.8.0/core_curate_registry_app/templates/core_curate_app/user/data-review/view_data.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:53.624176 core_curate_registry_app-2.8.0/core_curate_registry_app/templates/core_curate_registry_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:56.143034 core_curate_registry_app-2.8.0/core_curate_registry_app/templates/core_curate_registry_app/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1808 2024-03-12 18:57:48.000000 core_curate_registry_app-2.8.0/core_curate_registry_app/templates/core_curate_registry_app/user/curate.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      725 2024-03-12 18:57:48.000000 core_curate_registry_app-2.8.0/core_curate_registry_app/templates/core_curate_registry_app/user/index.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4544 2024-03-12 18:57:49.000000 core_curate_registry_app-2.8.0/core_curate_registry_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:56.187685 core_curate_registry_app-2.8.0/core_curate_registry_app/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:49.000000 core_curate_registry_app-2.8.0/core_curate_registry_app/utils/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      472 2024-03-12 18:57:49.000000 core_curate_registry_app-2.8.0/core_curate_registry_app/utils/jquery.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:56.210113 core_curate_registry_app-2.8.0/core_curate_registry_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:49.000000 core_curate_registry_app-2.8.0/core_curate_registry_app/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:56.279503 core_curate_registry_app-2.8.0/core_curate_registry_app/views/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:49.000000 core_curate_registry_app-2.8.0/core_curate_registry_app/views/user/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1463 2024-03-12 18:57:49.000000 core_curate_registry_app-2.8.0/core_curate_registry_app/views/user/ajax.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9664 2024-03-12 18:57:49.000000 core_curate_registry_app-2.8.0/core_curate_registry_app/views/user/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:53.924411 core_curate_registry_app-2.8.0/core_curate_registry_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1180 2024-03-12 18:57:50.000000 core_curate_registry_app-2.8.0/core_curate_registry_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2622 2024-03-12 18:57:51.000000 core_curate_registry_app-2.8.0/core_curate_registry_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2024-03-12 18:57:50.000000 core_curate_registry_app-2.8.0/core_curate_registry_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       60 2024-03-12 18:57:50.000000 core_curate_registry_app-2.8.0/core_curate_registry_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       31 2024-03-12 18:57:50.000000 core_curate_registry_app-2.8.0/core_curate_registry_app.egg-info/top_level.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2024-03-12 18:57:49.000000 core_curate_registry_app-2.8.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       53 2024-03-12 18:57:49.000000 core_curate_registry_app-2.8.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2024-03-12 18:57:56.503117 core_curate_registry_app-2.8.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1480 2024-03-12 18:57:49.000000 core_curate_registry_app-2.8.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:56.323612 core_curate_registry_app-2.8.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:49.000000 core_curate_registry_app-2.8.0/tests/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1352 2024-03-12 18:57:49.000000 core_curate_registry_app-2.8.0/tests/test_settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:56.392506 core_curate_registry_app-2.8.0/tests/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:49.000000 core_curate_registry_app-2.8.0/tests/utils/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      563 2024-03-12 18:57:49.000000 core_curate_registry_app-2.8.0/tests/utils/test_unit_urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1749 2024-03-12 18:57:49.000000 core_curate_registry_app-2.8.0/tests/utils/test_units.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:56.415802 core_curate_registry_app-2.8.0/tests/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:49.000000 core_curate_registry_app-2.8.0/tests/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:56.470894 core_curate_registry_app-2.8.0/tests/views/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:49.000000 core_curate_registry_app-2.8.0/tests/views/user/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1297 2024-03-12 18:57:49.000000 core_curate_registry_app-2.8.0/tests/views/user/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:22.891192 core_curate_registry_app-2.9.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2024-05-13 16:03:15.000000 core_curate_registry_app-2.9.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      156 2024-05-13 16:03:15.000000 core_curate_registry_app-2.9.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1180 2024-05-13 16:03:22.884258 core_curate_registry_app-2.9.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      644 2024-05-13 16:03:15.000000 core_curate_registry_app-2.9.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:21.722613 core_curate_registry_app-2.9.0/core_curate_registry_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:15.000000 core_curate_registry_app-2.9.0/core_curate_registry_app/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:21.842171 core_curate_registry_app-2.9.0/core_curate_registry_app/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:15.000000 core_curate_registry_app-2.9.0/core_curate_registry_app/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:21.886124 core_curate_registry_app-2.9.0/core_curate_registry_app/components/curate_data_structure/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:15.000000 core_curate_registry_app-2.9.0/core_curate_registry_app/components/curate_data_structure/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      620 2024-05-13 16:03:15.000000 core_curate_registry_app-2.9.0/core_curate_registry_app/components/curate_data_structure/api.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:21.962137 core_curate_registry_app-2.9.0/core_curate_registry_app/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:15.000000 core_curate_registry_app-2.9.0/core_curate_registry_app/rest/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      332 2024-05-13 16:03:15.000000 core_curate_registry_app-2.9.0/core_curate_registry_app/rest/urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      809 2024-05-13 16:03:15.000000 core_curate_registry_app-2.9.0/core_curate_registry_app/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:21.222388 core_curate_registry_app-2.9.0/core_curate_registry_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:21.209725 core_curate_registry_app-2.9.0/core_curate_registry_app/static/core_curate_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:21.213515 core_curate_registry_app-2.9.0/core_curate_registry_app/static/core_curate_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:22.046664 core_curate_registry_app-2.9.0/core_curate_registry_app/static/core_curate_app/user/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       75 2024-05-13 16:03:15.000000 core_curate_registry_app-2.9.0/core_curate_registry_app/static/core_curate_app/user/js/select_template.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2047 2024-05-13 16:03:15.000000 core_curate_registry_app-2.9.0/core_curate_registry_app/static/core_curate_app/user/js/view_data_registry.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      181 2024-05-13 16:03:15.000000 core_curate_registry_app-2.9.0/core_curate_registry_app/static/core_curate_app/user/js/view_data_registry.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:21.283384 core_curate_registry_app-2.9.0/core_curate_registry_app/static/core_curate_registry_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:21.375651 core_curate_registry_app-2.9.0/core_curate_registry_app/static/core_curate_registry_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:22.074860 core_curate_registry_app-2.9.0/core_curate_registry_app/static/core_curate_registry_app/user/css/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       61 2024-05-13 16:03:15.000000 core_curate_registry_app-2.9.0/core_curate_registry_app/static/core_curate_registry_app/user/css/index.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:22.215564 core_curate_registry_app-2.9.0/core_curate_registry_app/static/core_curate_registry_app/user/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      348 2024-05-13 16:03:15.000000 core_curate_registry_app-2.9.0/core_curate_registry_app/static/core_curate_registry_app/user/js/banner.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1056 2024-05-13 16:03:15.000000 core_curate_registry_app-2.9.0/core_curate_registry_app/static/core_curate_registry_app/user/js/enter_data_registry.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       86 2024-05-13 16:03:15.000000 core_curate_registry_app-2.9.0/core_curate_registry_app/static/core_curate_registry_app/user/js/enter_data_registry.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      945 2024-05-13 16:03:15.000000 core_curate_registry_app-2.9.0/core_curate_registry_app/static/core_curate_registry_app/user/js/role.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      871 2024-05-13 16:03:15.000000 core_curate_registry_app-2.9.0/core_curate_registry_app/static/core_curate_registry_app/user/js/start_curate.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1158 2024-05-13 16:03:15.000000 core_curate_registry_app-2.9.0/core_curate_registry_app/static/core_curate_registry_app/user/js/title.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       45 2024-05-13 16:03:15.000000 core_curate_registry_app-2.9.0/core_curate_registry_app/static/core_curate_registry_app/user/js/title.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:21.424021 core_curate_registry_app-2.9.0/core_curate_registry_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:21.393204 core_curate_registry_app-2.9.0/core_curate_registry_app/templates/core_curate_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:22.241736 core_curate_registry_app-2.9.0/core_curate_registry_app/templates/core_curate_app/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      543 2024-05-13 16:03:15.000000 core_curate_registry_app-2.9.0/core_curate_registry_app/templates/core_curate_app/user/curate_start.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:22.264993 core_curate_registry_app-2.9.0/core_curate_registry_app/templates/core_curate_app/user/data-entry/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2942 2024-05-13 16:03:15.000000 core_curate_registry_app-2.9.0/core_curate_registry_app/templates/core_curate_app/user/data-entry/enter_data.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:22.305804 core_curate_registry_app-2.9.0/core_curate_registry_app/templates/core_curate_app/user/data-entry/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      786 2024-05-13 16:03:15.000000 core_curate_registry_app-2.9.0/core_curate_registry_app/templates/core_curate_app/user/data-entry/modals/xml-valid-registry.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:22.328824 core_curate_registry_app-2.9.0/core_curate_registry_app/templates/core_curate_app/user/data-review/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:22.350781 core_curate_registry_app-2.9.0/core_curate_registry_app/templates/core_curate_app/user/data-review/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1314 2024-05-13 16:03:15.000000 core_curate_registry_app-2.9.0/core_curate_registry_app/templates/core_curate_app/user/data-review/modals/save-form-registry.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1896 2024-05-13 16:03:15.000000 core_curate_registry_app-2.9.0/core_curate_registry_app/templates/core_curate_app/user/data-review/view_data.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:21.428206 core_curate_registry_app-2.9.0/core_curate_registry_app/templates/core_curate_registry_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:22.445091 core_curate_registry_app-2.9.0/core_curate_registry_app/templates/core_curate_registry_app/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1808 2024-05-13 16:03:15.000000 core_curate_registry_app-2.9.0/core_curate_registry_app/templates/core_curate_registry_app/user/curate.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      725 2024-05-13 16:03:15.000000 core_curate_registry_app-2.9.0/core_curate_registry_app/templates/core_curate_registry_app/user/index.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4544 2024-05-13 16:03:15.000000 core_curate_registry_app-2.9.0/core_curate_registry_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:22.526932 core_curate_registry_app-2.9.0/core_curate_registry_app/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:15.000000 core_curate_registry_app-2.9.0/core_curate_registry_app/utils/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      472 2024-05-13 16:03:15.000000 core_curate_registry_app-2.9.0/core_curate_registry_app/utils/jquery.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:22.549244 core_curate_registry_app-2.9.0/core_curate_registry_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:15.000000 core_curate_registry_app-2.9.0/core_curate_registry_app/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:22.638840 core_curate_registry_app-2.9.0/core_curate_registry_app/views/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:15.000000 core_curate_registry_app-2.9.0/core_curate_registry_app/views/user/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1463 2024-05-13 16:03:16.000000 core_curate_registry_app-2.9.0/core_curate_registry_app/views/user/ajax.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9664 2024-05-13 16:03:16.000000 core_curate_registry_app-2.9.0/core_curate_registry_app/views/user/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:21.820502 core_curate_registry_app-2.9.0/core_curate_registry_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1180 2024-05-13 16:03:17.000000 core_curate_registry_app-2.9.0/core_curate_registry_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2622 2024-05-13 16:03:18.000000 core_curate_registry_app-2.9.0/core_curate_registry_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2024-05-13 16:03:17.000000 core_curate_registry_app-2.9.0/core_curate_registry_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       60 2024-05-13 16:03:17.000000 core_curate_registry_app-2.9.0/core_curate_registry_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       31 2024-05-13 16:03:17.000000 core_curate_registry_app-2.9.0/core_curate_registry_app.egg-info/top_level.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2024-05-13 16:03:16.000000 core_curate_registry_app-2.9.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       53 2024-05-13 16:03:16.000000 core_curate_registry_app-2.9.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2024-05-13 16:03:22.894097 core_curate_registry_app-2.9.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1480 2024-05-13 16:03:16.000000 core_curate_registry_app-2.9.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:22.679809 core_curate_registry_app-2.9.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:16.000000 core_curate_registry_app-2.9.0/tests/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1352 2024-05-13 16:03:16.000000 core_curate_registry_app-2.9.0/tests/test_settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:22.739868 core_curate_registry_app-2.9.0/tests/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:16.000000 core_curate_registry_app-2.9.0/tests/utils/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      563 2024-05-13 16:03:16.000000 core_curate_registry_app-2.9.0/tests/utils/test_unit_urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1749 2024-05-13 16:03:16.000000 core_curate_registry_app-2.9.0/tests/utils/test_units.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:22.762746 core_curate_registry_app-2.9.0/tests/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:16.000000 core_curate_registry_app-2.9.0/tests/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:22.834853 core_curate_registry_app-2.9.0/tests/views/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:16.000000 core_curate_registry_app-2.9.0/tests/views/user/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1297 2024-05-13 16:03:16.000000 core_curate_registry_app-2.9.0/tests/views/user/test_unit.py
```

### Comparing `core_curate_registry_app-2.8.0/LICENSE.md` & `core_curate_registry_app-2.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `core_curate_registry_app-2.8.0/PKG-INFO` & `core_curate_registry_app-2.9.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_curate_registry_app
-Version: 2.8.0
+Version: 2.9.0
 Summary: Curation functionalities specific to Registry applications for the curator core project
 Home-page: https://github.com/usnistgov/core_curate_registry_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: Core Curate Registry App
         ========================
```

### Comparing `core_curate_registry_app-2.8.0/README.rst` & `core_curate_registry_app-2.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_curate_registry_app-2.8.0/core_curate_registry_app/components/curate_data_structure/api.py` & `core_curate_registry_app-2.9.0/core_curate_registry_app/components/curate_data_structure/api.py`

 * *Files identical despite different names*

### Comparing `core_curate_registry_app-2.8.0/core_curate_registry_app/settings.py` & `core_curate_registry_app-2.9.0/core_curate_registry_app/settings.py`

 * *Files identical despite different names*

### Comparing `core_curate_registry_app-2.8.0/core_curate_registry_app/static/core_curate_app/user/js/view_data_registry.js` & `core_curate_registry_app-2.9.0/core_curate_registry_app/static/core_curate_app/user/js/view_data_registry.js`

 * *Files identical despite different names*

### Comparing `core_curate_registry_app-2.8.0/core_curate_registry_app/static/core_curate_registry_app/user/js/enter_data_registry.js` & `core_curate_registry_app-2.9.0/core_curate_registry_app/static/core_curate_registry_app/user/js/enter_data_registry.js`

 * *Files identical despite different names*

### Comparing `core_curate_registry_app-2.8.0/core_curate_registry_app/static/core_curate_registry_app/user/js/role.js` & `core_curate_registry_app-2.9.0/core_curate_registry_app/static/core_curate_registry_app/user/js/role.js`

 * *Files identical despite different names*

### Comparing `core_curate_registry_app-2.8.0/core_curate_registry_app/static/core_curate_registry_app/user/js/start_curate.js` & `core_curate_registry_app-2.9.0/core_curate_registry_app/static/core_curate_registry_app/user/js/start_curate.js`

 * *Files identical despite different names*

### Comparing `core_curate_registry_app-2.8.0/core_curate_registry_app/static/core_curate_registry_app/user/js/title.js` & `core_curate_registry_app-2.9.0/core_curate_registry_app/static/core_curate_registry_app/user/js/title.js`

 * *Files identical despite different names*

### Comparing `core_curate_registry_app-2.8.0/core_curate_registry_app/templates/core_curate_app/user/curate_start.html` & `core_curate_registry_app-2.9.0/core_curate_registry_app/templates/core_curate_app/user/curate_start.html`

 * *Files identical despite different names*

### Comparing `core_curate_registry_app-2.8.0/core_curate_registry_app/templates/core_curate_app/user/data-entry/enter_data.html` & `core_curate_registry_app-2.9.0/core_curate_registry_app/templates/core_curate_app/user/data-entry/enter_data.html`

 * *Files identical despite different names*

### Comparing `core_curate_registry_app-2.8.0/core_curate_registry_app/templates/core_curate_app/user/data-entry/modals/xml-valid-registry.html` & `core_curate_registry_app-2.9.0/core_curate_registry_app/templates/core_curate_app/user/data-entry/modals/xml-valid-registry.html`

 * *Files identical despite different names*

### Comparing `core_curate_registry_app-2.8.0/core_curate_registry_app/templates/core_curate_app/user/data-review/modals/save-form-registry.html` & `core_curate_registry_app-2.9.0/core_curate_registry_app/templates/core_curate_app/user/data-review/modals/save-form-registry.html`

 * *Files identical despite different names*

### Comparing `core_curate_registry_app-2.8.0/core_curate_registry_app/templates/core_curate_app/user/data-review/view_data.html` & `core_curate_registry_app-2.9.0/core_curate_registry_app/templates/core_curate_app/user/data-review/view_data.html`

 * *Files identical despite different names*

### Comparing `core_curate_registry_app-2.8.0/core_curate_registry_app/templates/core_curate_registry_app/user/curate.html` & `core_curate_registry_app-2.9.0/core_curate_registry_app/templates/core_curate_registry_app/user/curate.html`

 * *Files identical despite different names*

### Comparing `core_curate_registry_app-2.8.0/core_curate_registry_app/templates/core_curate_registry_app/user/index.html` & `core_curate_registry_app-2.9.0/core_curate_registry_app/templates/core_curate_registry_app/user/index.html`

 * *Files identical despite different names*

### Comparing `core_curate_registry_app-2.8.0/core_curate_registry_app/urls.py` & `core_curate_registry_app-2.9.0/core_curate_registry_app/urls.py`

 * *Files identical despite different names*

### Comparing `core_curate_registry_app-2.8.0/core_curate_registry_app/views/user/ajax.py` & `core_curate_registry_app-2.9.0/core_curate_registry_app/views/user/ajax.py`

 * *Files identical despite different names*

### Comparing `core_curate_registry_app-2.8.0/core_curate_registry_app/views/user/views.py` & `core_curate_registry_app-2.9.0/core_curate_registry_app/views/user/views.py`

 * *Files identical despite different names*

### Comparing `core_curate_registry_app-2.8.0/core_curate_registry_app.egg-info/PKG-INFO` & `core_curate_registry_app-2.9.0/core_curate_registry_app.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-curate-registry-app
-Version: 2.8.0
+Version: 2.9.0
 Summary: Curation functionalities specific to Registry applications for the curator core project
 Home-page: https://github.com/usnistgov/core_curate_registry_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: Core Curate Registry App
         ========================
```

### Comparing `core_curate_registry_app-2.8.0/core_curate_registry_app.egg-info/SOURCES.txt` & `core_curate_registry_app-2.9.0/core_curate_registry_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `core_curate_registry_app-2.8.0/setup.py` & `core_curate_registry_app-2.9.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 chdir(normpath(join(abspath(__file__), pardir)))
 
 dep_links = [r for r in required if r.startswith("https://")]
 required = [req_link(r) if r.startswith("https://") else r for r in required]
 
 setup(
     name="core_curate_registry_app",
-    version="2.8.0",
+    version="2.9.0",
     description="Curation functionalities specific to Registry applications for the curator core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_curate_registry_app",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `core_curate_registry_app-2.8.0/tests/test_settings.py` & `core_curate_registry_app-2.9.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `core_curate_registry_app-2.8.0/tests/utils/test_unit_urls.py` & `core_curate_registry_app-2.9.0/tests/utils/test_unit_urls.py`

 * *Files identical despite different names*

### Comparing `core_curate_registry_app-2.8.0/tests/utils/test_units.py` & `core_curate_registry_app-2.9.0/tests/utils/test_units.py`

 * *Files identical despite different names*

### Comparing `core_curate_registry_app-2.8.0/tests/views/user/test_unit.py` & `core_curate_registry_app-2.9.0/tests/views/user/test_unit.py`

 * *Files identical despite different names*

