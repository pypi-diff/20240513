# Comparing `tmp/core_exporters_app-2.8.0.tar.gz` & `tmp/core_exporters_app-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_exporters_app-2.8.0.tar", last modified: Tue Mar 12 19:00:59 2024, max compression
+gzip compressed data, was "core_exporters_app-2.9.0.tar", last modified: Mon May 13 16:06:35 2024, max compression
```

## Comparing `core_exporters_app-2.8.0.tar` & `core_exporters_app-2.9.0.tar`

### file list

```diff
@@ -1,218 +1,230 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:59.013963 core_exporters_app-2.8.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2024-03-12 19:00:46.000000 core_exporters_app-2.8.0/LICENSE.md
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      292 2024-03-12 19:00:46.000000 core_exporters_app-2.8.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1017 2024-03-12 19:00:59.007990 core_exporters_app-2.8.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      542 2024-03-12 19:00:46.000000 core_exporters_app-2.8.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:56.261701 core_exporters_app-2.8.0/core_exporters_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       93 2024-03-12 19:00:46.000000 core_exporters_app-2.8.0/core_exporters_app/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:56.387510 core_exporters_app-2.8.0/core_exporters_app/access_control/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:46.000000 core_exporters_app-2.8.0/core_exporters_app/access_control/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      931 2024-03-12 19:00:46.000000 core_exporters_app-2.8.0/core_exporters_app/access_control/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1764 2024-03-12 19:00:46.000000 core_exporters_app-2.8.0/core_exporters_app/admin.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      778 2024-03-12 19:00:46.000000 core_exporters_app-2.8.0/core_exporters_app/apps.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:56.433780 core_exporters_app-2.8.0/core_exporters_app/commons/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:46.000000 core_exporters_app-2.8.0/core_exporters_app/commons/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      311 2024-03-12 19:00:46.000000 core_exporters_app-2.8.0/core_exporters_app/commons/constants.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:56.456795 core_exporters_app-2.8.0/core_exporters_app/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:46.000000 core_exporters_app-2.8.0/core_exporters_app/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:56.546068 core_exporters_app-2.8.0/core_exporters_app/components/exported_compressed_file/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:46.000000 core_exporters_app-2.8.0/core_exporters_app/components/exported_compressed_file/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      404 2024-03-12 19:00:46.000000 core_exporters_app-2.8.0/core_exporters_app/components/exported_compressed_file/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      778 2024-03-12 19:00:46.000000 core_exporters_app-2.8.0/core_exporters_app/components/exported_compressed_file/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1365 2024-03-12 19:00:46.000000 core_exporters_app-2.8.0/core_exporters_app/components/exported_compressed_file/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:56.656978 core_exporters_app-2.8.0/core_exporters_app/components/exporter/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:46.000000 core_exporters_app-2.8.0/core_exporters_app/components/exporter/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      318 2024-03-12 19:00:46.000000 core_exporters_app-2.8.0/core_exporters_app/components/exporter/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1638 2024-03-12 19:00:46.000000 core_exporters_app-2.8.0/core_exporters_app/components/exporter/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7200 2024-03-12 19:00:46.000000 core_exporters_app-2.8.0/core_exporters_app/components/exporter/models.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1746 2024-03-12 19:00:46.000000 core_exporters_app-2.8.0/core_exporters_app/components/exporter/watch.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:56.753821 core_exporters_app-2.8.0/core_exporters_app/exporters/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:46.000000 core_exporters_app-2.8.0/core_exporters_app/exporters/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:56.819342 core_exporters_app-2.8.0/core_exporters_app/exporters/blob/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:46.000000 core_exporters_app-2.8.0/core_exporters_app/exporters/blob/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4552 2024-03-12 19:00:46.000000 core_exporters_app-2.8.0/core_exporters_app/exporters/blob/models.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      221 2024-03-12 19:00:46.000000 core_exporters_app-2.8.0/core_exporters_app/exporters/blob/urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4538 2024-03-12 19:00:46.000000 core_exporters_app-2.8.0/core_exporters_app/exporters/discover.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5910 2024-03-12 19:00:46.000000 core_exporters_app-2.8.0/core_exporters_app/exporters/exporter.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:56.880114 core_exporters_app-2.8.0/core_exporters_app/exporters/json_exporter/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:46.000000 core_exporters_app-2.8.0/core_exporters_app/exporters/json_exporter/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2508 2024-03-12 19:00:46.000000 core_exporters_app-2.8.0/core_exporters_app/exporters/json_exporter/models.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      230 2024-03-12 19:00:46.000000 core_exporters_app-2.8.0/core_exporters_app/exporters/json_exporter/urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      323 2024-03-12 19:00:46.000000 core_exporters_app-2.8.0/core_exporters_app/exporters/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:56.938413 core_exporters_app-2.8.0/core_exporters_app/exporters/xml/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:46.000000 core_exporters_app-2.8.0/core_exporters_app/exporters/xml/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1762 2024-03-12 19:00:46.000000 core_exporters_app-2.8.0/core_exporters_app/exporters/xml/models.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      216 2024-03-12 19:00:46.000000 core_exporters_app-2.8.0/core_exporters_app/exporters/xml/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:57.035678 core_exporters_app-2.8.0/core_exporters_app/exporters/xsl/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:46.000000 core_exporters_app-2.8.0/core_exporters_app/exporters/xsl/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2801 2024-03-12 19:00:46.000000 core_exporters_app-2.8.0/core_exporters_app/exporters/xsl/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3331 2024-03-12 19:00:46.000000 core_exporters_app-2.8.0/core_exporters_app/exporters/xsl/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:55.548871 core_exporters_app-2.8.0/core_exporters_app/exporters/xsl/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:55.552934 core_exporters_app-2.8.0/core_exporters_app/exporters/xsl/static/xsl/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:55.557165 core_exporters_app-2.8.0/core_exporters_app/exporters/xsl/static/xsl/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:55.561290 core_exporters_app-2.8.0/core_exporters_app/exporters/xsl/static/xsl/admin/js/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:55.565335 core_exporters_app-2.8.0/core_exporters_app/exporters/xsl/static/xsl/admin/js/exporters/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:55.591532 core_exporters_app-2.8.0/core_exporters_app/exporters/xsl/static/xsl/admin/js/exporters/list/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:57.102029 core_exporters_app-2.8.0/core_exporters_app/exporters/xsl/static/xsl/admin/js/exporters/list/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1722 2024-03-12 19:00:46.000000 core_exporters_app-2.8.0/core_exporters_app/exporters/xsl/static/xsl/admin/js/exporters/list/modals/add.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       82 2024-03-12 19:00:46.000000 core_exporters_app-2.8.0/core_exporters_app/exporters/xsl/static/xsl/admin/js/exporters/list/modals/add.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:55.609022 core_exporters_app-2.8.0/core_exporters_app/exporters/xsl/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:55.613063 core_exporters_app-2.8.0/core_exporters_app/exporters/xsl/templates/xsl/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:55.617360 core_exporters_app-2.8.0/core_exporters_app/exporters/xsl/templates/xsl/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:55.621545 core_exporters_app-2.8.0/core_exporters_app/exporters/xsl/templates/xsl/admin/exporters/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:57.161091 core_exporters_app-2.8.0/core_exporters_app/exporters/xsl/templates/xsl/admin/exporters/list/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       40 2024-03-12 19:00:46.000000 core_exporters_app-2.8.0/core_exporters_app/exporters/xsl/templates/xsl/admin/exporters/list/add_base.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1965 2024-03-12 19:00:46.000000 core_exporters_app-2.8.0/core_exporters_app/exporters/xsl/templates/xsl/admin/exporters/list/list_base.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:57.183696 core_exporters_app-2.8.0/core_exporters_app/exporters/xsl/templates/xsl/admin/exporters/list/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1126 2024-03-12 19:00:46.000000 core_exporters_app-2.8.0/core_exporters_app/exporters/xsl/templates/xsl/admin/exporters/list/modals/add.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      336 2024-03-12 19:00:46.000000 core_exporters_app-2.8.0/core_exporters_app/exporters/xsl/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:57.205023 core_exporters_app-2.8.0/core_exporters_app/exporters/xsl/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:46.000000 core_exporters_app-2.8.0/core_exporters_app/exporters/xsl/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:57.270420 core_exporters_app-2.8.0/core_exporters_app/exporters/xsl/views/admin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:46.000000 core_exporters_app-2.8.0/core_exporters_app/exporters/xsl/views/admin/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3073 2024-03-12 19:00:46.000000 core_exporters_app-2.8.0/core_exporters_app/exporters/xsl/views/admin/ajax.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      833 2024-03-12 19:00:46.000000 core_exporters_app-2.8.0/core_exporters_app/exporters/xsl/views/admin/forms.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      332 2024-03-12 19:00:46.000000 core_exporters_app-2.8.0/core_exporters_app/menus.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:57.309985 core_exporters_app-2.8.0/core_exporters_app/migrations/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3588 2024-03-12 19:00:46.000000 core_exporters_app-2.8.0/core_exporters_app/migrations/0001_initial.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:46.000000 core_exporters_app-2.8.0/core_exporters_app/migrations/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:57.358877 core_exporters_app-2.8.0/core_exporters_app/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:46.000000 core_exporters_app-2.8.0/core_exporters_app/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:57.382713 core_exporters_app-2.8.0/core_exporters_app/rest/export/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:46.000000 core_exporters_app-2.8.0/core_exporters_app/rest/export/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:57.448750 core_exporters_app-2.8.0/core_exporters_app/rest/export/data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:46.000000 core_exporters_app-2.8.0/core_exporters_app/rest/export/data/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6855 2024-03-12 19:00:46.000000 core_exporters_app-2.8.0/core_exporters_app/rest/export/data/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:57.516258 core_exporters_app-2.8.0/core_exporters_app/rest/exporters/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:46.000000 core_exporters_app-2.8.0/core_exporters_app/rest/exporters/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1967 2024-03-12 19:00:46.000000 core_exporters_app-2.8.0/core_exporters_app/rest/exporters/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8794 2024-03-12 19:00:46.000000 core_exporters_app-2.8.0/core_exporters_app/rest/exporters/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:57.563012 core_exporters_app-2.8.0/core_exporters_app/rest/exporters/xsl/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:46.000000 core_exporters_app-2.8.0/core_exporters_app/rest/exporters/xsl/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4291 2024-03-12 19:00:46.000000 core_exporters_app-2.8.0/core_exporters_app/rest/exporters/xsl/views.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1516 2024-03-12 19:00:46.000000 core_exporters_app-2.8.0/core_exporters_app/rest/urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      862 2024-03-12 19:00:46.000000 core_exporters_app-2.8.0/core_exporters_app/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:55.696180 core_exporters_app-2.8.0/core_exporters_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:55.757259 core_exporters_app-2.8.0/core_exporters_app/static/core_exporters_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:55.735102 core_exporters_app-2.8.0/core_exporters_app/static/core_exporters_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:55.719620 core_exporters_app-2.8.0/core_exporters_app/static/core_exporters_app/admin/css/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:55.723860 core_exporters_app-2.8.0/core_exporters_app/static/core_exporters_app/admin/css/exporters/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:57.607044 core_exporters_app-2.8.0/core_exporters_app/static/core_exporters_app/admin/css/exporters/list/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      115 2024-03-12 19:00:47.000000 core_exporters_app-2.8.0/core_exporters_app/static/core_exporters_app/admin/css/exporters/list/list_exporters.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:55.739237 core_exporters_app-2.8.0/core_exporters_app/static/core_exporters_app/admin/js/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:55.743625 core_exporters_app-2.8.0/core_exporters_app/static/core_exporters_app/admin/js/exporters/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:55.747717 core_exporters_app-2.8.0/core_exporters_app/static/core_exporters_app/admin/js/exporters/list/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:57.653736 core_exporters_app-2.8.0/core_exporters_app/static/core_exporters_app/admin/js/exporters/list/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1990 2024-03-12 19:00:47.000000 core_exporters_app-2.8.0/core_exporters_app/static/core_exporters_app/admin/js/exporters/list/modals/associated_templates.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      103 2024-03-12 19:00:47.000000 core_exporters_app-2.8.0/core_exporters_app/static/core_exporters_app/admin/js/exporters/list/modals/associated_templates.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:55.761215 core_exporters_app-2.8.0/core_exporters_app/static/core_exporters_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:55.794300 core_exporters_app-2.8.0/core_exporters_app/static/core_exporters_app/user/js/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:57.700965 core_exporters_app-2.8.0/core_exporters_app/static/core_exporters_app/user/js/exporter_compressed_file/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      962 2024-03-12 19:00:47.000000 core_exporters_app-2.8.0/core_exporters_app/static/core_exporters_app/user/js/exporter_compressed_file/download.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       82 2024-03-12 19:00:47.000000 core_exporters_app-2.8.0/core_exporters_app/static/core_exporters_app/user/js/exporter_compressed_file/download.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:55.798587 core_exporters_app-2.8.0/core_exporters_app/static/core_exporters_app/user/js/exporters/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:55.802982 core_exporters_app-2.8.0/core_exporters_app/static/core_exporters_app/user/js/exporters/list/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:57.746996 core_exporters_app-2.8.0/core_exporters_app/static/core_exporters_app/user/js/exporters/list/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5272 2024-03-12 19:00:47.000000 core_exporters_app-2.8.0/core_exporters_app/static/core_exporters_app/user/js/exporters/list/modals/list_exporters_selector.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      160 2024-03-12 19:00:47.000000 core_exporters_app-2.8.0/core_exporters_app/static/core_exporters_app/user/js/exporters/list/modals/list_exporters_selector.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:57.790447 core_exporters_app-2.8.0/core_exporters_app/system/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:47.000000 core_exporters_app-2.8.0/core_exporters_app/system/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      561 2024-03-12 19:00:47.000000 core_exporters_app-2.8.0/core_exporters_app/system/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3982 2024-03-12 19:00:47.000000 core_exporters_app-2.8.0/core_exporters_app/tasks.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:55.824190 core_exporters_app-2.8.0/core_exporters_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:55.851097 core_exporters_app-2.8.0/core_exporters_app/templates/core_exporters_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:55.832253 core_exporters_app-2.8.0/core_exporters_app/templates/core_exporters_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:57.823708 core_exporters_app-2.8.0/core_exporters_app/templates/core_exporters_app/admin/exporters/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:57.864730 core_exporters_app-2.8.0/core_exporters_app/templates/core_exporters_app/admin/exporters/list/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      338 2024-03-12 19:00:47.000000 core_exporters_app-2.8.0/core_exporters_app/templates/core_exporters_app/admin/exporters/list/associated_templates_base.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1620 2024-03-12 19:00:47.000000 core_exporters_app-2.8.0/core_exporters_app/templates/core_exporters_app/admin/exporters/list/list_base.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:57.886659 core_exporters_app-2.8.0/core_exporters_app/templates/core_exporters_app/admin/exporters/list/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1186 2024-03-12 19:00:47.000000 core_exporters_app-2.8.0/core_exporters_app/templates/core_exporters_app/admin/exporters/list/modals/associated_templates.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      324 2024-03-12 19:00:47.000000 core_exporters_app-2.8.0/core_exporters_app/templates/core_exporters_app/admin/exporters/list_exporters.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:55.862820 core_exporters_app-2.8.0/core_exporters_app/templates/core_exporters_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:57.910262 core_exporters_app-2.8.0/core_exporters_app/templates/core_exporters_app/user/exported_compressed_file/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      265 2024-03-12 19:00:47.000000 core_exporters_app-2.8.0/core_exporters_app/templates/core_exporters_app/user/exported_compressed_file/download.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:55.867209 core_exporters_app-2.8.0/core_exporters_app/templates/core_exporters_app/user/exporters/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:57.951380 core_exporters_app-2.8.0/core_exporters_app/templates/core_exporters_app/user/exporters/list/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       41 2024-03-12 19:00:47.000000 core_exporters_app-2.8.0/core_exporters_app/templates/core_exporters_app/user/exporters/list/link_exporters_selector.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       27 2024-03-12 19:00:47.000000 core_exporters_app-2.8.0/core_exporters_app/templates/core_exporters_app/user/exporters/list/list_exporters_selector_base.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:57.974090 core_exporters_app-2.8.0/core_exporters_app/templates/core_exporters_app/user/exporters/list/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1142 2024-03-12 19:00:47.000000 core_exporters_app-2.8.0/core_exporters_app/templates/core_exporters_app/user/exporters/list/modals/list_exporters_selector.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      922 2024-03-12 19:00:47.000000 core_exporters_app-2.8.0/core_exporters_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:57.995752 core_exporters_app-2.8.0/core_exporters_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:47.000000 core_exporters_app-2.8.0/core_exporters_app/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:58.092064 core_exporters_app-2.8.0/core_exporters_app/views/admin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:47.000000 core_exporters_app-2.8.0/core_exporters_app/views/admin/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3974 2024-03-12 19:00:47.000000 core_exporters_app-2.8.0/core_exporters_app/views/admin/ajax.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1526 2024-03-12 19:00:47.000000 core_exporters_app-2.8.0/core_exporters_app/views/admin/forms.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1650 2024-03-12 19:00:47.000000 core_exporters_app-2.8.0/core_exporters_app/views/admin/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:58.175497 core_exporters_app-2.8.0/core_exporters_app/views/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:47.000000 core_exporters_app-2.8.0/core_exporters_app/views/user/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7615 2024-03-12 19:00:47.000000 core_exporters_app-2.8.0/core_exporters_app/views/user/ajax.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3067 2024-03-12 19:00:47.000000 core_exporters_app-2.8.0/core_exporters_app/views/user/forms.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2122 2024-03-12 19:00:47.000000 core_exporters_app-2.8.0/core_exporters_app/views/user/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:56.347145 core_exporters_app-2.8.0/core_exporters_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1017 2024-03-12 19:00:54.000000 core_exporters_app-2.8.0/core_exporters_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6264 2024-03-12 19:00:55.000000 core_exporters_app-2.8.0/core_exporters_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2024-03-12 19:00:54.000000 core_exporters_app-2.8.0/core_exporters_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      114 2024-03-12 19:00:54.000000 core_exporters_app-2.8.0/core_exporters_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       30 2024-03-12 19:00:54.000000 core_exporters_app-2.8.0/core_exporters_app.egg-info/top_level.txt
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:58.233973 core_exporters_app-2.8.0/docs/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:47.000000 core_exporters_app-2.8.0/docs/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11096 2024-03-12 19:00:47.000000 core_exporters_app-2.8.0/docs/conf.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      292 2024-03-12 19:00:47.000000 core_exporters_app-2.8.0/docs/conf_urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2024-03-12 19:00:51.000000 core_exporters_app-2.8.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       52 2024-03-12 19:00:51.000000 core_exporters_app-2.8.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       62 2024-03-12 19:00:51.000000 core_exporters_app-2.8.0/requirements.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2024-03-12 19:00:59.016264 core_exporters_app-2.8.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1393 2024-03-12 19:00:51.000000 core_exporters_app-2.8.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:58.275572 core_exporters_app-2.8.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:51.000000 core_exporters_app-2.8.0/tests/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:58.294955 core_exporters_app-2.8.0/tests/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:51.000000 core_exporters_app-2.8.0/tests/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:58.340136 core_exporters_app-2.8.0/tests/components/exported_compressed_file/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:51.000000 core_exporters_app-2.8.0/tests/components/exported_compressed_file/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:58.386505 core_exporters_app-2.8.0/tests/components/exported_compressed_file/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:51.000000 core_exporters_app-2.8.0/tests/components/exported_compressed_file/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1744 2024-03-12 19:00:51.000000 core_exporters_app-2.8.0/tests/components/exported_compressed_file/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6477 2024-03-12 19:00:51.000000 core_exporters_app-2.8.0/tests/components/exported_compressed_file/tests_int.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:58.431026 core_exporters_app-2.8.0/tests/components/exporter/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:51.000000 core_exporters_app-2.8.0/tests/components/exporter/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5848 2024-03-12 19:00:52.000000 core_exporters_app-2.8.0/tests/components/exporter/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:58.452481 core_exporters_app-2.8.0/tests/exporters/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:52.000000 core_exporters_app-2.8.0/tests/exporters/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:58.501229 core_exporters_app-2.8.0/tests/exporters/blob/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:52.000000 core_exporters_app-2.8.0/tests/exporters/blob/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      827 2024-03-12 19:00:52.000000 core_exporters_app-2.8.0/tests/exporters/blob/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:58.523280 core_exporters_app-2.8.0/tests/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:52.000000 core_exporters_app-2.8.0/tests/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:58.604914 core_exporters_app-2.8.0/tests/rest/export/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:52.000000 core_exporters_app-2.8.0/tests/rest/export/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:58.673148 core_exporters_app-2.8.0/tests/rest/export/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:52.000000 core_exporters_app-2.8.0/tests/rest/export/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2524 2024-03-12 19:00:52.000000 core_exporters_app-2.8.0/tests/rest/export/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8721 2024-03-12 19:00:52.000000 core_exporters_app-2.8.0/tests/rest/export/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7069 2024-03-12 19:00:52.000000 core_exporters_app-2.8.0/tests/rest/export/tests_permissions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5042 2024-03-12 19:00:52.000000 core_exporters_app-2.8.0/tests/rest/export/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:58.757473 core_exporters_app-2.8.0/tests/rest/exporter/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:52.000000 core_exporters_app-2.8.0/tests/rest/exporter/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:58.801158 core_exporters_app-2.8.0/tests/rest/exporter/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:52.000000 core_exporters_app-2.8.0/tests/rest/exporter/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      877 2024-03-12 19:00:52.000000 core_exporters_app-2.8.0/tests/rest/exporter/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4051 2024-03-12 19:00:52.000000 core_exporters_app-2.8.0/tests/rest/exporter/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8034 2024-03-12 19:00:52.000000 core_exporters_app-2.8.0/tests/rest/exporter/tests_permissions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1051 2024-03-12 19:00:52.000000 core_exporters_app-2.8.0/tests/rest/exporter/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:58.847613 core_exporters_app-2.8.0/tests/rest/exporter/xsl/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:52.000000 core_exporters_app-2.8.0/tests/rest/exporter/xsl/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5101 2024-03-12 19:00:52.000000 core_exporters_app-2.8.0/tests/rest/exporter/xsl/tests_permissions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1606 2024-03-12 19:00:52.000000 core_exporters_app-2.8.0/tests/test_settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:58.869356 core_exporters_app-2.8.0/tests/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:52.000000 core_exporters_app-2.8.0/tests/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:58.895136 core_exporters_app-2.8.0/tests/views/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:52.000000 core_exporters_app-2.8.0/tests/views/user/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:58.941312 core_exporters_app-2.8.0/tests/views/user/ajax/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:52.000000 core_exporters_app-2.8.0/tests/views/user/ajax/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      925 2024-03-12 19:00:52.000000 core_exporters_app-2.8.0/tests/views/user/ajax/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:58.987806 core_exporters_app-2.8.0/tests/views/user/forms/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:00:52.000000 core_exporters_app-2.8.0/tests/views/user/forms/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2627 2024-03-12 19:00:52.000000 core_exporters_app-2.8.0/tests/views/user/forms/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:35.474560 core_exporters_app-2.9.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2024-05-13 16:06:24.000000 core_exporters_app-2.9.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      292 2024-05-13 16:06:24.000000 core_exporters_app-2.9.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1017 2024-05-13 16:06:35.467667 core_exporters_app-2.9.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      542 2024-05-13 16:06:24.000000 core_exporters_app-2.9.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:32.054314 core_exporters_app-2.9.0/core_exporters_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       93 2024-05-13 16:06:24.000000 core_exporters_app-2.9.0/core_exporters_app/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:32.210447 core_exporters_app-2.9.0/core_exporters_app/access_control/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:24.000000 core_exporters_app-2.9.0/core_exporters_app/access_control/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      931 2024-05-13 16:06:24.000000 core_exporters_app-2.9.0/core_exporters_app/access_control/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1764 2024-05-13 16:06:24.000000 core_exporters_app-2.9.0/core_exporters_app/admin.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      547 2024-05-13 16:06:24.000000 core_exporters_app-2.9.0/core_exporters_app/apps.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:32.256962 core_exporters_app-2.9.0/core_exporters_app/commons/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:24.000000 core_exporters_app-2.9.0/core_exporters_app/commons/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      311 2024-05-13 16:06:24.000000 core_exporters_app-2.9.0/core_exporters_app/commons/constants.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:32.284284 core_exporters_app-2.9.0/core_exporters_app/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:24.000000 core_exporters_app-2.9.0/core_exporters_app/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:32.364182 core_exporters_app-2.9.0/core_exporters_app/components/exported_compressed_file/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:24.000000 core_exporters_app-2.9.0/core_exporters_app/components/exported_compressed_file/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      404 2024-05-13 16:06:24.000000 core_exporters_app-2.9.0/core_exporters_app/components/exported_compressed_file/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      778 2024-05-13 16:06:24.000000 core_exporters_app-2.9.0/core_exporters_app/components/exported_compressed_file/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1365 2024-05-13 16:06:24.000000 core_exporters_app-2.9.0/core_exporters_app/components/exported_compressed_file/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:32.493873 core_exporters_app-2.9.0/core_exporters_app/components/exporter/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:24.000000 core_exporters_app-2.9.0/core_exporters_app/components/exporter/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      318 2024-05-13 16:06:24.000000 core_exporters_app-2.9.0/core_exporters_app/components/exporter/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1638 2024-05-13 16:06:25.000000 core_exporters_app-2.9.0/core_exporters_app/components/exporter/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7200 2024-05-13 16:06:25.000000 core_exporters_app-2.9.0/core_exporters_app/components/exporter/models.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1746 2024-05-13 16:06:25.000000 core_exporters_app-2.9.0/core_exporters_app/components/exporter/watch.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:32.567198 core_exporters_app-2.9.0/core_exporters_app/exporters/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:25.000000 core_exporters_app-2.9.0/core_exporters_app/exporters/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:32.625919 core_exporters_app-2.9.0/core_exporters_app/exporters/blob/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:25.000000 core_exporters_app-2.9.0/core_exporters_app/exporters/blob/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4552 2024-05-13 16:06:25.000000 core_exporters_app-2.9.0/core_exporters_app/exporters/blob/models.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      221 2024-05-13 16:06:25.000000 core_exporters_app-2.9.0/core_exporters_app/exporters/blob/urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4556 2024-05-13 16:06:25.000000 core_exporters_app-2.9.0/core_exporters_app/exporters/discover.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5910 2024-05-13 16:06:25.000000 core_exporters_app-2.9.0/core_exporters_app/exporters/exporter.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:32.688542 core_exporters_app-2.9.0/core_exporters_app/exporters/json_exporter/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:25.000000 core_exporters_app-2.9.0/core_exporters_app/exporters/json_exporter/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2508 2024-05-13 16:06:25.000000 core_exporters_app-2.9.0/core_exporters_app/exporters/json_exporter/models.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      230 2024-05-13 16:06:25.000000 core_exporters_app-2.9.0/core_exporters_app/exporters/json_exporter/urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      323 2024-05-13 16:06:25.000000 core_exporters_app-2.9.0/core_exporters_app/exporters/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:32.782366 core_exporters_app-2.9.0/core_exporters_app/exporters/xml/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:25.000000 core_exporters_app-2.9.0/core_exporters_app/exporters/xml/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1762 2024-05-13 16:06:25.000000 core_exporters_app-2.9.0/core_exporters_app/exporters/xml/models.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      216 2024-05-13 16:06:25.000000 core_exporters_app-2.9.0/core_exporters_app/exporters/xml/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:32.862637 core_exporters_app-2.9.0/core_exporters_app/exporters/xsl/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:25.000000 core_exporters_app-2.9.0/core_exporters_app/exporters/xsl/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2801 2024-05-13 16:06:25.000000 core_exporters_app-2.9.0/core_exporters_app/exporters/xsl/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3331 2024-05-13 16:06:25.000000 core_exporters_app-2.9.0/core_exporters_app/exporters/xsl/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:31.285590 core_exporters_app-2.9.0/core_exporters_app/exporters/xsl/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:31.298812 core_exporters_app-2.9.0/core_exporters_app/exporters/xsl/static/xsl/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:31.307906 core_exporters_app-2.9.0/core_exporters_app/exporters/xsl/static/xsl/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:31.311675 core_exporters_app-2.9.0/core_exporters_app/exporters/xsl/static/xsl/admin/js/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:31.315208 core_exporters_app-2.9.0/core_exporters_app/exporters/xsl/static/xsl/admin/js/exporters/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:31.331303 core_exporters_app-2.9.0/core_exporters_app/exporters/xsl/static/xsl/admin/js/exporters/list/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:32.950918 core_exporters_app-2.9.0/core_exporters_app/exporters/xsl/static/xsl/admin/js/exporters/list/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1722 2024-05-13 16:06:25.000000 core_exporters_app-2.9.0/core_exporters_app/exporters/xsl/static/xsl/admin/js/exporters/list/modals/add.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       82 2024-05-13 16:06:25.000000 core_exporters_app-2.9.0/core_exporters_app/exporters/xsl/static/xsl/admin/js/exporters/list/modals/add.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:31.346889 core_exporters_app-2.9.0/core_exporters_app/exporters/xsl/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:31.350608 core_exporters_app-2.9.0/core_exporters_app/exporters/xsl/templates/xsl/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:31.357459 core_exporters_app-2.9.0/core_exporters_app/exporters/xsl/templates/xsl/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:31.361129 core_exporters_app-2.9.0/core_exporters_app/exporters/xsl/templates/xsl/admin/exporters/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:33.024567 core_exporters_app-2.9.0/core_exporters_app/exporters/xsl/templates/xsl/admin/exporters/list/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       40 2024-05-13 16:06:25.000000 core_exporters_app-2.9.0/core_exporters_app/exporters/xsl/templates/xsl/admin/exporters/list/add_base.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1965 2024-05-13 16:06:25.000000 core_exporters_app-2.9.0/core_exporters_app/exporters/xsl/templates/xsl/admin/exporters/list/list_base.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:33.045706 core_exporters_app-2.9.0/core_exporters_app/exporters/xsl/templates/xsl/admin/exporters/list/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1126 2024-05-13 16:06:25.000000 core_exporters_app-2.9.0/core_exporters_app/exporters/xsl/templates/xsl/admin/exporters/list/modals/add.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      336 2024-05-13 16:06:25.000000 core_exporters_app-2.9.0/core_exporters_app/exporters/xsl/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:33.078305 core_exporters_app-2.9.0/core_exporters_app/exporters/xsl/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:25.000000 core_exporters_app-2.9.0/core_exporters_app/exporters/xsl/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:33.149083 core_exporters_app-2.9.0/core_exporters_app/exporters/xsl/views/admin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:25.000000 core_exporters_app-2.9.0/core_exporters_app/exporters/xsl/views/admin/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3073 2024-05-13 16:06:25.000000 core_exporters_app-2.9.0/core_exporters_app/exporters/xsl/views/admin/ajax.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      833 2024-05-13 16:06:25.000000 core_exporters_app-2.9.0/core_exporters_app/exporters/xsl/views/admin/forms.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:33.191789 core_exporters_app-2.9.0/core_exporters_app/management/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:25.000000 core_exporters_app-2.9.0/core_exporters_app/management/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:33.246991 core_exporters_app-2.9.0/core_exporters_app/management/commands/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:25.000000 core_exporters_app-2.9.0/core_exporters_app/management/commands/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      582 2024-05-13 16:06:25.000000 core_exporters_app-2.9.0/core_exporters_app/management/commands/loadexporters.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      332 2024-05-13 16:06:25.000000 core_exporters_app-2.9.0/core_exporters_app/menus.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:33.288989 core_exporters_app-2.9.0/core_exporters_app/migrations/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3588 2024-05-13 16:06:25.000000 core_exporters_app-2.9.0/core_exporters_app/migrations/0001_initial.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:25.000000 core_exporters_app-2.9.0/core_exporters_app/migrations/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:33.340474 core_exporters_app-2.9.0/core_exporters_app/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:25.000000 core_exporters_app-2.9.0/core_exporters_app/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:33.362716 core_exporters_app-2.9.0/core_exporters_app/rest/export/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:25.000000 core_exporters_app-2.9.0/core_exporters_app/rest/export/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:33.429046 core_exporters_app-2.9.0/core_exporters_app/rest/export/data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:25.000000 core_exporters_app-2.9.0/core_exporters_app/rest/export/data/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6855 2024-05-13 16:06:25.000000 core_exporters_app-2.9.0/core_exporters_app/rest/export/data/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:33.500846 core_exporters_app-2.9.0/core_exporters_app/rest/exporters/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:25.000000 core_exporters_app-2.9.0/core_exporters_app/rest/exporters/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1967 2024-05-13 16:06:25.000000 core_exporters_app-2.9.0/core_exporters_app/rest/exporters/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8794 2024-05-13 16:06:25.000000 core_exporters_app-2.9.0/core_exporters_app/rest/exporters/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:33.544698 core_exporters_app-2.9.0/core_exporters_app/rest/exporters/xsl/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:25.000000 core_exporters_app-2.9.0/core_exporters_app/rest/exporters/xsl/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4291 2024-05-13 16:06:25.000000 core_exporters_app-2.9.0/core_exporters_app/rest/exporters/xsl/views.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1516 2024-05-13 16:06:25.000000 core_exporters_app-2.9.0/core_exporters_app/rest/urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      862 2024-05-13 16:06:25.000000 core_exporters_app-2.9.0/core_exporters_app/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:31.450997 core_exporters_app-2.9.0/core_exporters_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:31.494573 core_exporters_app-2.9.0/core_exporters_app/static/core_exporters_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:31.475325 core_exporters_app-2.9.0/core_exporters_app/static/core_exporters_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:31.462245 core_exporters_app-2.9.0/core_exporters_app/static/core_exporters_app/admin/css/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:31.465839 core_exporters_app-2.9.0/core_exporters_app/static/core_exporters_app/admin/css/exporters/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:33.588896 core_exporters_app-2.9.0/core_exporters_app/static/core_exporters_app/admin/css/exporters/list/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      115 2024-05-13 16:06:25.000000 core_exporters_app-2.9.0/core_exporters_app/static/core_exporters_app/admin/css/exporters/list/list_exporters.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:31.478776 core_exporters_app-2.9.0/core_exporters_app/static/core_exporters_app/admin/js/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:31.482992 core_exporters_app-2.9.0/core_exporters_app/static/core_exporters_app/admin/js/exporters/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:31.486618 core_exporters_app-2.9.0/core_exporters_app/static/core_exporters_app/admin/js/exporters/list/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:33.640013 core_exporters_app-2.9.0/core_exporters_app/static/core_exporters_app/admin/js/exporters/list/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1990 2024-05-13 16:06:25.000000 core_exporters_app-2.9.0/core_exporters_app/static/core_exporters_app/admin/js/exporters/list/modals/associated_templates.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      103 2024-05-13 16:06:25.000000 core_exporters_app-2.9.0/core_exporters_app/static/core_exporters_app/admin/js/exporters/list/modals/associated_templates.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:31.498046 core_exporters_app-2.9.0/core_exporters_app/static/core_exporters_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:31.509800 core_exporters_app-2.9.0/core_exporters_app/static/core_exporters_app/user/js/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:33.682367 core_exporters_app-2.9.0/core_exporters_app/static/core_exporters_app/user/js/exporter_compressed_file/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      962 2024-05-13 16:06:25.000000 core_exporters_app-2.9.0/core_exporters_app/static/core_exporters_app/user/js/exporter_compressed_file/download.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       82 2024-05-13 16:06:25.000000 core_exporters_app-2.9.0/core_exporters_app/static/core_exporters_app/user/js/exporter_compressed_file/download.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:31.513557 core_exporters_app-2.9.0/core_exporters_app/static/core_exporters_app/user/js/exporters/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:31.517074 core_exporters_app-2.9.0/core_exporters_app/static/core_exporters_app/user/js/exporters/list/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:33.777965 core_exporters_app-2.9.0/core_exporters_app/static/core_exporters_app/user/js/exporters/list/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5272 2024-05-13 16:06:25.000000 core_exporters_app-2.9.0/core_exporters_app/static/core_exporters_app/user/js/exporters/list/modals/list_exporters_selector.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      160 2024-05-13 16:06:25.000000 core_exporters_app-2.9.0/core_exporters_app/static/core_exporters_app/user/js/exporters/list/modals/list_exporters_selector.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:33.820391 core_exporters_app-2.9.0/core_exporters_app/system/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:25.000000 core_exporters_app-2.9.0/core_exporters_app/system/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      561 2024-05-13 16:06:25.000000 core_exporters_app-2.9.0/core_exporters_app/system/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3982 2024-05-13 16:06:25.000000 core_exporters_app-2.9.0/core_exporters_app/tasks.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:31.535805 core_exporters_app-2.9.0/core_exporters_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:31.572423 core_exporters_app-2.9.0/core_exporters_app/templates/core_exporters_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:31.543105 core_exporters_app-2.9.0/core_exporters_app/templates/core_exporters_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:33.853081 core_exporters_app-2.9.0/core_exporters_app/templates/core_exporters_app/admin/exporters/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:33.894608 core_exporters_app-2.9.0/core_exporters_app/templates/core_exporters_app/admin/exporters/list/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      338 2024-05-13 16:06:26.000000 core_exporters_app-2.9.0/core_exporters_app/templates/core_exporters_app/admin/exporters/list/associated_templates_base.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1620 2024-05-13 16:06:26.000000 core_exporters_app-2.9.0/core_exporters_app/templates/core_exporters_app/admin/exporters/list/list_base.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:33.916084 core_exporters_app-2.9.0/core_exporters_app/templates/core_exporters_app/admin/exporters/list/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1186 2024-05-13 16:06:26.000000 core_exporters_app-2.9.0/core_exporters_app/templates/core_exporters_app/admin/exporters/list/modals/associated_templates.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      324 2024-05-13 16:06:26.000000 core_exporters_app-2.9.0/core_exporters_app/templates/core_exporters_app/admin/exporters/list_exporters.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:31.593224 core_exporters_app-2.9.0/core_exporters_app/templates/core_exporters_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:33.959692 core_exporters_app-2.9.0/core_exporters_app/templates/core_exporters_app/user/exported_compressed_file/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      265 2024-05-13 16:06:26.000000 core_exporters_app-2.9.0/core_exporters_app/templates/core_exporters_app/user/exported_compressed_file/download.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:31.597290 core_exporters_app-2.9.0/core_exporters_app/templates/core_exporters_app/user/exporters/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:34.026490 core_exporters_app-2.9.0/core_exporters_app/templates/core_exporters_app/user/exporters/list/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       41 2024-05-13 16:06:26.000000 core_exporters_app-2.9.0/core_exporters_app/templates/core_exporters_app/user/exporters/list/link_exporters_selector.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       27 2024-05-13 16:06:26.000000 core_exporters_app-2.9.0/core_exporters_app/templates/core_exporters_app/user/exporters/list/list_exporters_selector_base.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:34.054462 core_exporters_app-2.9.0/core_exporters_app/templates/core_exporters_app/user/exporters/list/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1142 2024-05-13 16:06:26.000000 core_exporters_app-2.9.0/core_exporters_app/templates/core_exporters_app/user/exporters/list/modals/list_exporters_selector.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      922 2024-05-13 16:06:26.000000 core_exporters_app-2.9.0/core_exporters_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:34.076115 core_exporters_app-2.9.0/core_exporters_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:26.000000 core_exporters_app-2.9.0/core_exporters_app/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:34.169693 core_exporters_app-2.9.0/core_exporters_app/views/admin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:26.000000 core_exporters_app-2.9.0/core_exporters_app/views/admin/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3961 2024-05-13 16:06:26.000000 core_exporters_app-2.9.0/core_exporters_app/views/admin/ajax.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1526 2024-05-13 16:06:26.000000 core_exporters_app-2.9.0/core_exporters_app/views/admin/forms.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1650 2024-05-13 16:06:26.000000 core_exporters_app-2.9.0/core_exporters_app/views/admin/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:34.282188 core_exporters_app-2.9.0/core_exporters_app/views/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:26.000000 core_exporters_app-2.9.0/core_exporters_app/views/user/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7615 2024-05-13 16:06:26.000000 core_exporters_app-2.9.0/core_exporters_app/views/user/ajax.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3067 2024-05-13 16:06:26.000000 core_exporters_app-2.9.0/core_exporters_app/views/user/forms.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2122 2024-05-13 16:06:26.000000 core_exporters_app-2.9.0/core_exporters_app/views/user/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:32.158430 core_exporters_app-2.9.0/core_exporters_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1017 2024-05-13 16:06:30.000000 core_exporters_app-2.9.0/core_exporters_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6539 2024-05-13 16:06:31.000000 core_exporters_app-2.9.0/core_exporters_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2024-05-13 16:06:30.000000 core_exporters_app-2.9.0/core_exporters_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      114 2024-05-13 16:06:30.000000 core_exporters_app-2.9.0/core_exporters_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       30 2024-05-13 16:06:30.000000 core_exporters_app-2.9.0/core_exporters_app.egg-info/top_level.txt
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:34.377248 core_exporters_app-2.9.0/docs/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:26.000000 core_exporters_app-2.9.0/docs/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11096 2024-05-13 16:06:26.000000 core_exporters_app-2.9.0/docs/conf.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      292 2024-05-13 16:06:26.000000 core_exporters_app-2.9.0/docs/conf_urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2024-05-13 16:06:27.000000 core_exporters_app-2.9.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       52 2024-05-13 16:06:27.000000 core_exporters_app-2.9.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       62 2024-05-13 16:06:27.000000 core_exporters_app-2.9.0/requirements.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2024-05-13 16:06:35.477386 core_exporters_app-2.9.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1393 2024-05-13 16:06:27.000000 core_exporters_app-2.9.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:34.452745 core_exporters_app-2.9.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:27.000000 core_exporters_app-2.9.0/tests/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:34.495855 core_exporters_app-2.9.0/tests/commands/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:27.000000 core_exporters_app-2.9.0/tests/commands/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      414 2024-05-13 16:06:27.000000 core_exporters_app-2.9.0/tests/commands/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:34.553833 core_exporters_app-2.9.0/tests/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:27.000000 core_exporters_app-2.9.0/tests/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:34.598320 core_exporters_app-2.9.0/tests/components/exported_compressed_file/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:27.000000 core_exporters_app-2.9.0/tests/components/exported_compressed_file/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:34.638854 core_exporters_app-2.9.0/tests/components/exported_compressed_file/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:27.000000 core_exporters_app-2.9.0/tests/components/exported_compressed_file/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1744 2024-05-13 16:06:27.000000 core_exporters_app-2.9.0/tests/components/exported_compressed_file/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6477 2024-05-13 16:06:27.000000 core_exporters_app-2.9.0/tests/components/exported_compressed_file/tests_int.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:34.677904 core_exporters_app-2.9.0/tests/components/exporter/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:27.000000 core_exporters_app-2.9.0/tests/components/exporter/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5848 2024-05-13 16:06:27.000000 core_exporters_app-2.9.0/tests/components/exporter/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:34.750900 core_exporters_app-2.9.0/tests/discover/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:27.000000 core_exporters_app-2.9.0/tests/discover/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1374 2024-05-13 16:06:27.000000 core_exporters_app-2.9.0/tests/discover/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:34.770578 core_exporters_app-2.9.0/tests/exporters/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:27.000000 core_exporters_app-2.9.0/tests/exporters/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:34.820015 core_exporters_app-2.9.0/tests/exporters/blob/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:27.000000 core_exporters_app-2.9.0/tests/exporters/blob/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      827 2024-05-13 16:06:27.000000 core_exporters_app-2.9.0/tests/exporters/blob/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:34.841014 core_exporters_app-2.9.0/tests/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:27.000000 core_exporters_app-2.9.0/tests/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:34.922725 core_exporters_app-2.9.0/tests/rest/export/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:27.000000 core_exporters_app-2.9.0/tests/rest/export/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:34.968508 core_exporters_app-2.9.0/tests/rest/export/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:27.000000 core_exporters_app-2.9.0/tests/rest/export/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2524 2024-05-13 16:06:27.000000 core_exporters_app-2.9.0/tests/rest/export/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8721 2024-05-13 16:06:27.000000 core_exporters_app-2.9.0/tests/rest/export/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7069 2024-05-13 16:06:27.000000 core_exporters_app-2.9.0/tests/rest/export/tests_permissions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5042 2024-05-13 16:06:27.000000 core_exporters_app-2.9.0/tests/rest/export/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:35.051011 core_exporters_app-2.9.0/tests/rest/exporter/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:27.000000 core_exporters_app-2.9.0/tests/rest/exporter/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:35.100382 core_exporters_app-2.9.0/tests/rest/exporter/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:27.000000 core_exporters_app-2.9.0/tests/rest/exporter/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      877 2024-05-13 16:06:27.000000 core_exporters_app-2.9.0/tests/rest/exporter/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4051 2024-05-13 16:06:27.000000 core_exporters_app-2.9.0/tests/rest/exporter/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8034 2024-05-13 16:06:27.000000 core_exporters_app-2.9.0/tests/rest/exporter/tests_permissions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1051 2024-05-13 16:06:27.000000 core_exporters_app-2.9.0/tests/rest/exporter/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:35.147346 core_exporters_app-2.9.0/tests/rest/exporter/xsl/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:27.000000 core_exporters_app-2.9.0/tests/rest/exporter/xsl/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5101 2024-05-13 16:06:27.000000 core_exporters_app-2.9.0/tests/rest/exporter/xsl/tests_permissions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1635 2024-05-13 16:06:27.000000 core_exporters_app-2.9.0/tests/test_settings.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       17 2024-05-13 16:06:27.000000 core_exporters_app-2.9.0/tests/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:35.169046 core_exporters_app-2.9.0/tests/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:27.000000 core_exporters_app-2.9.0/tests/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:35.195307 core_exporters_app-2.9.0/tests/views/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:27.000000 core_exporters_app-2.9.0/tests/views/user/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:35.251037 core_exporters_app-2.9.0/tests/views/user/ajax/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:27.000000 core_exporters_app-2.9.0/tests/views/user/ajax/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      925 2024-05-13 16:06:27.000000 core_exporters_app-2.9.0/tests/views/user/ajax/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:35.445963 core_exporters_app-2.9.0/tests/views/user/forms/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:06:27.000000 core_exporters_app-2.9.0/tests/views/user/forms/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2627 2024-05-13 16:06:27.000000 core_exporters_app-2.9.0/tests/views/user/forms/test_unit.py
```

### Comparing `core_exporters_app-2.8.0/LICENSE.md` & `core_exporters_app-2.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.8.0/PKG-INFO` & `core_exporters_app-2.9.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_exporters_app
-Version: 2.8.0
+Version: 2.9.0
 Summary: Exporters for the curator core project
 Home-page: https://github.com/usnistgov/core_exporters_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: ==================
         Core Exporters App
```

### Comparing `core_exporters_app-2.8.0/README.rst` & `core_exporters_app-2.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.8.0/core_exporters_app/access_control/api.py` & `core_exporters_app-2.9.0/core_exporters_app/access_control/api.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.8.0/core_exporters_app/admin.py` & `core_exporters_app-2.9.0/core_exporters_app/admin.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.8.0/core_exporters_app/apps.py` & `core_exporters_app-2.9.0/core_exporters_app/apps.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 """ Core exporters apps config
 """
 import sys
 
 from django.apps import AppConfig
 
 
-# TODO: loaded two times (not a problem and may not happen in production)
-# see http://stackoverflow.com/a/16111968
 class CoreExportersAppConfig(AppConfig):
     """Exporters configuration"""
 
     name = "core_exporters_app"
     verbose_name = "Core Exporters App"
 
     def ready(self):
         """Run once at startup"""
         if "migrate" not in sys.argv:
             import core_exporters_app.components.exporter.watch as exporter_watch
             from core_exporters_app.exporters import discover
-            from core_exporters_app.exporters import urls
 
             discover.init_periodic_tasks()
-            discover.discover_exporter(urls.urlpatterns)
             exporter_watch.init()
```

### Comparing `core_exporters_app-2.8.0/core_exporters_app/components/exported_compressed_file/api.py` & `core_exporters_app-2.9.0/core_exporters_app/components/exported_compressed_file/api.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.8.0/core_exporters_app/components/exported_compressed_file/models.py` & `core_exporters_app-2.9.0/core_exporters_app/components/exported_compressed_file/models.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.8.0/core_exporters_app/components/exporter/api.py` & `core_exporters_app-2.9.0/core_exporters_app/components/exporter/api.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.8.0/core_exporters_app/components/exporter/models.py` & `core_exporters_app-2.9.0/core_exporters_app/components/exporter/models.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.8.0/core_exporters_app/components/exporter/watch.py` & `core_exporters_app-2.9.0/core_exporters_app/components/exporter/watch.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.8.0/core_exporters_app/exporters/blob/models.py` & `core_exporters_app-2.9.0/core_exporters_app/exporters/blob/models.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.8.0/core_exporters_app/exporters/discover.py` & `core_exporters_app-2.9.0/core_exporters_app/exporters/discover.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,15 +106,16 @@
                     if exporter_added.enable_by_default is True:
                         exporter_added.templates.set(
                             system_api.get_all_templates()
                         )
             except Exception as exception:
                 logger.error(
                     "Impossible to load the following exporter, class %s not found, exception: %s",
-                    (pattern["view"], str(exception)),
+                    pattern["view"],
+                    str(exception),
                 )
     except ValidationError as exception:
         raise Exception(
             f"A validation error occurred during the exporter discovery: {str(exception)}"
         )
     except Exception as exception:
         raise exception
```

### Comparing `core_exporters_app-2.8.0/core_exporters_app/exporters/exporter.py` & `core_exporters_app-2.9.0/core_exporters_app/exporters/exporter.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.8.0/core_exporters_app/exporters/json_exporter/models.py` & `core_exporters_app-2.9.0/core_exporters_app/exporters/json_exporter/models.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.8.0/core_exporters_app/exporters/xml/models.py` & `core_exporters_app-2.9.0/core_exporters_app/exporters/xml/models.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.8.0/core_exporters_app/exporters/xsl/api.py` & `core_exporters_app-2.9.0/core_exporters_app/exporters/xsl/api.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.8.0/core_exporters_app/exporters/xsl/models.py` & `core_exporters_app-2.9.0/core_exporters_app/exporters/xsl/models.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.8.0/core_exporters_app/exporters/xsl/static/xsl/admin/js/exporters/list/modals/add.js` & `core_exporters_app-2.9.0/core_exporters_app/exporters/xsl/static/xsl/admin/js/exporters/list/modals/add.js`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.8.0/core_exporters_app/exporters/xsl/templates/xsl/admin/exporters/list/list_base.html` & `core_exporters_app-2.9.0/core_exporters_app/exporters/xsl/templates/xsl/admin/exporters/list/list_base.html`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.8.0/core_exporters_app/exporters/xsl/templates/xsl/admin/exporters/list/modals/add.html` & `core_exporters_app-2.9.0/core_exporters_app/exporters/xsl/templates/xsl/admin/exporters/list/modals/add.html`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.8.0/core_exporters_app/exporters/xsl/views/admin/ajax.py` & `core_exporters_app-2.9.0/core_exporters_app/exporters/xsl/views/admin/ajax.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.8.0/core_exporters_app/exporters/xsl/views/admin/forms.py` & `core_exporters_app-2.9.0/core_exporters_app/exporters/xsl/views/admin/forms.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.8.0/core_exporters_app/migrations/0001_initial.py` & `core_exporters_app-2.9.0/core_exporters_app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.8.0/core_exporters_app/rest/export/data/views.py` & `core_exporters_app-2.9.0/core_exporters_app/rest/export/data/views.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.8.0/core_exporters_app/rest/exporters/serializers.py` & `core_exporters_app-2.9.0/core_exporters_app/rest/exporters/serializers.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.8.0/core_exporters_app/rest/exporters/views.py` & `core_exporters_app-2.9.0/core_exporters_app/rest/exporters/views.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.8.0/core_exporters_app/rest/exporters/xsl/views.py` & `core_exporters_app-2.9.0/core_exporters_app/rest/exporters/xsl/views.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.8.0/core_exporters_app/rest/urls.py` & `core_exporters_app-2.9.0/core_exporters_app/rest/urls.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.8.0/core_exporters_app/settings.py` & `core_exporters_app-2.9.0/core_exporters_app/settings.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.8.0/core_exporters_app/static/core_exporters_app/admin/js/exporters/list/modals/associated_templates.js` & `core_exporters_app-2.9.0/core_exporters_app/static/core_exporters_app/admin/js/exporters/list/modals/associated_templates.js`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.8.0/core_exporters_app/static/core_exporters_app/user/js/exporter_compressed_file/download.js` & `core_exporters_app-2.9.0/core_exporters_app/static/core_exporters_app/user/js/exporter_compressed_file/download.js`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.8.0/core_exporters_app/static/core_exporters_app/user/js/exporters/list/modals/list_exporters_selector.js` & `core_exporters_app-2.9.0/core_exporters_app/static/core_exporters_app/user/js/exporters/list/modals/list_exporters_selector.js`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.8.0/core_exporters_app/system/api.py` & `core_exporters_app-2.9.0/core_exporters_app/system/api.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.8.0/core_exporters_app/tasks.py` & `core_exporters_app-2.9.0/core_exporters_app/tasks.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.8.0/core_exporters_app/templates/core_exporters_app/admin/exporters/list/list_base.html` & `core_exporters_app-2.9.0/core_exporters_app/templates/core_exporters_app/admin/exporters/list/list_base.html`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.8.0/core_exporters_app/templates/core_exporters_app/admin/exporters/list/modals/associated_templates.html` & `core_exporters_app-2.9.0/core_exporters_app/templates/core_exporters_app/admin/exporters/list/modals/associated_templates.html`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.8.0/core_exporters_app/templates/core_exporters_app/user/exporters/list/modals/list_exporters_selector.html` & `core_exporters_app-2.9.0/core_exporters_app/templates/core_exporters_app/user/exporters/list/modals/list_exporters_selector.html`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.8.0/core_exporters_app/urls.py` & `core_exporters_app-2.9.0/core_exporters_app/urls.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.8.0/core_exporters_app/views/admin/ajax.py` & `core_exporters_app-2.9.0/core_exporters_app/views/admin/ajax.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 class EditExporterView(EditObjectModalView):
     """Edit Exporter View"""
 
     form_class = EditExporterForm
     model = Exporter
     success_url = reverse_lazy("core-admin:core_exporters_app_exporters")
-    success_message = "Exporter edited with success."
+    success_message = "Exporter edited."
 
     def _save(self, form):
         # Save treatment.
         try:
             exporter_api.upsert(self.object)
         except Exception as exception:
             form.add_error(None, str(exception))
```

### Comparing `core_exporters_app-2.8.0/core_exporters_app/views/admin/forms.py` & `core_exporters_app-2.9.0/core_exporters_app/views/admin/forms.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.8.0/core_exporters_app/views/admin/views.py` & `core_exporters_app-2.9.0/core_exporters_app/views/admin/views.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.8.0/core_exporters_app/views/user/ajax.py` & `core_exporters_app-2.9.0/core_exporters_app/views/user/ajax.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.8.0/core_exporters_app/views/user/forms.py` & `core_exporters_app-2.9.0/core_exporters_app/views/user/forms.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.8.0/core_exporters_app/views/user/views.py` & `core_exporters_app-2.9.0/core_exporters_app/views/user/views.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.8.0/core_exporters_app.egg-info/PKG-INFO` & `core_exporters_app-2.9.0/core_exporters_app.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-exporters-app
-Version: 2.8.0
+Version: 2.9.0
 Summary: Exporters for the curator core project
 Home-page: https://github.com/usnistgov/core_exporters_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: ==================
         Core Exporters App
```

### Comparing `core_exporters_app-2.8.0/core_exporters_app.egg-info/SOURCES.txt` & `core_exporters_app-2.9.0/core_exporters_app.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,17 @@
 core_exporters_app/exporters/xsl/templates/xsl/admin/exporters/list/add_base.html
 core_exporters_app/exporters/xsl/templates/xsl/admin/exporters/list/list_base.html
 core_exporters_app/exporters/xsl/templates/xsl/admin/exporters/list/modals/add.html
 core_exporters_app/exporters/xsl/views/__init__.py
 core_exporters_app/exporters/xsl/views/admin/__init__.py
 core_exporters_app/exporters/xsl/views/admin/ajax.py
 core_exporters_app/exporters/xsl/views/admin/forms.py
+core_exporters_app/management/__init__.py
+core_exporters_app/management/commands/__init__.py
+core_exporters_app/management/commands/loadexporters.py
 core_exporters_app/migrations/0001_initial.py
 core_exporters_app/migrations/__init__.py
 core_exporters_app/rest/__init__.py
 core_exporters_app/rest/urls.py
 core_exporters_app/rest/export/__init__.py
 core_exporters_app/rest/export/data/__init__.py
 core_exporters_app/rest/export/data/views.py
@@ -96,21 +99,26 @@
 core_exporters_app/views/user/forms.py
 core_exporters_app/views/user/views.py
 docs/__init__.py
 docs/conf.py
 docs/conf_urls.py
 tests/__init__.py
 tests/test_settings.py
+tests/urls.py
+tests/commands/__init__.py
+tests/commands/tests_unit.py
 tests/components/__init__.py
 tests/components/exported_compressed_file/__init__.py
 tests/components/exported_compressed_file/tests_int.py
 tests/components/exported_compressed_file/fixtures/__init__.py
 tests/components/exported_compressed_file/fixtures/fixtures.py
 tests/components/exporter/__init__.py
 tests/components/exporter/tests_unit.py
+tests/discover/__init__.py
+tests/discover/tests_unit.py
 tests/exporters/__init__.py
 tests/exporters/blob/__init__.py
 tests/exporters/blob/test_unit.py
 tests/rest/__init__.py
 tests/rest/export/__init__.py
 tests/rest/export/tests_int.py
 tests/rest/export/tests_permissions.py
```

### Comparing `core_exporters_app-2.8.0/docs/conf.py` & `core_exporters_app-2.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.8.0/setup.py` & `core_exporters_app-2.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_exporters_app",
-    version="2.8.0",
+    version="2.9.0",
     description="Exporters for the curator core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_exporters_app",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `core_exporters_app-2.8.0/tests/components/exported_compressed_file/fixtures/fixtures.py` & `core_exporters_app-2.9.0/tests/components/exported_compressed_file/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.8.0/tests/components/exported_compressed_file/tests_int.py` & `core_exporters_app-2.9.0/tests/components/exported_compressed_file/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.8.0/tests/components/exporter/tests_unit.py` & `core_exporters_app-2.9.0/tests/components/exporter/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.8.0/tests/exporters/blob/test_unit.py` & `core_exporters_app-2.9.0/tests/exporters/blob/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.8.0/tests/rest/export/fixtures/fixtures.py` & `core_exporters_app-2.9.0/tests/rest/export/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.8.0/tests/rest/export/tests_int.py` & `core_exporters_app-2.9.0/tests/rest/export/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.8.0/tests/rest/export/tests_permissions.py` & `core_exporters_app-2.9.0/tests/rest/export/tests_permissions.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.8.0/tests/rest/export/tests_unit.py` & `core_exporters_app-2.9.0/tests/rest/export/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.8.0/tests/rest/exporter/fixtures/fixtures.py` & `core_exporters_app-2.9.0/tests/rest/exporter/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.8.0/tests/rest/exporter/tests_int.py` & `core_exporters_app-2.9.0/tests/rest/exporter/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.8.0/tests/rest/exporter/tests_permissions.py` & `core_exporters_app-2.9.0/tests/rest/exporter/tests_permissions.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.8.0/tests/rest/exporter/tests_unit.py` & `core_exporters_app-2.9.0/tests/rest/exporter/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.8.0/tests/rest/exporter/xsl/tests_permissions.py` & `core_exporters_app-2.9.0/tests/rest/exporter/xsl/tests_permissions.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.8.0/tests/test_settings.py` & `core_exporters_app-2.9.0/tests/test_settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,7 +55,9 @@
 
 DEFAULT_AUTO_FIELD = "django.db.models.AutoField"
 CAN_ANONYMOUS_ACCESS_PUBLIC_DOCUMENT = False
 CELERYBEAT_SCHEDULER = "django_celery_beat.schedulers:DatabaseScheduler"
 
 MONGODB_INDEXING = False
 MONGODB_ASYNC_SAVE = False
+
+ROOT_URLCONF = "tests.urls"
```

### Comparing `core_exporters_app-2.8.0/tests/views/user/ajax/test_unit.py` & `core_exporters_app-2.9.0/tests/views/user/ajax/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_exporters_app-2.8.0/tests/views/user/forms/test_unit.py` & `core_exporters_app-2.9.0/tests/views/user/forms/test_unit.py`

 * *Files identical despite different names*

