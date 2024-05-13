# Comparing `tmp/core_federated_search_app-2.8.0.tar.gz` & `tmp/core_federated_search_app-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_federated_search_app-2.8.0.tar", last modified: Tue Mar 12 19:01:13 2024, max compression
+gzip compressed data, was "core_federated_search_app-2.9.0.tar", last modified: Mon May 13 16:06:54 2024, max compression
```

## Comparing `core_federated_search_app-2.8.0.tar` & `core_federated_search_app-2.9.0.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:13.796783 core_federated_search_app-2.8.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2024-03-12 19:01:08.000000 core_federated_search_app-2.8.0/LICENSE.md
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      183 2024-03-12 19:01:08.000000 core_federated_search_app-2.8.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1232 2024-03-12 19:01:13.789729 core_federated_search_app-2.8.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      720 2024-03-12 19:01:08.000000 core_federated_search_app-2.8.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:12.464902 core_federated_search_app-2.8.0/core_federated_search_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       91 2024-03-12 19:01:08.000000 core_federated_search_app-2.8.0/core_federated_search_app/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1343 2024-03-12 19:01:08.000000 core_federated_search_app-2.8.0/core_federated_search_app/admin.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      270 2024-03-12 19:01:08.000000 core_federated_search_app-2.8.0/core_federated_search_app/apps.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:12.603505 core_federated_search_app-2.8.0/core_federated_search_app/commons/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:08.000000 core_federated_search_app-2.8.0/core_federated_search_app/commons/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      229 2024-03-12 19:01:08.000000 core_federated_search_app-2.8.0/core_federated_search_app/commons/exceptions.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:12.626610 core_federated_search_app-2.8.0/core_federated_search_app/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:08.000000 core_federated_search_app-2.8.0/core_federated_search_app/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:12.698821 core_federated_search_app-2.8.0/core_federated_search_app/components/instance/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:08.000000 core_federated_search_app-2.8.0/core_federated_search_app/components/instance/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5844 2024-03-12 19:01:08.000000 core_federated_search_app-2.8.0/core_federated_search_app/components/instance/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3739 2024-03-12 19:01:08.000000 core_federated_search_app-2.8.0/core_federated_search_app/components/instance/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:12.718842 core_federated_search_app-2.8.0/core_federated_search_app/components/instance/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:08.000000 core_federated_search_app-2.8.0/core_federated_search_app/components/instance/tests/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      501 2024-03-12 19:01:08.000000 core_federated_search_app-2.8.0/core_federated_search_app/menus.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:12.760724 core_federated_search_app-2.8.0/core_federated_search_app/migrations/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1476 2024-03-12 19:01:08.000000 core_federated_search_app-2.8.0/core_federated_search_app/migrations/0001_initial.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:08.000000 core_federated_search_app-2.8.0/core_federated_search_app/migrations/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:12.879400 core_federated_search_app-2.8.0/core_federated_search_app/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:08.000000 core_federated_search_app-2.8.0/core_federated_search_app/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:12.943572 core_federated_search_app-2.8.0/core_federated_search_app/rest/instance/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:08.000000 core_federated_search_app-2.8.0/core_federated_search_app/rest/instance/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1697 2024-03-12 19:01:08.000000 core_federated_search_app-2.8.0/core_federated_search_app/rest/instance/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8872 2024-03-12 19:01:08.000000 core_federated_search_app-2.8.0/core_federated_search_app/rest/instance/views.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      775 2024-03-12 19:01:08.000000 core_federated_search_app-2.8.0/core_federated_search_app/rest/urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      382 2024-03-12 19:01:08.000000 core_federated_search_app-2.8.0/core_federated_search_app/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:12.086393 core_federated_search_app-2.8.0/core_federated_search_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:12.090402 core_federated_search_app-2.8.0/core_federated_search_app/static/core_federated_search_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:12.106218 core_federated_search_app-2.8.0/core_federated_search_app/static/core_federated_search_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:12.969859 core_federated_search_app-2.8.0/core_federated_search_app/static/core_federated_search_app/admin/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       40 2024-03-12 19:01:08.000000 core_federated_search_app-2.8.0/core_federated_search_app/static/core_federated_search_app/admin/css/repositories.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:12.110433 core_federated_search_app-2.8.0/core_federated_search_app/static/core_federated_search_app/admin/js/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:12.114639 core_federated_search_app-2.8.0/core_federated_search_app/static/core_federated_search_app/admin/js/repositories/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:12.132011 core_federated_search_app-2.8.0/core_federated_search_app/static/core_federated_search_app/admin/js/repositories/list/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:13.075584 core_federated_search_app-2.8.0/core_federated_search_app/static/core_federated_search_app/admin/js/repositories/list/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      986 2024-03-12 19:01:08.000000 core_federated_search_app-2.8.0/core_federated_search_app/static/core_federated_search_app/admin/js/repositories/list/modals/delete.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      101 2024-03-12 19:01:08.000000 core_federated_search_app-2.8.0/core_federated_search_app/static/core_federated_search_app/admin/js/repositories/list/modals/delete.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1965 2024-03-12 19:01:08.000000 core_federated_search_app-2.8.0/core_federated_search_app/static/core_federated_search_app/admin/js/repositories/list/modals/refresh.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       99 2024-03-12 19:01:08.000000 core_federated_search_app-2.8.0/core_federated_search_app/static/core_federated_search_app/admin/js/repositories/list/modals/refresh.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:12.147596 core_federated_search_app-2.8.0/core_federated_search_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:12.152563 core_federated_search_app-2.8.0/core_federated_search_app/templates/core_federated_search_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:12.156872 core_federated_search_app-2.8.0/core_federated_search_app/templates/core_federated_search_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:13.129486 core_federated_search_app-2.8.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:13.147407 core_federated_search_app-2.8.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/add/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1576 2024-03-12 19:01:08.000000 core_federated_search_app-2.8.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/add/add_base.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      300 2024-03-12 19:01:08.000000 core_federated_search_app-2.8.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/add_repository.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:13.206620 core_federated_search_app-2.8.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/list/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2279 2024-03-12 19:01:08.000000 core_federated_search_app-2.8.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/list/list_base.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:13.260797 core_federated_search_app-2.8.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/list/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      842 2024-03-12 19:01:09.000000 core_federated_search_app-2.8.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/list/modals/delete.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1231 2024-03-12 19:01:09.000000 core_federated_search_app-2.8.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/list/modals/refresh.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       18 2024-03-12 19:01:09.000000 core_federated_search_app-2.8.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/list/refresh_form.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      349 2024-03-12 19:01:09.000000 core_federated_search_app-2.8.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/list_repositories.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      216 2024-03-12 19:01:09.000000 core_federated_search_app-2.8.0/core_federated_search_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:13.282451 core_federated_search_app-2.8.0/core_federated_search_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:09.000000 core_federated_search_app-2.8.0/core_federated_search_app/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:13.368487 core_federated_search_app-2.8.0/core_federated_search_app/views/admin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:09.000000 core_federated_search_app-2.8.0/core_federated_search_app/views/admin/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3647 2024-03-12 19:01:09.000000 core_federated_search_app-2.8.0/core_federated_search_app/views/admin/ajax.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2712 2024-03-12 19:01:09.000000 core_federated_search_app-2.8.0/core_federated_search_app/views/admin/forms.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3477 2024-03-12 19:01:09.000000 core_federated_search_app-2.8.0/core_federated_search_app/views/admin/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:12.560738 core_federated_search_app-2.8.0/core_federated_search_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1232 2024-03-12 19:01:11.000000 core_federated_search_app-2.8.0/core_federated_search_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3231 2024-03-12 19:01:11.000000 core_federated_search_app-2.8.0/core_federated_search_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2024-03-12 19:01:11.000000 core_federated_search_app-2.8.0/core_federated_search_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      135 2024-03-12 19:01:11.000000 core_federated_search_app-2.8.0/core_federated_search_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       37 2024-03-12 19:01:11.000000 core_federated_search_app-2.8.0/core_federated_search_app.egg-info/top_level.txt
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:13.430112 core_federated_search_app-2.8.0/docs/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:09.000000 core_federated_search_app-2.8.0/docs/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11132 2024-03-12 19:01:09.000000 core_federated_search_app-2.8.0/docs/conf.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      314 2024-03-12 19:01:09.000000 core_federated_search_app-2.8.0/docs/conf_urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2024-03-12 19:01:09.000000 core_federated_search_app-2.8.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       52 2024-03-12 19:01:09.000000 core_federated_search_app-2.8.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       83 2024-03-12 19:01:09.000000 core_federated_search_app-2.8.0/requirements.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2024-03-12 19:01:13.798978 core_federated_search_app-2.8.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1430 2024-03-12 19:01:09.000000 core_federated_search_app-2.8.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:13.496878 core_federated_search_app-2.8.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:09.000000 core_federated_search_app-2.8.0/tests/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:13.517803 core_federated_search_app-2.8.0/tests/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:09.000000 core_federated_search_app-2.8.0/tests/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:13.543447 core_federated_search_app-2.8.0/tests/components/instance/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:09.000000 core_federated_search_app-2.8.0/tests/components/instance/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:13.591679 core_federated_search_app-2.8.0/tests/components/instance/api/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:09.000000 core_federated_search_app-2.8.0/tests/components/instance/api/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4950 2024-03-12 19:01:09.000000 core_federated_search_app-2.8.0/tests/components/instance/api/tests_unit.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      150 2024-03-12 19:01:09.000000 core_federated_search_app-2.8.0/tests/mocks.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:13.612409 core_federated_search_app-2.8.0/tests/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:09.000000 core_federated_search_app-2.8.0/tests/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:13.721528 core_federated_search_app-2.8.0/tests/rest/instance/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:09.000000 core_federated_search_app-2.8.0/tests/rest/instance/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:13.770030 core_federated_search_app-2.8.0/tests/rest/instance/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:09.000000 core_federated_search_app-2.8.0/tests/rest/instance/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      962 2024-03-12 19:01:09.000000 core_federated_search_app-2.8.0/tests/rest/instance/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7935 2024-03-12 19:01:09.000000 core_federated_search_app-2.8.0/tests/rest/instance/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10748 2024-03-12 19:01:09.000000 core_federated_search_app-2.8.0/tests/rest/instance/tests_permission.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2214 2024-03-12 19:01:09.000000 core_federated_search_app-2.8.0/tests/rest/instance/tests_unit.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1645 2024-03-12 19:01:09.000000 core_federated_search_app-2.8.0/tests/test_settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:54.348112 core_federated_search_app-2.9.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2024-05-13 16:06:49.000000 core_federated_search_app-2.9.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      183 2024-05-13 16:06:49.000000 core_federated_search_app-2.9.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1232 2024-05-13 16:06:54.341380 core_federated_search_app-2.9.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      720 2024-05-13 16:06:49.000000 core_federated_search_app-2.9.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:52.977100 core_federated_search_app-2.9.0/core_federated_search_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       91 2024-05-13 16:06:49.000000 core_federated_search_app-2.9.0/core_federated_search_app/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1343 2024-05-13 16:06:49.000000 core_federated_search_app-2.9.0/core_federated_search_app/admin.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      270 2024-05-13 16:06:49.000000 core_federated_search_app-2.9.0/core_federated_search_app/apps.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:53.125011 core_federated_search_app-2.9.0/core_federated_search_app/commons/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:49.000000 core_federated_search_app-2.9.0/core_federated_search_app/commons/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      229 2024-05-13 16:06:49.000000 core_federated_search_app-2.9.0/core_federated_search_app/commons/exceptions.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:53.153881 core_federated_search_app-2.9.0/core_federated_search_app/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:49.000000 core_federated_search_app-2.9.0/core_federated_search_app/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:53.214052 core_federated_search_app-2.9.0/core_federated_search_app/components/instance/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:49.000000 core_federated_search_app-2.9.0/core_federated_search_app/components/instance/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5844 2024-05-13 16:06:49.000000 core_federated_search_app-2.9.0/core_federated_search_app/components/instance/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3739 2024-05-13 16:06:49.000000 core_federated_search_app-2.9.0/core_federated_search_app/components/instance/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:53.233048 core_federated_search_app-2.9.0/core_federated_search_app/components/instance/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:49.000000 core_federated_search_app-2.9.0/core_federated_search_app/components/instance/tests/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      501 2024-05-13 16:06:49.000000 core_federated_search_app-2.9.0/core_federated_search_app/menus.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:53.272494 core_federated_search_app-2.9.0/core_federated_search_app/migrations/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1476 2024-05-13 16:06:49.000000 core_federated_search_app-2.9.0/core_federated_search_app/migrations/0001_initial.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:49.000000 core_federated_search_app-2.9.0/core_federated_search_app/migrations/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:53.322524 core_federated_search_app-2.9.0/core_federated_search_app/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:49.000000 core_federated_search_app-2.9.0/core_federated_search_app/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:53.390145 core_federated_search_app-2.9.0/core_federated_search_app/rest/instance/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:49.000000 core_federated_search_app-2.9.0/core_federated_search_app/rest/instance/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1697 2024-05-13 16:06:49.000000 core_federated_search_app-2.9.0/core_federated_search_app/rest/instance/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8872 2024-05-13 16:06:49.000000 core_federated_search_app-2.9.0/core_federated_search_app/rest/instance/views.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      775 2024-05-13 16:06:49.000000 core_federated_search_app-2.9.0/core_federated_search_app/rest/urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      382 2024-05-13 16:06:49.000000 core_federated_search_app-2.9.0/core_federated_search_app/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:52.551376 core_federated_search_app-2.9.0/core_federated_search_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:52.562137 core_federated_search_app-2.9.0/core_federated_search_app/static/core_federated_search_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:52.578419 core_federated_search_app-2.9.0/core_federated_search_app/static/core_federated_search_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:53.414625 core_federated_search_app-2.9.0/core_federated_search_app/static/core_federated_search_app/admin/css/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       40 2024-05-13 16:06:49.000000 core_federated_search_app-2.9.0/core_federated_search_app/static/core_federated_search_app/admin/css/repositories.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:52.583179 core_federated_search_app-2.9.0/core_federated_search_app/static/core_federated_search_app/admin/js/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:52.588020 core_federated_search_app-2.9.0/core_federated_search_app/static/core_federated_search_app/admin/js/repositories/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:52.592754 core_federated_search_app-2.9.0/core_federated_search_app/static/core_federated_search_app/admin/js/repositories/list/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:53.512916 core_federated_search_app-2.9.0/core_federated_search_app/static/core_federated_search_app/admin/js/repositories/list/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      986 2024-05-13 16:06:49.000000 core_federated_search_app-2.9.0/core_federated_search_app/static/core_federated_search_app/admin/js/repositories/list/modals/delete.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      101 2024-05-13 16:06:49.000000 core_federated_search_app-2.9.0/core_federated_search_app/static/core_federated_search_app/admin/js/repositories/list/modals/delete.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1965 2024-05-13 16:06:49.000000 core_federated_search_app-2.9.0/core_federated_search_app/static/core_federated_search_app/admin/js/repositories/list/modals/refresh.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       99 2024-05-13 16:06:49.000000 core_federated_search_app-2.9.0/core_federated_search_app/static/core_federated_search_app/admin/js/repositories/list/modals/refresh.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:52.609085 core_federated_search_app-2.9.0/core_federated_search_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:52.613155 core_federated_search_app-2.9.0/core_federated_search_app/templates/core_federated_search_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:52.618035 core_federated_search_app-2.9.0/core_federated_search_app/templates/core_federated_search_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:53.560835 core_federated_search_app-2.9.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:53.582520 core_federated_search_app-2.9.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/add/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1576 2024-05-13 16:06:49.000000 core_federated_search_app-2.9.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/add/add_base.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      300 2024-05-13 16:06:49.000000 core_federated_search_app-2.9.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/add_repository.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:53.635311 core_federated_search_app-2.9.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/list/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2279 2024-05-13 16:06:49.000000 core_federated_search_app-2.9.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/list/list_base.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:53.706804 core_federated_search_app-2.9.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/list/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      842 2024-05-13 16:06:49.000000 core_federated_search_app-2.9.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/list/modals/delete.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1231 2024-05-13 16:06:49.000000 core_federated_search_app-2.9.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/list/modals/refresh.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       18 2024-05-13 16:06:49.000000 core_federated_search_app-2.9.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/list/refresh_form.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      349 2024-05-13 16:06:49.000000 core_federated_search_app-2.9.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/list_repositories.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      216 2024-05-13 16:06:49.000000 core_federated_search_app-2.9.0/core_federated_search_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:53.729501 core_federated_search_app-2.9.0/core_federated_search_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:49.000000 core_federated_search_app-2.9.0/core_federated_search_app/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:53.827869 core_federated_search_app-2.9.0/core_federated_search_app/views/admin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:49.000000 core_federated_search_app-2.9.0/core_federated_search_app/views/admin/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3634 2024-05-13 16:06:49.000000 core_federated_search_app-2.9.0/core_federated_search_app/views/admin/ajax.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2712 2024-05-13 16:06:49.000000 core_federated_search_app-2.9.0/core_federated_search_app/views/admin/forms.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3477 2024-05-13 16:06:49.000000 core_federated_search_app-2.9.0/core_federated_search_app/views/admin/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:53.075820 core_federated_search_app-2.9.0/core_federated_search_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1232 2024-05-13 16:06:51.000000 core_federated_search_app-2.9.0/core_federated_search_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3231 2024-05-13 16:06:52.000000 core_federated_search_app-2.9.0/core_federated_search_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2024-05-13 16:06:51.000000 core_federated_search_app-2.9.0/core_federated_search_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      135 2024-05-13 16:06:51.000000 core_federated_search_app-2.9.0/core_federated_search_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       37 2024-05-13 16:06:52.000000 core_federated_search_app-2.9.0/core_federated_search_app.egg-info/top_level.txt
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:53.891512 core_federated_search_app-2.9.0/docs/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:49.000000 core_federated_search_app-2.9.0/docs/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11132 2024-05-13 16:06:49.000000 core_federated_search_app-2.9.0/docs/conf.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      314 2024-05-13 16:06:49.000000 core_federated_search_app-2.9.0/docs/conf_urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2024-05-13 16:06:50.000000 core_federated_search_app-2.9.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       52 2024-05-13 16:06:50.000000 core_federated_search_app-2.9.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       83 2024-05-13 16:06:50.000000 core_federated_search_app-2.9.0/requirements.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2024-05-13 16:06:54.357334 core_federated_search_app-2.9.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1430 2024-05-13 16:06:50.000000 core_federated_search_app-2.9.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:53.997356 core_federated_search_app-2.9.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:50.000000 core_federated_search_app-2.9.0/tests/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:54.020405 core_federated_search_app-2.9.0/tests/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:50.000000 core_federated_search_app-2.9.0/tests/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:54.072098 core_federated_search_app-2.9.0/tests/components/instance/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:50.000000 core_federated_search_app-2.9.0/tests/components/instance/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:54.123034 core_federated_search_app-2.9.0/tests/components/instance/api/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:50.000000 core_federated_search_app-2.9.0/tests/components/instance/api/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4950 2024-05-13 16:06:50.000000 core_federated_search_app-2.9.0/tests/components/instance/api/tests_unit.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      150 2024-05-13 16:06:50.000000 core_federated_search_app-2.9.0/tests/mocks.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:54.145887 core_federated_search_app-2.9.0/tests/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:50.000000 core_federated_search_app-2.9.0/tests/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:54.259134 core_federated_search_app-2.9.0/tests/rest/instance/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:50.000000 core_federated_search_app-2.9.0/tests/rest/instance/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:54.306614 core_federated_search_app-2.9.0/tests/rest/instance/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:50.000000 core_federated_search_app-2.9.0/tests/rest/instance/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      962 2024-05-13 16:06:50.000000 core_federated_search_app-2.9.0/tests/rest/instance/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7935 2024-05-13 16:06:50.000000 core_federated_search_app-2.9.0/tests/rest/instance/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10748 2024-05-13 16:06:50.000000 core_federated_search_app-2.9.0/tests/rest/instance/tests_permission.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2214 2024-05-13 16:06:50.000000 core_federated_search_app-2.9.0/tests/rest/instance/tests_unit.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1645 2024-05-13 16:06:50.000000 core_federated_search_app-2.9.0/tests/test_settings.py
```

### Comparing `core_federated_search_app-2.8.0/LICENSE.md` & `core_federated_search_app-2.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `core_federated_search_app-2.8.0/PKG-INFO` & `core_federated_search_app-2.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_federated_search_app
-Version: 2.8.0
+Version: 2.9.0
 Summary: Federated search backend for the curator core project
 Home-page: https://github.com/usnistgov/core_federated_search_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: =========================
         Core Federated Search App
```

### Comparing `core_federated_search_app-2.8.0/README.rst` & `core_federated_search_app-2.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_federated_search_app-2.8.0/core_federated_search_app/admin.py` & `core_federated_search_app-2.9.0/core_federated_search_app/admin.py`

 * *Files identical despite different names*

### Comparing `core_federated_search_app-2.8.0/core_federated_search_app/components/instance/api.py` & `core_federated_search_app-2.9.0/core_federated_search_app/components/instance/api.py`

 * *Files identical despite different names*

### Comparing `core_federated_search_app-2.8.0/core_federated_search_app/components/instance/models.py` & `core_federated_search_app-2.9.0/core_federated_search_app/components/instance/models.py`

 * *Files identical despite different names*

### Comparing `core_federated_search_app-2.8.0/core_federated_search_app/migrations/0001_initial.py` & `core_federated_search_app-2.9.0/core_federated_search_app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `core_federated_search_app-2.8.0/core_federated_search_app/rest/instance/serializers.py` & `core_federated_search_app-2.9.0/core_federated_search_app/rest/instance/serializers.py`

 * *Files identical despite different names*

### Comparing `core_federated_search_app-2.8.0/core_federated_search_app/rest/instance/views.py` & `core_federated_search_app-2.9.0/core_federated_search_app/rest/instance/views.py`

 * *Files identical despite different names*

### Comparing `core_federated_search_app-2.8.0/core_federated_search_app/rest/urls.py` & `core_federated_search_app-2.9.0/core_federated_search_app/rest/urls.py`

 * *Files identical despite different names*

### Comparing `core_federated_search_app-2.8.0/core_federated_search_app/static/core_federated_search_app/admin/js/repositories/list/modals/delete.js` & `core_federated_search_app-2.9.0/core_federated_search_app/static/core_federated_search_app/admin/js/repositories/list/modals/delete.js`

 * *Files identical despite different names*

### Comparing `core_federated_search_app-2.8.0/core_federated_search_app/static/core_federated_search_app/admin/js/repositories/list/modals/refresh.js` & `core_federated_search_app-2.9.0/core_federated_search_app/static/core_federated_search_app/admin/js/repositories/list/modals/refresh.js`

 * *Files identical despite different names*

### Comparing `core_federated_search_app-2.8.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/add/add_base.html` & `core_federated_search_app-2.9.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/add/add_base.html`

 * *Files identical despite different names*

### Comparing `core_federated_search_app-2.8.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/list/list_base.html` & `core_federated_search_app-2.9.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/list/list_base.html`

 * *Files identical despite different names*

### Comparing `core_federated_search_app-2.8.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/list/modals/delete.html` & `core_federated_search_app-2.9.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/list/modals/delete.html`

 * *Files identical despite different names*

### Comparing `core_federated_search_app-2.8.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/list/modals/refresh.html` & `core_federated_search_app-2.9.0/core_federated_search_app/templates/core_federated_search_app/admin/repositories/list/modals/refresh.html`

 * *Files identical despite different names*

### Comparing `core_federated_search_app-2.8.0/core_federated_search_app/views/admin/ajax.py` & `core_federated_search_app-2.9.0/core_federated_search_app/views/admin/ajax.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 class EditRepositoryView(EditObjectModalView):
     form_class = EditRepositoryForm
     model = Instance
     success_url = reverse_lazy(
         "core-admin:core_federated_search_app_repositories"
     )
-    success_message = "Repository edited with success."
+    success_message = "Repository edited."
 
     def _save(self, form):
         # Save treatment.
         try:
             instance_api.upsert(self.object)
         except Exception as exception:
             form.add_error(None, str(exception))
```

### Comparing `core_federated_search_app-2.8.0/core_federated_search_app/views/admin/forms.py` & `core_federated_search_app-2.9.0/core_federated_search_app/views/admin/forms.py`

 * *Files identical despite different names*

### Comparing `core_federated_search_app-2.8.0/core_federated_search_app/views/admin/views.py` & `core_federated_search_app-2.9.0/core_federated_search_app/views/admin/views.py`

 * *Files identical despite different names*

### Comparing `core_federated_search_app-2.8.0/core_federated_search_app.egg-info/PKG-INFO` & `core_federated_search_app-2.9.0/core_federated_search_app.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-federated-search-app
-Version: 2.8.0
+Version: 2.9.0
 Summary: Federated search backend for the curator core project
 Home-page: https://github.com/usnistgov/core_federated_search_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: =========================
         Core Federated Search App
```

### Comparing `core_federated_search_app-2.8.0/core_federated_search_app.egg-info/SOURCES.txt` & `core_federated_search_app-2.9.0/core_federated_search_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `core_federated_search_app-2.8.0/docs/conf.py` & `core_federated_search_app-2.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `core_federated_search_app-2.8.0/setup.py` & `core_federated_search_app-2.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_federated_search_app",
-    version="2.8.0",
+    version="2.9.0",
     description="Federated search backend for the curator core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_federated_search_app",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `core_federated_search_app-2.8.0/tests/components/instance/api/tests_unit.py` & `core_federated_search_app-2.9.0/tests/components/instance/api/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_federated_search_app-2.8.0/tests/rest/instance/fixtures/fixtures.py` & `core_federated_search_app-2.9.0/tests/rest/instance/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_federated_search_app-2.8.0/tests/rest/instance/tests_int.py` & `core_federated_search_app-2.9.0/tests/rest/instance/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_federated_search_app-2.8.0/tests/rest/instance/tests_permission.py` & `core_federated_search_app-2.9.0/tests/rest/instance/tests_permission.py`

 * *Files identical despite different names*

### Comparing `core_federated_search_app-2.8.0/tests/rest/instance/tests_unit.py` & `core_federated_search_app-2.9.0/tests/rest/instance/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_federated_search_app-2.8.0/tests/test_settings.py` & `core_federated_search_app-2.9.0/tests/test_settings.py`

 * *Files identical despite different names*

