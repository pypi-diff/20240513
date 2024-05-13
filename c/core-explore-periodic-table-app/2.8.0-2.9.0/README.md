# Comparing `tmp/core_explore_periodic_table_app-2.8.0.tar.gz` & `tmp/core_explore_periodic_table_app-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_explore_periodic_table_app-2.8.0.tar", last modified: Tue Mar 12 19:00:35 2024, max compression
+gzip compressed data, was "core_explore_periodic_table_app-2.9.0.tar", last modified: Mon May 13 16:06:15 2024, max compression
```

## Comparing `core_explore_periodic_table_app-2.8.0.tar` & `core_explore_periodic_table_app-2.9.0.tar`

### file list

```diff
@@ -1,128 +1,132 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:35.075777 core_explore_periodic_table_app-2.8.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2024-03-12 19:00:29.000000 core_explore_periodic_table_app-2.8.0/LICENSE.md
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      194 2024-03-12 19:00:29.000000 core_explore_periodic_table_app-2.8.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2483 2024-03-12 19:00:35.069596 core_explore_periodic_table_app-2.8.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1671 2024-03-12 19:00:29.000000 core_explore_periodic_table_app-2.8.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:33.356788 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      128 2024-03-12 19:00:29.000000 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1189 2024-03-12 19:00:29.000000 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/admin.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      525 2024-03-12 19:00:29.000000 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/apps.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:33.465753 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:29.000000 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:33.540906 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/components/persistent_query_periodic_table/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:29.000000 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/components/persistent_query_periodic_table/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      391 2024-03-12 19:00:29.000000 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/components/persistent_query_periodic_table/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2524 2024-03-12 19:00:29.000000 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/components/persistent_query_periodic_table/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2094 2024-03-12 19:00:29.000000 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/components/persistent_query_periodic_table/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:33.752049 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/components/search_operator_mapping/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:29.000000 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/components/search_operator_mapping/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      342 2024-03-12 19:00:29.000000 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/components/search_operator_mapping/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1124 2024-03-12 19:00:29.000000 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/components/search_operator_mapping/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1053 2024-03-12 19:00:29.000000 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/components/search_operator_mapping/models.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      498 2024-03-12 19:00:29.000000 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/menus.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:33.823657 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/migrations/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3194 2024-03-12 19:00:29.000000 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/migrations/0001_initial.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:29.000000 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/migrations/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      597 2024-03-12 19:00:29.000000 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:33.888333 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/permissions/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:29.000000 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/permissions/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1166 2024-03-12 19:00:29.000000 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/permissions/discover.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      187 2024-03-12 19:00:29.000000 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/permissions/rights.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:33.931573 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:29.000000 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:33.999177 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/rest/persistent_query_periodic_table/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:29.000000 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/rest/persistent_query_periodic_table/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3598 2024-03-12 19:00:29.000000 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/rest/persistent_query_periodic_table/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    13622 2024-03-12 19:00:29.000000 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/rest/persistent_query_periodic_table/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:34.067933 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/rest/search_operator_mapping/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:29.000000 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/rest/search_operator_mapping/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1455 2024-03-12 19:00:29.000000 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/rest/search_operator_mapping/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8161 2024-03-12 19:00:29.000000 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/rest/search_operator_mapping/views.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1947 2024-03-12 19:00:29.000000 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/rest/urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      135 2024-03-12 19:00:29.000000 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:32.876485 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:32.902496 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:34.100362 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/admin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       97 2024-03-12 19:00:29.000000 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/admin/form.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:32.893082 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/common/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:34.127408 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/common/xsd/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5699 2024-03-12 19:00:29.000000 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/common/xsd/default_chemical_element_type.xsd
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:32.940338 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:32.934552 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/user/css/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:34.160826 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/user/css/periodic_table/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1747 2024-03-12 19:00:29.000000 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/user/css/periodic_table/periodic.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:34.184746 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/user/js/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:34.207672 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/user/js/periodic_table/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5531 2024-03-12 19:00:29.000000 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/user/js/periodic_table/periodic.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      354 2024-03-12 19:00:29.000000 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/user/js/persistent_query.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:32.961534 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:32.993734 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:32.981374 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:34.240599 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/admin/periodic_table_type/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      382 2024-03-12 19:00:29.000000 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/admin/periodic_table_type/manage_periodic_table_type.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:34.262282 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/admin/periodic_table_type/selector/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      425 2024-03-12 19:00:29.000000 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/admin/periodic_table_type/selector/selector.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:34.282014 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      914 2024-03-12 19:00:29.000000 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/user/index.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:34.302547 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/user/periodic_table/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7406 2024-03-12 19:00:29.000000 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/user/periodic_table/periodic.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:34.323144 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/user/selector/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      250 2024-03-12 19:00:29.000000 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/user/selector/data_sources_selector.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      996 2024-03-12 19:00:29.000000 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:34.343521 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:30.000000 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:34.411234 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/views/admin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:30.000000 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/views/admin/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1570 2024-03-12 19:00:30.000000 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/views/admin/forms.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3603 2024-03-12 19:00:30.000000 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/views/admin/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:34.497340 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/views/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:30.000000 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/views/user/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      728 2024-03-12 19:00:30.000000 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/views/user/ajax.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2016 2024-03-12 19:00:30.000000 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/views/user/form.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14617 2024-03-12 19:00:30.000000 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/views/user/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:33.442303 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2483 2024-03-12 19:00:32.000000 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4827 2024-03-12 19:00:32.000000 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2024-03-12 19:00:32.000000 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      110 2024-03-12 19:00:32.000000 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2024-03-12 19:00:32.000000 core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app.egg-info/top_level.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      170 2024-03-12 19:00:30.000000 core_explore_periodic_table_app-2.8.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       84 2024-03-12 19:00:30.000000 core_explore_periodic_table_app-2.8.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       26 2024-03-12 19:00:30.000000 core_explore_periodic_table_app-2.8.0/requirements.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2024-03-12 19:00:35.078977 core_explore_periodic_table_app-2.8.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1463 2024-03-12 19:00:30.000000 core_explore_periodic_table_app-2.8.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:34.544654 core_explore_periodic_table_app-2.8.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:30.000000 core_explore_periodic_table_app-2.8.0/tests/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:34.565977 core_explore_periodic_table_app-2.8.0/tests/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:30.000000 core_explore_periodic_table_app-2.8.0/tests/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:34.647403 core_explore_periodic_table_app-2.8.0/tests/components/persistent_query_periodic_table/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:30.000000 core_explore_periodic_table_app-2.8.0/tests/components/persistent_query_periodic_table/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:34.689320 core_explore_periodic_table_app-2.8.0/tests/components/persistent_query_periodic_table/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:30.000000 core_explore_periodic_table_app-2.8.0/tests/components/persistent_query_periodic_table/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1788 2024-03-12 19:00:30.000000 core_explore_periodic_table_app-2.8.0/tests/components/persistent_query_periodic_table/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    17193 2024-03-12 19:00:30.000000 core_explore_periodic_table_app-2.8.0/tests/components/persistent_query_periodic_table/tests_int_access_control.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7296 2024-03-12 19:00:30.000000 core_explore_periodic_table_app-2.8.0/tests/components/persistent_query_periodic_table/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:34.735181 core_explore_periodic_table_app-2.8.0/tests/components/search_operators_mapping/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:30.000000 core_explore_periodic_table_app-2.8.0/tests/components/search_operators_mapping/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4467 2024-03-12 19:00:30.000000 core_explore_periodic_table_app-2.8.0/tests/components/search_operators_mapping/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:34.758439 core_explore_periodic_table_app-2.8.0/tests/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:30.000000 core_explore_periodic_table_app-2.8.0/tests/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:34.825133 core_explore_periodic_table_app-2.8.0/tests/rest/persistent_query_periodic_table/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:30.000000 core_explore_periodic_table_app-2.8.0/tests/rest/persistent_query_periodic_table/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    12797 2024-03-12 19:00:30.000000 core_explore_periodic_table_app-2.8.0/tests/rest/persistent_query_periodic_table/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    18854 2024-03-12 19:00:30.000000 core_explore_periodic_table_app-2.8.0/tests/rest/persistent_query_periodic_table/tests_permissions.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:34.890496 core_explore_periodic_table_app-2.8.0/tests/rest/search_operators_mapping/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:30.000000 core_explore_periodic_table_app-2.8.0/tests/rest/search_operators_mapping/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:34.933604 core_explore_periodic_table_app-2.8.0/tests/rest/search_operators_mapping/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:30.000000 core_explore_periodic_table_app-2.8.0/tests/rest/search_operators_mapping/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3042 2024-03-12 19:00:30.000000 core_explore_periodic_table_app-2.8.0/tests/rest/search_operators_mapping/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4434 2024-03-12 19:00:30.000000 core_explore_periodic_table_app-2.8.0/tests/rest/search_operators_mapping/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11061 2024-03-12 19:00:30.000000 core_explore_periodic_table_app-2.8.0/tests/rest/search_operators_mapping/tests_permissions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1855 2024-03-12 19:00:30.000000 core_explore_periodic_table_app-2.8.0/tests/test_settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:34.955642 core_explore_periodic_table_app-2.8.0/tests/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:30.000000 core_explore_periodic_table_app-2.8.0/tests/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:34.981011 core_explore_periodic_table_app-2.8.0/tests/views/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:30.000000 core_explore_periodic_table_app-2.8.0/tests/views/user/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:35.027207 core_explore_periodic_table_app-2.8.0/tests/views/user/forms/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:30.000000 core_explore_periodic_table_app-2.8.0/tests/views/user/forms/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1902 2024-03-12 19:00:30.000000 core_explore_periodic_table_app-2.8.0/tests/views/user/forms/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:15.057268 core_explore_periodic_table_app-2.9.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2024-05-13 16:06:09.000000 core_explore_periodic_table_app-2.9.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      194 2024-05-13 16:06:09.000000 core_explore_periodic_table_app-2.9.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2483 2024-05-13 16:06:15.051353 core_explore_periodic_table_app-2.9.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1671 2024-05-13 16:06:09.000000 core_explore_periodic_table_app-2.9.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:13.462344 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      128 2024-05-13 16:06:09.000000 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1189 2024-05-13 16:06:09.000000 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/admin.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      525 2024-05-13 16:06:09.000000 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/apps.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:13.583607 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:09.000000 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:13.662486 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/components/persistent_query_periodic_table/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:09.000000 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/components/persistent_query_periodic_table/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      391 2024-05-13 16:06:09.000000 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/components/persistent_query_periodic_table/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2524 2024-05-13 16:06:09.000000 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/components/persistent_query_periodic_table/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2094 2024-05-13 16:06:09.000000 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/components/persistent_query_periodic_table/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:13.747520 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/components/search_operator_mapping/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:09.000000 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/components/search_operator_mapping/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      342 2024-05-13 16:06:09.000000 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/components/search_operator_mapping/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1124 2024-05-13 16:06:09.000000 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/components/search_operator_mapping/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1053 2024-05-13 16:06:09.000000 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/components/search_operator_mapping/models.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      498 2024-05-13 16:06:09.000000 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/menus.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:13.784193 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/migrations/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3194 2024-05-13 16:06:09.000000 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/migrations/0001_initial.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:09.000000 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/migrations/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      597 2024-05-13 16:06:09.000000 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:13.858903 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/permissions/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:09.000000 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/permissions/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1166 2024-05-13 16:06:09.000000 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/permissions/discover.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      187 2024-05-13 16:06:09.000000 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/permissions/rights.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:13.921262 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:09.000000 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:13.983735 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/rest/persistent_query_periodic_table/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:09.000000 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/rest/persistent_query_periodic_table/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3598 2024-05-13 16:06:09.000000 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/rest/persistent_query_periodic_table/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    13622 2024-05-13 16:06:09.000000 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/rest/persistent_query_periodic_table/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:14.045606 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/rest/search_operator_mapping/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:09.000000 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/rest/search_operator_mapping/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1455 2024-05-13 16:06:09.000000 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/rest/search_operator_mapping/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8161 2024-05-13 16:06:09.000000 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/rest/search_operator_mapping/views.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1947 2024-05-13 16:06:09.000000 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/rest/urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      135 2024-05-13 16:06:09.000000 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:12.984235 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:13.019195 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:14.072694 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/admin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       97 2024-05-13 16:06:09.000000 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/admin/form.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:13.009421 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/common/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:14.096457 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/common/xsd/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5699 2024-05-13 16:06:09.000000 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/common/xsd/default_chemical_element_type.xsd
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:13.032839 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:13.027104 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/user/css/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:14.123592 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/user/css/periodic_table/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1747 2024-05-13 16:06:09.000000 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/user/css/periodic_table/periodic.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:14.143881 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/user/js/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:14.164935 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/user/js/periodic_table/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5531 2024-05-13 16:06:09.000000 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/user/js/periodic_table/periodic.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      354 2024-05-13 16:06:09.000000 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/user/js/persistent_query.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:13.054139 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:13.077068 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:13.063299 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:14.200172 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/admin/periodic_table_type/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      382 2024-05-13 16:06:09.000000 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/admin/periodic_table_type/manage_periodic_table_type.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:14.222306 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/admin/periodic_table_type/selector/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      425 2024-05-13 16:06:09.000000 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/admin/periodic_table_type/selector/selector.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:14.244620 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      914 2024-05-13 16:06:09.000000 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/user/index.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:14.267953 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/user/periodic_table/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7406 2024-05-13 16:06:09.000000 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/user/periodic_table/periodic.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:14.289768 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/user/selector/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      250 2024-05-13 16:06:09.000000 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/user/selector/data_sources_selector.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      996 2024-05-13 16:06:09.000000 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:14.312343 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:09.000000 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:14.387955 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/views/admin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:09.000000 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/views/admin/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1570 2024-05-13 16:06:09.000000 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/views/admin/forms.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3576 2024-05-13 16:06:10.000000 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/views/admin/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:14.472012 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/views/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:10.000000 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/views/user/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      728 2024-05-13 16:06:10.000000 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/views/user/ajax.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2016 2024-05-13 16:06:10.000000 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/views/user/form.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14617 2024-05-13 16:06:10.000000 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/views/user/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:13.558461 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2483 2024-05-13 16:06:12.000000 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4902 2024-05-13 16:06:12.000000 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2024-05-13 16:06:12.000000 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      110 2024-05-13 16:06:12.000000 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2024-05-13 16:06:12.000000 core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app.egg-info/top_level.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      170 2024-05-13 16:06:10.000000 core_explore_periodic_table_app-2.9.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       84 2024-05-13 16:06:10.000000 core_explore_periodic_table_app-2.9.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       26 2024-05-13 16:06:10.000000 core_explore_periodic_table_app-2.9.0/requirements.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2024-05-13 16:06:15.059842 core_explore_periodic_table_app-2.9.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1463 2024-05-13 16:06:10.000000 core_explore_periodic_table_app-2.9.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:14.537844 core_explore_periodic_table_app-2.9.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:10.000000 core_explore_periodic_table_app-2.9.0/tests/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:14.559152 core_explore_periodic_table_app-2.9.0/tests/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:10.000000 core_explore_periodic_table_app-2.9.0/tests/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:14.629706 core_explore_periodic_table_app-2.9.0/tests/components/persistent_query_periodic_table/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:10.000000 core_explore_periodic_table_app-2.9.0/tests/components/persistent_query_periodic_table/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:14.669853 core_explore_periodic_table_app-2.9.0/tests/components/persistent_query_periodic_table/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:10.000000 core_explore_periodic_table_app-2.9.0/tests/components/persistent_query_periodic_table/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1788 2024-05-13 16:06:10.000000 core_explore_periodic_table_app-2.9.0/tests/components/persistent_query_periodic_table/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    17193 2024-05-13 16:06:10.000000 core_explore_periodic_table_app-2.9.0/tests/components/persistent_query_periodic_table/tests_int_access_control.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7296 2024-05-13 16:06:10.000000 core_explore_periodic_table_app-2.9.0/tests/components/persistent_query_periodic_table/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:14.722520 core_explore_periodic_table_app-2.9.0/tests/components/search_operators_mapping/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:10.000000 core_explore_periodic_table_app-2.9.0/tests/components/search_operators_mapping/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4467 2024-05-13 16:06:10.000000 core_explore_periodic_table_app-2.9.0/tests/components/search_operators_mapping/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:14.742841 core_explore_periodic_table_app-2.9.0/tests/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:10.000000 core_explore_periodic_table_app-2.9.0/tests/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:14.803004 core_explore_periodic_table_app-2.9.0/tests/rest/persistent_query_periodic_table/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:10.000000 core_explore_periodic_table_app-2.9.0/tests/rest/persistent_query_periodic_table/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    12797 2024-05-13 16:06:10.000000 core_explore_periodic_table_app-2.9.0/tests/rest/persistent_query_periodic_table/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    18854 2024-05-13 16:06:10.000000 core_explore_periodic_table_app-2.9.0/tests/rest/persistent_query_periodic_table/tests_permissions.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:14.858164 core_explore_periodic_table_app-2.9.0/tests/rest/search_operators_mapping/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:10.000000 core_explore_periodic_table_app-2.9.0/tests/rest/search_operators_mapping/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:14.897309 core_explore_periodic_table_app-2.9.0/tests/rest/search_operators_mapping/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:10.000000 core_explore_periodic_table_app-2.9.0/tests/rest/search_operators_mapping/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3042 2024-05-13 16:06:10.000000 core_explore_periodic_table_app-2.9.0/tests/rest/search_operators_mapping/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4434 2024-05-13 16:06:10.000000 core_explore_periodic_table_app-2.9.0/tests/rest/search_operators_mapping/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11061 2024-05-13 16:06:10.000000 core_explore_periodic_table_app-2.9.0/tests/rest/search_operators_mapping/tests_permissions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1948 2024-05-13 16:06:10.000000 core_explore_periodic_table_app-2.9.0/tests/test_settings.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      369 2024-05-13 16:06:10.000000 core_explore_periodic_table_app-2.9.0/tests/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:14.916944 core_explore_periodic_table_app-2.9.0/tests/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:10.000000 core_explore_periodic_table_app-2.9.0/tests/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:14.966458 core_explore_periodic_table_app-2.9.0/tests/views/admin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:10.000000 core_explore_periodic_table_app-2.9.0/tests/views/admin/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      754 2024-05-13 16:06:10.000000 core_explore_periodic_table_app-2.9.0/tests/views/admin/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:14.984227 core_explore_periodic_table_app-2.9.0/tests/views/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:10.000000 core_explore_periodic_table_app-2.9.0/tests/views/user/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:15.027299 core_explore_periodic_table_app-2.9.0/tests/views/user/forms/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:10.000000 core_explore_periodic_table_app-2.9.0/tests/views/user/forms/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1902 2024-05-13 16:06:10.000000 core_explore_periodic_table_app-2.9.0/tests/views/user/forms/tests_unit.py
```

### Comparing `core_explore_periodic_table_app-2.8.0/LICENSE.md` & `core_explore_periodic_table_app-2.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.8.0/PKG-INFO` & `core_explore_periodic_table_app-2.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_explore_periodic_table_app
-Version: 2.8.0
+Version: 2.9.0
 Summary: Core explore periodic table capabilities for the curator core project
 Home-page: https://github.com/usnistgov/core_explore_periodic_table_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: core_explore_periodic_table_app
         ===============================
```

### Comparing `core_explore_periodic_table_app-2.8.0/README.rst` & `core_explore_periodic_table_app-2.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/admin.py` & `core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/admin.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/apps.py` & `core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/apps.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/components/persistent_query_periodic_table/api.py` & `core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/components/persistent_query_periodic_table/api.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/components/persistent_query_periodic_table/models.py` & `core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/components/persistent_query_periodic_table/models.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/components/search_operator_mapping/api.py` & `core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/components/search_operator_mapping/api.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/components/search_operator_mapping/models.py` & `core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/components/search_operator_mapping/models.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/migrations/0001_initial.py` & `core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/models.py` & `core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/models.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/permissions/discover.py` & `core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/permissions/discover.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/rest/persistent_query_periodic_table/serializers.py` & `core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/rest/persistent_query_periodic_table/serializers.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/rest/persistent_query_periodic_table/views.py` & `core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/rest/persistent_query_periodic_table/views.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/rest/search_operator_mapping/serializers.py` & `core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/rest/search_operator_mapping/serializers.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/rest/search_operator_mapping/views.py` & `core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/rest/search_operator_mapping/views.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/rest/urls.py` & `core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/rest/urls.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/common/xsd/default_chemical_element_type.xsd` & `core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/common/xsd/default_chemical_element_type.xsd`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/user/css/periodic_table/periodic.css` & `core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/user/css/periodic_table/periodic.css`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/user/js/periodic_table/periodic.js` & `core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/static/core_explore_periodic_table_app/user/js/periodic_table/periodic.js`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/user/index.html` & `core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/user/index.html`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/user/periodic_table/periodic.html` & `core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/templates/core_explore_periodic_table_app/user/periodic_table/periodic.html`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/urls.py` & `core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/urls.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/views/admin/forms.py` & `core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/views/admin/forms.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/views/admin/views.py` & `core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/views/admin/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,17 +110,15 @@
 
     # load the form
     associated_form = AssociatedPeriodicTableSearchOperatorForm()
     assets = {"css": ["core_explore_periodic_table_app/admin/form.css"]}
 
     context = {"associated_form": associated_form}
 
-    messages.add_message(
-        request, messages.SUCCESS, "Information saved with success."
-    )
+    messages.add_message(request, messages.SUCCESS, "Information saved.")
 
     return admin_render(
         request,
         "core_explore_periodic_table_app/admin/periodic_table_type/manage_periodic_table_type.html",
         context=context,
         assets=assets,
     )
```

### Comparing `core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/views/user/ajax.py` & `core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/views/user/ajax.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/views/user/form.py` & `core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/views/user/form.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app/views/user/views.py` & `core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app/views/user/views.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app.egg-info/PKG-INFO` & `core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-explore-periodic-table-app
-Version: 2.8.0
+Version: 2.9.0
 Summary: Core explore periodic table capabilities for the curator core project
 Home-page: https://github.com/usnistgov/core_explore_periodic_table_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: core_explore_periodic_table_app
         ===============================
```

### Comparing `core_explore_periodic_table_app-2.8.0/core_explore_periodic_table_app.egg-info/SOURCES.txt` & `core_explore_periodic_table_app-2.9.0/core_explore_periodic_table_app.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -55,14 +55,15 @@
 core_explore_periodic_table_app/views/admin/views.py
 core_explore_periodic_table_app/views/user/__init__.py
 core_explore_periodic_table_app/views/user/ajax.py
 core_explore_periodic_table_app/views/user/form.py
 core_explore_periodic_table_app/views/user/views.py
 tests/__init__.py
 tests/test_settings.py
+tests/urls.py
 tests/components/__init__.py
 tests/components/persistent_query_periodic_table/__init__.py
 tests/components/persistent_query_periodic_table/tests_int_access_control.py
 tests/components/persistent_query_periodic_table/tests_unit.py
 tests/components/persistent_query_periodic_table/fixtures/__init__.py
 tests/components/persistent_query_periodic_table/fixtures/fixtures.py
 tests/components/search_operators_mapping/__init__.py
@@ -73,10 +74,12 @@
 tests/rest/persistent_query_periodic_table/tests_permissions.py
 tests/rest/search_operators_mapping/__init__.py
 tests/rest/search_operators_mapping/tests_int.py
 tests/rest/search_operators_mapping/tests_permissions.py
 tests/rest/search_operators_mapping/fixtures/__init__.py
 tests/rest/search_operators_mapping/fixtures/fixtures.py
 tests/views/__init__.py
+tests/views/admin/__init__.py
+tests/views/admin/test_unit.py
 tests/views/user/__init__.py
 tests/views/user/forms/__init__.py
 tests/views/user/forms/tests_unit.py
```

### Comparing `core_explore_periodic_table_app-2.8.0/setup.py` & `core_explore_periodic_table_app-2.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_explore_periodic_table_app",
-    version="2.8.0",
+    version="2.9.0",
     description="Core explore periodic table capabilities for the curator core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_explore_periodic_table_app",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `core_explore_periodic_table_app-2.8.0/tests/components/persistent_query_periodic_table/fixtures/fixtures.py` & `core_explore_periodic_table_app-2.9.0/tests/components/persistent_query_periodic_table/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.8.0/tests/components/persistent_query_periodic_table/tests_int_access_control.py` & `core_explore_periodic_table_app-2.9.0/tests/components/persistent_query_periodic_table/tests_int_access_control.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.8.0/tests/components/persistent_query_periodic_table/tests_unit.py` & `core_explore_periodic_table_app-2.9.0/tests/components/persistent_query_periodic_table/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.8.0/tests/components/search_operators_mapping/tests_unit.py` & `core_explore_periodic_table_app-2.9.0/tests/components/search_operators_mapping/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.8.0/tests/rest/persistent_query_periodic_table/tests_int.py` & `core_explore_periodic_table_app-2.9.0/tests/rest/persistent_query_periodic_table/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.8.0/tests/rest/persistent_query_periodic_table/tests_permissions.py` & `core_explore_periodic_table_app-2.9.0/tests/rest/persistent_query_periodic_table/tests_permissions.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.8.0/tests/rest/search_operators_mapping/fixtures/fixtures.py` & `core_explore_periodic_table_app-2.9.0/tests/rest/search_operators_mapping/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.8.0/tests/rest/search_operators_mapping/tests_int.py` & `core_explore_periodic_table_app-2.9.0/tests/rest/search_operators_mapping/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.8.0/tests/rest/search_operators_mapping/tests_permissions.py` & `core_explore_periodic_table_app-2.9.0/tests/rest/search_operators_mapping/tests_permissions.py`

 * *Files identical despite different names*

### Comparing `core_explore_periodic_table_app-2.8.0/tests/test_settings.py` & `core_explore_periodic_table_app-2.9.0/tests/test_settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     "django.contrib.auth",
     "django.contrib.contenttypes",
     "django.contrib.sessions",
     "django.contrib.messages",
     "django.contrib.sites",
     "django.contrib.staticfiles",
     "django_celery_beat",
+    "menu",
     # Local apps
     "tests",
     "core_main_app",
     "core_explore_common_app",
     "core_explore_keyword_app",
     "core_explore_periodic_table_app",
 ]
@@ -58,12 +59,14 @@
                 "core_main_app.utils.custom_context_processors.domain_context_processor",  # Needed by any curator app
                 "django.template.context_processors.i18n",
             ],
         },
     },
 ]
 
-
+ROOT_URLCONF = "tests.urls"
 DEFAULT_AUTO_FIELD = "django.db.models.BigAutoField"
 CELERYBEAT_SCHEDULER = "django_celery_beat.schedulers:DatabaseScheduler"
 MONGODB_INDEXING = False
 MONGODB_ASYNC_SAVE = False
+STATIC_URL = "/static/"
+ENABLE_SAML2_SSO_AUTH = False
```

### Comparing `core_explore_periodic_table_app-2.8.0/tests/views/user/forms/tests_unit.py` & `core_explore_periodic_table_app-2.9.0/tests/views/user/forms/tests_unit.py`

 * *Files identical despite different names*

