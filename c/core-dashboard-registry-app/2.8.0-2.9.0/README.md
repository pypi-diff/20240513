# Comparing `tmp/core_dashboard_registry_app-2.8.0.tar.gz` & `tmp/core_dashboard_registry_app-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_dashboard_registry_app-2.8.0.tar", last modified: Tue Mar 12 18:58:40 2024, max compression
+gzip compressed data, was "core_dashboard_registry_app-2.9.0.tar", last modified: Mon May 13 16:04:10 2024, max compression
```

## Comparing `core_dashboard_registry_app-2.8.0.tar` & `core_dashboard_registry_app-2.9.0.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:39.972976 core_dashboard_registry_app-2.8.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2024-03-12 18:58:35.000000 core_dashboard_registry_app-2.8.0/LICENSE.md
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      162 2024-03-12 18:58:35.000000 core_dashboard_registry_app-2.8.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1145 2024-03-12 18:58:39.966597 core_dashboard_registry_app-2.8.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      633 2024-03-12 18:58:36.000000 core_dashboard_registry_app-2.8.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:39.036946 core_dashboard_registry_app-2.8.0/core_dashboard_registry_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:36.000000 core_dashboard_registry_app-2.8.0/core_dashboard_registry_app/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3446 2024-03-12 18:58:36.000000 core_dashboard_registry_app-2.8.0/core_dashboard_registry_app/admin.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      661 2024-03-12 18:58:36.000000 core_dashboard_registry_app-2.8.0/core_dashboard_registry_app/constants.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2803 2024-03-12 18:58:36.000000 core_dashboard_registry_app-2.8.0/core_dashboard_registry_app/menus.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      415 2024-03-12 18:58:36.000000 core_dashboard_registry_app-2.8.0/core_dashboard_registry_app/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:38.677058 core_dashboard_registry_app-2.8.0/core_dashboard_registry_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:38.681500 core_dashboard_registry_app-2.8.0/core_dashboard_registry_app/static/core_dashboard_registry_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:38.700589 core_dashboard_registry_app-2.8.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:39.164580 core_dashboard_registry_app-2.8.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       98 2024-03-12 18:58:36.000000 core_dashboard_registry_app-2.8.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/css/home.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:39.188211 core_dashboard_registry_app-2.8.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/css/list/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1722 2024-03-12 18:58:36.000000 core_dashboard_registry_app-2.8.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/css/list/records.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:39.255979 core_dashboard_registry_app-2.8.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1056 2024-03-12 18:58:36.000000 core_dashboard_registry_app-2.8.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/get_url.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      107 2024-03-12 18:58:36.000000 core_dashboard_registry_app-2.8.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/get_url.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:39.345139 core_dashboard_registry_app-2.8.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/list/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       69 2024-03-12 18:58:36.000000 core_dashboard_registry_app-2.8.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/list/open_form.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      637 2024-03-12 18:58:36.000000 core_dashboard_registry_app-2.8.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/list/publish.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       72 2024-03-12 18:58:36.000000 core_dashboard_registry_app-2.8.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/list/publish.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1732 2024-03-12 18:58:36.000000 core_dashboard_registry_app-2.8.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/list/records.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       78 2024-03-12 18:58:36.000000 core_dashboard_registry_app-2.8.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/list/records.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1657 2024-03-12 18:58:36.000000 core_dashboard_registry_app-2.8.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/record_registry.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      226 2024-03-12 18:58:36.000000 core_dashboard_registry_app-2.8.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/record_registry.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:38.733915 core_dashboard_registry_app-2.8.0/core_dashboard_registry_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:39.366974 core_dashboard_registry_app-2.8.0/core_dashboard_registry_app/templates/core_dashboard_common_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:39.417356 core_dashboard_registry_app-2.8.0/core_dashboard_registry_app/templates/core_dashboard_common_app/list/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4023 2024-03-12 18:58:36.000000 core_dashboard_registry_app-2.8.0/core_dashboard_registry_app/templates/core_dashboard_common_app/list/my_dashboard_my_forms_table.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8151 2024-03-12 18:58:36.000000 core_dashboard_registry_app-2.8.0/core_dashboard_registry_app/templates/core_dashboard_common_app/list/my_dashboard_my_records_table.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      194 2024-03-12 18:58:36.000000 core_dashboard_registry_app-2.8.0/core_dashboard_registry_app/templates/core_dashboard_common_app/list/my_dashboard_my_records_table_pagination.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3205 2024-03-12 18:58:36.000000 core_dashboard_registry_app-2.8.0/core_dashboard_registry_app/templates/core_dashboard_common_app/my_dashboard.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:39.436610 core_dashboard_registry_app-2.8.0/core_dashboard_registry_app/templates/core_dashboard_registry_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1180 2024-03-12 18:58:36.000000 core_dashboard_registry_app-2.8.0/core_dashboard_registry_app/templates/core_dashboard_registry_app/home.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:39.509974 core_dashboard_registry_app-2.8.0/core_dashboard_registry_app/templates/core_dashboard_registry_app/list/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2473 2024-03-12 18:58:36.000000 core_dashboard_registry_app-2.8.0/core_dashboard_registry_app/templates/core_dashboard_registry_app/list/my_dashboard_my_forms_table.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      192 2024-03-12 18:58:36.000000 core_dashboard_registry_app-2.8.0/core_dashboard_registry_app/templates/core_dashboard_registry_app/list/my_dashboard_my_forms_table_pagination.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7931 2024-03-12 18:58:36.000000 core_dashboard_registry_app-2.8.0/core_dashboard_registry_app/templates/core_dashboard_registry_app/list/my_dashboard_my_records_table.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      194 2024-03-12 18:58:36.000000 core_dashboard_registry_app-2.8.0/core_dashboard_registry_app/templates/core_dashboard_registry_app/list/my_dashboard_my_records_table_pagination.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3442 2024-03-12 18:58:36.000000 core_dashboard_registry_app-2.8.0/core_dashboard_registry_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:39.530767 core_dashboard_registry_app-2.8.0/core_dashboard_registry_app/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:36.000000 core_dashboard_registry_app-2.8.0/core_dashboard_registry_app/utils/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:39.559319 core_dashboard_registry_app-2.8.0/core_dashboard_registry_app/utils/query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:36.000000 core_dashboard_registry_app-2.8.0/core_dashboard_registry_app/utils/query/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:39.605938 core_dashboard_registry_app-2.8.0/core_dashboard_registry_app/utils/query/django/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:36.000000 core_dashboard_registry_app-2.8.0/core_dashboard_registry_app/utils/query/django/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      622 2024-03-12 18:58:36.000000 core_dashboard_registry_app-2.8.0/core_dashboard_registry_app/utils/query/django/prepare.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:39.644145 core_dashboard_registry_app-2.8.0/core_dashboard_registry_app/utils/query/mongo/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:36.000000 core_dashboard_registry_app-2.8.0/core_dashboard_registry_app/utils/query/mongo/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2100 2024-03-12 18:58:36.000000 core_dashboard_registry_app-2.8.0/core_dashboard_registry_app/utils/query/mongo/prepare.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:39.674518 core_dashboard_registry_app-2.8.0/core_dashboard_registry_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:36.000000 core_dashboard_registry_app-2.8.0/core_dashboard_registry_app/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:39.765798 core_dashboard_registry_app-2.8.0/core_dashboard_registry_app/views/common/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:36.000000 core_dashboard_registry_app-2.8.0/core_dashboard_registry_app/views/common/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3843 2024-03-12 18:58:36.000000 core_dashboard_registry_app-2.8.0/core_dashboard_registry_app/views/common/ajax.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      515 2024-03-12 18:58:36.000000 core_dashboard_registry_app-2.8.0/core_dashboard_registry_app/views/common/forms.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    20298 2024-03-12 18:58:36.000000 core_dashboard_registry_app-2.8.0/core_dashboard_registry_app/views/common/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:39.140528 core_dashboard_registry_app-2.8.0/core_dashboard_registry_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1145 2024-03-12 18:58:38.000000 core_dashboard_registry_app-2.8.0/core_dashboard_registry_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3224 2024-03-12 18:58:38.000000 core_dashboard_registry_app-2.8.0/core_dashboard_registry_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2024-03-12 18:58:38.000000 core_dashboard_registry_app-2.8.0/core_dashboard_registry_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      120 2024-03-12 18:58:38.000000 core_dashboard_registry_app-2.8.0/core_dashboard_registry_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       34 2024-03-12 18:58:38.000000 core_dashboard_registry_app-2.8.0/core_dashboard_registry_app.egg-info/top_level.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2024-03-12 18:58:36.000000 core_dashboard_registry_app-2.8.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       94 2024-03-12 18:58:36.000000 core_dashboard_registry_app-2.8.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2024-03-12 18:58:39.975530 core_dashboard_registry_app-2.8.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1104 2024-03-12 18:58:36.000000 core_dashboard_registry_app-2.8.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:39.827181 core_dashboard_registry_app-2.8.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:36.000000 core_dashboard_registry_app-2.8.0/tests/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1817 2024-03-12 18:58:36.000000 core_dashboard_registry_app-2.8.0/tests/test_settings.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      486 2024-03-12 18:58:36.000000 core_dashboard_registry_app-2.8.0/tests/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:39.849408 core_dashboard_registry_app-2.8.0/tests/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:36.000000 core_dashboard_registry_app-2.8.0/tests/utils/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:39.895811 core_dashboard_registry_app-2.8.0/tests/utils/query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:36.000000 core_dashboard_registry_app-2.8.0/tests/utils/query/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9706 2024-03-12 18:58:36.000000 core_dashboard_registry_app-2.8.0/tests/utils/query/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:39.941961 core_dashboard_registry_app-2.8.0/tests/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:36.000000 core_dashboard_registry_app-2.8.0/tests/views/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    24459 2024-03-12 18:58:36.000000 core_dashboard_registry_app-2.8.0/tests/views/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:10.755899 core_dashboard_registry_app-2.9.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2024-05-13 16:04:05.000000 core_dashboard_registry_app-2.9.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      162 2024-05-13 16:04:05.000000 core_dashboard_registry_app-2.9.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1145 2024-05-13 16:04:10.748777 core_dashboard_registry_app-2.9.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      633 2024-05-13 16:04:05.000000 core_dashboard_registry_app-2.9.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:09.431617 core_dashboard_registry_app-2.9.0/core_dashboard_registry_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:05.000000 core_dashboard_registry_app-2.9.0/core_dashboard_registry_app/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3446 2024-05-13 16:04:05.000000 core_dashboard_registry_app-2.9.0/core_dashboard_registry_app/admin.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      661 2024-05-13 16:04:05.000000 core_dashboard_registry_app-2.9.0/core_dashboard_registry_app/constants.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2803 2024-05-13 16:04:05.000000 core_dashboard_registry_app-2.9.0/core_dashboard_registry_app/menus.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      415 2024-05-13 16:04:05.000000 core_dashboard_registry_app-2.9.0/core_dashboard_registry_app/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:08.761914 core_dashboard_registry_app-2.9.0/core_dashboard_registry_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:08.765865 core_dashboard_registry_app-2.9.0/core_dashboard_registry_app/static/core_dashboard_registry_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:08.780492 core_dashboard_registry_app-2.9.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:09.577107 core_dashboard_registry_app-2.9.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/css/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       98 2024-05-13 16:04:05.000000 core_dashboard_registry_app-2.9.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/css/home.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:09.598682 core_dashboard_registry_app-2.9.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/css/list/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1722 2024-05-13 16:04:05.000000 core_dashboard_registry_app-2.9.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/css/list/records.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:09.707098 core_dashboard_registry_app-2.9.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1056 2024-05-13 16:04:06.000000 core_dashboard_registry_app-2.9.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/get_url.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      107 2024-05-13 16:04:06.000000 core_dashboard_registry_app-2.9.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/get_url.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:09.840811 core_dashboard_registry_app-2.9.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/list/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       69 2024-05-13 16:04:06.000000 core_dashboard_registry_app-2.9.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/list/open_form.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      637 2024-05-13 16:04:06.000000 core_dashboard_registry_app-2.9.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/list/publish.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       72 2024-05-13 16:04:06.000000 core_dashboard_registry_app-2.9.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/list/publish.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1732 2024-05-13 16:04:06.000000 core_dashboard_registry_app-2.9.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/list/records.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       78 2024-05-13 16:04:06.000000 core_dashboard_registry_app-2.9.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/list/records.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1657 2024-05-13 16:04:06.000000 core_dashboard_registry_app-2.9.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/record_registry.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      226 2024-05-13 16:04:06.000000 core_dashboard_registry_app-2.9.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/record_registry.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:08.808068 core_dashboard_registry_app-2.9.0/core_dashboard_registry_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:09.865010 core_dashboard_registry_app-2.9.0/core_dashboard_registry_app/templates/core_dashboard_common_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:09.973652 core_dashboard_registry_app-2.9.0/core_dashboard_registry_app/templates/core_dashboard_common_app/list/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4023 2024-05-13 16:04:06.000000 core_dashboard_registry_app-2.9.0/core_dashboard_registry_app/templates/core_dashboard_common_app/list/my_dashboard_my_forms_table.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8151 2024-05-13 16:04:06.000000 core_dashboard_registry_app-2.9.0/core_dashboard_registry_app/templates/core_dashboard_common_app/list/my_dashboard_my_records_table.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      194 2024-05-13 16:04:06.000000 core_dashboard_registry_app-2.9.0/core_dashboard_registry_app/templates/core_dashboard_common_app/list/my_dashboard_my_records_table_pagination.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3205 2024-05-13 16:04:06.000000 core_dashboard_registry_app-2.9.0/core_dashboard_registry_app/templates/core_dashboard_common_app/my_dashboard.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:09.993975 core_dashboard_registry_app-2.9.0/core_dashboard_registry_app/templates/core_dashboard_registry_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1180 2024-05-13 16:04:06.000000 core_dashboard_registry_app-2.9.0/core_dashboard_registry_app/templates/core_dashboard_registry_app/home.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:10.097212 core_dashboard_registry_app-2.9.0/core_dashboard_registry_app/templates/core_dashboard_registry_app/list/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2473 2024-05-13 16:04:06.000000 core_dashboard_registry_app-2.9.0/core_dashboard_registry_app/templates/core_dashboard_registry_app/list/my_dashboard_my_forms_table.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      192 2024-05-13 16:04:06.000000 core_dashboard_registry_app-2.9.0/core_dashboard_registry_app/templates/core_dashboard_registry_app/list/my_dashboard_my_forms_table_pagination.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7931 2024-05-13 16:04:06.000000 core_dashboard_registry_app-2.9.0/core_dashboard_registry_app/templates/core_dashboard_registry_app/list/my_dashboard_my_records_table.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      194 2024-05-13 16:04:06.000000 core_dashboard_registry_app-2.9.0/core_dashboard_registry_app/templates/core_dashboard_registry_app/list/my_dashboard_my_records_table_pagination.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3442 2024-05-13 16:04:06.000000 core_dashboard_registry_app-2.9.0/core_dashboard_registry_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:10.151858 core_dashboard_registry_app-2.9.0/core_dashboard_registry_app/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:06.000000 core_dashboard_registry_app-2.9.0/core_dashboard_registry_app/utils/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:10.235184 core_dashboard_registry_app-2.9.0/core_dashboard_registry_app/utils/query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:06.000000 core_dashboard_registry_app-2.9.0/core_dashboard_registry_app/utils/query/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:10.308300 core_dashboard_registry_app-2.9.0/core_dashboard_registry_app/utils/query/django/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:06.000000 core_dashboard_registry_app-2.9.0/core_dashboard_registry_app/utils/query/django/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      622 2024-05-13 16:04:06.000000 core_dashboard_registry_app-2.9.0/core_dashboard_registry_app/utils/query/django/prepare.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:10.351845 core_dashboard_registry_app-2.9.0/core_dashboard_registry_app/utils/query/mongo/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:06.000000 core_dashboard_registry_app-2.9.0/core_dashboard_registry_app/utils/query/mongo/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2100 2024-05-13 16:04:06.000000 core_dashboard_registry_app-2.9.0/core_dashboard_registry_app/utils/query/mongo/prepare.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:10.374368 core_dashboard_registry_app-2.9.0/core_dashboard_registry_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:06.000000 core_dashboard_registry_app-2.9.0/core_dashboard_registry_app/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:10.485333 core_dashboard_registry_app-2.9.0/core_dashboard_registry_app/views/common/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:06.000000 core_dashboard_registry_app-2.9.0/core_dashboard_registry_app/views/common/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3817 2024-05-13 16:04:06.000000 core_dashboard_registry_app-2.9.0/core_dashboard_registry_app/views/common/ajax.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      515 2024-05-13 16:04:06.000000 core_dashboard_registry_app-2.9.0/core_dashboard_registry_app/views/common/forms.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    20298 2024-05-13 16:04:06.000000 core_dashboard_registry_app-2.9.0/core_dashboard_registry_app/views/common/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:09.548611 core_dashboard_registry_app-2.9.0/core_dashboard_registry_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1145 2024-05-13 16:04:08.000000 core_dashboard_registry_app-2.9.0/core_dashboard_registry_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3224 2024-05-13 16:04:08.000000 core_dashboard_registry_app-2.9.0/core_dashboard_registry_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2024-05-13 16:04:08.000000 core_dashboard_registry_app-2.9.0/core_dashboard_registry_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      120 2024-05-13 16:04:08.000000 core_dashboard_registry_app-2.9.0/core_dashboard_registry_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       34 2024-05-13 16:04:08.000000 core_dashboard_registry_app-2.9.0/core_dashboard_registry_app.egg-info/top_level.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2024-05-13 16:04:06.000000 core_dashboard_registry_app-2.9.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       94 2024-05-13 16:04:06.000000 core_dashboard_registry_app-2.9.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2024-05-13 16:04:10.758446 core_dashboard_registry_app-2.9.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1104 2024-05-13 16:04:06.000000 core_dashboard_registry_app-2.9.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:10.550212 core_dashboard_registry_app-2.9.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:06.000000 core_dashboard_registry_app-2.9.0/tests/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1817 2024-05-13 16:04:06.000000 core_dashboard_registry_app-2.9.0/tests/test_settings.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      486 2024-05-13 16:04:06.000000 core_dashboard_registry_app-2.9.0/tests/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:10.598892 core_dashboard_registry_app-2.9.0/tests/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:06.000000 core_dashboard_registry_app-2.9.0/tests/utils/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:10.654208 core_dashboard_registry_app-2.9.0/tests/utils/query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:06.000000 core_dashboard_registry_app-2.9.0/tests/utils/query/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9706 2024-05-13 16:04:06.000000 core_dashboard_registry_app-2.9.0/tests/utils/query/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:10.700245 core_dashboard_registry_app-2.9.0/tests/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:06.000000 core_dashboard_registry_app-2.9.0/tests/views/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    24459 2024-05-13 16:04:06.000000 core_dashboard_registry_app-2.9.0/tests/views/tests_unit.py
```

### Comparing `core_dashboard_registry_app-2.8.0/LICENSE.md` & `core_dashboard_registry_app-2.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `core_dashboard_registry_app-2.8.0/PKG-INFO` & `core_dashboard_registry_app-2.9.0/core_dashboard_registry_app.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
-Name: core_dashboard_registry_app
-Version: 2.8.0
+Name: core-dashboard-registry-app
+Version: 2.9.0
 Summary: Resource management via a dashboard for the registry core project
 Home-page: https://github.com/usnistgov/core_dashboard_registry_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: Core Dashboard Registry App
         ===========================
```

### Comparing `core_dashboard_registry_app-2.8.0/README.rst` & `core_dashboard_registry_app-2.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_dashboard_registry_app-2.8.0/core_dashboard_registry_app/admin.py` & `core_dashboard_registry_app-2.9.0/core_dashboard_registry_app/admin.py`

 * *Files identical despite different names*

### Comparing `core_dashboard_registry_app-2.8.0/core_dashboard_registry_app/constants.py` & `core_dashboard_registry_app-2.9.0/core_dashboard_registry_app/constants.py`

 * *Files identical despite different names*

### Comparing `core_dashboard_registry_app-2.8.0/core_dashboard_registry_app/menus.py` & `core_dashboard_registry_app-2.9.0/core_dashboard_registry_app/menus.py`

 * *Files identical despite different names*

### Comparing `core_dashboard_registry_app-2.8.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/css/list/records.css` & `core_dashboard_registry_app-2.9.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/css/list/records.css`

 * *Files identical despite different names*

### Comparing `core_dashboard_registry_app-2.8.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/get_url.js` & `core_dashboard_registry_app-2.9.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/get_url.js`

 * *Files identical despite different names*

### Comparing `core_dashboard_registry_app-2.8.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/list/publish.js` & `core_dashboard_registry_app-2.9.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/list/publish.js`

 * *Files identical despite different names*

### Comparing `core_dashboard_registry_app-2.8.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/list/records.js` & `core_dashboard_registry_app-2.9.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/list/records.js`

 * *Files identical despite different names*

### Comparing `core_dashboard_registry_app-2.8.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/record_registry.js` & `core_dashboard_registry_app-2.9.0/core_dashboard_registry_app/static/core_dashboard_registry_app/user/js/record_registry.js`

 * *Files identical despite different names*

### Comparing `core_dashboard_registry_app-2.8.0/core_dashboard_registry_app/templates/core_dashboard_common_app/list/my_dashboard_my_forms_table.html` & `core_dashboard_registry_app-2.9.0/core_dashboard_registry_app/templates/core_dashboard_common_app/list/my_dashboard_my_forms_table.html`

 * *Files identical despite different names*

### Comparing `core_dashboard_registry_app-2.8.0/core_dashboard_registry_app/templates/core_dashboard_common_app/list/my_dashboard_my_records_table.html` & `core_dashboard_registry_app-2.9.0/core_dashboard_registry_app/templates/core_dashboard_common_app/list/my_dashboard_my_records_table.html`

 * *Files identical despite different names*

### Comparing `core_dashboard_registry_app-2.8.0/core_dashboard_registry_app/templates/core_dashboard_common_app/my_dashboard.html` & `core_dashboard_registry_app-2.9.0/core_dashboard_registry_app/templates/core_dashboard_common_app/my_dashboard.html`

 * *Files identical despite different names*

### Comparing `core_dashboard_registry_app-2.8.0/core_dashboard_registry_app/templates/core_dashboard_registry_app/home.html` & `core_dashboard_registry_app-2.9.0/core_dashboard_registry_app/templates/core_dashboard_registry_app/home.html`

 * *Files identical despite different names*

### Comparing `core_dashboard_registry_app-2.8.0/core_dashboard_registry_app/templates/core_dashboard_registry_app/list/my_dashboard_my_forms_table.html` & `core_dashboard_registry_app-2.9.0/core_dashboard_registry_app/templates/core_dashboard_registry_app/list/my_dashboard_my_forms_table.html`

 * *Files identical despite different names*

### Comparing `core_dashboard_registry_app-2.8.0/core_dashboard_registry_app/templates/core_dashboard_registry_app/list/my_dashboard_my_records_table.html` & `core_dashboard_registry_app-2.9.0/core_dashboard_registry_app/templates/core_dashboard_registry_app/list/my_dashboard_my_records_table.html`

 * *Files identical despite different names*

### Comparing `core_dashboard_registry_app-2.8.0/core_dashboard_registry_app/urls.py` & `core_dashboard_registry_app-2.9.0/core_dashboard_registry_app/urls.py`

 * *Files identical despite different names*

### Comparing `core_dashboard_registry_app-2.8.0/core_dashboard_registry_app/utils/query/django/prepare.py` & `core_dashboard_registry_app-2.9.0/core_dashboard_registry_app/utils/query/django/prepare.py`

 * *Files identical despite different names*

### Comparing `core_dashboard_registry_app-2.8.0/core_dashboard_registry_app/utils/query/mongo/prepare.py` & `core_dashboard_registry_app-2.9.0/core_dashboard_registry_app/utils/query/mongo/prepare.py`

 * *Files identical despite different names*

### Comparing `core_dashboard_registry_app-2.8.0/core_dashboard_registry_app/views/common/ajax.py` & `core_dashboard_registry_app-2.9.0/core_dashboard_registry_app/views/common/ajax.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         data_id = request.POST.get("data_id", None)
         if data_id is not None:
             data = data_api.get_by_id(data_id, request.user)
             data_registry_api.publish(data, request.user)
             messages.add_message(
                 request,
                 messages.SUCCESS,
-                get_data_label().capitalize() + " published with success.",
+                get_data_label().capitalize() + " published.",
             )
         else:
             return HttpResponseBadRequest(
                 json.dumps({"message": "The data id is required"}),
                 content_type="application/javascript",
             )
     except exceptions.DoesNotExist as dne:
@@ -97,15 +97,15 @@
 
 @method_decorator(login_required, name="dispatch")
 class EditDataView(EditObjectModalView):
     """EditDataView"""
 
     form_class = EditDataForm
     model = Data
-    success_message = "Title edited with success."
+    success_message = "Title edited."
 
     def _save(self, form):
         # Save treatment.
         try:
             data_api.upsert(self.object, self.request)
         except Exception as exception:
             form.add_error(None, str(exception))
```

### Comparing `core_dashboard_registry_app-2.8.0/core_dashboard_registry_app/views/common/forms.py` & `core_dashboard_registry_app-2.9.0/core_dashboard_registry_app/views/common/forms.py`

 * *Files identical despite different names*

### Comparing `core_dashboard_registry_app-2.8.0/core_dashboard_registry_app/views/common/views.py` & `core_dashboard_registry_app-2.9.0/core_dashboard_registry_app/views/common/views.py`

 * *Files identical despite different names*

### Comparing `core_dashboard_registry_app-2.8.0/core_dashboard_registry_app.egg-info/PKG-INFO` & `core_dashboard_registry_app-2.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
-Name: core-dashboard-registry-app
-Version: 2.8.0
+Name: core_dashboard_registry_app
+Version: 2.9.0
 Summary: Resource management via a dashboard for the registry core project
 Home-page: https://github.com/usnistgov/core_dashboard_registry_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: Core Dashboard Registry App
         ===========================
```

### Comparing `core_dashboard_registry_app-2.8.0/core_dashboard_registry_app.egg-info/SOURCES.txt` & `core_dashboard_registry_app-2.9.0/core_dashboard_registry_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `core_dashboard_registry_app-2.8.0/setup.py` & `core_dashboard_registry_app-2.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_dashboard_registry_app",
-    version="2.8.0",
+    version="2.9.0",
     description="Resource management via a dashboard for the registry core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_dashboard_registry_app",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `core_dashboard_registry_app-2.8.0/tests/test_settings.py` & `core_dashboard_registry_app-2.9.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `core_dashboard_registry_app-2.8.0/tests/utils/query/test_unit.py` & `core_dashboard_registry_app-2.9.0/tests/utils/query/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_dashboard_registry_app-2.8.0/tests/views/tests_unit.py` & `core_dashboard_registry_app-2.9.0/tests/views/tests_unit.py`

 * *Files identical despite different names*

