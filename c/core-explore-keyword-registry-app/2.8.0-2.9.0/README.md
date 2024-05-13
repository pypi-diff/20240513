# Comparing `tmp/core_explore_keyword_registry_app-2.8.0.tar.gz` & `tmp/core_explore_keyword_registry_app-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_explore_keyword_registry_app-2.8.0.tar", last modified: Tue Mar 12 19:00:07 2024, max compression
+gzip compressed data, was "core_explore_keyword_registry_app-2.9.0.tar", last modified: Mon May 13 16:05:47 2024, max compression
```

## Comparing `core_explore_keyword_registry_app-2.8.0.tar` & `core_explore_keyword_registry_app-2.9.0.tar`

### file list

```diff
@@ -1,80 +1,76 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:07.321414 core_explore_keyword_registry_app-2.8.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2024-03-12 19:00:03.000000 core_explore_keyword_registry_app-2.8.0/LICENSE.md
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      199 2024-03-12 19:00:03.000000 core_explore_keyword_registry_app-2.8.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1581 2024-03-12 19:00:07.315225 core_explore_keyword_registry_app-2.8.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1042 2024-03-12 19:00:03.000000 core_explore_keyword_registry_app-2.8.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:06.486532 core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      120 2024-03-12 19:00:03.000000 core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      710 2024-03-12 19:00:03.000000 core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app/apps.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3508 2024-03-12 19:00:03.000000 core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app/discover.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:06.629764 core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app/permissions/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:03.000000 core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app/permissions/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1063 2024-03-12 19:00:03.000000 core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app/permissions/discover.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      883 2024-03-12 19:00:03.000000 core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:06.110090 core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:06.167700 core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:06.153315 core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:06.131198 core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/css/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:06.679507 core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/css/fancytree/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      861 2024-03-12 19:00:03.000000 core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/css/fancytree/fancytree.custom.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:06.719824 core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/css/search/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      310 2024-03-12 19:00:03.000000 core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/css/search/filters.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1016 2024-03-12 19:00:03.000000 core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/css/search/search.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:06.143519 core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:06.869289 core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/search/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3328 2024-03-12 19:00:03.000000 core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/search/fancytree.custom.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       76 2024-03-12 19:00:03.000000 core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/search/fancytree.custom.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2544 2024-03-12 19:00:03.000000 core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/search/filters.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9169 2024-03-12 19:00:03.000000 core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/search/resource_type_icons_table.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      257 2024-03-12 19:00:03.000000 core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/search/resource_type_icons_table.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      322 2024-03-12 19:00:03.000000 core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/search/search.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      650 2024-03-12 19:00:03.000000 core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/search/tagit.custom.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:06.157549 core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/libs/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:06.161945 core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/libs/jquery-shorten/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:06.899105 core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/libs/jquery-shorten/1.1.0/
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     6230 2024-03-12 19:00:03.000000 core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/libs/jquery-shorten/1.1.0/jquery.shorten.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:06.938093 core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/xsl/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6861 2024-03-12 19:00:03.000000 core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/xsl/registry-detail.xsl
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4230 2024-03-12 19:00:03.000000 core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/xsl/registry-list.xsl
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:06.213238 core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:06.188519 core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app/templates/core_explore_common_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:06.192820 core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app/templates/core_explore_common_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:06.983759 core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app/templates/core_explore_common_app/user/results/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1483 2024-03-12 19:00:03.000000 core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app/templates/core_explore_common_app/user/results/data_source_info.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1209 2024-03-12 19:00:03.000000 core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app/templates/core_explore_common_app/user/results/data_source_results.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:06.205285 core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app/templates/core_explore_keyword_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:07.007184 core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app/templates/core_explore_keyword_app/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1870 2024-03-12 19:00:03.000000 core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app/templates/core_explore_keyword_app/user/index.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:06.217403 core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app/templates/core_explore_keyword_registry_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:07.034490 core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app/templates/core_explore_keyword_registry_app/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1063 2024-03-12 19:00:03.000000 core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app/templates/core_explore_keyword_registry_app/user/refinements.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:07.087994 core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app/templatetags/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:03.000000 core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app/templatetags/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1016 2024-03-12 19:00:03.000000 core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app/templatetags/render_extras.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1446 2024-03-12 19:00:03.000000 core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:07.111879 core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:03.000000 core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:07.193286 core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app/views/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:03.000000 core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app/views/user/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    13271 2024-03-12 19:00:03.000000 core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app/views/user/ajax.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1475 2024-03-12 19:00:03.000000 core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app/views/user/forms.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    12762 2024-03-12 19:00:03.000000 core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app/views/user/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:06.584132 core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1581 2024-03-12 19:00:05.000000 core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3044 2024-03-12 19:00:05.000000 core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2024-03-12 19:00:05.000000 core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       88 2024-03-12 19:00:05.000000 core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       40 2024-03-12 19:00:05.000000 core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app.egg-info/top_level.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2024-03-12 19:00:03.000000 core_explore_keyword_registry_app-2.8.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       62 2024-03-12 19:00:03.000000 core_explore_keyword_registry_app-2.8.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       26 2024-03-12 19:00:03.000000 core_explore_keyword_registry_app-2.8.0/requirements.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2024-03-12 19:00:07.323720 core_explore_keyword_registry_app-2.8.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1090 2024-03-12 19:00:03.000000 core_explore_keyword_registry_app-2.8.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:07.231424 core_explore_keyword_registry_app-2.8.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:03.000000 core_explore_keyword_registry_app-2.8.0/tests/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1793 2024-03-12 19:00:03.000000 core_explore_keyword_registry_app-2.8.0/tests/test_settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:07.251331 core_explore_keyword_registry_app-2.8.0/tests/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:04.000000 core_explore_keyword_registry_app-2.8.0/tests/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:07.296447 core_explore_keyword_registry_app-2.8.0/tests/views/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:04.000000 core_explore_keyword_registry_app-2.8.0/tests/views/user/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5842 2024-03-12 19:00:04.000000 core_explore_keyword_registry_app-2.8.0/tests/views/user/tests_views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:47.594123 core_explore_keyword_registry_app-2.9.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2024-05-13 16:05:43.000000 core_explore_keyword_registry_app-2.9.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      199 2024-05-13 16:05:43.000000 core_explore_keyword_registry_app-2.9.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1581 2024-05-13 16:05:47.588082 core_explore_keyword_registry_app-2.9.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1042 2024-05-13 16:05:43.000000 core_explore_keyword_registry_app-2.9.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:46.737352 core_explore_keyword_registry_app-2.9.0/core_explore_keyword_registry_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      120 2024-05-13 16:05:43.000000 core_explore_keyword_registry_app-2.9.0/core_explore_keyword_registry_app/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      554 2024-05-13 16:05:43.000000 core_explore_keyword_registry_app-2.9.0/core_explore_keyword_registry_app/apps.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:46.902775 core_explore_keyword_registry_app-2.9.0/core_explore_keyword_registry_app/permissions/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:43.000000 core_explore_keyword_registry_app-2.9.0/core_explore_keyword_registry_app/permissions/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1063 2024-05-13 16:05:43.000000 core_explore_keyword_registry_app-2.9.0/core_explore_keyword_registry_app/permissions/discover.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      286 2024-05-13 16:05:43.000000 core_explore_keyword_registry_app-2.9.0/core_explore_keyword_registry_app/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:46.277485 core_explore_keyword_registry_app-2.9.0/core_explore_keyword_registry_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:46.282245 core_explore_keyword_registry_app-2.9.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:46.363227 core_explore_keyword_registry_app-2.9.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:46.300075 core_explore_keyword_registry_app-2.9.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/css/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:46.931689 core_explore_keyword_registry_app-2.9.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/css/fancytree/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      861 2024-05-13 16:05:43.000000 core_explore_keyword_registry_app-2.9.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/css/fancytree/fancytree.custom.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:46.983136 core_explore_keyword_registry_app-2.9.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/css/search/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      310 2024-05-13 16:05:43.000000 core_explore_keyword_registry_app-2.9.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/css/search/filters.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1016 2024-05-13 16:05:43.000000 core_explore_keyword_registry_app-2.9.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/css/search/search.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:46.345082 core_explore_keyword_registry_app-2.9.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:47.124093 core_explore_keyword_registry_app-2.9.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/search/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3328 2024-05-13 16:05:43.000000 core_explore_keyword_registry_app-2.9.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/search/fancytree.custom.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       76 2024-05-13 16:05:43.000000 core_explore_keyword_registry_app-2.9.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/search/fancytree.custom.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2544 2024-05-13 16:05:43.000000 core_explore_keyword_registry_app-2.9.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/search/filters.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9169 2024-05-13 16:05:43.000000 core_explore_keyword_registry_app-2.9.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/search/resource_type_icons_table.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      257 2024-05-13 16:05:44.000000 core_explore_keyword_registry_app-2.9.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/search/resource_type_icons_table.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      322 2024-05-13 16:05:44.000000 core_explore_keyword_registry_app-2.9.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/search/search.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      650 2024-05-13 16:05:44.000000 core_explore_keyword_registry_app-2.9.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/search/tagit.custom.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:46.368007 core_explore_keyword_registry_app-2.9.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/libs/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:46.379462 core_explore_keyword_registry_app-2.9.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/libs/jquery-shorten/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:47.150145 core_explore_keyword_registry_app-2.9.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/libs/jquery-shorten/1.1.0/
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     6230 2024-05-13 16:05:44.000000 core_explore_keyword_registry_app-2.9.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/libs/jquery-shorten/1.1.0/jquery.shorten.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:46.433407 core_explore_keyword_registry_app-2.9.0/core_explore_keyword_registry_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:46.400600 core_explore_keyword_registry_app-2.9.0/core_explore_keyword_registry_app/templates/core_explore_common_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:46.405243 core_explore_keyword_registry_app-2.9.0/core_explore_keyword_registry_app/templates/core_explore_common_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:47.195532 core_explore_keyword_registry_app-2.9.0/core_explore_keyword_registry_app/templates/core_explore_common_app/user/results/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1483 2024-05-13 16:05:44.000000 core_explore_keyword_registry_app-2.9.0/core_explore_keyword_registry_app/templates/core_explore_common_app/user/results/data_source_info.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1209 2024-05-13 16:05:44.000000 core_explore_keyword_registry_app-2.9.0/core_explore_keyword_registry_app/templates/core_explore_common_app/user/results/data_source_results.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:46.425092 core_explore_keyword_registry_app-2.9.0/core_explore_keyword_registry_app/templates/core_explore_keyword_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:47.217521 core_explore_keyword_registry_app-2.9.0/core_explore_keyword_registry_app/templates/core_explore_keyword_app/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1870 2024-05-13 16:05:44.000000 core_explore_keyword_registry_app-2.9.0/core_explore_keyword_registry_app/templates/core_explore_keyword_app/user/index.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:46.438091 core_explore_keyword_registry_app-2.9.0/core_explore_keyword_registry_app/templates/core_explore_keyword_registry_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:47.247923 core_explore_keyword_registry_app-2.9.0/core_explore_keyword_registry_app/templates/core_explore_keyword_registry_app/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1063 2024-05-13 16:05:44.000000 core_explore_keyword_registry_app-2.9.0/core_explore_keyword_registry_app/templates/core_explore_keyword_registry_app/user/refinements.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:47.288939 core_explore_keyword_registry_app-2.9.0/core_explore_keyword_registry_app/templatetags/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:44.000000 core_explore_keyword_registry_app-2.9.0/core_explore_keyword_registry_app/templatetags/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1016 2024-05-13 16:05:44.000000 core_explore_keyword_registry_app-2.9.0/core_explore_keyword_registry_app/templatetags/render_extras.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1446 2024-05-13 16:05:44.000000 core_explore_keyword_registry_app-2.9.0/core_explore_keyword_registry_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:47.346508 core_explore_keyword_registry_app-2.9.0/core_explore_keyword_registry_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:44.000000 core_explore_keyword_registry_app-2.9.0/core_explore_keyword_registry_app/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:47.444643 core_explore_keyword_registry_app-2.9.0/core_explore_keyword_registry_app/views/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:44.000000 core_explore_keyword_registry_app-2.9.0/core_explore_keyword_registry_app/views/user/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    13271 2024-05-13 16:05:44.000000 core_explore_keyword_registry_app-2.9.0/core_explore_keyword_registry_app/views/user/ajax.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1475 2024-05-13 16:05:44.000000 core_explore_keyword_registry_app-2.9.0/core_explore_keyword_registry_app/views/user/forms.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    12762 2024-05-13 16:05:44.000000 core_explore_keyword_registry_app-2.9.0/core_explore_keyword_registry_app/views/user/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:46.846285 core_explore_keyword_registry_app-2.9.0/core_explore_keyword_registry_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1581 2024-05-13 16:05:45.000000 core_explore_keyword_registry_app-2.9.0/core_explore_keyword_registry_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2802 2024-05-13 16:05:46.000000 core_explore_keyword_registry_app-2.9.0/core_explore_keyword_registry_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2024-05-13 16:05:45.000000 core_explore_keyword_registry_app-2.9.0/core_explore_keyword_registry_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       88 2024-05-13 16:05:45.000000 core_explore_keyword_registry_app-2.9.0/core_explore_keyword_registry_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       40 2024-05-13 16:05:45.000000 core_explore_keyword_registry_app-2.9.0/core_explore_keyword_registry_app.egg-info/top_level.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2024-05-13 16:05:44.000000 core_explore_keyword_registry_app-2.9.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       62 2024-05-13 16:05:44.000000 core_explore_keyword_registry_app-2.9.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       26 2024-05-13 16:05:44.000000 core_explore_keyword_registry_app-2.9.0/requirements.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2024-05-13 16:05:47.596367 core_explore_keyword_registry_app-2.9.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1090 2024-05-13 16:05:44.000000 core_explore_keyword_registry_app-2.9.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:47.486556 core_explore_keyword_registry_app-2.9.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:44.000000 core_explore_keyword_registry_app-2.9.0/tests/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1793 2024-05-13 16:05:44.000000 core_explore_keyword_registry_app-2.9.0/tests/test_settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:47.507044 core_explore_keyword_registry_app-2.9.0/tests/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:44.000000 core_explore_keyword_registry_app-2.9.0/tests/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:47.573264 core_explore_keyword_registry_app-2.9.0/tests/views/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:44.000000 core_explore_keyword_registry_app-2.9.0/tests/views/user/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5842 2024-05-13 16:05:44.000000 core_explore_keyword_registry_app-2.9.0/tests/views/user/tests_views.py
```

### Comparing `core_explore_keyword_registry_app-2.8.0/LICENSE.md` & `core_explore_keyword_registry_app-2.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_registry_app-2.8.0/PKG-INFO` & `core_explore_keyword_registry_app-2.9.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_explore_keyword_registry_app
-Version: 2.8.0
+Version: 2.9.0
 Summary: Exploration by keywords for the registry project
 Home-page: https://github.com/usnistgov/core_explore_keyword_registry_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: =================================
         Core Explore Keyword Registry App
```

### Comparing `core_explore_keyword_registry_app-2.8.0/README.rst` & `core_explore_keyword_registry_app-2.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app/apps.py` & `core_explore_keyword_registry_app-2.9.0/core_explore_keyword_registry_app/apps.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,13 +17,8 @@
     def ready(self):
         """Run when the app is ready.
 
         Returns:
 
         """
         if "migrate" not in sys.argv:
-            from core_explore_keyword_registry_app import (
-                discover as discover_xslt,
-            )
-
-            discover_xslt.init_xslt()
             discover_permissions.init_permissions(self.apps)
```

### Comparing `core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app/permissions/discover.py` & `core_explore_keyword_registry_app-2.9.0/core_explore_keyword_registry_app/permissions/discover.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/css/fancytree/fancytree.custom.css` & `core_explore_keyword_registry_app-2.9.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/css/fancytree/fancytree.custom.css`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/css/search/search.css` & `core_explore_keyword_registry_app-2.9.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/css/search/search.css`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/search/fancytree.custom.js` & `core_explore_keyword_registry_app-2.9.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/search/fancytree.custom.js`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/search/filters.js` & `core_explore_keyword_registry_app-2.9.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/search/filters.js`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/search/resource_type_icons_table.js` & `core_explore_keyword_registry_app-2.9.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/search/resource_type_icons_table.js`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/search/tagit.custom.js` & `core_explore_keyword_registry_app-2.9.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/search/tagit.custom.js`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/libs/jquery-shorten/1.1.0/jquery.shorten.js` & `core_explore_keyword_registry_app-2.9.0/core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/libs/jquery-shorten/1.1.0/jquery.shorten.js`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app/templates/core_explore_common_app/user/results/data_source_info.html` & `core_explore_keyword_registry_app-2.9.0/core_explore_keyword_registry_app/templates/core_explore_common_app/user/results/data_source_info.html`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app/templates/core_explore_common_app/user/results/data_source_results.html` & `core_explore_keyword_registry_app-2.9.0/core_explore_keyword_registry_app/templates/core_explore_common_app/user/results/data_source_results.html`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app/templates/core_explore_keyword_app/user/index.html` & `core_explore_keyword_registry_app-2.9.0/core_explore_keyword_registry_app/templates/core_explore_keyword_app/user/index.html`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app/templates/core_explore_keyword_registry_app/user/refinements.html` & `core_explore_keyword_registry_app-2.9.0/core_explore_keyword_registry_app/templates/core_explore_keyword_registry_app/user/refinements.html`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app/templatetags/render_extras.py` & `core_explore_keyword_registry_app-2.9.0/core_explore_keyword_registry_app/templatetags/render_extras.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app/urls.py` & `core_explore_keyword_registry_app-2.9.0/core_explore_keyword_registry_app/urls.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app/views/user/ajax.py` & `core_explore_keyword_registry_app-2.9.0/core_explore_keyword_registry_app/views/user/ajax.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app/views/user/forms.py` & `core_explore_keyword_registry_app-2.9.0/core_explore_keyword_registry_app/views/user/forms.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app/views/user/views.py` & `core_explore_keyword_registry_app-2.9.0/core_explore_keyword_registry_app/views/user/views.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app.egg-info/PKG-INFO` & `core_explore_keyword_registry_app-2.9.0/core_explore_keyword_registry_app.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-explore-keyword-registry-app
-Version: 2.8.0
+Version: 2.9.0
 Summary: Exploration by keywords for the registry project
 Home-page: https://github.com/usnistgov/core_explore_keyword_registry_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: =================================
         Core Explore Keyword Registry App
```

### Comparing `core_explore_keyword_registry_app-2.8.0/core_explore_keyword_registry_app.egg-info/SOURCES.txt` & `core_explore_keyword_registry_app-2.9.0/core_explore_keyword_registry_app.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 README.rst
 pyproject.toml
 requirements.core.txt
 requirements.txt
 setup.py
 core_explore_keyword_registry_app/__init__.py
 core_explore_keyword_registry_app/apps.py
-core_explore_keyword_registry_app/discover.py
 core_explore_keyword_registry_app/settings.py
 core_explore_keyword_registry_app/urls.py
 core_explore_keyword_registry_app.egg-info/PKG-INFO
 core_explore_keyword_registry_app.egg-info/SOURCES.txt
 core_explore_keyword_registry_app.egg-info/dependency_links.txt
 core_explore_keyword_registry_app.egg-info/requires.txt
 core_explore_keyword_registry_app.egg-info/top_level.txt
@@ -24,16 +23,14 @@
 core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/search/fancytree.custom.raw.js
 core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/search/filters.js
 core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/search/resource_type_icons_table.js
 core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/search/resource_type_icons_table.raw.js
 core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/search/search.js
 core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/js/search/tagit.custom.js
 core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/user/libs/jquery-shorten/1.1.0/jquery.shorten.js
-core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/xsl/registry-detail.xsl
-core_explore_keyword_registry_app/static/core_explore_keyword_registry_app/xsl/registry-list.xsl
 core_explore_keyword_registry_app/templates/core_explore_common_app/user/results/data_source_info.html
 core_explore_keyword_registry_app/templates/core_explore_common_app/user/results/data_source_results.html
 core_explore_keyword_registry_app/templates/core_explore_keyword_app/user/index.html
 core_explore_keyword_registry_app/templates/core_explore_keyword_registry_app/user/refinements.html
 core_explore_keyword_registry_app/templatetags/__init__.py
 core_explore_keyword_registry_app/templatetags/render_extras.py
 core_explore_keyword_registry_app/views/__init__.py
```

### Comparing `core_explore_keyword_registry_app-2.8.0/setup.py` & `core_explore_keyword_registry_app-2.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_explore_keyword_registry_app",
-    version="2.8.0",
+    version="2.9.0",
     description="Exploration by keywords for the registry project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_explore_keyword_registry_app",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `core_explore_keyword_registry_app-2.8.0/tests/test_settings.py` & `core_explore_keyword_registry_app-2.9.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_registry_app-2.8.0/tests/views/user/tests_views.py` & `core_explore_keyword_registry_app-2.9.0/tests/views/user/tests_views.py`

 * *Files identical despite different names*

