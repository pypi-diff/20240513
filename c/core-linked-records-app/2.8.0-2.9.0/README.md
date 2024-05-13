# Comparing `tmp/core_linked_records_app-2.8.0.tar.gz` & `tmp/core_linked_records_app-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_linked_records_app-2.8.0.tar", last modified: Tue Mar 12 19:01:50 2024, max compression
+gzip compressed data, was "core_linked_records_app-2.9.0.tar", last modified: Mon May 13 16:07:29 2024, max compression
```

## Comparing `core_linked_records_app-2.8.0.tar` & `core_linked_records_app-2.9.0.tar`

### file list

```diff
@@ -1,376 +1,376 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:50.120289 core_linked_records_app-2.8.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2024-03-12 19:01:36.000000 core_linked_records_app-2.8.0/LICENSE.md
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      179 2024-03-12 19:01:36.000000 core_linked_records_app-2.8.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6496 2024-03-12 19:01:50.113846 core_linked_records_app-2.8.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4718 2024-03-12 19:01:36.000000 core_linked_records_app-2.8.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:44.460308 core_linked_records_app-2.8.0/core_linked_records_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      122 2024-03-12 19:01:36.000000 core_linked_records_app-2.8.0/core_linked_records_app/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:44.590005 core_linked_records_app-2.8.0/core_linked_records_app/access_control/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:36.000000 core_linked_records_app-2.8.0/core_linked_records_app/access_control/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1028 2024-03-12 19:01:36.000000 core_linked_records_app-2.8.0/core_linked_records_app/access_control/discover.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      134 2024-03-12 19:01:36.000000 core_linked_records_app-2.8.0/core_linked_records_app/access_control/rights.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1220 2024-03-12 19:01:36.000000 core_linked_records_app-2.8.0/core_linked_records_app/admin.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1218 2024-03-12 19:01:36.000000 core_linked_records_app-2.8.0/core_linked_records_app/apps.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:44.612188 core_linked_records_app-2.8.0/core_linked_records_app/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:36.000000 core_linked_records_app-2.8.0/core_linked_records_app/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:44.690933 core_linked_records_app-2.8.0/core_linked_records_app/components/blob/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:36.000000 core_linked_records_app-2.8.0/core_linked_records_app/components/blob/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1639 2024-03-12 19:01:36.000000 core_linked_records_app-2.8.0/core_linked_records_app/components/blob/access_control.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3910 2024-03-12 19:01:36.000000 core_linked_records_app-2.8.0/core_linked_records_app/components/blob/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6038 2024-03-12 19:01:36.000000 core_linked_records_app-2.8.0/core_linked_records_app/components/blob/watch.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:44.767300 core_linked_records_app-2.8.0/core_linked_records_app/components/data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:36.000000 core_linked_records_app-2.8.0/core_linked_records_app/components/data/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      859 2024-03-12 19:01:36.000000 core_linked_records_app-2.8.0/core_linked_records_app/components/data/access_control.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3457 2024-03-12 19:01:36.000000 core_linked_records_app-2.8.0/core_linked_records_app/components/data/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7306 2024-03-12 19:01:36.000000 core_linked_records_app-2.8.0/core_linked_records_app/components/data/watch.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:44.829426 core_linked_records_app-2.8.0/core_linked_records_app/components/local_id/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:36.000000 core_linked_records_app-2.8.0/core_linked_records_app/components/local_id/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      477 2024-03-12 19:01:36.000000 core_linked_records_app-2.8.0/core_linked_records_app/components/local_id/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2692 2024-03-12 19:01:36.000000 core_linked_records_app-2.8.0/core_linked_records_app/components/local_id/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:44.892761 core_linked_records_app-2.8.0/core_linked_records_app/components/oai_record/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:36.000000 core_linked_records_app-2.8.0/core_linked_records_app/components/oai_record/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      437 2024-03-12 19:01:36.000000 core_linked_records_app-2.8.0/core_linked_records_app/components/oai_record/access_control.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1492 2024-03-12 19:01:36.000000 core_linked_records_app-2.8.0/core_linked_records_app/components/oai_record/api.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:45.000701 core_linked_records_app-2.8.0/core_linked_records_app/components/pid_path/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:36.000000 core_linked_records_app-2.8.0/core_linked_records_app/components/pid_path/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      452 2024-03-12 19:01:36.000000 core_linked_records_app-2.8.0/core_linked_records_app/components/pid_path/access_control.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      196 2024-03-12 19:01:36.000000 core_linked_records_app-2.8.0/core_linked_records_app/components/pid_path/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2019 2024-03-12 19:01:36.000000 core_linked_records_app-2.8.0/core_linked_records_app/components/pid_path/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2116 2024-03-12 19:01:36.000000 core_linked_records_app-2.8.0/core_linked_records_app/components/pid_path/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:45.143540 core_linked_records_app-2.8.0/core_linked_records_app/components/pid_settings/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:36.000000 core_linked_records_app-2.8.0/core_linked_records_app/components/pid_settings/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1046 2024-03-12 19:01:36.000000 core_linked_records_app-2.8.0/core_linked_records_app/components/pid_settings/access_control.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      482 2024-03-12 19:01:36.000000 core_linked_records_app-2.8.0/core_linked_records_app/components/pid_settings/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      981 2024-03-12 19:01:36.000000 core_linked_records_app-2.8.0/core_linked_records_app/components/pid_settings/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      919 2024-03-12 19:01:36.000000 core_linked_records_app-2.8.0/core_linked_records_app/components/pid_settings/models.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      687 2024-03-12 19:01:36.000000 core_linked_records_app-2.8.0/core_linked_records_app/components/pid_settings/watch.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      470 2024-03-12 19:01:36.000000 core_linked_records_app-2.8.0/core_linked_records_app/menus.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:45.235843 core_linked_records_app-2.8.0/core_linked_records_app/migrations/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2838 2024-03-12 19:01:36.000000 core_linked_records_app-2.8.0/core_linked_records_app/migrations/0001_initial.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      660 2024-03-12 19:01:36.000000 core_linked_records_app-2.8.0/core_linked_records_app/migrations/0002_alter_pidxpath_xpath.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1008 2024-03-12 19:01:36.000000 core_linked_records_app-2.8.0/core_linked_records_app/migrations/0003_create_permissions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      439 2024-03-12 19:01:36.000000 core_linked_records_app-2.8.0/core_linked_records_app/migrations/0004_rename_pidxpath_to_pidpath.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:36.000000 core_linked_records_app-2.8.0/core_linked_records_app/migrations/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      533 2024-03-12 19:01:36.000000 core_linked_records_app-2.8.0/core_linked_records_app/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:45.281917 core_linked_records_app-2.8.0/core_linked_records_app/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:36.000000 core_linked_records_app-2.8.0/core_linked_records_app/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:45.323070 core_linked_records_app-2.8.0/core_linked_records_app/rest/blob/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:36.000000 core_linked_records_app-2.8.0/core_linked_records_app/rest/blob/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2549 2024-03-12 19:01:36.000000 core_linked_records_app-2.8.0/core_linked_records_app/rest/blob/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:45.343256 core_linked_records_app-2.8.0/core_linked_records_app/rest/data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:36.000000 core_linked_records_app-2.8.0/core_linked_records_app/rest/data/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:45.400617 core_linked_records_app-2.8.0/core_linked_records_app/rest/data/renderers/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:36.000000 core_linked_records_app-2.8.0/core_linked_records_app/rest/data/renderers/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3495 2024-03-12 19:01:36.000000 core_linked_records_app-2.8.0/core_linked_records_app/rest/data/renderers/data_html_user_renderer.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1146 2024-03-12 19:01:36.000000 core_linked_records_app-2.8.0/core_linked_records_app/rest/data/renderers/data_xml_renderer.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:45.454638 core_linked_records_app-2.8.0/core_linked_records_app/rest/pid/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:36.000000 core_linked_records_app-2.8.0/core_linked_records_app/rest/pid/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      467 2024-03-12 19:01:36.000000 core_linked_records_app-2.8.0/core_linked_records_app/rest/pid/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8350 2024-03-12 19:01:36.000000 core_linked_records_app-2.8.0/core_linked_records_app/rest/pid/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:45.533730 core_linked_records_app-2.8.0/core_linked_records_app/rest/pid_path/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:36.000000 core_linked_records_app-2.8.0/core_linked_records_app/rest/pid_path/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      359 2024-03-12 19:01:36.000000 core_linked_records_app-2.8.0/core_linked_records_app/rest/pid_path/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      828 2024-03-12 19:01:36.000000 core_linked_records_app-2.8.0/core_linked_records_app/rest/pid_path/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:45.798859 core_linked_records_app-2.8.0/core_linked_records_app/rest/pid_settings/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:36.000000 core_linked_records_app-2.8.0/core_linked_records_app/rest/pid_settings/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      847 2024-03-12 19:01:36.000000 core_linked_records_app-2.8.0/core_linked_records_app/rest/pid_settings/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2565 2024-03-12 19:01:36.000000 core_linked_records_app-2.8.0/core_linked_records_app/rest/pid_settings/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:45.839369 core_linked_records_app-2.8.0/core_linked_records_app/rest/providers/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:36.000000 core_linked_records_app-2.8.0/core_linked_records_app/rest/providers/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7029 2024-03-12 19:01:36.000000 core_linked_records_app-2.8.0/core_linked_records_app/rest/providers/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:45.871992 core_linked_records_app-2.8.0/core_linked_records_app/rest/query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:36.000000 core_linked_records_app-2.8.0/core_linked_records_app/rest/query/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      736 2024-03-12 19:01:36.000000 core_linked_records_app-2.8.0/core_linked_records_app/rest/query/views.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1964 2024-03-12 19:01:36.000000 core_linked_records_app-2.8.0/core_linked_records_app/rest/urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1971 2024-03-12 19:01:36.000000 core_linked_records_app-2.8.0/core_linked_records_app/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:43.580282 core_linked_records_app-2.8.0/core_linked_records_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:43.611021 core_linked_records_app-2.8.0/core_linked_records_app/static/core_linked_records_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:43.595894 core_linked_records_app-2.8.0/core_linked_records_app/static/core_linked_records_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:45.896154 core_linked_records_app-2.8.0/core_linked_records_app/static/core_linked_records_app/admin/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       72 2024-03-12 19:01:36.000000 core_linked_records_app-2.8.0/core_linked_records_app/static/core_linked_records_app/admin/css/pid_settings.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:43.599756 core_linked_records_app-2.8.0/core_linked_records_app/static/core_linked_records_app/admin/js/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:45.917083 core_linked_records_app-2.8.0/core_linked_records_app/static/core_linked_records_app/admin/js/pid_settings/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1683 2024-03-12 19:01:36.000000 core_linked_records_app-2.8.0/core_linked_records_app/static/core_linked_records_app/admin/js/pid_settings/auto_set_pid.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:43.623097 core_linked_records_app-2.8.0/core_linked_records_app/static/core_linked_records_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:46.167326 core_linked_records_app-2.8.0/core_linked_records_app/static/core_linked_records_app/user/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       43 2024-03-12 19:01:36.000000 core_linked_records_app-2.8.0/core_linked_records_app/static/core_linked_records_app/user/css/sharing.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:43.626977 core_linked_records_app-2.8.0/core_linked_records_app/static/core_linked_records_app/user/js/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:46.310226 core_linked_records_app-2.8.0/core_linked_records_app/static/core_linked_records_app/user/js/sharing/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      494 2024-03-12 19:01:36.000000 core_linked_records_app-2.8.0/core_linked_records_app/static/core_linked_records_app/user/js/sharing/blob_list.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       78 2024-03-12 19:01:36.000000 core_linked_records_app-2.8.0/core_linked_records_app/static/core_linked_records_app/user/js/sharing/blob_list.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      735 2024-03-12 19:01:36.000000 core_linked_records_app-2.8.0/core_linked_records_app/static/core_linked_records_app/user/js/sharing/common_list.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1199 2024-03-12 19:01:36.000000 core_linked_records_app-2.8.0/core_linked_records_app/static/core_linked_records_app/user/js/sharing/data_detail.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      236 2024-03-12 19:01:36.000000 core_linked_records_app-2.8.0/core_linked_records_app/static/core_linked_records_app/user/js/sharing/data_detail.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      494 2024-03-12 19:01:36.000000 core_linked_records_app-2.8.0/core_linked_records_app/static/core_linked_records_app/user/js/sharing/data_list.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       78 2024-03-12 19:01:36.000000 core_linked_records_app-2.8.0/core_linked_records_app/static/core_linked_records_app/user/js/sharing/data_list.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1309 2024-03-12 19:01:36.000000 core_linked_records_app-2.8.0/core_linked_records_app/static/core_linked_records_app/user/js/sharing/explore.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       78 2024-03-12 19:01:36.000000 core_linked_records_app-2.8.0/core_linked_records_app/static/core_linked_records_app/user/js/sharing/explore.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:46.325542 core_linked_records_app-2.8.0/core_linked_records_app/system/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:37.000000 core_linked_records_app-2.8.0/core_linked_records_app/system/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:46.358945 core_linked_records_app-2.8.0/core_linked_records_app/system/blob/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:37.000000 core_linked_records_app-2.8.0/core_linked_records_app/system/blob/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5201 2024-03-12 19:01:37.000000 core_linked_records_app-2.8.0/core_linked_records_app/system/blob/api.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:46.393904 core_linked_records_app-2.8.0/core_linked_records_app/system/data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:37.000000 core_linked_records_app-2.8.0/core_linked_records_app/system/data/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5172 2024-03-12 19:01:37.000000 core_linked_records_app-2.8.0/core_linked_records_app/system/data/api.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:46.432132 core_linked_records_app-2.8.0/core_linked_records_app/system/local_id/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:37.000000 core_linked_records_app-2.8.0/core_linked_records_app/system/local_id/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2208 2024-03-12 19:01:37.000000 core_linked_records_app-2.8.0/core_linked_records_app/system/local_id/api.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:46.471513 core_linked_records_app-2.8.0/core_linked_records_app/system/pid_path/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:37.000000 core_linked_records_app-2.8.0/core_linked_records_app/system/pid_path/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      631 2024-03-12 19:01:37.000000 core_linked_records_app-2.8.0/core_linked_records_app/system/pid_path/api.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:46.506590 core_linked_records_app-2.8.0/core_linked_records_app/system/pid_settings/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:37.000000 core_linked_records_app-2.8.0/core_linked_records_app/system/pid_settings/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1127 2024-03-12 19:01:37.000000 core_linked_records_app-2.8.0/core_linked_records_app/system/pid_settings/api.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:43.673542 core_linked_records_app-2.8.0/core_linked_records_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:43.698462 core_linked_records_app-2.8.0/core_linked_records_app/templates/core_linked_records_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:46.545834 core_linked_records_app-2.8.0/core_linked_records_app/templates/core_linked_records_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:46.563615 core_linked_records_app-2.8.0/core_linked_records_app/templates/core_linked_records_app/admin/pid_settings/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3190 2024-03-12 19:01:37.000000 core_linked_records_app-2.8.0/core_linked_records_app/templates/core_linked_records_app/admin/pid_settings/box.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      233 2024-03-12 19:01:37.000000 core_linked_records_app-2.8.0/core_linked_records_app/templates/core_linked_records_app/admin/pid_settings.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      290 2024-03-12 19:01:37.000000 core_linked_records_app-2.8.0/core_linked_records_app/templates/core_linked_records_app/admin/pid_settings_error.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:43.702595 core_linked_records_app-2.8.0/core_linked_records_app/templates/core_linked_records_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:43.712550 core_linked_records_app-2.8.0/core_linked_records_app/templates/core_linked_records_app/user/sharing/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:46.629702 core_linked_records_app-2.8.0/core_linked_records_app/templates/core_linked_records_app/user/sharing/data_detail/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      359 2024-03-12 19:01:37.000000 core_linked_records_app-2.8.0/core_linked_records_app/templates/core_linked_records_app/user/sharing/data_detail/button.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      236 2024-03-12 19:01:37.000000 core_linked_records_app-2.8.0/core_linked_records_app/templates/core_linked_records_app/user/sharing/data_detail/button_inline.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      283 2024-03-12 19:01:37.000000 core_linked_records_app-2.8.0/core_linked_records_app/templates/core_linked_records_app/user/sharing/data_detail/modal.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:46.665413 core_linked_records_app-2.8.0/core_linked_records_app/templates/core_linked_records_app/user/sharing/explore/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      246 2024-03-12 19:01:37.000000 core_linked_records_app-2.8.0/core_linked_records_app/templates/core_linked_records_app/user/sharing/explore/button.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      298 2024-03-12 19:01:37.000000 core_linked_records_app-2.8.0/core_linked_records_app/templates/core_linked_records_app/user/sharing/explore/modal.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      208 2024-03-12 19:01:37.000000 core_linked_records_app-2.8.0/core_linked_records_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:46.863705 core_linked_records_app-2.8.0/core_linked_records_app/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:37.000000 core_linked_records_app-2.8.0/core_linked_records_app/utils/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1596 2024-03-12 19:01:37.000000 core_linked_records_app-2.8.0/core_linked_records_app/utils/blob.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4352 2024-03-12 19:01:37.000000 core_linked_records_app-2.8.0/core_linked_records_app/utils/data.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1835 2024-03-12 19:01:37.000000 core_linked_records_app-2.8.0/core_linked_records_app/utils/dict.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1667 2024-03-12 19:01:37.000000 core_linked_records_app-2.8.0/core_linked_records_app/utils/exceptions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1921 2024-03-12 19:01:37.000000 core_linked_records_app-2.8.0/core_linked_records_app/utils/json.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      661 2024-03-12 19:01:37.000000 core_linked_records_app-2.8.0/core_linked_records_app/utils/path.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3050 2024-03-12 19:01:37.000000 core_linked_records_app-2.8.0/core_linked_records_app/utils/pid.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:46.923417 core_linked_records_app-2.8.0/core_linked_records_app/utils/providers/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5219 2024-03-12 19:01:37.000000 core_linked_records_app-2.8.0/core_linked_records_app/utils/providers/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4992 2024-03-12 19:01:37.000000 core_linked_records_app-2.8.0/core_linked_records_app/utils/providers/handle_net.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4766 2024-03-12 19:01:37.000000 core_linked_records_app-2.8.0/core_linked_records_app/utils/providers/local.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4901 2024-03-12 19:01:37.000000 core_linked_records_app-2.8.0/core_linked_records_app/utils/query.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4438 2024-03-12 19:01:37.000000 core_linked_records_app-2.8.0/core_linked_records_app/utils/xml.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:46.947857 core_linked_records_app-2.8.0/core_linked_records_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:37.000000 core_linked_records_app-2.8.0/core_linked_records_app/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:46.994507 core_linked_records_app-2.8.0/core_linked_records_app/views/admin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:37.000000 core_linked_records_app-2.8.0/core_linked_records_app/views/admin/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2914 2024-03-12 19:01:37.000000 core_linked_records_app-2.8.0/core_linked_records_app/views/admin/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:44.536470 core_linked_records_app-2.8.0/core_linked_records_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6496 2024-03-12 19:01:42.000000 core_linked_records_app-2.8.0/core_linked_records_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11574 2024-03-12 19:01:43.000000 core_linked_records_app-2.8.0/core_linked_records_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2024-03-12 19:01:42.000000 core_linked_records_app-2.8.0/core_linked_records_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      119 2024-03-12 19:01:42.000000 core_linked_records_app-2.8.0/core_linked_records_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       30 2024-03-12 19:01:42.000000 core_linked_records_app-2.8.0/core_linked_records_app.egg-info/top_level.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2024-03-12 19:01:37.000000 core_linked_records_app-2.8.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       52 2024-03-12 19:01:37.000000 core_linked_records_app-2.8.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       67 2024-03-12 19:01:37.000000 core_linked_records_app-2.8.0/requirements.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2024-03-12 19:01:50.122868 core_linked_records_app-2.8.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1034 2024-03-12 19:01:37.000000 core_linked_records_app-2.8.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:47.085718 core_linked_records_app-2.8.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       49 2024-03-12 19:01:37.000000 core_linked_records_app-2.8.0/tests/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:47.107157 core_linked_records_app-2.8.0/tests/access_control/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:37.000000 core_linked_records_app-2.8.0/tests/access_control/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:47.153120 core_linked_records_app-2.8.0/tests/access_control/discover/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:37.000000 core_linked_records_app-2.8.0/tests/access_control/discover/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4225 2024-03-12 19:01:37.000000 core_linked_records_app-2.8.0/tests/access_control/discover/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:47.176693 core_linked_records_app-2.8.0/tests/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:37.000000 core_linked_records_app-2.8.0/tests/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:47.202787 core_linked_records_app-2.8.0/tests/components/blob/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:37.000000 core_linked_records_app-2.8.0/tests/components/blob/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:47.249911 core_linked_records_app-2.8.0/tests/components/blob/access_control/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:37.000000 core_linked_records_app-2.8.0/tests/components/blob/access_control/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8361 2024-03-12 19:01:37.000000 core_linked_records_app-2.8.0/tests/components/blob/access_control/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:47.307823 core_linked_records_app-2.8.0/tests/components/blob/api/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:37.000000 core_linked_records_app-2.8.0/tests/components/blob/api/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    15647 2024-03-12 19:01:37.000000 core_linked_records_app-2.8.0/tests/components/blob/api/tests_acl.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8457 2024-03-12 19:01:37.000000 core_linked_records_app-2.8.0/tests/components/blob/api/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:47.353126 core_linked_records_app-2.8.0/tests/components/blob/watch/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:37.000000 core_linked_records_app-2.8.0/tests/components/blob/watch/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    17285 2024-03-12 19:01:37.000000 core_linked_records_app-2.8.0/tests/components/blob/watch/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:47.375563 core_linked_records_app-2.8.0/tests/components/data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:37.000000 core_linked_records_app-2.8.0/tests/components/data/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:47.425172 core_linked_records_app-2.8.0/tests/components/data/access_control/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:37.000000 core_linked_records_app-2.8.0/tests/components/data/access_control/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5702 2024-03-12 19:01:37.000000 core_linked_records_app-2.8.0/tests/components/data/access_control/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:47.555845 core_linked_records_app-2.8.0/tests/components/data/api/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:37.000000 core_linked_records_app-2.8.0/tests/components/data/api/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    15404 2024-03-12 19:01:37.000000 core_linked_records_app-2.8.0/tests/components/data/api/test_acl.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11975 2024-03-12 19:01:37.000000 core_linked_records_app-2.8.0/tests/components/data/api/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:47.622956 core_linked_records_app-2.8.0/tests/components/data/watch/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:37.000000 core_linked_records_app-2.8.0/tests/components/data/watch/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    13854 2024-03-12 19:01:37.000000 core_linked_records_app-2.8.0/tests/components/data/watch/tests_integration.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    25994 2024-03-12 19:01:37.000000 core_linked_records_app-2.8.0/tests/components/data/watch/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:47.649938 core_linked_records_app-2.8.0/tests/components/local_id/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:37.000000 core_linked_records_app-2.8.0/tests/components/local_id/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:47.693748 core_linked_records_app-2.8.0/tests/components/local_id/admin_site/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:37.000000 core_linked_records_app-2.8.0/tests/components/local_id/admin_site/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      952 2024-03-12 19:01:37.000000 core_linked_records_app-2.8.0/tests/components/local_id/admin_site/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:47.734711 core_linked_records_app-2.8.0/tests/components/local_id/models/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:37.000000 core_linked_records_app-2.8.0/tests/components/local_id/models/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4057 2024-03-12 19:01:37.000000 core_linked_records_app-2.8.0/tests/components/local_id/models/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:47.755535 core_linked_records_app-2.8.0/tests/components/oai_record/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:37.000000 core_linked_records_app-2.8.0/tests/components/oai_record/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:47.801188 core_linked_records_app-2.8.0/tests/components/oai_record/access_control/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:37.000000 core_linked_records_app-2.8.0/tests/components/oai_record/access_control/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2147 2024-03-12 19:01:37.000000 core_linked_records_app-2.8.0/tests/components/oai_record/access_control/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:47.870524 core_linked_records_app-2.8.0/tests/components/oai_record/api/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:37.000000 core_linked_records_app-2.8.0/tests/components/oai_record/api/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4891 2024-03-12 19:01:37.000000 core_linked_records_app-2.8.0/tests/components/oai_record/api/test_acl.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3363 2024-03-12 19:01:37.000000 core_linked_records_app-2.8.0/tests/components/oai_record/api/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:47.905156 core_linked_records_app-2.8.0/tests/components/pid_path/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:37.000000 core_linked_records_app-2.8.0/tests/components/pid_path/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:48.007162 core_linked_records_app-2.8.0/tests/components/pid_path/access_control/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:38.000000 core_linked_records_app-2.8.0/tests/components/pid_path/access_control/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2092 2024-03-12 19:01:38.000000 core_linked_records_app-2.8.0/tests/components/pid_path/access_control/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:48.086681 core_linked_records_app-2.8.0/tests/components/pid_path/admin_site/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:38.000000 core_linked_records_app-2.8.0/tests/components/pid_path/admin_site/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      559 2024-03-12 19:01:38.000000 core_linked_records_app-2.8.0/tests/components/pid_path/admin_site/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:48.142595 core_linked_records_app-2.8.0/tests/components/pid_path/api/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:38.000000 core_linked_records_app-2.8.0/tests/components/pid_path/api/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4086 2024-03-12 19:01:38.000000 core_linked_records_app-2.8.0/tests/components/pid_path/api/test_acl.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4552 2024-03-12 19:01:38.000000 core_linked_records_app-2.8.0/tests/components/pid_path/api/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:48.186721 core_linked_records_app-2.8.0/tests/components/pid_path/models/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:38.000000 core_linked_records_app-2.8.0/tests/components/pid_path/models/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3653 2024-03-12 19:01:38.000000 core_linked_records_app-2.8.0/tests/components/pid_path/models/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:48.210022 core_linked_records_app-2.8.0/tests/components/pid_settings/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:38.000000 core_linked_records_app-2.8.0/tests/components/pid_settings/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:48.254507 core_linked_records_app-2.8.0/tests/components/pid_settings/access_control/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:38.000000 core_linked_records_app-2.8.0/tests/components/pid_settings/access_control/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3734 2024-03-12 19:01:38.000000 core_linked_records_app-2.8.0/tests/components/pid_settings/access_control/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:48.315456 core_linked_records_app-2.8.0/tests/components/pid_settings/api/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:38.000000 core_linked_records_app-2.8.0/tests/components/pid_settings/api/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3365 2024-03-12 19:01:38.000000 core_linked_records_app-2.8.0/tests/components/pid_settings/api/test_acl.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2564 2024-03-12 19:01:38.000000 core_linked_records_app-2.8.0/tests/components/pid_settings/api/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:48.358463 core_linked_records_app-2.8.0/tests/components/pid_settings/models/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:38.000000 core_linked_records_app-2.8.0/tests/components/pid_settings/models/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1460 2024-03-12 19:01:38.000000 core_linked_records_app-2.8.0/tests/components/pid_settings/models/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:48.399479 core_linked_records_app-2.8.0/tests/components/pid_settings/watch/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:38.000000 core_linked_records_app-2.8.0/tests/components/pid_settings/watch/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2782 2024-03-12 19:01:38.000000 core_linked_records_app-2.8.0/tests/components/pid_settings/watch/test_unit.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2280 2024-03-12 19:01:38.000000 core_linked_records_app-2.8.0/tests/fixtures.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:48.456810 core_linked_records_app-2.8.0/tests/menus/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:38.000000 core_linked_records_app-2.8.0/tests/menus/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      553 2024-03-12 19:01:38.000000 core_linked_records_app-2.8.0/tests/menus/test_unit.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4216 2024-03-12 19:01:38.000000 core_linked_records_app-2.8.0/tests/mocks.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:48.477847 core_linked_records_app-2.8.0/tests/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:38.000000 core_linked_records_app-2.8.0/tests/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:48.508325 core_linked_records_app-2.8.0/tests/rest/blob/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:38.000000 core_linked_records_app-2.8.0/tests/rest/blob/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:48.569565 core_linked_records_app-2.8.0/tests/rest/blob/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:38.000000 core_linked_records_app-2.8.0/tests/rest/blob/views/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2649 2024-03-12 19:01:38.000000 core_linked_records_app-2.8.0/tests/rest/blob/views/test_permissions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5157 2024-03-12 19:01:38.000000 core_linked_records_app-2.8.0/tests/rest/blob/views/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:48.589046 core_linked_records_app-2.8.0/tests/rest/data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:38.000000 core_linked_records_app-2.8.0/tests/rest/data/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:48.615331 core_linked_records_app-2.8.0/tests/rest/data/renderers/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:38.000000 core_linked_records_app-2.8.0/tests/rest/data/renderers/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:48.677030 core_linked_records_app-2.8.0/tests/rest/data/renderers/data_html_user_renderer/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:38.000000 core_linked_records_app-2.8.0/tests/rest/data/renderers/data_html_user_renderer/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1247 2024-03-12 19:01:38.000000 core_linked_records_app-2.8.0/tests/rest/data/renderers/data_html_user_renderer/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:48.717797 core_linked_records_app-2.8.0/tests/rest/data/renderers/data_xml_renderer/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:38.000000 core_linked_records_app-2.8.0/tests/rest/data/renderers/data_xml_renderer/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      609 2024-03-12 19:01:38.000000 core_linked_records_app-2.8.0/tests/rest/data/renderers/data_xml_renderer/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:48.750304 core_linked_records_app-2.8.0/tests/rest/pid/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:38.000000 core_linked_records_app-2.8.0/tests/rest/pid/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:48.815657 core_linked_records_app-2.8.0/tests/rest/pid/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:38.000000 core_linked_records_app-2.8.0/tests/rest/pid/views/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6123 2024-03-12 19:01:38.000000 core_linked_records_app-2.8.0/tests/rest/pid/views/test_permissions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    17555 2024-03-12 19:01:38.000000 core_linked_records_app-2.8.0/tests/rest/pid/views/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:48.839046 core_linked_records_app-2.8.0/tests/rest/pid_path/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:38.000000 core_linked_records_app-2.8.0/tests/rest/pid_path/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:48.890083 core_linked_records_app-2.8.0/tests/rest/pid_path/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:38.000000 core_linked_records_app-2.8.0/tests/rest/pid_path/views/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7599 2024-03-12 19:01:38.000000 core_linked_records_app-2.8.0/tests/rest/pid_path/views/test_permissions.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:48.910814 core_linked_records_app-2.8.0/tests/rest/pid_settings/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:38.000000 core_linked_records_app-2.8.0/tests/rest/pid_settings/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:48.979741 core_linked_records_app-2.8.0/tests/rest/pid_settings/serializers/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:38.000000 core_linked_records_app-2.8.0/tests/rest/pid_settings/serializers/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1643 2024-03-12 19:01:38.000000 core_linked_records_app-2.8.0/tests/rest/pid_settings/serializers/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:49.044895 core_linked_records_app-2.8.0/tests/rest/pid_settings/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:38.000000 core_linked_records_app-2.8.0/tests/rest/pid_settings/views/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4248 2024-03-12 19:01:38.000000 core_linked_records_app-2.8.0/tests/rest/pid_settings/views/test_permissions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5818 2024-03-12 19:01:38.000000 core_linked_records_app-2.8.0/tests/rest/pid_settings/views/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:49.065089 core_linked_records_app-2.8.0/tests/rest/providers/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:38.000000 core_linked_records_app-2.8.0/tests/rest/providers/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:49.124003 core_linked_records_app-2.8.0/tests/rest/providers/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:38.000000 core_linked_records_app-2.8.0/tests/rest/providers/views/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8187 2024-03-12 19:01:38.000000 core_linked_records_app-2.8.0/tests/rest/providers/views/test_permissions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    17141 2024-03-12 19:01:38.000000 core_linked_records_app-2.8.0/tests/rest/providers/views/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:49.164292 core_linked_records_app-2.8.0/tests/rest/query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:38.000000 core_linked_records_app-2.8.0/tests/rest/query/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1800 2024-03-12 19:01:38.000000 core_linked_records_app-2.8.0/tests/rest/query/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:49.182990 core_linked_records_app-2.8.0/tests/system/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:38.000000 core_linked_records_app-2.8.0/tests/system/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:49.206911 core_linked_records_app-2.8.0/tests/system/blob/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:38.000000 core_linked_records_app-2.8.0/tests/system/blob/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:49.260986 core_linked_records_app-2.8.0/tests/system/blob/api/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:38.000000 core_linked_records_app-2.8.0/tests/system/blob/api/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    15772 2024-03-12 19:01:38.000000 core_linked_records_app-2.8.0/tests/system/blob/api/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:49.281118 core_linked_records_app-2.8.0/tests/system/data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:38.000000 core_linked_records_app-2.8.0/tests/system/data/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:49.323573 core_linked_records_app-2.8.0/tests/system/data/api/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:38.000000 core_linked_records_app-2.8.0/tests/system/data/api/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    16292 2024-03-12 19:01:38.000000 core_linked_records_app-2.8.0/tests/system/data/api/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:49.343034 core_linked_records_app-2.8.0/tests/system/local_id/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:38.000000 core_linked_records_app-2.8.0/tests/system/local_id/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:49.385004 core_linked_records_app-2.8.0/tests/system/local_id/api/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:38.000000 core_linked_records_app-2.8.0/tests/system/local_id/api/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5159 2024-03-12 19:01:38.000000 core_linked_records_app-2.8.0/tests/system/local_id/api/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:49.405382 core_linked_records_app-2.8.0/tests/system/pid_path/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:38.000000 core_linked_records_app-2.8.0/tests/system/pid_path/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:49.451099 core_linked_records_app-2.8.0/tests/system/pid_path/api/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:38.000000 core_linked_records_app-2.8.0/tests/system/pid_path/api/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1905 2024-03-12 19:01:38.000000 core_linked_records_app-2.8.0/tests/system/pid_path/api/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:49.471534 core_linked_records_app-2.8.0/tests/system/pid_settings/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:38.000000 core_linked_records_app-2.8.0/tests/system/pid_settings/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:49.518514 core_linked_records_app-2.8.0/tests/system/pid_settings/api/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:38.000000 core_linked_records_app-2.8.0/tests/system/pid_settings/api/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2214 2024-03-12 19:01:39.000000 core_linked_records_app-2.8.0/tests/system/pid_settings/api/tests_unit.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2202 2024-03-12 19:01:39.000000 core_linked_records_app-2.8.0/tests/test_settings.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      458 2024-03-12 19:01:39.000000 core_linked_records_app-2.8.0/tests/test_urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:49.538558 core_linked_records_app-2.8.0/tests/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:39.000000 core_linked_records_app-2.8.0/tests/utils/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:49.580546 core_linked_records_app-2.8.0/tests/utils/blob/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:39.000000 core_linked_records_app-2.8.0/tests/utils/blob/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5004 2024-03-12 19:01:39.000000 core_linked_records_app-2.8.0/tests/utils/blob/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:49.617428 core_linked_records_app-2.8.0/tests/utils/data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:39.000000 core_linked_records_app-2.8.0/tests/utils/data/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    21359 2024-03-12 19:01:39.000000 core_linked_records_app-2.8.0/tests/utils/data/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:49.655281 core_linked_records_app-2.8.0/tests/utils/dict/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:39.000000 core_linked_records_app-2.8.0/tests/utils/dict/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4213 2024-03-12 19:01:39.000000 core_linked_records_app-2.8.0/tests/utils/dict/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:49.696134 core_linked_records_app-2.8.0/tests/utils/json/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:39.000000 core_linked_records_app-2.8.0/tests/utils/json/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4119 2024-03-12 19:01:39.000000 core_linked_records_app-2.8.0/tests/utils/json/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:49.737908 core_linked_records_app-2.8.0/tests/utils/path/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:39.000000 core_linked_records_app-2.8.0/tests/utils/path/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      378 2024-03-12 19:01:39.000000 core_linked_records_app-2.8.0/tests/utils/path/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:49.779607 core_linked_records_app-2.8.0/tests/utils/pid/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:39.000000 core_linked_records_app-2.8.0/tests/utils/pid/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6009 2024-03-12 19:01:39.000000 core_linked_records_app-2.8.0/tests/utils/pid/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:49.825113 core_linked_records_app-2.8.0/tests/utils/providers/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:39.000000 core_linked_records_app-2.8.0/tests/utils/providers/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:49.870337 core_linked_records_app-2.8.0/tests/utils/providers/handle_net/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:39.000000 core_linked_records_app-2.8.0/tests/utils/providers/handle_net/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3952 2024-03-12 19:01:39.000000 core_linked_records_app-2.8.0/tests/utils/providers/handle_net/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:49.912274 core_linked_records_app-2.8.0/tests/utils/providers/local/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:39.000000 core_linked_records_app-2.8.0/tests/utils/providers/local/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11884 2024-03-12 19:01:39.000000 core_linked_records_app-2.8.0/tests/utils/providers/local/tests_unit.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1499 2024-03-12 19:01:39.000000 core_linked_records_app-2.8.0/tests/utils/providers/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:49.955598 core_linked_records_app-2.8.0/tests/utils/query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:39.000000 core_linked_records_app-2.8.0/tests/utils/query/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9302 2024-03-12 19:01:39.000000 core_linked_records_app-2.8.0/tests/utils/query/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:49.998826 core_linked_records_app-2.8.0/tests/utils/xml/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:39.000000 core_linked_records_app-2.8.0/tests/utils/xml/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10936 2024-03-12 19:01:39.000000 core_linked_records_app-2.8.0/tests/utils/xml/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:50.020541 core_linked_records_app-2.8.0/tests/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:39.000000 core_linked_records_app-2.8.0/tests/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:50.046228 core_linked_records_app-2.8.0/tests/views/admin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:39.000000 core_linked_records_app-2.8.0/tests/views/admin/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:50.094334 core_linked_records_app-2.8.0/tests/views/admin/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:01:39.000000 core_linked_records_app-2.8.0/tests/views/admin/views/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6729 2024-03-12 19:01:39.000000 core_linked_records_app-2.8.0/tests/views/admin/views/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:29.417512 core_linked_records_app-2.9.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2024-05-13 16:07:14.000000 core_linked_records_app-2.9.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      179 2024-05-13 16:07:14.000000 core_linked_records_app-2.9.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6496 2024-05-13 16:07:29.410823 core_linked_records_app-2.9.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4718 2024-05-13 16:07:14.000000 core_linked_records_app-2.9.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:23.891915 core_linked_records_app-2.9.0/core_linked_records_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      122 2024-05-13 16:07:14.000000 core_linked_records_app-2.9.0/core_linked_records_app/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:24.043723 core_linked_records_app-2.9.0/core_linked_records_app/access_control/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:14.000000 core_linked_records_app-2.9.0/core_linked_records_app/access_control/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1028 2024-05-13 16:07:14.000000 core_linked_records_app-2.9.0/core_linked_records_app/access_control/discover.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      134 2024-05-13 16:07:14.000000 core_linked_records_app-2.9.0/core_linked_records_app/access_control/rights.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1220 2024-05-13 16:07:14.000000 core_linked_records_app-2.9.0/core_linked_records_app/admin.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1218 2024-05-13 16:07:14.000000 core_linked_records_app-2.9.0/core_linked_records_app/apps.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:24.065145 core_linked_records_app-2.9.0/core_linked_records_app/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:14.000000 core_linked_records_app-2.9.0/core_linked_records_app/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:24.150381 core_linked_records_app-2.9.0/core_linked_records_app/components/blob/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:14.000000 core_linked_records_app-2.9.0/core_linked_records_app/components/blob/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1639 2024-05-13 16:07:14.000000 core_linked_records_app-2.9.0/core_linked_records_app/components/blob/access_control.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3910 2024-05-13 16:07:14.000000 core_linked_records_app-2.9.0/core_linked_records_app/components/blob/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6038 2024-05-13 16:07:14.000000 core_linked_records_app-2.9.0/core_linked_records_app/components/blob/watch.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:24.218388 core_linked_records_app-2.9.0/core_linked_records_app/components/data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:14.000000 core_linked_records_app-2.9.0/core_linked_records_app/components/data/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      859 2024-05-13 16:07:14.000000 core_linked_records_app-2.9.0/core_linked_records_app/components/data/access_control.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3457 2024-05-13 16:07:14.000000 core_linked_records_app-2.9.0/core_linked_records_app/components/data/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7306 2024-05-13 16:07:14.000000 core_linked_records_app-2.9.0/core_linked_records_app/components/data/watch.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:24.270606 core_linked_records_app-2.9.0/core_linked_records_app/components/local_id/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:14.000000 core_linked_records_app-2.9.0/core_linked_records_app/components/local_id/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      477 2024-05-13 16:07:14.000000 core_linked_records_app-2.9.0/core_linked_records_app/components/local_id/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2692 2024-05-13 16:07:14.000000 core_linked_records_app-2.9.0/core_linked_records_app/components/local_id/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:24.341430 core_linked_records_app-2.9.0/core_linked_records_app/components/oai_record/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:14.000000 core_linked_records_app-2.9.0/core_linked_records_app/components/oai_record/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      437 2024-05-13 16:07:14.000000 core_linked_records_app-2.9.0/core_linked_records_app/components/oai_record/access_control.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1492 2024-05-13 16:07:14.000000 core_linked_records_app-2.9.0/core_linked_records_app/components/oai_record/api.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:24.452134 core_linked_records_app-2.9.0/core_linked_records_app/components/pid_path/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:14.000000 core_linked_records_app-2.9.0/core_linked_records_app/components/pid_path/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      452 2024-05-13 16:07:14.000000 core_linked_records_app-2.9.0/core_linked_records_app/components/pid_path/access_control.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      196 2024-05-13 16:07:14.000000 core_linked_records_app-2.9.0/core_linked_records_app/components/pid_path/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2019 2024-05-13 16:07:14.000000 core_linked_records_app-2.9.0/core_linked_records_app/components/pid_path/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2116 2024-05-13 16:07:14.000000 core_linked_records_app-2.9.0/core_linked_records_app/components/pid_path/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:24.594797 core_linked_records_app-2.9.0/core_linked_records_app/components/pid_settings/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:14.000000 core_linked_records_app-2.9.0/core_linked_records_app/components/pid_settings/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1046 2024-05-13 16:07:14.000000 core_linked_records_app-2.9.0/core_linked_records_app/components/pid_settings/access_control.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      482 2024-05-13 16:07:14.000000 core_linked_records_app-2.9.0/core_linked_records_app/components/pid_settings/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      981 2024-05-13 16:07:14.000000 core_linked_records_app-2.9.0/core_linked_records_app/components/pid_settings/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      919 2024-05-13 16:07:14.000000 core_linked_records_app-2.9.0/core_linked_records_app/components/pid_settings/models.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      687 2024-05-13 16:07:14.000000 core_linked_records_app-2.9.0/core_linked_records_app/components/pid_settings/watch.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      470 2024-05-13 16:07:14.000000 core_linked_records_app-2.9.0/core_linked_records_app/menus.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:24.729108 core_linked_records_app-2.9.0/core_linked_records_app/migrations/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2838 2024-05-13 16:07:14.000000 core_linked_records_app-2.9.0/core_linked_records_app/migrations/0001_initial.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      660 2024-05-13 16:07:14.000000 core_linked_records_app-2.9.0/core_linked_records_app/migrations/0002_alter_pidxpath_xpath.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1008 2024-05-13 16:07:14.000000 core_linked_records_app-2.9.0/core_linked_records_app/migrations/0003_create_permissions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      439 2024-05-13 16:07:14.000000 core_linked_records_app-2.9.0/core_linked_records_app/migrations/0004_rename_pidxpath_to_pidpath.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:14.000000 core_linked_records_app-2.9.0/core_linked_records_app/migrations/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      533 2024-05-13 16:07:14.000000 core_linked_records_app-2.9.0/core_linked_records_app/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:24.784925 core_linked_records_app-2.9.0/core_linked_records_app/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:14.000000 core_linked_records_app-2.9.0/core_linked_records_app/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:24.837572 core_linked_records_app-2.9.0/core_linked_records_app/rest/blob/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:14.000000 core_linked_records_app-2.9.0/core_linked_records_app/rest/blob/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2549 2024-05-13 16:07:14.000000 core_linked_records_app-2.9.0/core_linked_records_app/rest/blob/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:24.859195 core_linked_records_app-2.9.0/core_linked_records_app/rest/data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:14.000000 core_linked_records_app-2.9.0/core_linked_records_app/rest/data/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:24.919648 core_linked_records_app-2.9.0/core_linked_records_app/rest/data/renderers/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:15.000000 core_linked_records_app-2.9.0/core_linked_records_app/rest/data/renderers/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3495 2024-05-13 16:07:15.000000 core_linked_records_app-2.9.0/core_linked_records_app/rest/data/renderers/data_html_user_renderer.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1146 2024-05-13 16:07:15.000000 core_linked_records_app-2.9.0/core_linked_records_app/rest/data/renderers/data_xml_renderer.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:24.973462 core_linked_records_app-2.9.0/core_linked_records_app/rest/pid/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:15.000000 core_linked_records_app-2.9.0/core_linked_records_app/rest/pid/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      467 2024-05-13 16:07:15.000000 core_linked_records_app-2.9.0/core_linked_records_app/rest/pid/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8350 2024-05-13 16:07:15.000000 core_linked_records_app-2.9.0/core_linked_records_app/rest/pid/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:25.027697 core_linked_records_app-2.9.0/core_linked_records_app/rest/pid_path/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:15.000000 core_linked_records_app-2.9.0/core_linked_records_app/rest/pid_path/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      359 2024-05-13 16:07:15.000000 core_linked_records_app-2.9.0/core_linked_records_app/rest/pid_path/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      828 2024-05-13 16:07:15.000000 core_linked_records_app-2.9.0/core_linked_records_app/rest/pid_path/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:25.092295 core_linked_records_app-2.9.0/core_linked_records_app/rest/pid_settings/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:15.000000 core_linked_records_app-2.9.0/core_linked_records_app/rest/pid_settings/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      847 2024-05-13 16:07:15.000000 core_linked_records_app-2.9.0/core_linked_records_app/rest/pid_settings/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2565 2024-05-13 16:07:15.000000 core_linked_records_app-2.9.0/core_linked_records_app/rest/pid_settings/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:25.127119 core_linked_records_app-2.9.0/core_linked_records_app/rest/providers/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:15.000000 core_linked_records_app-2.9.0/core_linked_records_app/rest/providers/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7029 2024-05-13 16:07:15.000000 core_linked_records_app-2.9.0/core_linked_records_app/rest/providers/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:25.162124 core_linked_records_app-2.9.0/core_linked_records_app/rest/query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:15.000000 core_linked_records_app-2.9.0/core_linked_records_app/rest/query/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      736 2024-05-13 16:07:15.000000 core_linked_records_app-2.9.0/core_linked_records_app/rest/query/views.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1964 2024-05-13 16:07:15.000000 core_linked_records_app-2.9.0/core_linked_records_app/rest/urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1971 2024-05-13 16:07:15.000000 core_linked_records_app-2.9.0/core_linked_records_app/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:22.929810 core_linked_records_app-2.9.0/core_linked_records_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:22.977235 core_linked_records_app-2.9.0/core_linked_records_app/static/core_linked_records_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:22.953300 core_linked_records_app-2.9.0/core_linked_records_app/static/core_linked_records_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:25.187990 core_linked_records_app-2.9.0/core_linked_records_app/static/core_linked_records_app/admin/css/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       72 2024-05-13 16:07:15.000000 core_linked_records_app-2.9.0/core_linked_records_app/static/core_linked_records_app/admin/css/pid_settings.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:22.957271 core_linked_records_app-2.9.0/core_linked_records_app/static/core_linked_records_app/admin/js/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:25.208239 core_linked_records_app-2.9.0/core_linked_records_app/static/core_linked_records_app/admin/js/pid_settings/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1683 2024-05-13 16:07:15.000000 core_linked_records_app-2.9.0/core_linked_records_app/static/core_linked_records_app/admin/js/pid_settings/auto_set_pid.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:22.990509 core_linked_records_app-2.9.0/core_linked_records_app/static/core_linked_records_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:25.229617 core_linked_records_app-2.9.0/core_linked_records_app/static/core_linked_records_app/user/css/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       43 2024-05-13 16:07:15.000000 core_linked_records_app-2.9.0/core_linked_records_app/static/core_linked_records_app/user/css/sharing.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:22.994471 core_linked_records_app-2.9.0/core_linked_records_app/static/core_linked_records_app/user/js/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:25.395460 core_linked_records_app-2.9.0/core_linked_records_app/static/core_linked_records_app/user/js/sharing/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      494 2024-05-13 16:07:15.000000 core_linked_records_app-2.9.0/core_linked_records_app/static/core_linked_records_app/user/js/sharing/blob_list.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       78 2024-05-13 16:07:15.000000 core_linked_records_app-2.9.0/core_linked_records_app/static/core_linked_records_app/user/js/sharing/blob_list.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      735 2024-05-13 16:07:15.000000 core_linked_records_app-2.9.0/core_linked_records_app/static/core_linked_records_app/user/js/sharing/common_list.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1199 2024-05-13 16:07:15.000000 core_linked_records_app-2.9.0/core_linked_records_app/static/core_linked_records_app/user/js/sharing/data_detail.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      236 2024-05-13 16:07:15.000000 core_linked_records_app-2.9.0/core_linked_records_app/static/core_linked_records_app/user/js/sharing/data_detail.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      494 2024-05-13 16:07:15.000000 core_linked_records_app-2.9.0/core_linked_records_app/static/core_linked_records_app/user/js/sharing/data_list.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       78 2024-05-13 16:07:15.000000 core_linked_records_app-2.9.0/core_linked_records_app/static/core_linked_records_app/user/js/sharing/data_list.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1309 2024-05-13 16:07:15.000000 core_linked_records_app-2.9.0/core_linked_records_app/static/core_linked_records_app/user/js/sharing/explore.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       78 2024-05-13 16:07:15.000000 core_linked_records_app-2.9.0/core_linked_records_app/static/core_linked_records_app/user/js/sharing/explore.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:25.413174 core_linked_records_app-2.9.0/core_linked_records_app/system/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:15.000000 core_linked_records_app-2.9.0/core_linked_records_app/system/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:25.453360 core_linked_records_app-2.9.0/core_linked_records_app/system/blob/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:15.000000 core_linked_records_app-2.9.0/core_linked_records_app/system/blob/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5201 2024-05-13 16:07:15.000000 core_linked_records_app-2.9.0/core_linked_records_app/system/blob/api.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:25.494142 core_linked_records_app-2.9.0/core_linked_records_app/system/data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:15.000000 core_linked_records_app-2.9.0/core_linked_records_app/system/data/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5172 2024-05-13 16:07:15.000000 core_linked_records_app-2.9.0/core_linked_records_app/system/data/api.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:25.553927 core_linked_records_app-2.9.0/core_linked_records_app/system/local_id/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:15.000000 core_linked_records_app-2.9.0/core_linked_records_app/system/local_id/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2208 2024-05-13 16:07:15.000000 core_linked_records_app-2.9.0/core_linked_records_app/system/local_id/api.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:25.593475 core_linked_records_app-2.9.0/core_linked_records_app/system/pid_path/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:15.000000 core_linked_records_app-2.9.0/core_linked_records_app/system/pid_path/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      631 2024-05-13 16:07:15.000000 core_linked_records_app-2.9.0/core_linked_records_app/system/pid_path/api.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:25.641073 core_linked_records_app-2.9.0/core_linked_records_app/system/pid_settings/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:15.000000 core_linked_records_app-2.9.0/core_linked_records_app/system/pid_settings/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1127 2024-05-13 16:07:15.000000 core_linked_records_app-2.9.0/core_linked_records_app/system/pid_settings/api.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:23.048455 core_linked_records_app-2.9.0/core_linked_records_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:23.076431 core_linked_records_app-2.9.0/core_linked_records_app/templates/core_linked_records_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:25.681661 core_linked_records_app-2.9.0/core_linked_records_app/templates/core_linked_records_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:25.699814 core_linked_records_app-2.9.0/core_linked_records_app/templates/core_linked_records_app/admin/pid_settings/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3190 2024-05-13 16:07:15.000000 core_linked_records_app-2.9.0/core_linked_records_app/templates/core_linked_records_app/admin/pid_settings/box.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      233 2024-05-13 16:07:15.000000 core_linked_records_app-2.9.0/core_linked_records_app/templates/core_linked_records_app/admin/pid_settings.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      290 2024-05-13 16:07:15.000000 core_linked_records_app-2.9.0/core_linked_records_app/templates/core_linked_records_app/admin/pid_settings_error.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:23.080872 core_linked_records_app-2.9.0/core_linked_records_app/templates/core_linked_records_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:23.091495 core_linked_records_app-2.9.0/core_linked_records_app/templates/core_linked_records_app/user/sharing/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:25.781665 core_linked_records_app-2.9.0/core_linked_records_app/templates/core_linked_records_app/user/sharing/data_detail/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      359 2024-05-13 16:07:15.000000 core_linked_records_app-2.9.0/core_linked_records_app/templates/core_linked_records_app/user/sharing/data_detail/button.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      236 2024-05-13 16:07:15.000000 core_linked_records_app-2.9.0/core_linked_records_app/templates/core_linked_records_app/user/sharing/data_detail/button_inline.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      283 2024-05-13 16:07:15.000000 core_linked_records_app-2.9.0/core_linked_records_app/templates/core_linked_records_app/user/sharing/data_detail/modal.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:25.819751 core_linked_records_app-2.9.0/core_linked_records_app/templates/core_linked_records_app/user/sharing/explore/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      246 2024-05-13 16:07:15.000000 core_linked_records_app-2.9.0/core_linked_records_app/templates/core_linked_records_app/user/sharing/explore/button.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      298 2024-05-13 16:07:15.000000 core_linked_records_app-2.9.0/core_linked_records_app/templates/core_linked_records_app/user/sharing/explore/modal.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      208 2024-05-13 16:07:15.000000 core_linked_records_app-2.9.0/core_linked_records_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:26.007316 core_linked_records_app-2.9.0/core_linked_records_app/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:15.000000 core_linked_records_app-2.9.0/core_linked_records_app/utils/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1596 2024-05-13 16:07:15.000000 core_linked_records_app-2.9.0/core_linked_records_app/utils/blob.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4352 2024-05-13 16:07:15.000000 core_linked_records_app-2.9.0/core_linked_records_app/utils/data.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1835 2024-05-13 16:07:15.000000 core_linked_records_app-2.9.0/core_linked_records_app/utils/dict.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1667 2024-05-13 16:07:15.000000 core_linked_records_app-2.9.0/core_linked_records_app/utils/exceptions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1921 2024-05-13 16:07:15.000000 core_linked_records_app-2.9.0/core_linked_records_app/utils/json.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      661 2024-05-13 16:07:15.000000 core_linked_records_app-2.9.0/core_linked_records_app/utils/path.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3050 2024-05-13 16:07:15.000000 core_linked_records_app-2.9.0/core_linked_records_app/utils/pid.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:26.066799 core_linked_records_app-2.9.0/core_linked_records_app/utils/providers/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5219 2024-05-13 16:07:15.000000 core_linked_records_app-2.9.0/core_linked_records_app/utils/providers/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4992 2024-05-13 16:07:15.000000 core_linked_records_app-2.9.0/core_linked_records_app/utils/providers/handle_net.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4766 2024-05-13 16:07:15.000000 core_linked_records_app-2.9.0/core_linked_records_app/utils/providers/local.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4901 2024-05-13 16:07:15.000000 core_linked_records_app-2.9.0/core_linked_records_app/utils/query.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4438 2024-05-13 16:07:15.000000 core_linked_records_app-2.9.0/core_linked_records_app/utils/xml.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:26.088900 core_linked_records_app-2.9.0/core_linked_records_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:16.000000 core_linked_records_app-2.9.0/core_linked_records_app/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:26.137323 core_linked_records_app-2.9.0/core_linked_records_app/views/admin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:16.000000 core_linked_records_app-2.9.0/core_linked_records_app/views/admin/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2914 2024-05-13 16:07:16.000000 core_linked_records_app-2.9.0/core_linked_records_app/views/admin/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:23.979049 core_linked_records_app-2.9.0/core_linked_records_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6496 2024-05-13 16:07:21.000000 core_linked_records_app-2.9.0/core_linked_records_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11574 2024-05-13 16:07:22.000000 core_linked_records_app-2.9.0/core_linked_records_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2024-05-13 16:07:21.000000 core_linked_records_app-2.9.0/core_linked_records_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      119 2024-05-13 16:07:21.000000 core_linked_records_app-2.9.0/core_linked_records_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       30 2024-05-13 16:07:21.000000 core_linked_records_app-2.9.0/core_linked_records_app.egg-info/top_level.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2024-05-13 16:07:16.000000 core_linked_records_app-2.9.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       52 2024-05-13 16:07:16.000000 core_linked_records_app-2.9.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       67 2024-05-13 16:07:16.000000 core_linked_records_app-2.9.0/requirements.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2024-05-13 16:07:29.429694 core_linked_records_app-2.9.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1034 2024-05-13 16:07:16.000000 core_linked_records_app-2.9.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:26.234653 core_linked_records_app-2.9.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       49 2024-05-13 16:07:16.000000 core_linked_records_app-2.9.0/tests/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:26.256276 core_linked_records_app-2.9.0/tests/access_control/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:16.000000 core_linked_records_app-2.9.0/tests/access_control/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:26.305262 core_linked_records_app-2.9.0/tests/access_control/discover/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:16.000000 core_linked_records_app-2.9.0/tests/access_control/discover/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4225 2024-05-13 16:07:16.000000 core_linked_records_app-2.9.0/tests/access_control/discover/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:26.327751 core_linked_records_app-2.9.0/tests/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:16.000000 core_linked_records_app-2.9.0/tests/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:26.354963 core_linked_records_app-2.9.0/tests/components/blob/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:16.000000 core_linked_records_app-2.9.0/tests/components/blob/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:26.406867 core_linked_records_app-2.9.0/tests/components/blob/access_control/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:16.000000 core_linked_records_app-2.9.0/tests/components/blob/access_control/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8361 2024-05-13 16:07:16.000000 core_linked_records_app-2.9.0/tests/components/blob/access_control/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:26.472760 core_linked_records_app-2.9.0/tests/components/blob/api/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:16.000000 core_linked_records_app-2.9.0/tests/components/blob/api/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    15647 2024-05-13 16:07:16.000000 core_linked_records_app-2.9.0/tests/components/blob/api/tests_acl.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8457 2024-05-13 16:07:16.000000 core_linked_records_app-2.9.0/tests/components/blob/api/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:26.554489 core_linked_records_app-2.9.0/tests/components/blob/watch/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:16.000000 core_linked_records_app-2.9.0/tests/components/blob/watch/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    17285 2024-05-13 16:07:16.000000 core_linked_records_app-2.9.0/tests/components/blob/watch/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:26.574797 core_linked_records_app-2.9.0/tests/components/data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:16.000000 core_linked_records_app-2.9.0/tests/components/data/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:26.628586 core_linked_records_app-2.9.0/tests/components/data/access_control/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:16.000000 core_linked_records_app-2.9.0/tests/components/data/access_control/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5702 2024-05-13 16:07:16.000000 core_linked_records_app-2.9.0/tests/components/data/access_control/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:26.693559 core_linked_records_app-2.9.0/tests/components/data/api/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:16.000000 core_linked_records_app-2.9.0/tests/components/data/api/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    15404 2024-05-13 16:07:16.000000 core_linked_records_app-2.9.0/tests/components/data/api/test_acl.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11975 2024-05-13 16:07:16.000000 core_linked_records_app-2.9.0/tests/components/data/api/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:26.757412 core_linked_records_app-2.9.0/tests/components/data/watch/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:16.000000 core_linked_records_app-2.9.0/tests/components/data/watch/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    13854 2024-05-13 16:07:16.000000 core_linked_records_app-2.9.0/tests/components/data/watch/tests_integration.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    25994 2024-05-13 16:07:16.000000 core_linked_records_app-2.9.0/tests/components/data/watch/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:26.780497 core_linked_records_app-2.9.0/tests/components/local_id/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:16.000000 core_linked_records_app-2.9.0/tests/components/local_id/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:26.830606 core_linked_records_app-2.9.0/tests/components/local_id/admin_site/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:16.000000 core_linked_records_app-2.9.0/tests/components/local_id/admin_site/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      952 2024-05-13 16:07:16.000000 core_linked_records_app-2.9.0/tests/components/local_id/admin_site/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:26.875999 core_linked_records_app-2.9.0/tests/components/local_id/models/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:16.000000 core_linked_records_app-2.9.0/tests/components/local_id/models/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4057 2024-05-13 16:07:16.000000 core_linked_records_app-2.9.0/tests/components/local_id/models/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:26.899584 core_linked_records_app-2.9.0/tests/components/oai_record/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:16.000000 core_linked_records_app-2.9.0/tests/components/oai_record/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:26.944193 core_linked_records_app-2.9.0/tests/components/oai_record/access_control/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:16.000000 core_linked_records_app-2.9.0/tests/components/oai_record/access_control/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2147 2024-05-13 16:07:16.000000 core_linked_records_app-2.9.0/tests/components/oai_record/access_control/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:27.006397 core_linked_records_app-2.9.0/tests/components/oai_record/api/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:16.000000 core_linked_records_app-2.9.0/tests/components/oai_record/api/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4891 2024-05-13 16:07:16.000000 core_linked_records_app-2.9.0/tests/components/oai_record/api/test_acl.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3363 2024-05-13 16:07:16.000000 core_linked_records_app-2.9.0/tests/components/oai_record/api/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:27.035241 core_linked_records_app-2.9.0/tests/components/pid_path/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:16.000000 core_linked_records_app-2.9.0/tests/components/pid_path/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:27.081353 core_linked_records_app-2.9.0/tests/components/pid_path/access_control/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:16.000000 core_linked_records_app-2.9.0/tests/components/pid_path/access_control/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2092 2024-05-13 16:07:16.000000 core_linked_records_app-2.9.0/tests/components/pid_path/access_control/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:27.128055 core_linked_records_app-2.9.0/tests/components/pid_path/admin_site/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:16.000000 core_linked_records_app-2.9.0/tests/components/pid_path/admin_site/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      559 2024-05-13 16:07:16.000000 core_linked_records_app-2.9.0/tests/components/pid_path/admin_site/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:27.190386 core_linked_records_app-2.9.0/tests/components/pid_path/api/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:16.000000 core_linked_records_app-2.9.0/tests/components/pid_path/api/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4086 2024-05-13 16:07:16.000000 core_linked_records_app-2.9.0/tests/components/pid_path/api/test_acl.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4552 2024-05-13 16:07:16.000000 core_linked_records_app-2.9.0/tests/components/pid_path/api/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:27.231684 core_linked_records_app-2.9.0/tests/components/pid_path/models/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:16.000000 core_linked_records_app-2.9.0/tests/components/pid_path/models/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3653 2024-05-13 16:07:16.000000 core_linked_records_app-2.9.0/tests/components/pid_path/models/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:27.251930 core_linked_records_app-2.9.0/tests/components/pid_settings/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:16.000000 core_linked_records_app-2.9.0/tests/components/pid_settings/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:27.296008 core_linked_records_app-2.9.0/tests/components/pid_settings/access_control/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:16.000000 core_linked_records_app-2.9.0/tests/components/pid_settings/access_control/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3734 2024-05-13 16:07:16.000000 core_linked_records_app-2.9.0/tests/components/pid_settings/access_control/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:27.354848 core_linked_records_app-2.9.0/tests/components/pid_settings/api/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:16.000000 core_linked_records_app-2.9.0/tests/components/pid_settings/api/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3365 2024-05-13 16:07:16.000000 core_linked_records_app-2.9.0/tests/components/pid_settings/api/test_acl.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2564 2024-05-13 16:07:16.000000 core_linked_records_app-2.9.0/tests/components/pid_settings/api/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:27.395175 core_linked_records_app-2.9.0/tests/components/pid_settings/models/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:16.000000 core_linked_records_app-2.9.0/tests/components/pid_settings/models/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1460 2024-05-13 16:07:16.000000 core_linked_records_app-2.9.0/tests/components/pid_settings/models/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:27.437196 core_linked_records_app-2.9.0/tests/components/pid_settings/watch/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:16.000000 core_linked_records_app-2.9.0/tests/components/pid_settings/watch/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2782 2024-05-13 16:07:16.000000 core_linked_records_app-2.9.0/tests/components/pid_settings/watch/test_unit.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2280 2024-05-13 16:07:16.000000 core_linked_records_app-2.9.0/tests/fixtures.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:27.480697 core_linked_records_app-2.9.0/tests/menus/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:16.000000 core_linked_records_app-2.9.0/tests/menus/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      553 2024-05-13 16:07:17.000000 core_linked_records_app-2.9.0/tests/menus/test_unit.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4216 2024-05-13 16:07:17.000000 core_linked_records_app-2.9.0/tests/mocks.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:27.501935 core_linked_records_app-2.9.0/tests/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:17.000000 core_linked_records_app-2.9.0/tests/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:27.539486 core_linked_records_app-2.9.0/tests/rest/blob/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:17.000000 core_linked_records_app-2.9.0/tests/rest/blob/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:27.605074 core_linked_records_app-2.9.0/tests/rest/blob/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:17.000000 core_linked_records_app-2.9.0/tests/rest/blob/views/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2649 2024-05-13 16:07:17.000000 core_linked_records_app-2.9.0/tests/rest/blob/views/test_permissions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5157 2024-05-13 16:07:17.000000 core_linked_records_app-2.9.0/tests/rest/blob/views/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:27.626672 core_linked_records_app-2.9.0/tests/rest/data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:17.000000 core_linked_records_app-2.9.0/tests/rest/data/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:27.650887 core_linked_records_app-2.9.0/tests/rest/data/renderers/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:17.000000 core_linked_records_app-2.9.0/tests/rest/data/renderers/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:27.693819 core_linked_records_app-2.9.0/tests/rest/data/renderers/data_html_user_renderer/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:17.000000 core_linked_records_app-2.9.0/tests/rest/data/renderers/data_html_user_renderer/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1247 2024-05-13 16:07:17.000000 core_linked_records_app-2.9.0/tests/rest/data/renderers/data_html_user_renderer/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:27.731915 core_linked_records_app-2.9.0/tests/rest/data/renderers/data_xml_renderer/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:17.000000 core_linked_records_app-2.9.0/tests/rest/data/renderers/data_xml_renderer/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      609 2024-05-13 16:07:17.000000 core_linked_records_app-2.9.0/tests/rest/data/renderers/data_xml_renderer/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:27.759981 core_linked_records_app-2.9.0/tests/rest/pid/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:17.000000 core_linked_records_app-2.9.0/tests/rest/pid/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:27.818493 core_linked_records_app-2.9.0/tests/rest/pid/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:17.000000 core_linked_records_app-2.9.0/tests/rest/pid/views/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6123 2024-05-13 16:07:17.000000 core_linked_records_app-2.9.0/tests/rest/pid/views/test_permissions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    17555 2024-05-13 16:07:17.000000 core_linked_records_app-2.9.0/tests/rest/pid/views/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:27.838085 core_linked_records_app-2.9.0/tests/rest/pid_path/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:17.000000 core_linked_records_app-2.9.0/tests/rest/pid_path/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:27.878348 core_linked_records_app-2.9.0/tests/rest/pid_path/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:17.000000 core_linked_records_app-2.9.0/tests/rest/pid_path/views/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7599 2024-05-13 16:07:17.000000 core_linked_records_app-2.9.0/tests/rest/pid_path/views/test_permissions.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:27.896949 core_linked_records_app-2.9.0/tests/rest/pid_settings/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:17.000000 core_linked_records_app-2.9.0/tests/rest/pid_settings/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:27.941324 core_linked_records_app-2.9.0/tests/rest/pid_settings/serializers/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:17.000000 core_linked_records_app-2.9.0/tests/rest/pid_settings/serializers/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1643 2024-05-13 16:07:17.000000 core_linked_records_app-2.9.0/tests/rest/pid_settings/serializers/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:28.028277 core_linked_records_app-2.9.0/tests/rest/pid_settings/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:17.000000 core_linked_records_app-2.9.0/tests/rest/pid_settings/views/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4248 2024-05-13 16:07:17.000000 core_linked_records_app-2.9.0/tests/rest/pid_settings/views/test_permissions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5818 2024-05-13 16:07:17.000000 core_linked_records_app-2.9.0/tests/rest/pid_settings/views/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:28.048096 core_linked_records_app-2.9.0/tests/rest/providers/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:17.000000 core_linked_records_app-2.9.0/tests/rest/providers/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:28.115160 core_linked_records_app-2.9.0/tests/rest/providers/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:17.000000 core_linked_records_app-2.9.0/tests/rest/providers/views/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8187 2024-05-13 16:07:17.000000 core_linked_records_app-2.9.0/tests/rest/providers/views/test_permissions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    17141 2024-05-13 16:07:17.000000 core_linked_records_app-2.9.0/tests/rest/providers/views/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:28.154695 core_linked_records_app-2.9.0/tests/rest/query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:17.000000 core_linked_records_app-2.9.0/tests/rest/query/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1800 2024-05-13 16:07:17.000000 core_linked_records_app-2.9.0/tests/rest/query/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:28.178093 core_linked_records_app-2.9.0/tests/system/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:17.000000 core_linked_records_app-2.9.0/tests/system/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:28.202242 core_linked_records_app-2.9.0/tests/system/blob/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:18.000000 core_linked_records_app-2.9.0/tests/system/blob/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:28.259245 core_linked_records_app-2.9.0/tests/system/blob/api/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:18.000000 core_linked_records_app-2.9.0/tests/system/blob/api/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    15772 2024-05-13 16:07:18.000000 core_linked_records_app-2.9.0/tests/system/blob/api/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:28.278760 core_linked_records_app-2.9.0/tests/system/data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:18.000000 core_linked_records_app-2.9.0/tests/system/data/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:28.329529 core_linked_records_app-2.9.0/tests/system/data/api/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:18.000000 core_linked_records_app-2.9.0/tests/system/data/api/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    16292 2024-05-13 16:07:18.000000 core_linked_records_app-2.9.0/tests/system/data/api/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:28.350725 core_linked_records_app-2.9.0/tests/system/local_id/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:18.000000 core_linked_records_app-2.9.0/tests/system/local_id/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:28.398755 core_linked_records_app-2.9.0/tests/system/local_id/api/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:18.000000 core_linked_records_app-2.9.0/tests/system/local_id/api/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5159 2024-05-13 16:07:18.000000 core_linked_records_app-2.9.0/tests/system/local_id/api/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:28.440593 core_linked_records_app-2.9.0/tests/system/pid_path/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:18.000000 core_linked_records_app-2.9.0/tests/system/pid_path/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:28.488727 core_linked_records_app-2.9.0/tests/system/pid_path/api/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:18.000000 core_linked_records_app-2.9.0/tests/system/pid_path/api/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1905 2024-05-13 16:07:18.000000 core_linked_records_app-2.9.0/tests/system/pid_path/api/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:28.509986 core_linked_records_app-2.9.0/tests/system/pid_settings/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:18.000000 core_linked_records_app-2.9.0/tests/system/pid_settings/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:28.557594 core_linked_records_app-2.9.0/tests/system/pid_settings/api/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:18.000000 core_linked_records_app-2.9.0/tests/system/pid_settings/api/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2214 2024-05-13 16:07:18.000000 core_linked_records_app-2.9.0/tests/system/pid_settings/api/tests_unit.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2202 2024-05-13 16:07:18.000000 core_linked_records_app-2.9.0/tests/test_settings.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      458 2024-05-13 16:07:18.000000 core_linked_records_app-2.9.0/tests/test_urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:28.615667 core_linked_records_app-2.9.0/tests/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:18.000000 core_linked_records_app-2.9.0/tests/utils/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:28.662745 core_linked_records_app-2.9.0/tests/utils/blob/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:18.000000 core_linked_records_app-2.9.0/tests/utils/blob/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5004 2024-05-13 16:07:18.000000 core_linked_records_app-2.9.0/tests/utils/blob/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:28.701821 core_linked_records_app-2.9.0/tests/utils/data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:18.000000 core_linked_records_app-2.9.0/tests/utils/data/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    21359 2024-05-13 16:07:18.000000 core_linked_records_app-2.9.0/tests/utils/data/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:28.747184 core_linked_records_app-2.9.0/tests/utils/dict/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:18.000000 core_linked_records_app-2.9.0/tests/utils/dict/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4213 2024-05-13 16:07:18.000000 core_linked_records_app-2.9.0/tests/utils/dict/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:28.785412 core_linked_records_app-2.9.0/tests/utils/json/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:18.000000 core_linked_records_app-2.9.0/tests/utils/json/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4119 2024-05-13 16:07:18.000000 core_linked_records_app-2.9.0/tests/utils/json/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:28.972737 core_linked_records_app-2.9.0/tests/utils/path/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:18.000000 core_linked_records_app-2.9.0/tests/utils/path/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      378 2024-05-13 16:07:18.000000 core_linked_records_app-2.9.0/tests/utils/path/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:29.014522 core_linked_records_app-2.9.0/tests/utils/pid/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:18.000000 core_linked_records_app-2.9.0/tests/utils/pid/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6009 2024-05-13 16:07:18.000000 core_linked_records_app-2.9.0/tests/utils/pid/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:29.091327 core_linked_records_app-2.9.0/tests/utils/providers/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:18.000000 core_linked_records_app-2.9.0/tests/utils/providers/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:29.140195 core_linked_records_app-2.9.0/tests/utils/providers/handle_net/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:18.000000 core_linked_records_app-2.9.0/tests/utils/providers/handle_net/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3952 2024-05-13 16:07:18.000000 core_linked_records_app-2.9.0/tests/utils/providers/handle_net/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:29.190036 core_linked_records_app-2.9.0/tests/utils/providers/local/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:18.000000 core_linked_records_app-2.9.0/tests/utils/providers/local/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11884 2024-05-13 16:07:18.000000 core_linked_records_app-2.9.0/tests/utils/providers/local/tests_unit.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1499 2024-05-13 16:07:18.000000 core_linked_records_app-2.9.0/tests/utils/providers/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:29.235366 core_linked_records_app-2.9.0/tests/utils/query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:18.000000 core_linked_records_app-2.9.0/tests/utils/query/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9302 2024-05-13 16:07:18.000000 core_linked_records_app-2.9.0/tests/utils/query/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:29.291570 core_linked_records_app-2.9.0/tests/utils/xml/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:18.000000 core_linked_records_app-2.9.0/tests/utils/xml/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10936 2024-05-13 16:07:18.000000 core_linked_records_app-2.9.0/tests/utils/xml/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:29.311400 core_linked_records_app-2.9.0/tests/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:18.000000 core_linked_records_app-2.9.0/tests/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:29.345406 core_linked_records_app-2.9.0/tests/views/admin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:18.000000 core_linked_records_app-2.9.0/tests/views/admin/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:29.390416 core_linked_records_app-2.9.0/tests/views/admin/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:07:18.000000 core_linked_records_app-2.9.0/tests/views/admin/views/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6729 2024-05-13 16:07:18.000000 core_linked_records_app-2.9.0/tests/views/admin/views/test_unit.py
```

### Comparing `core_linked_records_app-2.8.0/LICENSE.md` & `core_linked_records_app-2.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/PKG-INFO` & `core_linked_records_app-2.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_linked_records_app
-Version: 2.8.0
+Version: 2.9.0
 Summary: Linked records for the core project
 Home-page: https://github.com/usnistgov/core_linked_records_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: =======================
         core_linked_records_app
```

### Comparing `core_linked_records_app-2.8.0/README.rst` & `core_linked_records_app-2.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/core_linked_records_app/access_control/discover.py` & `core_linked_records_app-2.9.0/core_linked_records_app/access_control/discover.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/core_linked_records_app/admin.py` & `core_linked_records_app-2.9.0/core_linked_records_app/admin.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/core_linked_records_app/apps.py` & `core_linked_records_app-2.9.0/core_linked_records_app/apps.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/core_linked_records_app/components/blob/access_control.py` & `core_linked_records_app-2.9.0/core_linked_records_app/components/blob/access_control.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/core_linked_records_app/components/blob/api.py` & `core_linked_records_app-2.9.0/core_linked_records_app/components/blob/api.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/core_linked_records_app/components/blob/watch.py` & `core_linked_records_app-2.9.0/core_linked_records_app/components/blob/watch.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/core_linked_records_app/components/data/access_control.py` & `core_linked_records_app-2.9.0/core_linked_records_app/components/data/access_control.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/core_linked_records_app/components/data/api.py` & `core_linked_records_app-2.9.0/core_linked_records_app/components/data/api.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/core_linked_records_app/components/data/watch.py` & `core_linked_records_app-2.9.0/core_linked_records_app/components/data/watch.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/core_linked_records_app/components/local_id/models.py` & `core_linked_records_app-2.9.0/core_linked_records_app/components/local_id/models.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/core_linked_records_app/components/oai_record/api.py` & `core_linked_records_app-2.9.0/core_linked_records_app/components/oai_record/api.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/core_linked_records_app/components/pid_path/api.py` & `core_linked_records_app-2.9.0/core_linked_records_app/components/pid_path/api.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/core_linked_records_app/components/pid_path/models.py` & `core_linked_records_app-2.9.0/core_linked_records_app/components/pid_path/models.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/core_linked_records_app/components/pid_settings/access_control.py` & `core_linked_records_app-2.9.0/core_linked_records_app/components/pid_settings/access_control.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/core_linked_records_app/components/pid_settings/api.py` & `core_linked_records_app-2.9.0/core_linked_records_app/components/pid_settings/api.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/core_linked_records_app/components/pid_settings/models.py` & `core_linked_records_app-2.9.0/core_linked_records_app/components/pid_settings/models.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/core_linked_records_app/components/pid_settings/watch.py` & `core_linked_records_app-2.9.0/core_linked_records_app/components/pid_settings/watch.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/core_linked_records_app/migrations/0001_initial.py` & `core_linked_records_app-2.9.0/core_linked_records_app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/core_linked_records_app/migrations/0002_alter_pidxpath_xpath.py` & `core_linked_records_app-2.9.0/core_linked_records_app/migrations/0002_alter_pidxpath_xpath.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/core_linked_records_app/migrations/0003_create_permissions.py` & `core_linked_records_app-2.9.0/core_linked_records_app/migrations/0003_create_permissions.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/core_linked_records_app/models.py` & `core_linked_records_app-2.9.0/core_linked_records_app/models.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/core_linked_records_app/rest/blob/views.py` & `core_linked_records_app-2.9.0/core_linked_records_app/rest/blob/views.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/core_linked_records_app/rest/data/renderers/data_html_user_renderer.py` & `core_linked_records_app-2.9.0/core_linked_records_app/rest/data/renderers/data_html_user_renderer.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/core_linked_records_app/rest/data/renderers/data_xml_renderer.py` & `core_linked_records_app-2.9.0/core_linked_records_app/rest/data/renderers/data_xml_renderer.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/core_linked_records_app/rest/pid/views.py` & `core_linked_records_app-2.9.0/core_linked_records_app/rest/pid/views.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/core_linked_records_app/rest/pid_path/views.py` & `core_linked_records_app-2.9.0/core_linked_records_app/rest/pid_path/views.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/core_linked_records_app/rest/pid_settings/serializers.py` & `core_linked_records_app-2.9.0/core_linked_records_app/rest/pid_settings/serializers.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/core_linked_records_app/rest/pid_settings/views.py` & `core_linked_records_app-2.9.0/core_linked_records_app/rest/pid_settings/views.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/core_linked_records_app/rest/providers/views.py` & `core_linked_records_app-2.9.0/core_linked_records_app/rest/providers/views.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/core_linked_records_app/rest/query/views.py` & `core_linked_records_app-2.9.0/core_linked_records_app/rest/query/views.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/core_linked_records_app/rest/urls.py` & `core_linked_records_app-2.9.0/core_linked_records_app/rest/urls.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/core_linked_records_app/settings.py` & `core_linked_records_app-2.9.0/core_linked_records_app/settings.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/core_linked_records_app/static/core_linked_records_app/admin/js/pid_settings/auto_set_pid.js` & `core_linked_records_app-2.9.0/core_linked_records_app/static/core_linked_records_app/admin/js/pid_settings/auto_set_pid.js`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/core_linked_records_app/static/core_linked_records_app/user/js/sharing/common_list.js` & `core_linked_records_app-2.9.0/core_linked_records_app/static/core_linked_records_app/user/js/sharing/common_list.js`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/core_linked_records_app/static/core_linked_records_app/user/js/sharing/data_detail.js` & `core_linked_records_app-2.9.0/core_linked_records_app/static/core_linked_records_app/user/js/sharing/data_detail.js`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/core_linked_records_app/static/core_linked_records_app/user/js/sharing/explore.js` & `core_linked_records_app-2.9.0/core_linked_records_app/static/core_linked_records_app/user/js/sharing/explore.js`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/core_linked_records_app/system/blob/api.py` & `core_linked_records_app-2.9.0/core_linked_records_app/system/blob/api.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/core_linked_records_app/system/data/api.py` & `core_linked_records_app-2.9.0/core_linked_records_app/system/data/api.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/core_linked_records_app/system/local_id/api.py` & `core_linked_records_app-2.9.0/core_linked_records_app/system/local_id/api.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/core_linked_records_app/system/pid_path/api.py` & `core_linked_records_app-2.9.0/core_linked_records_app/system/pid_path/api.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/core_linked_records_app/system/pid_settings/api.py` & `core_linked_records_app-2.9.0/core_linked_records_app/system/pid_settings/api.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/core_linked_records_app/templates/core_linked_records_app/admin/pid_settings/box.html` & `core_linked_records_app-2.9.0/core_linked_records_app/templates/core_linked_records_app/admin/pid_settings/box.html`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/core_linked_records_app/utils/blob.py` & `core_linked_records_app-2.9.0/core_linked_records_app/utils/blob.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/core_linked_records_app/utils/data.py` & `core_linked_records_app-2.9.0/core_linked_records_app/utils/data.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/core_linked_records_app/utils/dict.py` & `core_linked_records_app-2.9.0/core_linked_records_app/utils/dict.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/core_linked_records_app/utils/exceptions.py` & `core_linked_records_app-2.9.0/core_linked_records_app/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/core_linked_records_app/utils/json.py` & `core_linked_records_app-2.9.0/core_linked_records_app/utils/json.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/core_linked_records_app/utils/path.py` & `core_linked_records_app-2.9.0/core_linked_records_app/utils/path.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/core_linked_records_app/utils/pid.py` & `core_linked_records_app-2.9.0/core_linked_records_app/utils/pid.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/core_linked_records_app/utils/providers/__init__.py` & `core_linked_records_app-2.9.0/core_linked_records_app/utils/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/core_linked_records_app/utils/providers/handle_net.py` & `core_linked_records_app-2.9.0/core_linked_records_app/utils/providers/handle_net.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/core_linked_records_app/utils/providers/local.py` & `core_linked_records_app-2.9.0/core_linked_records_app/utils/providers/local.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/core_linked_records_app/utils/query.py` & `core_linked_records_app-2.9.0/core_linked_records_app/utils/query.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/core_linked_records_app/utils/xml.py` & `core_linked_records_app-2.9.0/core_linked_records_app/utils/xml.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/core_linked_records_app/views/admin/views.py` & `core_linked_records_app-2.9.0/core_linked_records_app/views/admin/views.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/core_linked_records_app.egg-info/PKG-INFO` & `core_linked_records_app-2.9.0/core_linked_records_app.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-linked-records-app
-Version: 2.8.0
+Version: 2.9.0
 Summary: Linked records for the core project
 Home-page: https://github.com/usnistgov/core_linked_records_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: =======================
         core_linked_records_app
```

### Comparing `core_linked_records_app-2.8.0/core_linked_records_app.egg-info/SOURCES.txt` & `core_linked_records_app-2.9.0/core_linked_records_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/setup.py` & `core_linked_records_app-2.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_linked_records_app",
-    version="2.8.0",
+    version="2.9.0",
     description="Linked records for the core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_linked_records_app",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `core_linked_records_app-2.8.0/tests/access_control/discover/tests_unit.py` & `core_linked_records_app-2.9.0/tests/access_control/discover/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/tests/components/blob/access_control/tests_unit.py` & `core_linked_records_app-2.9.0/tests/components/blob/access_control/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/tests/components/blob/api/tests_acl.py` & `core_linked_records_app-2.9.0/tests/components/blob/api/tests_acl.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/tests/components/blob/api/tests_unit.py` & `core_linked_records_app-2.9.0/tests/components/blob/api/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/tests/components/blob/watch/tests_unit.py` & `core_linked_records_app-2.9.0/tests/components/blob/watch/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/tests/components/data/access_control/tests_unit.py` & `core_linked_records_app-2.9.0/tests/components/data/access_control/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/tests/components/data/api/test_acl.py` & `core_linked_records_app-2.9.0/tests/components/data/api/test_acl.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/tests/components/data/api/test_unit.py` & `core_linked_records_app-2.9.0/tests/components/data/api/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/tests/components/data/watch/tests_integration.py` & `core_linked_records_app-2.9.0/tests/components/data/watch/tests_integration.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/tests/components/data/watch/tests_unit.py` & `core_linked_records_app-2.9.0/tests/components/data/watch/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/tests/components/local_id/admin_site/test_unit.py` & `core_linked_records_app-2.9.0/tests/components/local_id/admin_site/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/tests/components/local_id/models/test_unit.py` & `core_linked_records_app-2.9.0/tests/components/local_id/models/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/tests/components/oai_record/access_control/tests_unit.py` & `core_linked_records_app-2.9.0/tests/components/oai_record/access_control/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/tests/components/oai_record/api/test_acl.py` & `core_linked_records_app-2.9.0/tests/components/oai_record/api/test_acl.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/tests/components/oai_record/api/test_unit.py` & `core_linked_records_app-2.9.0/tests/components/oai_record/api/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/tests/components/pid_path/access_control/tests_unit.py` & `core_linked_records_app-2.9.0/tests/components/pid_path/access_control/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/tests/components/pid_path/admin_site/test_unit.py` & `core_linked_records_app-2.9.0/tests/components/pid_path/admin_site/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/tests/components/pid_path/api/test_acl.py` & `core_linked_records_app-2.9.0/tests/components/pid_path/api/test_acl.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/tests/components/pid_path/api/test_unit.py` & `core_linked_records_app-2.9.0/tests/components/pid_path/api/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/tests/components/pid_path/models/test_unit.py` & `core_linked_records_app-2.9.0/tests/components/pid_path/models/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/tests/components/pid_settings/access_control/tests_unit.py` & `core_linked_records_app-2.9.0/tests/components/pid_settings/access_control/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/tests/components/pid_settings/api/test_acl.py` & `core_linked_records_app-2.9.0/tests/components/pid_settings/api/test_acl.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/tests/components/pid_settings/api/test_unit.py` & `core_linked_records_app-2.9.0/tests/components/pid_settings/api/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/tests/components/pid_settings/models/test_unit.py` & `core_linked_records_app-2.9.0/tests/components/pid_settings/models/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/tests/components/pid_settings/watch/test_unit.py` & `core_linked_records_app-2.9.0/tests/components/pid_settings/watch/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/tests/fixtures.py` & `core_linked_records_app-2.9.0/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/tests/menus/test_unit.py` & `core_linked_records_app-2.9.0/tests/menus/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/tests/mocks.py` & `core_linked_records_app-2.9.0/tests/mocks.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/tests/rest/blob/views/test_permissions.py` & `core_linked_records_app-2.9.0/tests/rest/blob/views/test_permissions.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/tests/rest/blob/views/test_unit.py` & `core_linked_records_app-2.9.0/tests/rest/blob/views/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/tests/rest/data/renderers/data_html_user_renderer/tests_unit.py` & `core_linked_records_app-2.9.0/tests/rest/data/renderers/data_html_user_renderer/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/tests/rest/data/renderers/data_xml_renderer/tests_unit.py` & `core_linked_records_app-2.9.0/tests/rest/data/renderers/data_xml_renderer/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/tests/rest/pid/views/test_permissions.py` & `core_linked_records_app-2.9.0/tests/rest/pid/views/test_permissions.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/tests/rest/pid/views/test_unit.py` & `core_linked_records_app-2.9.0/tests/rest/pid/views/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/tests/rest/pid_path/views/test_permissions.py` & `core_linked_records_app-2.9.0/tests/rest/pid_path/views/test_permissions.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/tests/rest/pid_settings/serializers/tests_unit.py` & `core_linked_records_app-2.9.0/tests/rest/pid_settings/serializers/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/tests/rest/pid_settings/views/test_permissions.py` & `core_linked_records_app-2.9.0/tests/rest/pid_settings/views/test_permissions.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/tests/rest/pid_settings/views/test_unit.py` & `core_linked_records_app-2.9.0/tests/rest/pid_settings/views/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/tests/rest/providers/views/test_permissions.py` & `core_linked_records_app-2.9.0/tests/rest/providers/views/test_permissions.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/tests/rest/providers/views/test_unit.py` & `core_linked_records_app-2.9.0/tests/rest/providers/views/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/tests/rest/query/test_unit.py` & `core_linked_records_app-2.9.0/tests/rest/query/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/tests/system/blob/api/tests_unit.py` & `core_linked_records_app-2.9.0/tests/system/blob/api/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/tests/system/data/api/tests_unit.py` & `core_linked_records_app-2.9.0/tests/system/data/api/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/tests/system/local_id/api/tests_unit.py` & `core_linked_records_app-2.9.0/tests/system/local_id/api/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/tests/system/pid_path/api/tests_unit.py` & `core_linked_records_app-2.9.0/tests/system/pid_path/api/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/tests/system/pid_settings/api/tests_unit.py` & `core_linked_records_app-2.9.0/tests/system/pid_settings/api/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/tests/test_settings.py` & `core_linked_records_app-2.9.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/tests/utils/blob/test_unit.py` & `core_linked_records_app-2.9.0/tests/utils/blob/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/tests/utils/data/test_unit.py` & `core_linked_records_app-2.9.0/tests/utils/data/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/tests/utils/dict/test_unit.py` & `core_linked_records_app-2.9.0/tests/utils/dict/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/tests/utils/json/tests_unit.py` & `core_linked_records_app-2.9.0/tests/utils/json/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/tests/utils/pid/tests_unit.py` & `core_linked_records_app-2.9.0/tests/utils/pid/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/tests/utils/providers/handle_net/tests_unit.py` & `core_linked_records_app-2.9.0/tests/utils/providers/handle_net/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/tests/utils/providers/local/tests_unit.py` & `core_linked_records_app-2.9.0/tests/utils/providers/local/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/tests/utils/providers/tests_unit.py` & `core_linked_records_app-2.9.0/tests/utils/providers/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/tests/utils/query/test_unit.py` & `core_linked_records_app-2.9.0/tests/utils/query/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/tests/utils/xml/test_unit.py` & `core_linked_records_app-2.9.0/tests/utils/xml/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_linked_records_app-2.8.0/tests/views/admin/views/test_unit.py` & `core_linked_records_app-2.9.0/tests/views/admin/views/test_unit.py`

 * *Files identical despite different names*

