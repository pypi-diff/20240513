# Comparing `tmp/core_dashboard_app-2.8.0.tar.gz` & `tmp/core_dashboard_app-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_dashboard_app-2.8.0.tar", last modified: Tue Mar 12 18:58:10 2024, max compression
+gzip compressed data, was "core_dashboard_app-2.9.0.tar", last modified: Mon May 13 16:03:36 2024, max compression
```

## Comparing `core_dashboard_app-2.8.0.tar` & `core_dashboard_app-2.9.0.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:10.110494 core_dashboard_app-2.8.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2024-03-12 18:58:06.000000 core_dashboard_app-2.8.0/LICENSE.md
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      144 2024-03-12 18:58:06.000000 core_dashboard_app-2.8.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1080 2024-03-12 18:58:10.103824 core_dashboard_app-2.8.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      579 2024-03-12 18:58:06.000000 core_dashboard_app-2.8.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:09.459753 core_dashboard_app-2.8.0/core_dashboard_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:06.000000 core_dashboard_app-2.8.0/core_dashboard_app/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4595 2024-03-12 18:58:06.000000 core_dashboard_app-2.8.0/core_dashboard_app/admin.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3262 2024-03-12 18:58:06.000000 core_dashboard_app-2.8.0/core_dashboard_app/menus.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      407 2024-03-12 18:58:06.000000 core_dashboard_app-2.8.0/core_dashboard_app/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:09.127551 core_dashboard_app-2.8.0/core_dashboard_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:09.168708 core_dashboard_app-2.8.0/core_dashboard_app/static/core_dashboard_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:09.142750 core_dashboard_app-2.8.0/core_dashboard_app/static/core_dashboard_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:09.570520 core_dashboard_app-2.8.0/core_dashboard_app/static/core_dashboard_app/admin/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       93 2024-03-12 18:58:06.000000 core_dashboard_app-2.8.0/core_dashboard_app/static/core_dashboard_app/admin/js/my_dashboard_tabs.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:09.161288 core_dashboard_app-2.8.0/core_dashboard_app/static/core_dashboard_app/common/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:09.590985 core_dashboard_app-2.8.0/core_dashboard_app/static/core_dashboard_app/common/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       74 2024-03-12 18:58:06.000000 core_dashboard_app-2.8.0/core_dashboard_app/static/core_dashboard_app/common/css/my_dashboard_tabs.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:09.611173 core_dashboard_app-2.8.0/core_dashboard_app/static/core_dashboard_app/common/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      605 2024-03-12 18:58:06.000000 core_dashboard_app-2.8.0/core_dashboard_app/static/core_dashboard_app/common/js/my_dashboard_tabs.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:09.172754 core_dashboard_app-2.8.0/core_dashboard_app/static/core_dashboard_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:09.630464 core_dashboard_app-2.8.0/core_dashboard_app/static/core_dashboard_app/user/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       82 2024-03-12 18:58:06.000000 core_dashboard_app-2.8.0/core_dashboard_app/static/core_dashboard_app/user/js/my_dashboard_tabs.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:09.186997 core_dashboard_app-2.8.0/core_dashboard_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:09.214794 core_dashboard_app-2.8.0/core_dashboard_app/templates/core_dashboard_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:09.667661 core_dashboard_app-2.8.0/core_dashboard_app/templates/core_dashboard_app/admin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      323 2024-03-12 18:58:06.000000 core_dashboard_app-2.8.0/core_dashboard_app/templates/core_dashboard_app/admin/my_dashboard_container.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1256 2024-03-12 18:58:06.000000 core_dashboard_app-2.8.0/core_dashboard_app/templates/core_dashboard_app/admin/my_dashboard_content.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:09.209015 core_dashboard_app-2.8.0/core_dashboard_app/templates/core_dashboard_app/common/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:09.720513 core_dashboard_app-2.8.0/core_dashboard_app/templates/core_dashboard_app/common/list/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1720 2024-03-12 18:58:06.000000 core_dashboard_app-2.8.0/core_dashboard_app/templates/core_dashboard_app/common/list/my_dashboard_tabs.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      176 2024-03-12 18:58:06.000000 core_dashboard_app-2.8.0/core_dashboard_app/templates/core_dashboard_app/common/list/my_dashboard_tabs_file_pagination.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:09.740711 core_dashboard_app-2.8.0/core_dashboard_app/templates/core_dashboard_app/common/pagination/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2681 2024-03-12 18:58:06.000000 core_dashboard_app-2.8.0/core_dashboard_app/templates/core_dashboard_app/common/pagination/pagination_tab.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:09.761735 core_dashboard_app-2.8.0/core_dashboard_app/templates/core_dashboard_app/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      443 2024-03-12 18:58:06.000000 core_dashboard_app-2.8.0/core_dashboard_app/templates/core_dashboard_app/user/my_dashboard_container.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3488 2024-03-12 18:58:06.000000 core_dashboard_app-2.8.0/core_dashboard_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:09.784908 core_dashboard_app-2.8.0/core_dashboard_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:06.000000 core_dashboard_app-2.8.0/core_dashboard_app/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:09.829614 core_dashboard_app-2.8.0/core_dashboard_app/views/common/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:06.000000 core_dashboard_app-2.8.0/core_dashboard_app/views/common/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    13263 2024-03-12 18:58:06.000000 core_dashboard_app-2.8.0/core_dashboard_app/views/common/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:09.551989 core_dashboard_app-2.8.0/core_dashboard_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1080 2024-03-12 18:58:08.000000 core_dashboard_app-2.8.0/core_dashboard_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1673 2024-03-12 18:58:09.000000 core_dashboard_app-2.8.0/core_dashboard_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2024-03-12 18:58:08.000000 core_dashboard_app-2.8.0/core_dashboard_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      111 2024-03-12 18:58:08.000000 core_dashboard_app-2.8.0/core_dashboard_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       30 2024-03-12 18:58:08.000000 core_dashboard_app-2.8.0/core_dashboard_app.egg-info/top_level.txt
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:09.887605 core_dashboard_app-2.8.0/docs/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:06.000000 core_dashboard_app-2.8.0/docs/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11302 2024-03-12 18:58:06.000000 core_dashboard_app-2.8.0/docs/conf.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      292 2024-03-12 18:58:06.000000 core_dashboard_app-2.8.0/docs/conf_urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2024-03-12 18:58:06.000000 core_dashboard_app-2.8.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       85 2024-03-12 18:58:06.000000 core_dashboard_app-2.8.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2024-03-12 18:58:10.112812 core_dashboard_app-2.8.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1077 2024-03-12 18:58:07.000000 core_dashboard_app-2.8.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:09.957850 core_dashboard_app-2.8.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:07.000000 core_dashboard_app-2.8.0/tests/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1812 2024-03-12 18:58:07.000000 core_dashboard_app-2.8.0/tests/test_settings.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      467 2024-03-12 18:58:07.000000 core_dashboard_app-2.8.0/tests/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:10.002219 core_dashboard_app-2.8.0/tests/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:07.000000 core_dashboard_app-2.8.0/tests/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:10.024551 core_dashboard_app-2.8.0/tests/views/common/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:07.000000 core_dashboard_app-2.8.0/tests/views/common/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:10.087977 core_dashboard_app-2.8.0/tests/views/common/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:07.000000 core_dashboard_app-2.8.0/tests/views/common/views/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1226 2024-03-12 18:58:07.000000 core_dashboard_app-2.8.0/tests/views/common/views/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6501 2024-03-12 18:58:07.000000 core_dashboard_app-2.8.0/tests/views/common/views/tests_unit.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1897 2024-03-12 18:58:07.000000 core_dashboard_app-2.8.0/tests/views/fixtures.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:36.100361 core_dashboard_app-2.9.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2024-05-13 16:03:31.000000 core_dashboard_app-2.9.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      144 2024-05-13 16:03:31.000000 core_dashboard_app-2.9.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1080 2024-05-13 16:03:36.090333 core_dashboard_app-2.9.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      579 2024-05-13 16:03:31.000000 core_dashboard_app-2.9.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:35.403868 core_dashboard_app-2.9.0/core_dashboard_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:31.000000 core_dashboard_app-2.9.0/core_dashboard_app/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4595 2024-05-13 16:03:31.000000 core_dashboard_app-2.9.0/core_dashboard_app/admin.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3262 2024-05-13 16:03:31.000000 core_dashboard_app-2.9.0/core_dashboard_app/menus.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      407 2024-05-13 16:03:31.000000 core_dashboard_app-2.9.0/core_dashboard_app/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:34.973680 core_dashboard_app-2.9.0/core_dashboard_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:35.040717 core_dashboard_app-2.9.0/core_dashboard_app/static/core_dashboard_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:34.982816 core_dashboard_app-2.9.0/core_dashboard_app/static/core_dashboard_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:35.512423 core_dashboard_app-2.9.0/core_dashboard_app/static/core_dashboard_app/admin/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       93 2024-05-13 16:03:32.000000 core_dashboard_app-2.9.0/core_dashboard_app/static/core_dashboard_app/admin/js/my_dashboard_tabs.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:35.032703 core_dashboard_app-2.9.0/core_dashboard_app/static/core_dashboard_app/common/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:35.555365 core_dashboard_app-2.9.0/core_dashboard_app/static/core_dashboard_app/common/css/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       74 2024-05-13 16:03:32.000000 core_dashboard_app-2.9.0/core_dashboard_app/static/core_dashboard_app/common/css/my_dashboard_tabs.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:35.573049 core_dashboard_app-2.9.0/core_dashboard_app/static/core_dashboard_app/common/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      605 2024-05-13 16:03:32.000000 core_dashboard_app-2.9.0/core_dashboard_app/static/core_dashboard_app/common/js/my_dashboard_tabs.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:35.045059 core_dashboard_app-2.9.0/core_dashboard_app/static/core_dashboard_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:35.626936 core_dashboard_app-2.9.0/core_dashboard_app/static/core_dashboard_app/user/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       82 2024-05-13 16:03:32.000000 core_dashboard_app-2.9.0/core_dashboard_app/static/core_dashboard_app/user/js/my_dashboard_tabs.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:35.059059 core_dashboard_app-2.9.0/core_dashboard_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:35.087831 core_dashboard_app-2.9.0/core_dashboard_app/templates/core_dashboard_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:35.664995 core_dashboard_app-2.9.0/core_dashboard_app/templates/core_dashboard_app/admin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      323 2024-05-13 16:03:32.000000 core_dashboard_app-2.9.0/core_dashboard_app/templates/core_dashboard_app/admin/my_dashboard_container.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1256 2024-05-13 16:03:32.000000 core_dashboard_app-2.9.0/core_dashboard_app/templates/core_dashboard_app/admin/my_dashboard_content.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:35.082197 core_dashboard_app-2.9.0/core_dashboard_app/templates/core_dashboard_app/common/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:35.700893 core_dashboard_app-2.9.0/core_dashboard_app/templates/core_dashboard_app/common/list/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1720 2024-05-13 16:03:32.000000 core_dashboard_app-2.9.0/core_dashboard_app/templates/core_dashboard_app/common/list/my_dashboard_tabs.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      176 2024-05-13 16:03:32.000000 core_dashboard_app-2.9.0/core_dashboard_app/templates/core_dashboard_app/common/list/my_dashboard_tabs_file_pagination.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:35.716948 core_dashboard_app-2.9.0/core_dashboard_app/templates/core_dashboard_app/common/pagination/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2681 2024-05-13 16:03:32.000000 core_dashboard_app-2.9.0/core_dashboard_app/templates/core_dashboard_app/common/pagination/pagination_tab.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:35.733147 core_dashboard_app-2.9.0/core_dashboard_app/templates/core_dashboard_app/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      443 2024-05-13 16:03:32.000000 core_dashboard_app-2.9.0/core_dashboard_app/templates/core_dashboard_app/user/my_dashboard_container.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3488 2024-05-13 16:03:32.000000 core_dashboard_app-2.9.0/core_dashboard_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:35.753949 core_dashboard_app-2.9.0/core_dashboard_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:32.000000 core_dashboard_app-2.9.0/core_dashboard_app/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:35.797526 core_dashboard_app-2.9.0/core_dashboard_app/views/common/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:32.000000 core_dashboard_app-2.9.0/core_dashboard_app/views/common/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    13263 2024-05-13 16:03:32.000000 core_dashboard_app-2.9.0/core_dashboard_app/views/common/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:35.491224 core_dashboard_app-2.9.0/core_dashboard_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1080 2024-05-13 16:03:34.000000 core_dashboard_app-2.9.0/core_dashboard_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1673 2024-05-13 16:03:34.000000 core_dashboard_app-2.9.0/core_dashboard_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2024-05-13 16:03:34.000000 core_dashboard_app-2.9.0/core_dashboard_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      111 2024-05-13 16:03:34.000000 core_dashboard_app-2.9.0/core_dashboard_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       30 2024-05-13 16:03:34.000000 core_dashboard_app-2.9.0/core_dashboard_app.egg-info/top_level.txt
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:35.874573 core_dashboard_app-2.9.0/docs/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:32.000000 core_dashboard_app-2.9.0/docs/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11302 2024-05-13 16:03:32.000000 core_dashboard_app-2.9.0/docs/conf.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      292 2024-05-13 16:03:32.000000 core_dashboard_app-2.9.0/docs/conf_urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2024-05-13 16:03:32.000000 core_dashboard_app-2.9.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       85 2024-05-13 16:03:32.000000 core_dashboard_app-2.9.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2024-05-13 16:03:36.103756 core_dashboard_app-2.9.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1077 2024-05-13 16:03:32.000000 core_dashboard_app-2.9.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:35.927761 core_dashboard_app-2.9.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:32.000000 core_dashboard_app-2.9.0/tests/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1812 2024-05-13 16:03:32.000000 core_dashboard_app-2.9.0/tests/test_settings.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      467 2024-05-13 16:03:32.000000 core_dashboard_app-2.9.0/tests/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:35.964827 core_dashboard_app-2.9.0/tests/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:32.000000 core_dashboard_app-2.9.0/tests/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:35.982211 core_dashboard_app-2.9.0/tests/views/common/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:32.000000 core_dashboard_app-2.9.0/tests/views/common/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:36.041822 core_dashboard_app-2.9.0/tests/views/common/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:32.000000 core_dashboard_app-2.9.0/tests/views/common/views/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1226 2024-05-13 16:03:32.000000 core_dashboard_app-2.9.0/tests/views/common/views/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6501 2024-05-13 16:03:32.000000 core_dashboard_app-2.9.0/tests/views/common/views/tests_unit.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1897 2024-05-13 16:03:32.000000 core_dashboard_app-2.9.0/tests/views/fixtures.py
```

### Comparing `core_dashboard_app-2.8.0/LICENSE.md` & `core_dashboard_app-2.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `core_dashboard_app-2.8.0/PKG-INFO` & `core_dashboard_app-2.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_dashboard_app
-Version: 2.8.0
+Version: 2.9.0
 Summary: Resource management via a dashboard for the curator core project
 Home-page: https://github.com/usnistgov/core_dashboard_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: ==================
         Core Dashboard App
```

### Comparing `core_dashboard_app-2.8.0/README.rst` & `core_dashboard_app-2.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_dashboard_app-2.8.0/core_dashboard_app/admin.py` & `core_dashboard_app-2.9.0/core_dashboard_app/admin.py`

 * *Files identical despite different names*

### Comparing `core_dashboard_app-2.8.0/core_dashboard_app/menus.py` & `core_dashboard_app-2.9.0/core_dashboard_app/menus.py`

 * *Files identical despite different names*

### Comparing `core_dashboard_app-2.8.0/core_dashboard_app/static/core_dashboard_app/common/js/my_dashboard_tabs.js` & `core_dashboard_app-2.9.0/core_dashboard_app/static/core_dashboard_app/common/js/my_dashboard_tabs.js`

 * *Files identical despite different names*

### Comparing `core_dashboard_app-2.8.0/core_dashboard_app/templates/core_dashboard_app/admin/my_dashboard_content.html` & `core_dashboard_app-2.9.0/core_dashboard_app/templates/core_dashboard_app/admin/my_dashboard_content.html`

 * *Files identical despite different names*

### Comparing `core_dashboard_app-2.8.0/core_dashboard_app/templates/core_dashboard_app/common/list/my_dashboard_tabs.html` & `core_dashboard_app-2.9.0/core_dashboard_app/templates/core_dashboard_app/common/list/my_dashboard_tabs.html`

 * *Files identical despite different names*

### Comparing `core_dashboard_app-2.8.0/core_dashboard_app/templates/core_dashboard_app/common/pagination/pagination_tab.html` & `core_dashboard_app-2.9.0/core_dashboard_app/templates/core_dashboard_app/common/pagination/pagination_tab.html`

 * *Files identical despite different names*

### Comparing `core_dashboard_app-2.8.0/core_dashboard_app/urls.py` & `core_dashboard_app-2.9.0/core_dashboard_app/urls.py`

 * *Files identical despite different names*

### Comparing `core_dashboard_app-2.8.0/core_dashboard_app/views/common/views.py` & `core_dashboard_app-2.9.0/core_dashboard_app/views/common/views.py`

 * *Files identical despite different names*

### Comparing `core_dashboard_app-2.8.0/core_dashboard_app.egg-info/PKG-INFO` & `core_dashboard_app-2.9.0/core_dashboard_app.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-dashboard-app
-Version: 2.8.0
+Version: 2.9.0
 Summary: Resource management via a dashboard for the curator core project
 Home-page: https://github.com/usnistgov/core_dashboard_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: ==================
         Core Dashboard App
```

### Comparing `core_dashboard_app-2.8.0/core_dashboard_app.egg-info/SOURCES.txt` & `core_dashboard_app-2.9.0/core_dashboard_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `core_dashboard_app-2.8.0/docs/conf.py` & `core_dashboard_app-2.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `core_dashboard_app-2.8.0/setup.py` & `core_dashboard_app-2.9.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_dashboard_app",
-    version="2.8.0",
+    version="2.9.0",
     description="Resource management via a dashboard for the curator core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_dashboard_app",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `core_dashboard_app-2.8.0/tests/test_settings.py` & `core_dashboard_app-2.9.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `core_dashboard_app-2.8.0/tests/views/common/views/tests_int.py` & `core_dashboard_app-2.9.0/tests/views/common/views/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_dashboard_app-2.8.0/tests/views/common/views/tests_unit.py` & `core_dashboard_app-2.9.0/tests/views/common/views/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_dashboard_app-2.8.0/tests/views/fixtures.py` & `core_dashboard_app-2.9.0/tests/views/fixtures.py`

 * *Files identical despite different names*

