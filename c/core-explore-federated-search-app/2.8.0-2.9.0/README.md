# Comparing `tmp/core_explore_federated_search_app-2.8.0.tar.gz` & `tmp/core_explore_federated_search_app-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_explore_federated_search_app-2.8.0.tar", last modified: Tue Mar 12 18:59:34 2024, max compression
+gzip compressed data, was "core_explore_federated_search_app-2.9.0.tar", last modified: Mon May 13 16:05:13 2024, max compression
```

## Comparing `core_explore_federated_search_app-2.8.0.tar` & `core_explore_federated_search_app-2.9.0.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:34.885428 core_explore_federated_search_app-2.8.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2024-03-12 18:59:29.000000 core_explore_federated_search_app-2.8.0/LICENSE.md
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      174 2024-03-12 18:59:29.000000 core_explore_federated_search_app-2.8.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1555 2024-03-12 18:59:34.878586 core_explore_federated_search_app-2.8.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      967 2024-03-12 18:59:29.000000 core_explore_federated_search_app-2.8.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:33.586215 core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:29.000000 core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:33.703753 core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:29.000000 core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:33.746693 core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/components/data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:29.000000 core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/components/data/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      840 2024-03-12 18:59:29.000000 core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/components/data/api.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:33.767867 core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/migrations/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:29.000000 core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/migrations/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:33.814080 core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:29.000000 core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:33.875912 core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/rest/query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:29.000000 core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/rest/query/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      354 2024-03-12 18:59:29.000000 core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/rest/query/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5770 2024-03-12 18:59:29.000000 core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/rest/query/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:33.933323 core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/rest/result/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:30.000000 core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/rest/result/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      303 2024-03-12 18:59:30.000000 core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/rest/result/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2758 2024-03-12 18:59:30.000000 core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/rest/result/views.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      571 2024-03-12 18:59:30.000000 core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/rest/urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      637 2024-03-12 18:59:30.000000 core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:33.249043 core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:33.282832 core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/static/core_explore_federated_search_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:33.258231 core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:33.262635 core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/js/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:33.267073 core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/js/repositories/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:33.272924 core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/js/repositories/list/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:34.098385 core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/js/repositories/list/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      986 2024-03-12 18:59:30.000000 core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/js/repositories/list/modals/delete.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      109 2024-03-12 18:59:30.000000 core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/js/repositories/list/modals/delete.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1231 2024-03-12 18:59:30.000000 core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/js/repositories/list/modals/edit.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      105 2024-03-12 18:59:30.000000 core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/js/repositories/list/modals/edit.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1965 2024-03-12 18:59:30.000000 core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/js/repositories/list/modals/refresh.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      107 2024-03-12 18:59:30.000000 core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/js/repositories/list/modals/refresh.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:33.287238 core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/static/core_explore_federated_search_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:33.291174 core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/static/core_explore_federated_search_app/user/js/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:34.124131 core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/static/core_explore_federated_search_app/user/js/data_sources/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2419 2024-03-12 18:59:30.000000 core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/static/core_explore_federated_search_app/user/js/data_sources/list.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:33.306805 core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:33.340780 core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:33.315111 core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:34.177081 core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:34.199267 core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/add/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1563 2024-03-12 18:59:30.000000 core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/add/add_base.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      308 2024-03-12 18:59:30.000000 core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/add_repository.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:34.238676 core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/list/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2272 2024-03-12 18:59:30.000000 core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/list/list_base.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:34.334867 core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/list/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      842 2024-03-12 18:59:30.000000 core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/list/modals/delete.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1474 2024-03-12 18:59:30.000000 core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/list/modals/edit.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1221 2024-03-12 18:59:30.000000 core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/list/modals/refresh.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       18 2024-03-12 18:59:30.000000 core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/list/refresh_form.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      357 2024-03-12 18:59:30.000000 core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/list_repositories.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:33.344889 core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:34.381827 core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/user/data_sources/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      663 2024-03-12 18:59:30.000000 core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/user/data_sources/list-content.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1329 2024-03-12 18:59:30.000000 core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/user/data_sources/list.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      857 2024-03-12 18:59:30.000000 core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:34.401545 core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:30.000000 core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:34.462623 core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/views/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:30.000000 core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/views/user/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5623 2024-03-12 18:59:30.000000 core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/views/user/ajax.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2972 2024-03-12 18:59:30.000000 core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/views/user/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:33.684327 core_explore_federated_search_app-2.8.0/core_explore_federated_search_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1555 2024-03-12 18:59:32.000000 core_explore_federated_search_app-2.8.0/core_explore_federated_search_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3894 2024-03-12 18:59:33.000000 core_explore_federated_search_app-2.8.0/core_explore_federated_search_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2024-03-12 18:59:32.000000 core_explore_federated_search_app-2.8.0/core_explore_federated_search_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      117 2024-03-12 18:59:32.000000 core_explore_federated_search_app-2.8.0/core_explore_federated_search_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       40 2024-03-12 18:59:32.000000 core_explore_federated_search_app-2.8.0/core_explore_federated_search_app.egg-info/top_level.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2024-03-12 18:59:30.000000 core_explore_federated_search_app-2.8.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       85 2024-03-12 18:59:30.000000 core_explore_federated_search_app-2.8.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2024-03-12 18:59:34.888112 core_explore_federated_search_app-2.8.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1114 2024-03-12 18:59:30.000000 core_explore_federated_search_app-2.8.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:34.517856 core_explore_federated_search_app-2.8.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:30.000000 core_explore_federated_search_app-2.8.0/tests/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:34.538608 core_explore_federated_search_app-2.8.0/tests/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:30.000000 core_explore_federated_search_app-2.8.0/tests/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:34.606953 core_explore_federated_search_app-2.8.0/tests/components/data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:30.000000 core_explore_federated_search_app-2.8.0/tests/components/data/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1073 2024-03-12 18:59:30.000000 core_explore_federated_search_app-2.8.0/tests/components/data/tests_int_access_control.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:34.650097 core_explore_federated_search_app-2.8.0/tests/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:30.000000 core_explore_federated_search_app-2.8.0/tests/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3033 2024-03-12 18:59:30.000000 core_explore_federated_search_app-2.8.0/tests/fixtures/fixtures.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:34.671481 core_explore_federated_search_app-2.8.0/tests/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:30.000000 core_explore_federated_search_app-2.8.0/tests/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:34.718692 core_explore_federated_search_app-2.8.0/tests/rest/result/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:30.000000 core_explore_federated_search_app-2.8.0/tests/rest/result/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:34.761834 core_explore_federated_search_app-2.8.0/tests/rest/result/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:30.000000 core_explore_federated_search_app-2.8.0/tests/rest/result/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      956 2024-03-12 18:59:30.000000 core_explore_federated_search_app-2.8.0/tests/rest/result/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1864 2024-03-12 18:59:30.000000 core_explore_federated_search_app-2.8.0/tests/rest/result/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2101 2024-03-12 18:59:30.000000 core_explore_federated_search_app-2.8.0/tests/test_settings.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      907 2024-03-12 18:59:31.000000 core_explore_federated_search_app-2.8.0/tests/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:34.782591 core_explore_federated_search_app-2.8.0/tests/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:31.000000 core_explore_federated_search_app-2.8.0/tests/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:34.848267 core_explore_federated_search_app-2.8.0/tests/views/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:31.000000 core_explore_federated_search_app-2.8.0/tests/views/user/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5543 2024-03-12 18:59:31.000000 core_explore_federated_search_app-2.8.0/tests/views/user/tests_permissions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1459 2024-03-12 18:59:31.000000 core_explore_federated_search_app-2.8.0/tests/views/user/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:13.721749 core_explore_federated_search_app-2.9.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2024-05-13 16:05:08.000000 core_explore_federated_search_app-2.9.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      174 2024-05-13 16:05:08.000000 core_explore_federated_search_app-2.9.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1555 2024-05-13 16:05:13.715466 core_explore_federated_search_app-2.9.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      967 2024-05-13 16:05:08.000000 core_explore_federated_search_app-2.9.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:12.464948 core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:08.000000 core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:12.595499 core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:08.000000 core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:12.647511 core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/components/data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:08.000000 core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/components/data/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      840 2024-05-13 16:05:08.000000 core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/components/data/api.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:12.666490 core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/migrations/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:08.000000 core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/migrations/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:12.712067 core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:08.000000 core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:12.764466 core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/rest/query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:08.000000 core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/rest/query/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      354 2024-05-13 16:05:08.000000 core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/rest/query/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5770 2024-05-13 16:05:08.000000 core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/rest/query/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:12.823986 core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/rest/result/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:08.000000 core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/rest/result/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      303 2024-05-13 16:05:08.000000 core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/rest/result/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2758 2024-05-13 16:05:08.000000 core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/rest/result/views.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      571 2024-05-13 16:05:08.000000 core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/rest/urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      637 2024-05-13 16:05:08.000000 core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:12.058375 core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:12.121330 core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/static/core_explore_federated_search_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:12.066490 core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:12.070124 core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/js/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:12.107566 core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/js/repositories/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:12.111352 core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/js/repositories/list/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:12.958303 core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/js/repositories/list/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      986 2024-05-13 16:05:08.000000 core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/js/repositories/list/modals/delete.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      109 2024-05-13 16:05:08.000000 core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/js/repositories/list/modals/delete.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1231 2024-05-13 16:05:08.000000 core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/js/repositories/list/modals/edit.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      105 2024-05-13 16:05:08.000000 core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/js/repositories/list/modals/edit.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1965 2024-05-13 16:05:08.000000 core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/js/repositories/list/modals/refresh.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      107 2024-05-13 16:05:08.000000 core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/js/repositories/list/modals/refresh.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:12.125557 core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/static/core_explore_federated_search_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:12.129945 core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/static/core_explore_federated_search_app/user/js/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:12.988890 core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/static/core_explore_federated_search_app/user/js/data_sources/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2419 2024-05-13 16:05:08.000000 core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/static/core_explore_federated_search_app/user/js/data_sources/list.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:12.144577 core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:12.194484 core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:12.152862 core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:13.029876 core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:13.051345 core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/add/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1563 2024-05-13 16:05:08.000000 core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/add/add_base.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      308 2024-05-13 16:05:08.000000 core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/add_repository.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:13.084035 core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/list/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2272 2024-05-13 16:05:08.000000 core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/list/list_base.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:13.159864 core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/list/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      842 2024-05-13 16:05:08.000000 core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/list/modals/delete.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1474 2024-05-13 16:05:08.000000 core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/list/modals/edit.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1221 2024-05-13 16:05:08.000000 core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/list/modals/refresh.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       18 2024-05-13 16:05:08.000000 core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/list/refresh_form.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      357 2024-05-13 16:05:08.000000 core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/list_repositories.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:12.203573 core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:13.219104 core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/user/data_sources/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      663 2024-05-13 16:05:08.000000 core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/user/data_sources/list-content.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1329 2024-05-13 16:05:08.000000 core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/user/data_sources/list.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      857 2024-05-13 16:05:08.000000 core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:13.236127 core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:08.000000 core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:13.293759 core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/views/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:08.000000 core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/views/user/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5623 2024-05-13 16:05:08.000000 core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/views/user/ajax.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2972 2024-05-13 16:05:08.000000 core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/views/user/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:12.569001 core_explore_federated_search_app-2.9.0/core_explore_federated_search_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1555 2024-05-13 16:05:11.000000 core_explore_federated_search_app-2.9.0/core_explore_federated_search_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3894 2024-05-13 16:05:11.000000 core_explore_federated_search_app-2.9.0/core_explore_federated_search_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2024-05-13 16:05:11.000000 core_explore_federated_search_app-2.9.0/core_explore_federated_search_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      117 2024-05-13 16:05:11.000000 core_explore_federated_search_app-2.9.0/core_explore_federated_search_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       40 2024-05-13 16:05:11.000000 core_explore_federated_search_app-2.9.0/core_explore_federated_search_app.egg-info/top_level.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2024-05-13 16:05:09.000000 core_explore_federated_search_app-2.9.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       85 2024-05-13 16:05:09.000000 core_explore_federated_search_app-2.9.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2024-05-13 16:05:13.723698 core_explore_federated_search_app-2.9.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1114 2024-05-13 16:05:09.000000 core_explore_federated_search_app-2.9.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:13.386686 core_explore_federated_search_app-2.9.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:09.000000 core_explore_federated_search_app-2.9.0/tests/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:13.405964 core_explore_federated_search_app-2.9.0/tests/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:09.000000 core_explore_federated_search_app-2.9.0/tests/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:13.460577 core_explore_federated_search_app-2.9.0/tests/components/data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:09.000000 core_explore_federated_search_app-2.9.0/tests/components/data/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1073 2024-05-13 16:05:09.000000 core_explore_federated_search_app-2.9.0/tests/components/data/tests_int_access_control.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:13.502138 core_explore_federated_search_app-2.9.0/tests/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:09.000000 core_explore_federated_search_app-2.9.0/tests/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3033 2024-05-13 16:05:09.000000 core_explore_federated_search_app-2.9.0/tests/fixtures/fixtures.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:13.524942 core_explore_federated_search_app-2.9.0/tests/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:09.000000 core_explore_federated_search_app-2.9.0/tests/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:13.563494 core_explore_federated_search_app-2.9.0/tests/rest/result/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:09.000000 core_explore_federated_search_app-2.9.0/tests/rest/result/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:13.607733 core_explore_federated_search_app-2.9.0/tests/rest/result/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:09.000000 core_explore_federated_search_app-2.9.0/tests/rest/result/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      956 2024-05-13 16:05:09.000000 core_explore_federated_search_app-2.9.0/tests/rest/result/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1864 2024-05-13 16:05:09.000000 core_explore_federated_search_app-2.9.0/tests/rest/result/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2101 2024-05-13 16:05:09.000000 core_explore_federated_search_app-2.9.0/tests/test_settings.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      907 2024-05-13 16:05:09.000000 core_explore_federated_search_app-2.9.0/tests/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:13.623312 core_explore_federated_search_app-2.9.0/tests/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:09.000000 core_explore_federated_search_app-2.9.0/tests/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:13.700120 core_explore_federated_search_app-2.9.0/tests/views/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:09.000000 core_explore_federated_search_app-2.9.0/tests/views/user/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5543 2024-05-13 16:05:09.000000 core_explore_federated_search_app-2.9.0/tests/views/user/tests_permissions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1459 2024-05-13 16:05:09.000000 core_explore_federated_search_app-2.9.0/tests/views/user/tests_unit.py
```

### Comparing `core_explore_federated_search_app-2.8.0/LICENSE.md` & `core_explore_federated_search_app-2.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `core_explore_federated_search_app-2.8.0/PKG-INFO` & `core_explore_federated_search_app-2.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_explore_federated_search_app
-Version: 2.8.0
+Version: 2.9.0
 Summary: Federation exploration functions for curator core project
 Home-page: https://github.com/usnistgov/core_explore_federated_search_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: =================================
         Core Explore Federated Search App
```

### Comparing `core_explore_federated_search_app-2.8.0/README.rst` & `core_explore_federated_search_app-2.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/components/data/api.py` & `core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/components/data/api.py`

 * *Files identical despite different names*

### Comparing `core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/rest/query/views.py` & `core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/rest/query/views.py`

 * *Files identical despite different names*

### Comparing `core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/rest/result/views.py` & `core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/rest/result/views.py`

 * *Files identical despite different names*

### Comparing `core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/rest/urls.py` & `core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/rest/urls.py`

 * *Files identical despite different names*

### Comparing `core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/settings.py` & `core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/settings.py`

 * *Files identical despite different names*

### Comparing `core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/js/repositories/list/modals/delete.js` & `core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/js/repositories/list/modals/delete.js`

 * *Files identical despite different names*

### Comparing `core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/js/repositories/list/modals/edit.js` & `core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/js/repositories/list/modals/edit.js`

 * *Files identical despite different names*

### Comparing `core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/js/repositories/list/modals/refresh.js` & `core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/static/core_explore_federated_search_app/admin/js/repositories/list/modals/refresh.js`

 * *Files identical despite different names*

### Comparing `core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/static/core_explore_federated_search_app/user/js/data_sources/list.js` & `core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/static/core_explore_federated_search_app/user/js/data_sources/list.js`

 * *Files identical despite different names*

### Comparing `core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/add/add_base.html` & `core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/add/add_base.html`

 * *Files identical despite different names*

### Comparing `core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/list/list_base.html` & `core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/list/list_base.html`

 * *Files identical despite different names*

### Comparing `core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/list/modals/delete.html` & `core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/list/modals/delete.html`

 * *Files identical despite different names*

### Comparing `core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/list/modals/edit.html` & `core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/list/modals/edit.html`

 * *Files identical despite different names*

### Comparing `core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/list/modals/refresh.html` & `core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/admin/repositories/list/modals/refresh.html`

 * *Files identical despite different names*

### Comparing `core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/user/data_sources/list-content.html` & `core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/user/data_sources/list-content.html`

 * *Files identical despite different names*

### Comparing `core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/user/data_sources/list.html` & `core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/templates/core_explore_federated_search_app/user/data_sources/list.html`

 * *Files identical despite different names*

### Comparing `core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/urls.py` & `core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/urls.py`

 * *Files identical despite different names*

### Comparing `core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/views/user/ajax.py` & `core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/views/user/ajax.py`

 * *Files identical despite different names*

### Comparing `core_explore_federated_search_app-2.8.0/core_explore_federated_search_app/views/user/views.py` & `core_explore_federated_search_app-2.9.0/core_explore_federated_search_app/views/user/views.py`

 * *Files identical despite different names*

### Comparing `core_explore_federated_search_app-2.8.0/core_explore_federated_search_app.egg-info/PKG-INFO` & `core_explore_federated_search_app-2.9.0/core_explore_federated_search_app.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-explore-federated-search-app
-Version: 2.8.0
+Version: 2.9.0
 Summary: Federation exploration functions for curator core project
 Home-page: https://github.com/usnistgov/core_explore_federated_search_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: =================================
         Core Explore Federated Search App
```

### Comparing `core_explore_federated_search_app-2.8.0/core_explore_federated_search_app.egg-info/SOURCES.txt` & `core_explore_federated_search_app-2.9.0/core_explore_federated_search_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `core_explore_federated_search_app-2.8.0/setup.py` & `core_explore_federated_search_app-2.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_explore_federated_search_app",
-    version="2.8.0",
+    version="2.9.0",
     description="Federation exploration functions for curator core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_explore_federated_search_app",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `core_explore_federated_search_app-2.8.0/tests/components/data/tests_int_access_control.py` & `core_explore_federated_search_app-2.9.0/tests/components/data/tests_int_access_control.py`

 * *Files identical despite different names*

### Comparing `core_explore_federated_search_app-2.8.0/tests/fixtures/fixtures.py` & `core_explore_federated_search_app-2.9.0/tests/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_explore_federated_search_app-2.8.0/tests/rest/result/fixtures/fixtures.py` & `core_explore_federated_search_app-2.9.0/tests/rest/result/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_explore_federated_search_app-2.8.0/tests/rest/result/tests_int.py` & `core_explore_federated_search_app-2.9.0/tests/rest/result/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_explore_federated_search_app-2.8.0/tests/test_settings.py` & `core_explore_federated_search_app-2.9.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `core_explore_federated_search_app-2.8.0/tests/urls.py` & `core_explore_federated_search_app-2.9.0/tests/urls.py`

 * *Files identical despite different names*

### Comparing `core_explore_federated_search_app-2.8.0/tests/views/user/tests_permissions.py` & `core_explore_federated_search_app-2.9.0/tests/views/user/tests_permissions.py`

 * *Files identical despite different names*

### Comparing `core_explore_federated_search_app-2.8.0/tests/views/user/tests_unit.py` & `core_explore_federated_search_app-2.9.0/tests/views/user/tests_unit.py`

 * *Files identical despite different names*

