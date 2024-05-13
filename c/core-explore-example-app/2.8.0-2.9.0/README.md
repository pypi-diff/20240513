# Comparing `tmp/core_explore_example_app-2.8.0.tar.gz` & `tmp/core_explore_example_app-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_explore_example_app-2.8.0.tar", last modified: Tue Mar 12 18:59:20 2024, max compression
+gzip compressed data, was "core_explore_example_app-2.9.0.tar", last modified: Mon May 13 16:04:58 2024, max compression
```

## Comparing `core_explore_example_app-2.8.0.tar` & `core_explore_example_app-2.9.0.tar`

### file list

```diff
@@ -1,188 +1,188 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:20.243722 core_explore_example_app-2.8.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2024-03-12 18:59:11.000000 core_explore_example_app-2.8.0/LICENSE.md
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      156 2024-03-12 18:59:11.000000 core_explore_example_app-2.8.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1114 2024-03-12 18:59:20.237124 core_explore_example_app-2.8.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      614 2024-03-12 18:59:11.000000 core_explore_example_app-2.8.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:17.477286 core_explore_example_app-2.8.0/core_explore_example_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2024-03-12 18:59:11.000000 core_explore_example_app-2.8.0/core_explore_example_app/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1093 2024-03-12 18:59:11.000000 core_explore_example_app-2.8.0/core_explore_example_app/admin.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      634 2024-03-12 18:59:11.000000 core_explore_example_app-2.8.0/core_explore_example_app/apps.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:17.615349 core_explore_example_app-2.8.0/core_explore_example_app/commons/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:11.000000 core_explore_example_app-2.8.0/core_explore_example_app/commons/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      205 2024-03-12 18:59:11.000000 core_explore_example_app-2.8.0/core_explore_example_app/commons/exceptions.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:17.635437 core_explore_example_app-2.8.0/core_explore_example_app/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:11.000000 core_explore_example_app-2.8.0/core_explore_example_app/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:17.715606 core_explore_example_app-2.8.0/core_explore_example_app/components/explore_data_structure/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:11.000000 core_explore_example_app-2.8.0/core_explore_example_app/components/explore_data_structure/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      442 2024-03-12 18:59:11.000000 core_explore_example_app-2.8.0/core_explore_example_app/components/explore_data_structure/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2006 2024-03-12 18:59:11.000000 core_explore_example_app-2.8.0/core_explore_example_app/components/explore_data_structure/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1764 2024-03-12 18:59:11.000000 core_explore_example_app-2.8.0/core_explore_example_app/components/explore_data_structure/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:17.834763 core_explore_example_app-2.8.0/core_explore_example_app/components/persistent_query_example/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:11.000000 core_explore_example_app-2.8.0/core_explore_example_app/components/persistent_query_example/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      372 2024-03-12 18:59:11.000000 core_explore_example_app-2.8.0/core_explore_example_app/components/persistent_query_example/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2283 2024-03-12 18:59:11.000000 core_explore_example_app-2.8.0/core_explore_example_app/components/persistent_query_example/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1973 2024-03-12 18:59:11.000000 core_explore_example_app-2.8.0/core_explore_example_app/components/persistent_query_example/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:17.917501 core_explore_example_app-2.8.0/core_explore_example_app/components/saved_query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:11.000000 core_explore_example_app-2.8.0/core_explore_example_app/components/saved_query/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      356 2024-03-12 18:59:11.000000 core_explore_example_app-2.8.0/core_explore_example_app/components/saved_query/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      904 2024-03-12 18:59:11.000000 core_explore_example_app-2.8.0/core_explore_example_app/components/saved_query/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1565 2024-03-12 18:59:11.000000 core_explore_example_app-2.8.0/core_explore_example_app/components/saved_query/models.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      927 2024-03-12 18:59:11.000000 core_explore_example_app-2.8.0/core_explore_example_app/discover.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      321 2024-03-12 18:59:11.000000 core_explore_example_app-2.8.0/core_explore_example_app/menus.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:17.956656 core_explore_example_app-2.8.0/core_explore_example_app/migrations/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4401 2024-03-12 18:59:11.000000 core_explore_example_app-2.8.0/core_explore_example_app/migrations/0001_initial.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:11.000000 core_explore_example_app-2.8.0/core_explore_example_app/migrations/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1058 2024-03-12 18:59:11.000000 core_explore_example_app-2.8.0/core_explore_example_app/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:18.023478 core_explore_example_app-2.8.0/core_explore_example_app/permissions/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:11.000000 core_explore_example_app-2.8.0/core_explore_example_app/permissions/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1723 2024-03-12 18:59:11.000000 core_explore_example_app-2.8.0/core_explore_example_app/permissions/discover.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      320 2024-03-12 18:59:11.000000 core_explore_example_app-2.8.0/core_explore_example_app/permissions/rights.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:18.069163 core_explore_example_app-2.8.0/core_explore_example_app/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:11.000000 core_explore_example_app-2.8.0/core_explore_example_app/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:18.133865 core_explore_example_app-2.8.0/core_explore_example_app/rest/persistent_query_example/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:11.000000 core_explore_example_app-2.8.0/core_explore_example_app/rest/persistent_query_example/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3259 2024-03-12 18:59:11.000000 core_explore_example_app-2.8.0/core_explore_example_app/rest/persistent_query_example/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    13206 2024-03-12 18:59:11.000000 core_explore_example_app-2.8.0/core_explore_example_app/rest/persistent_query_example/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:18.208133 core_explore_example_app-2.8.0/core_explore_example_app/rest/saved_query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:11.000000 core_explore_example_app-2.8.0/core_explore_example_app/rest/saved_query/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      395 2024-03-12 18:59:11.000000 core_explore_example_app-2.8.0/core_explore_example_app/rest/saved_query/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4767 2024-03-12 18:59:11.000000 core_explore_example_app-2.8.0/core_explore_example_app/rest/saved_query/views.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1653 2024-03-12 18:59:11.000000 core_explore_example_app-2.8.0/core_explore_example_app/rest/urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      620 2024-03-12 18:59:11.000000 core_explore_example_app-2.8.0/core_explore_example_app/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:16.979942 core_explore_example_app-2.8.0/core_explore_example_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:16.984355 core_explore_example_app-2.8.0/core_explore_example_app/static/core_explore_example_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:17.005027 core_explore_example_app-2.8.0/core_explore_example_app/static/core_explore_example_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:18.279159 core_explore_example_app-2.8.0/core_explore_example_app/static/core_explore_example_app/user/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      724 2024-03-12 18:59:11.000000 core_explore_example_app-2.8.0/core_explore_example_app/static/core_explore_example_app/user/css/query_builder.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      465 2024-03-12 18:59:11.000000 core_explore_example_app-2.8.0/core_explore_example_app/static/core_explore_example_app/user/css/style.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      170 2024-03-12 18:59:12.000000 core_explore_example_app-2.8.0/core_explore_example_app/static/core_explore_example_app/user/css/xsd_form.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:18.463665 core_explore_example_app-2.8.0/core_explore_example_app/static/core_explore_example_app/user/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14448 2024-03-12 18:59:12.000000 core_explore_example_app-2.8.0/core_explore_example_app/static/core_explore_example_app/user/js/build_query.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1044 2024-03-12 18:59:12.000000 core_explore_example_app-2.8.0/core_explore_example_app/static/core_explore_example_app/user/js/build_query.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      147 2024-03-12 18:59:12.000000 core_explore_example_app-2.8.0/core_explore_example_app/static/core_explore_example_app/user/js/buttons.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       84 2024-03-12 18:59:12.000000 core_explore_example_app-2.8.0/core_explore_example_app/static/core_explore_example_app/user/js/choice.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      320 2024-03-12 18:59:12.000000 core_explore_example_app-2.8.0/core_explore_example_app/static/core_explore_example_app/user/js/persistent_query.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1408 2024-03-12 18:59:12.000000 core_explore_example_app-2.8.0/core_explore_example_app/static/core_explore_example_app/user/js/refresh_sorting.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       49 2024-03-12 18:59:12.000000 core_explore_example_app-2.8.0/core_explore_example_app/static/core_explore_example_app/user/js/refresh_sorting.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1268 2024-03-12 18:59:12.000000 core_explore_example_app-2.8.0/core_explore_example_app/static/core_explore_example_app/user/js/select_fields.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      138 2024-03-12 18:59:12.000000 core_explore_example_app-2.8.0/core_explore_example_app/static/core_explore_example_app/user/js/select_fields.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:18.508433 core_explore_example_app-2.8.0/core_explore_example_app/system/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:12.000000 core_explore_example_app-2.8.0/core_explore_example_app/system/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      371 2024-03-12 18:59:12.000000 core_explore_example_app-2.8.0/core_explore_example_app/system/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1140 2024-03-12 18:59:12.000000 core_explore_example_app-2.8.0/core_explore_example_app/tasks.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:17.039364 core_explore_example_app-2.8.0/core_explore_example_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:17.051925 core_explore_example_app-2.8.0/core_explore_example_app/templates/core_explore_example_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:18.617390 core_explore_example_app-2.8.0/core_explore_example_app/templates/core_explore_example_app/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3132 2024-03-12 18:59:12.000000 core_explore_example_app-2.8.0/core_explore_example_app/templates/core_explore_example_app/user/build_query.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       32 2024-03-12 18:59:12.000000 core_explore_example_app-2.8.0/core_explore_example_app/templates/core_explore_example_app/user/errors.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1044 2024-03-12 18:59:12.000000 core_explore_example_app-2.8.0/core_explore_example_app/templates/core_explore_example_app/user/index.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:18.637492 core_explore_example_app-2.8.0/core_explore_example_app/templates/core_explore_example_app/user/list/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      429 2024-03-12 18:59:12.000000 core_explore_example_app-2.8.0/core_explore_example_app/templates/core_explore_example_app/user/list/list.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:18.727559 core_explore_example_app-2.8.0/core_explore_example_app/templates/core_explore_example_app/user/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1136 2024-03-12 18:59:12.000000 core_explore_example_app-2.8.0/core_explore_example_app/templates/core_explore_example_app/user/modals/custom_tree.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      648 2024-03-12 18:59:12.000000 core_explore_example_app-2.8.0/core_explore_example_app/templates/core_explore_example_app/user/modals/delete_all_queries.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      678 2024-03-12 18:59:12.000000 core_explore_example_app-2.8.0/core_explore_example_app/templates/core_explore_example_app/user/modals/delete_query.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      504 2024-03-12 18:59:12.000000 core_explore_example_app-2.8.0/core_explore_example_app/templates/core_explore_example_app/user/modals/errors.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      765 2024-03-12 18:59:12.000000 core_explore_example_app-2.8.0/core_explore_example_app/templates/core_explore_example_app/user/modals/sub_elements_query_builder.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:19.040310 core_explore_example_app-2.8.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       86 2024-03-12 18:59:12.000000 core_explore_example_app-2.8.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/add.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      148 2024-03-12 18:59:12.000000 core_explore_example_app-2.8.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/and_or_not.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       97 2024-03-12 18:59:12.000000 core_explore_example_app-2.8.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/criteria_select.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      121 2024-03-12 18:59:12.000000 core_explore_example_app-2.8.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/enum.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      144 2024-03-12 18:59:12.000000 core_explore_example_app-2.8.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/field_input.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       89 2024-03-12 18:59:12.000000 core_explore_example_app-2.8.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/gregorian_strict_match.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      292 2024-03-12 18:59:12.000000 core_explore_example_app-2.8.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/initial_form.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       64 2024-03-12 18:59:12.000000 core_explore_example_app-2.8.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/input.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      403 2024-03-12 18:59:12.000000 core_explore_example_app-2.8.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/new_criteria.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      749 2024-03-12 18:59:12.000000 core_explore_example_app-2.8.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/new_query.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      244 2024-03-12 18:59:12.000000 core_explore_example_app-2.8.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/numeric_select.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      103 2024-03-12 18:59:12.000000 core_explore_example_app-2.8.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/remove.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      116 2024-03-12 18:59:12.000000 core_explore_example_app-2.8.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/string_select.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      493 2024-03-12 18:59:12.000000 core_explore_example_app-2.8.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/sub_elements_query.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      107 2024-03-12 18:59:12.000000 core_explore_example_app-2.8.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/yes_no.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      749 2024-03-12 18:59:12.000000 core_explore_example_app-2.8.0/core_explore_example_app/templates/core_explore_example_app/user/results.html
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      489 2024-03-12 18:59:12.000000 core_explore_example_app-2.8.0/core_explore_example_app/templates/core_explore_example_app/user/select_fields.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3787 2024-03-12 18:59:12.000000 core_explore_example_app-2.8.0/core_explore_example_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:19.174662 core_explore_example_app-2.8.0/core_explore_example_app/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:12.000000 core_explore_example_app-2.8.0/core_explore_example_app/utils/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1775 2024-03-12 18:59:12.000000 core_explore_example_app-2.8.0/core_explore_example_app/utils/custom_checkbox_renderer.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4373 2024-03-12 18:59:12.000000 core_explore_example_app-2.8.0/core_explore_example_app/utils/displayed_query.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    15354 2024-03-12 18:59:12.000000 core_explore_example_app-2.8.0/core_explore_example_app/utils/mongo_query.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2998 2024-03-12 18:59:12.000000 core_explore_example_app-2.8.0/core_explore_example_app/utils/parser.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10108 2024-03-12 18:59:12.000000 core_explore_example_app-2.8.0/core_explore_example_app/utils/query_builder.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1899 2024-03-12 18:59:12.000000 core_explore_example_app-2.8.0/core_explore_example_app/utils/xml.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:19.193470 core_explore_example_app-2.8.0/core_explore_example_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:12.000000 core_explore_example_app-2.8.0/core_explore_example_app/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:19.218963 core_explore_example_app-2.8.0/core_explore_example_app/views/admin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:12.000000 core_explore_example_app-2.8.0/core_explore_example_app/views/admin/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:19.282894 core_explore_example_app-2.8.0/core_explore_example_app/views/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:12.000000 core_explore_example_app-2.8.0/core_explore_example_app/views/user/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    21380 2024-03-12 18:59:12.000000 core_explore_example_app-2.8.0/core_explore_example_app/views/user/ajax.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    19823 2024-03-12 18:59:12.000000 core_explore_example_app-2.8.0/core_explore_example_app/views/user/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:17.572726 core_explore_example_app-2.8.0/core_explore_example_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1114 2024-03-12 18:59:16.000000 core_explore_example_app-2.8.0/core_explore_example_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7694 2024-03-12 18:59:16.000000 core_explore_example_app-2.8.0/core_explore_example_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2024-03-12 18:59:16.000000 core_explore_example_app-2.8.0/core_explore_example_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      128 2024-03-12 18:59:16.000000 core_explore_example_app-2.8.0/core_explore_example_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       36 2024-03-12 18:59:16.000000 core_explore_example_app-2.8.0/core_explore_example_app.egg-info/top_level.txt
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:19.344808 core_explore_example_app-2.8.0/docs/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:12.000000 core_explore_example_app-2.8.0/docs/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11127 2024-03-12 18:59:12.000000 core_explore_example_app-2.8.0/docs/conf.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      311 2024-03-12 18:59:12.000000 core_explore_example_app-2.8.0/docs/conf_urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2024-03-12 18:59:13.000000 core_explore_example_app-2.8.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       75 2024-03-12 18:59:13.000000 core_explore_example_app-2.8.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2024-03-12 18:59:20.246469 core_explore_example_app-2.8.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1420 2024-03-12 18:59:13.000000 core_explore_example_app-2.8.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:19.418087 core_explore_example_app-2.8.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:13.000000 core_explore_example_app-2.8.0/tests/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:19.439426 core_explore_example_app-2.8.0/tests/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:13.000000 core_explore_example_app-2.8.0/tests/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:19.464112 core_explore_example_app-2.8.0/tests/components/data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:13.000000 core_explore_example_app-2.8.0/tests/components/data/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:19.512464 core_explore_example_app-2.8.0/tests/components/data/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:13.000000 core_explore_example_app-2.8.0/tests/components/data/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3190 2024-03-12 18:59:13.000000 core_explore_example_app-2.8.0/tests/components/data/fixtures/fixtures.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:19.559762 core_explore_example_app-2.8.0/tests/components/explore_data_structure/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:13.000000 core_explore_example_app-2.8.0/tests/components/explore_data_structure/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2970 2024-03-12 18:59:13.000000 core_explore_example_app-2.8.0/tests/components/explore_data_structure/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:19.642494 core_explore_example_app-2.8.0/tests/components/persistent_query_example/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:13.000000 core_explore_example_app-2.8.0/tests/components/persistent_query_example/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:19.693313 core_explore_example_app-2.8.0/tests/components/persistent_query_example/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:13.000000 core_explore_example_app-2.8.0/tests/components/persistent_query_example/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1899 2024-03-12 18:59:13.000000 core_explore_example_app-2.8.0/tests/components/persistent_query_example/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    15632 2024-03-12 18:59:13.000000 core_explore_example_app-2.8.0/tests/components/persistent_query_example/tests_int_access_control.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6827 2024-03-12 18:59:13.000000 core_explore_example_app-2.8.0/tests/components/persistent_query_example/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:19.741948 core_explore_example_app-2.8.0/tests/components/saved_query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:13.000000 core_explore_example_app-2.8.0/tests/components/saved_query/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3113 2024-03-12 18:59:13.000000 core_explore_example_app-2.8.0/tests/components/saved_query/tests_unit.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      132 2024-03-12 18:59:13.000000 core_explore_example_app-2.8.0/tests/mocks.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:19.771737 core_explore_example_app-2.8.0/tests/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:13.000000 core_explore_example_app-2.8.0/tests/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:19.846060 core_explore_example_app-2.8.0/tests/rest/persistent_query_example/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:13.000000 core_explore_example_app-2.8.0/tests/rest/persistent_query_example/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11760 2024-03-12 18:59:13.000000 core_explore_example_app-2.8.0/tests/rest/persistent_query_example/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    17575 2024-03-12 18:59:13.000000 core_explore_example_app-2.8.0/tests/rest/persistent_query_example/tests_permissions.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:19.913258 core_explore_example_app-2.8.0/tests/rest/saved_query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:13.000000 core_explore_example_app-2.8.0/tests/rest/saved_query/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:19.961000 core_explore_example_app-2.8.0/tests/rest/saved_query/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:13.000000 core_explore_example_app-2.8.0/tests/rest/saved_query/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1333 2024-03-12 18:59:13.000000 core_explore_example_app-2.8.0/tests/rest/saved_query/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4655 2024-03-12 18:59:13.000000 core_explore_example_app-2.8.0/tests/rest/saved_query/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5717 2024-03-12 18:59:13.000000 core_explore_example_app-2.8.0/tests/rest/saved_query/tests_permissions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1614 2024-03-12 18:59:13.000000 core_explore_example_app-2.8.0/tests/test_settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:19.983725 core_explore_example_app-2.8.0/tests/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:13.000000 core_explore_example_app-2.8.0/tests/utils/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:20.034583 core_explore_example_app-2.8.0/tests/utils/mongo_query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:13.000000 core_explore_example_app-2.8.0/tests/utils/mongo_query/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7156 2024-03-12 18:59:13.000000 core_explore_example_app-2.8.0/tests/utils/mongo_query/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:20.082826 core_explore_example_app-2.8.0/tests/utils/xml/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:13.000000 core_explore_example_app-2.8.0/tests/utils/xml/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1633 2024-03-12 18:59:13.000000 core_explore_example_app-2.8.0/tests/utils/xml/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:20.106453 core_explore_example_app-2.8.0/tests/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:13.000000 core_explore_example_app-2.8.0/tests/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:20.161513 core_explore_example_app-2.8.0/tests/views/ajax/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:13.000000 core_explore_example_app-2.8.0/tests/views/ajax/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11066 2024-03-12 18:59:13.000000 core_explore_example_app-2.8.0/tests/views/ajax/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:20.214985 core_explore_example_app-2.8.0/tests/views/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:13.000000 core_explore_example_app-2.8.0/tests/views/views/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1694 2024-03-12 18:59:13.000000 core_explore_example_app-2.8.0/tests/views/views/tests_int.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:58.737960 core_explore_example_app-2.9.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2024-05-13 16:04:43.000000 core_explore_example_app-2.9.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      156 2024-05-13 16:04:43.000000 core_explore_example_app-2.9.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1114 2024-05-13 16:04:58.730936 core_explore_example_app-2.9.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      614 2024-05-13 16:04:43.000000 core_explore_example_app-2.9.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:50.753599 core_explore_example_app-2.9.0/core_explore_example_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2024-05-13 16:04:43.000000 core_explore_example_app-2.9.0/core_explore_example_app/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1093 2024-05-13 16:04:43.000000 core_explore_example_app-2.9.0/core_explore_example_app/admin.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      634 2024-05-13 16:04:43.000000 core_explore_example_app-2.9.0/core_explore_example_app/apps.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:50.902866 core_explore_example_app-2.9.0/core_explore_example_app/commons/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:43.000000 core_explore_example_app-2.9.0/core_explore_example_app/commons/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      205 2024-05-13 16:04:43.000000 core_explore_example_app-2.9.0/core_explore_example_app/commons/exceptions.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:50.924340 core_explore_example_app-2.9.0/core_explore_example_app/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:43.000000 core_explore_example_app-2.9.0/core_explore_example_app/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:51.007839 core_explore_example_app-2.9.0/core_explore_example_app/components/explore_data_structure/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:43.000000 core_explore_example_app-2.9.0/core_explore_example_app/components/explore_data_structure/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      442 2024-05-13 16:04:43.000000 core_explore_example_app-2.9.0/core_explore_example_app/components/explore_data_structure/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2006 2024-05-13 16:04:43.000000 core_explore_example_app-2.9.0/core_explore_example_app/components/explore_data_structure/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1764 2024-05-13 16:04:43.000000 core_explore_example_app-2.9.0/core_explore_example_app/components/explore_data_structure/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:51.097851 core_explore_example_app-2.9.0/core_explore_example_app/components/persistent_query_example/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:43.000000 core_explore_example_app-2.9.0/core_explore_example_app/components/persistent_query_example/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      372 2024-05-13 16:04:43.000000 core_explore_example_app-2.9.0/core_explore_example_app/components/persistent_query_example/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2283 2024-05-13 16:04:43.000000 core_explore_example_app-2.9.0/core_explore_example_app/components/persistent_query_example/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1973 2024-05-13 16:04:43.000000 core_explore_example_app-2.9.0/core_explore_example_app/components/persistent_query_example/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:51.186154 core_explore_example_app-2.9.0/core_explore_example_app/components/saved_query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:43.000000 core_explore_example_app-2.9.0/core_explore_example_app/components/saved_query/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      356 2024-05-13 16:04:43.000000 core_explore_example_app-2.9.0/core_explore_example_app/components/saved_query/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      904 2024-05-13 16:04:43.000000 core_explore_example_app-2.9.0/core_explore_example_app/components/saved_query/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1565 2024-05-13 16:04:43.000000 core_explore_example_app-2.9.0/core_explore_example_app/components/saved_query/models.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      927 2024-05-13 16:04:43.000000 core_explore_example_app-2.9.0/core_explore_example_app/discover.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      321 2024-05-13 16:04:43.000000 core_explore_example_app-2.9.0/core_explore_example_app/menus.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:51.227596 core_explore_example_app-2.9.0/core_explore_example_app/migrations/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4401 2024-05-13 16:04:43.000000 core_explore_example_app-2.9.0/core_explore_example_app/migrations/0001_initial.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:43.000000 core_explore_example_app-2.9.0/core_explore_example_app/migrations/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1058 2024-05-13 16:04:43.000000 core_explore_example_app-2.9.0/core_explore_example_app/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:51.292508 core_explore_example_app-2.9.0/core_explore_example_app/permissions/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:43.000000 core_explore_example_app-2.9.0/core_explore_example_app/permissions/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1723 2024-05-13 16:04:43.000000 core_explore_example_app-2.9.0/core_explore_example_app/permissions/discover.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      320 2024-05-13 16:04:43.000000 core_explore_example_app-2.9.0/core_explore_example_app/permissions/rights.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:51.335911 core_explore_example_app-2.9.0/core_explore_example_app/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:43.000000 core_explore_example_app-2.9.0/core_explore_example_app/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:51.397621 core_explore_example_app-2.9.0/core_explore_example_app/rest/persistent_query_example/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:43.000000 core_explore_example_app-2.9.0/core_explore_example_app/rest/persistent_query_example/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3259 2024-05-13 16:04:43.000000 core_explore_example_app-2.9.0/core_explore_example_app/rest/persistent_query_example/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    13206 2024-05-13 16:04:43.000000 core_explore_example_app-2.9.0/core_explore_example_app/rest/persistent_query_example/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:51.578376 core_explore_example_app-2.9.0/core_explore_example_app/rest/saved_query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:43.000000 core_explore_example_app-2.9.0/core_explore_example_app/rest/saved_query/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      395 2024-05-13 16:04:43.000000 core_explore_example_app-2.9.0/core_explore_example_app/rest/saved_query/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4767 2024-05-13 16:04:43.000000 core_explore_example_app-2.9.0/core_explore_example_app/rest/saved_query/views.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1653 2024-05-13 16:04:43.000000 core_explore_example_app-2.9.0/core_explore_example_app/rest/urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      620 2024-05-13 16:04:43.000000 core_explore_example_app-2.9.0/core_explore_example_app/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:50.195340 core_explore_example_app-2.9.0/core_explore_example_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:50.200151 core_explore_example_app-2.9.0/core_explore_example_app/static/core_explore_example_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:50.211012 core_explore_example_app-2.9.0/core_explore_example_app/static/core_explore_example_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:51.637776 core_explore_example_app-2.9.0/core_explore_example_app/static/core_explore_example_app/user/css/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      724 2024-05-13 16:04:43.000000 core_explore_example_app-2.9.0/core_explore_example_app/static/core_explore_example_app/user/css/query_builder.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      465 2024-05-13 16:04:43.000000 core_explore_example_app-2.9.0/core_explore_example_app/static/core_explore_example_app/user/css/style.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      170 2024-05-13 16:04:43.000000 core_explore_example_app-2.9.0/core_explore_example_app/static/core_explore_example_app/user/css/xsd_form.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:56.638563 core_explore_example_app-2.9.0/core_explore_example_app/static/core_explore_example_app/user/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14448 2024-05-13 16:04:43.000000 core_explore_example_app-2.9.0/core_explore_example_app/static/core_explore_example_app/user/js/build_query.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1044 2024-05-13 16:04:43.000000 core_explore_example_app-2.9.0/core_explore_example_app/static/core_explore_example_app/user/js/build_query.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      147 2024-05-13 16:04:43.000000 core_explore_example_app-2.9.0/core_explore_example_app/static/core_explore_example_app/user/js/buttons.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       84 2024-05-13 16:04:43.000000 core_explore_example_app-2.9.0/core_explore_example_app/static/core_explore_example_app/user/js/choice.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      320 2024-05-13 16:04:43.000000 core_explore_example_app-2.9.0/core_explore_example_app/static/core_explore_example_app/user/js/persistent_query.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1408 2024-05-13 16:04:43.000000 core_explore_example_app-2.9.0/core_explore_example_app/static/core_explore_example_app/user/js/refresh_sorting.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       49 2024-05-13 16:04:43.000000 core_explore_example_app-2.9.0/core_explore_example_app/static/core_explore_example_app/user/js/refresh_sorting.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1268 2024-05-13 16:04:43.000000 core_explore_example_app-2.9.0/core_explore_example_app/static/core_explore_example_app/user/js/select_fields.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      138 2024-05-13 16:04:43.000000 core_explore_example_app-2.9.0/core_explore_example_app/static/core_explore_example_app/user/js/select_fields.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:56.682638 core_explore_example_app-2.9.0/core_explore_example_app/system/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:43.000000 core_explore_example_app-2.9.0/core_explore_example_app/system/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      371 2024-05-13 16:04:43.000000 core_explore_example_app-2.9.0/core_explore_example_app/system/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1140 2024-05-13 16:04:43.000000 core_explore_example_app-2.9.0/core_explore_example_app/tasks.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:50.236641 core_explore_example_app-2.9.0/core_explore_example_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:50.247266 core_explore_example_app-2.9.0/core_explore_example_app/templates/core_explore_example_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:56.881187 core_explore_example_app-2.9.0/core_explore_example_app/templates/core_explore_example_app/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3132 2024-05-13 16:04:43.000000 core_explore_example_app-2.9.0/core_explore_example_app/templates/core_explore_example_app/user/build_query.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       32 2024-05-13 16:04:43.000000 core_explore_example_app-2.9.0/core_explore_example_app/templates/core_explore_example_app/user/errors.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1044 2024-05-13 16:04:43.000000 core_explore_example_app-2.9.0/core_explore_example_app/templates/core_explore_example_app/user/index.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:56.900869 core_explore_example_app-2.9.0/core_explore_example_app/templates/core_explore_example_app/user/list/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      429 2024-05-13 16:04:43.000000 core_explore_example_app-2.9.0/core_explore_example_app/templates/core_explore_example_app/user/list/list.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:57.030661 core_explore_example_app-2.9.0/core_explore_example_app/templates/core_explore_example_app/user/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1136 2024-05-13 16:04:43.000000 core_explore_example_app-2.9.0/core_explore_example_app/templates/core_explore_example_app/user/modals/custom_tree.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      648 2024-05-13 16:04:43.000000 core_explore_example_app-2.9.0/core_explore_example_app/templates/core_explore_example_app/user/modals/delete_all_queries.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      678 2024-05-13 16:04:43.000000 core_explore_example_app-2.9.0/core_explore_example_app/templates/core_explore_example_app/user/modals/delete_query.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      504 2024-05-13 16:04:44.000000 core_explore_example_app-2.9.0/core_explore_example_app/templates/core_explore_example_app/user/modals/errors.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      765 2024-05-13 16:04:44.000000 core_explore_example_app-2.9.0/core_explore_example_app/templates/core_explore_example_app/user/modals/sub_elements_query_builder.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:57.504554 core_explore_example_app-2.9.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       86 2024-05-13 16:04:44.000000 core_explore_example_app-2.9.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/add.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      148 2024-05-13 16:04:44.000000 core_explore_example_app-2.9.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/and_or_not.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       97 2024-05-13 16:04:44.000000 core_explore_example_app-2.9.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/criteria_select.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      121 2024-05-13 16:04:44.000000 core_explore_example_app-2.9.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/enum.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      144 2024-05-13 16:04:44.000000 core_explore_example_app-2.9.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/field_input.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       89 2024-05-13 16:04:44.000000 core_explore_example_app-2.9.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/gregorian_strict_match.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      292 2024-05-13 16:04:44.000000 core_explore_example_app-2.9.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/initial_form.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       64 2024-05-13 16:04:44.000000 core_explore_example_app-2.9.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/input.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      403 2024-05-13 16:04:44.000000 core_explore_example_app-2.9.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/new_criteria.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      749 2024-05-13 16:04:44.000000 core_explore_example_app-2.9.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/new_query.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      244 2024-05-13 16:04:44.000000 core_explore_example_app-2.9.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/numeric_select.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      103 2024-05-13 16:04:44.000000 core_explore_example_app-2.9.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/remove.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      116 2024-05-13 16:04:44.000000 core_explore_example_app-2.9.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/string_select.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      493 2024-05-13 16:04:44.000000 core_explore_example_app-2.9.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/sub_elements_query.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      107 2024-05-13 16:04:44.000000 core_explore_example_app-2.9.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/yes_no.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      749 2024-05-13 16:04:44.000000 core_explore_example_app-2.9.0/core_explore_example_app/templates/core_explore_example_app/user/results.html
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      489 2024-05-13 16:04:44.000000 core_explore_example_app-2.9.0/core_explore_example_app/templates/core_explore_example_app/user/select_fields.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3787 2024-05-13 16:04:44.000000 core_explore_example_app-2.9.0/core_explore_example_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:57.657521 core_explore_example_app-2.9.0/core_explore_example_app/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:44.000000 core_explore_example_app-2.9.0/core_explore_example_app/utils/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1775 2024-05-13 16:04:44.000000 core_explore_example_app-2.9.0/core_explore_example_app/utils/custom_checkbox_renderer.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4373 2024-05-13 16:04:44.000000 core_explore_example_app-2.9.0/core_explore_example_app/utils/displayed_query.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    15354 2024-05-13 16:04:44.000000 core_explore_example_app-2.9.0/core_explore_example_app/utils/mongo_query.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2998 2024-05-13 16:04:44.000000 core_explore_example_app-2.9.0/core_explore_example_app/utils/parser.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10108 2024-05-13 16:04:44.000000 core_explore_example_app-2.9.0/core_explore_example_app/utils/query_builder.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1899 2024-05-13 16:04:44.000000 core_explore_example_app-2.9.0/core_explore_example_app/utils/xml.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:57.678799 core_explore_example_app-2.9.0/core_explore_example_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:44.000000 core_explore_example_app-2.9.0/core_explore_example_app/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:57.707076 core_explore_example_app-2.9.0/core_explore_example_app/views/admin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:44.000000 core_explore_example_app-2.9.0/core_explore_example_app/views/admin/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:57.776855 core_explore_example_app-2.9.0/core_explore_example_app/views/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:44.000000 core_explore_example_app-2.9.0/core_explore_example_app/views/user/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    21380 2024-05-13 16:04:44.000000 core_explore_example_app-2.9.0/core_explore_example_app/views/user/ajax.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    19823 2024-05-13 16:04:44.000000 core_explore_example_app-2.9.0/core_explore_example_app/views/user/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:50.861006 core_explore_example_app-2.9.0/core_explore_example_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1114 2024-05-13 16:04:49.000000 core_explore_example_app-2.9.0/core_explore_example_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7694 2024-05-13 16:04:49.000000 core_explore_example_app-2.9.0/core_explore_example_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2024-05-13 16:04:49.000000 core_explore_example_app-2.9.0/core_explore_example_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      128 2024-05-13 16:04:49.000000 core_explore_example_app-2.9.0/core_explore_example_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       36 2024-05-13 16:04:49.000000 core_explore_example_app-2.9.0/core_explore_example_app.egg-info/top_level.txt
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:57.844946 core_explore_example_app-2.9.0/docs/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:44.000000 core_explore_example_app-2.9.0/docs/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11127 2024-05-13 16:04:44.000000 core_explore_example_app-2.9.0/docs/conf.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      311 2024-05-13 16:04:44.000000 core_explore_example_app-2.9.0/docs/conf_urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2024-05-13 16:04:45.000000 core_explore_example_app-2.9.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       75 2024-05-13 16:04:45.000000 core_explore_example_app-2.9.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2024-05-13 16:04:58.740514 core_explore_example_app-2.9.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1420 2024-05-13 16:04:45.000000 core_explore_example_app-2.9.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:57.909808 core_explore_example_app-2.9.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:45.000000 core_explore_example_app-2.9.0/tests/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:57.931270 core_explore_example_app-2.9.0/tests/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:45.000000 core_explore_example_app-2.9.0/tests/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:57.958201 core_explore_example_app-2.9.0/tests/components/data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:45.000000 core_explore_example_app-2.9.0/tests/components/data/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:58.011508 core_explore_example_app-2.9.0/tests/components/data/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:45.000000 core_explore_example_app-2.9.0/tests/components/data/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3190 2024-05-13 16:04:45.000000 core_explore_example_app-2.9.0/tests/components/data/fixtures/fixtures.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:58.058744 core_explore_example_app-2.9.0/tests/components/explore_data_structure/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:45.000000 core_explore_example_app-2.9.0/tests/components/explore_data_structure/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2970 2024-05-13 16:04:46.000000 core_explore_example_app-2.9.0/tests/components/explore_data_structure/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:58.121101 core_explore_example_app-2.9.0/tests/components/persistent_query_example/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:46.000000 core_explore_example_app-2.9.0/tests/components/persistent_query_example/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:58.177426 core_explore_example_app-2.9.0/tests/components/persistent_query_example/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:46.000000 core_explore_example_app-2.9.0/tests/components/persistent_query_example/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1899 2024-05-13 16:04:46.000000 core_explore_example_app-2.9.0/tests/components/persistent_query_example/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    15632 2024-05-13 16:04:46.000000 core_explore_example_app-2.9.0/tests/components/persistent_query_example/tests_int_access_control.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6827 2024-05-13 16:04:46.000000 core_explore_example_app-2.9.0/tests/components/persistent_query_example/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:58.224683 core_explore_example_app-2.9.0/tests/components/saved_query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:46.000000 core_explore_example_app-2.9.0/tests/components/saved_query/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3113 2024-05-13 16:04:46.000000 core_explore_example_app-2.9.0/tests/components/saved_query/tests_unit.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      132 2024-05-13 16:04:46.000000 core_explore_example_app-2.9.0/tests/mocks.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:58.246798 core_explore_example_app-2.9.0/tests/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:46.000000 core_explore_example_app-2.9.0/tests/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:58.324427 core_explore_example_app-2.9.0/tests/rest/persistent_query_example/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:46.000000 core_explore_example_app-2.9.0/tests/rest/persistent_query_example/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11760 2024-05-13 16:04:46.000000 core_explore_example_app-2.9.0/tests/rest/persistent_query_example/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    17575 2024-05-13 16:04:46.000000 core_explore_example_app-2.9.0/tests/rest/persistent_query_example/tests_permissions.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:58.388588 core_explore_example_app-2.9.0/tests/rest/saved_query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:46.000000 core_explore_example_app-2.9.0/tests/rest/saved_query/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:58.439486 core_explore_example_app-2.9.0/tests/rest/saved_query/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:47.000000 core_explore_example_app-2.9.0/tests/rest/saved_query/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1333 2024-05-13 16:04:47.000000 core_explore_example_app-2.9.0/tests/rest/saved_query/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4655 2024-05-13 16:04:47.000000 core_explore_example_app-2.9.0/tests/rest/saved_query/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5717 2024-05-13 16:04:47.000000 core_explore_example_app-2.9.0/tests/rest/saved_query/tests_permissions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1614 2024-05-13 16:04:47.000000 core_explore_example_app-2.9.0/tests/test_settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:58.461729 core_explore_example_app-2.9.0/tests/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:47.000000 core_explore_example_app-2.9.0/tests/utils/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:58.510273 core_explore_example_app-2.9.0/tests/utils/mongo_query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:47.000000 core_explore_example_app-2.9.0/tests/utils/mongo_query/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7156 2024-05-13 16:04:47.000000 core_explore_example_app-2.9.0/tests/utils/mongo_query/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:58.572977 core_explore_example_app-2.9.0/tests/utils/xml/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:47.000000 core_explore_example_app-2.9.0/tests/utils/xml/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1633 2024-05-13 16:04:47.000000 core_explore_example_app-2.9.0/tests/utils/xml/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:58.594471 core_explore_example_app-2.9.0/tests/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:47.000000 core_explore_example_app-2.9.0/tests/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:58.654039 core_explore_example_app-2.9.0/tests/views/ajax/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:47.000000 core_explore_example_app-2.9.0/tests/views/ajax/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11066 2024-05-13 16:04:47.000000 core_explore_example_app-2.9.0/tests/views/ajax/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:58.700404 core_explore_example_app-2.9.0/tests/views/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:47.000000 core_explore_example_app-2.9.0/tests/views/views/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1694 2024-05-13 16:04:47.000000 core_explore_example_app-2.9.0/tests/views/views/tests_int.py
```

### Comparing `core_explore_example_app-2.8.0/LICENSE.md` & `core_explore_example_app-2.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.8.0/PKG-INFO` & `core_explore_example_app-2.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_explore_example_app
-Version: 2.8.0
+Version: 2.9.0
 Summary: Exploration by example for the curator core project
 Home-page: https://github.com/usnistgov/core_explore_example_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: ========================
         Core Explore Example App
```

### Comparing `core_explore_example_app-2.8.0/README.rst` & `core_explore_example_app-2.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.8.0/core_explore_example_app/admin.py` & `core_explore_example_app-2.9.0/core_explore_example_app/admin.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.8.0/core_explore_example_app/apps.py` & `core_explore_example_app-2.9.0/core_explore_example_app/apps.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.8.0/core_explore_example_app/components/explore_data_structure/api.py` & `core_explore_example_app-2.9.0/core_explore_example_app/components/explore_data_structure/api.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.8.0/core_explore_example_app/components/explore_data_structure/models.py` & `core_explore_example_app-2.9.0/core_explore_example_app/components/explore_data_structure/models.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.8.0/core_explore_example_app/components/persistent_query_example/api.py` & `core_explore_example_app-2.9.0/core_explore_example_app/components/persistent_query_example/api.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.8.0/core_explore_example_app/components/persistent_query_example/models.py` & `core_explore_example_app-2.9.0/core_explore_example_app/components/persistent_query_example/models.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.8.0/core_explore_example_app/components/saved_query/api.py` & `core_explore_example_app-2.9.0/core_explore_example_app/components/saved_query/api.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.8.0/core_explore_example_app/components/saved_query/models.py` & `core_explore_example_app-2.9.0/core_explore_example_app/components/saved_query/models.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.8.0/core_explore_example_app/discover.py` & `core_explore_example_app-2.9.0/core_explore_example_app/discover.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.8.0/core_explore_example_app/migrations/0001_initial.py` & `core_explore_example_app-2.9.0/core_explore_example_app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.8.0/core_explore_example_app/models.py` & `core_explore_example_app-2.9.0/core_explore_example_app/models.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.8.0/core_explore_example_app/permissions/discover.py` & `core_explore_example_app-2.9.0/core_explore_example_app/permissions/discover.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.8.0/core_explore_example_app/rest/persistent_query_example/serializers.py` & `core_explore_example_app-2.9.0/core_explore_example_app/rest/persistent_query_example/serializers.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.8.0/core_explore_example_app/rest/persistent_query_example/views.py` & `core_explore_example_app-2.9.0/core_explore_example_app/rest/persistent_query_example/views.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.8.0/core_explore_example_app/rest/saved_query/views.py` & `core_explore_example_app-2.9.0/core_explore_example_app/rest/saved_query/views.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.8.0/core_explore_example_app/rest/urls.py` & `core_explore_example_app-2.9.0/core_explore_example_app/rest/urls.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.8.0/core_explore_example_app/settings.py` & `core_explore_example_app-2.9.0/core_explore_example_app/settings.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.8.0/core_explore_example_app/static/core_explore_example_app/user/css/query_builder.css` & `core_explore_example_app-2.9.0/core_explore_example_app/static/core_explore_example_app/user/css/query_builder.css`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.8.0/core_explore_example_app/static/core_explore_example_app/user/js/build_query.js` & `core_explore_example_app-2.9.0/core_explore_example_app/static/core_explore_example_app/user/js/build_query.js`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.8.0/core_explore_example_app/static/core_explore_example_app/user/js/build_query.raw.js` & `core_explore_example_app-2.9.0/core_explore_example_app/static/core_explore_example_app/user/js/build_query.raw.js`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.8.0/core_explore_example_app/static/core_explore_example_app/user/js/refresh_sorting.js` & `core_explore_example_app-2.9.0/core_explore_example_app/static/core_explore_example_app/user/js/refresh_sorting.js`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.8.0/core_explore_example_app/static/core_explore_example_app/user/js/select_fields.js` & `core_explore_example_app-2.9.0/core_explore_example_app/static/core_explore_example_app/user/js/select_fields.js`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.8.0/core_explore_example_app/tasks.py` & `core_explore_example_app-2.9.0/core_explore_example_app/tasks.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.8.0/core_explore_example_app/templates/core_explore_example_app/user/build_query.html` & `core_explore_example_app-2.9.0/core_explore_example_app/templates/core_explore_example_app/user/build_query.html`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.8.0/core_explore_example_app/templates/core_explore_example_app/user/index.html` & `core_explore_example_app-2.9.0/core_explore_example_app/templates/core_explore_example_app/user/index.html`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.8.0/core_explore_example_app/templates/core_explore_example_app/user/modals/custom_tree.html` & `core_explore_example_app-2.9.0/core_explore_example_app/templates/core_explore_example_app/user/modals/custom_tree.html`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.8.0/core_explore_example_app/templates/core_explore_example_app/user/modals/delete_all_queries.html` & `core_explore_example_app-2.9.0/core_explore_example_app/templates/core_explore_example_app/user/modals/delete_all_queries.html`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.8.0/core_explore_example_app/templates/core_explore_example_app/user/modals/delete_query.html` & `core_explore_example_app-2.9.0/core_explore_example_app/templates/core_explore_example_app/user/modals/delete_query.html`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.8.0/core_explore_example_app/templates/core_explore_example_app/user/modals/sub_elements_query_builder.html` & `core_explore_example_app-2.9.0/core_explore_example_app/templates/core_explore_example_app/user/modals/sub_elements_query_builder.html`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.8.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/new_query.html` & `core_explore_example_app-2.9.0/core_explore_example_app/templates/core_explore_example_app/user/query_builder/new_query.html`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.8.0/core_explore_example_app/templates/core_explore_example_app/user/results.html` & `core_explore_example_app-2.9.0/core_explore_example_app/templates/core_explore_example_app/user/results.html`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.8.0/core_explore_example_app/urls.py` & `core_explore_example_app-2.9.0/core_explore_example_app/urls.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.8.0/core_explore_example_app/utils/custom_checkbox_renderer.py` & `core_explore_example_app-2.9.0/core_explore_example_app/utils/custom_checkbox_renderer.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.8.0/core_explore_example_app/utils/displayed_query.py` & `core_explore_example_app-2.9.0/core_explore_example_app/utils/displayed_query.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.8.0/core_explore_example_app/utils/mongo_query.py` & `core_explore_example_app-2.9.0/core_explore_example_app/utils/mongo_query.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.8.0/core_explore_example_app/utils/parser.py` & `core_explore_example_app-2.9.0/core_explore_example_app/utils/parser.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.8.0/core_explore_example_app/utils/query_builder.py` & `core_explore_example_app-2.9.0/core_explore_example_app/utils/query_builder.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.8.0/core_explore_example_app/utils/xml.py` & `core_explore_example_app-2.9.0/core_explore_example_app/utils/xml.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.8.0/core_explore_example_app/views/user/ajax.py` & `core_explore_example_app-2.9.0/core_explore_example_app/views/user/ajax.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.8.0/core_explore_example_app/views/user/views.py` & `core_explore_example_app-2.9.0/core_explore_example_app/views/user/views.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.8.0/core_explore_example_app.egg-info/PKG-INFO` & `core_explore_example_app-2.9.0/core_explore_example_app.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-explore-example-app
-Version: 2.8.0
+Version: 2.9.0
 Summary: Exploration by example for the curator core project
 Home-page: https://github.com/usnistgov/core_explore_example_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: ========================
         Core Explore Example App
```

### Comparing `core_explore_example_app-2.8.0/core_explore_example_app.egg-info/SOURCES.txt` & `core_explore_example_app-2.9.0/core_explore_example_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.8.0/docs/conf.py` & `core_explore_example_app-2.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.8.0/setup.py` & `core_explore_example_app-2.9.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_explore_example_app",
-    version="2.8.0",
+    version="2.9.0",
     description="Exploration by example for the curator core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_explore_example_app",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `core_explore_example_app-2.8.0/tests/components/data/fixtures/fixtures.py` & `core_explore_example_app-2.9.0/tests/components/data/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.8.0/tests/components/explore_data_structure/tests_unit.py` & `core_explore_example_app-2.9.0/tests/components/explore_data_structure/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.8.0/tests/components/persistent_query_example/fixtures/fixtures.py` & `core_explore_example_app-2.9.0/tests/components/persistent_query_example/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.8.0/tests/components/persistent_query_example/tests_int_access_control.py` & `core_explore_example_app-2.9.0/tests/components/persistent_query_example/tests_int_access_control.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.8.0/tests/components/persistent_query_example/tests_unit.py` & `core_explore_example_app-2.9.0/tests/components/persistent_query_example/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.8.0/tests/components/saved_query/tests_unit.py` & `core_explore_example_app-2.9.0/tests/components/saved_query/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.8.0/tests/rest/persistent_query_example/tests_int.py` & `core_explore_example_app-2.9.0/tests/rest/persistent_query_example/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.8.0/tests/rest/persistent_query_example/tests_permissions.py` & `core_explore_example_app-2.9.0/tests/rest/persistent_query_example/tests_permissions.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.8.0/tests/rest/saved_query/fixtures/fixtures.py` & `core_explore_example_app-2.9.0/tests/rest/saved_query/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.8.0/tests/rest/saved_query/tests_int.py` & `core_explore_example_app-2.9.0/tests/rest/saved_query/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.8.0/tests/rest/saved_query/tests_permissions.py` & `core_explore_example_app-2.9.0/tests/rest/saved_query/tests_permissions.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.8.0/tests/test_settings.py` & `core_explore_example_app-2.9.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.8.0/tests/utils/mongo_query/tests_unit.py` & `core_explore_example_app-2.9.0/tests/utils/mongo_query/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.8.0/tests/utils/xml/tests_unit.py` & `core_explore_example_app-2.9.0/tests/utils/xml/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.8.0/tests/views/ajax/tests_unit.py` & `core_explore_example_app-2.9.0/tests/views/ajax/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_explore_example_app-2.8.0/tests/views/views/tests_int.py` & `core_explore_example_app-2.9.0/tests/views/views/tests_int.py`

 * *Files identical despite different names*

