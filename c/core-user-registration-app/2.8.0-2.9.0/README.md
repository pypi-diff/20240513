# Comparing `tmp/core_user_registration_app-2.8.0.tar.gz` & `tmp/core_user_registration_app-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_user_registration_app-2.8.0.tar", last modified: Tue Mar 12 19:07:12 2024, max compression
+gzip compressed data, was "core_user_registration_app-2.9.0.tar", last modified: Mon May 13 16:12:25 2024, max compression
```

## Comparing `core_user_registration_app-2.8.0.tar` & `core_user_registration_app-2.9.0.tar`

### file list

```diff
@@ -1,146 +1,150 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:12.957060 core_user_registration_app-2.8.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2024-03-12 19:07:06.000000 core_user_registration_app-2.8.0/LICENSE.md
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      185 2024-03-12 19:07:06.000000 core_user_registration_app-2.8.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1068 2024-03-12 19:07:12.950692 core_user_registration_app-2.8.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      586 2024-03-12 19:07:06.000000 core_user_registration_app-2.8.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:11.025449 core_user_registration_app-2.8.0/core_user_registration_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       89 2024-03-12 19:07:06.000000 core_user_registration_app-2.8.0/core_user_registration_app/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:11.166492 core_user_registration_app-2.8.0/core_user_registration_app/access_control/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:06.000000 core_user_registration_app-2.8.0/core_user_registration_app/access_control/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3113 2024-03-12 19:07:06.000000 core_user_registration_app-2.8.0/core_user_registration_app/access_control/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2683 2024-03-12 19:07:06.000000 core_user_registration_app-2.8.0/core_user_registration_app/admin.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      521 2024-03-12 19:07:06.000000 core_user_registration_app-2.8.0/core_user_registration_app/apps.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:11.190811 core_user_registration_app-2.8.0/core_user_registration_app/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:06.000000 core_user_registration_app-2.8.0/core_user_registration_app/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:11.269168 core_user_registration_app-2.8.0/core_user_registration_app/components/account_request_metadata/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:06.000000 core_user_registration_app-2.8.0/core_user_registration_app/components/account_request_metadata/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2833 2024-03-12 19:07:06.000000 core_user_registration_app-2.8.0/core_user_registration_app/components/account_request_metadata/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      721 2024-03-12 19:07:06.000000 core_user_registration_app-2.8.0/core_user_registration_app/components/account_request_metadata/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:11.344879 core_user_registration_app-2.8.0/core_user_registration_app/components/user_data_structure/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:06.000000 core_user_registration_app-2.8.0/core_user_registration_app/components/user_data_structure/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2624 2024-03-12 19:07:06.000000 core_user_registration_app-2.8.0/core_user_registration_app/components/user_data_structure/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5373 2024-03-12 19:07:06.000000 core_user_registration_app-2.8.0/core_user_registration_app/components/user_data_structure/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:11.410976 core_user_registration_app-2.8.0/core_user_registration_app/components/user_metadata/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:07.000000 core_user_registration_app-2.8.0/core_user_registration_app/components/user_metadata/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1566 2024-03-12 19:07:07.000000 core_user_registration_app-2.8.0/core_user_registration_app/components/user_metadata/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3149 2024-03-12 19:07:07.000000 core_user_registration_app-2.8.0/core_user_registration_app/components/user_metadata/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:11.494799 core_user_registration_app-2.8.0/core_user_registration_app/components/user_template_version_manager/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:07.000000 core_user_registration_app-2.8.0/core_user_registration_app/components/user_template_version_manager/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1299 2024-03-12 19:07:07.000000 core_user_registration_app-2.8.0/core_user_registration_app/components/user_template_version_manager/access_control.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3416 2024-03-12 19:07:07.000000 core_user_registration_app-2.8.0/core_user_registration_app/components/user_template_version_manager/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2628 2024-03-12 19:07:07.000000 core_user_registration_app-2.8.0/core_user_registration_app/components/user_template_version_manager/models.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6592 2024-03-12 19:07:07.000000 core_user_registration_app-2.8.0/core_user_registration_app/discover.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      514 2024-03-12 19:07:07.000000 core_user_registration_app-2.8.0/core_user_registration_app/menus.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:11.556737 core_user_registration_app-2.8.0/core_user_registration_app/migrations/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7426 2024-03-12 19:07:07.000000 core_user_registration_app-2.8.0/core_user_registration_app/migrations/0001_initial.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      418 2024-03-12 19:07:07.000000 core_user_registration_app-2.8.0/core_user_registration_app/migrations/0002_template_formats.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:07.000000 core_user_registration_app-2.8.0/core_user_registration_app/migrations/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      642 2024-03-12 19:07:07.000000 core_user_registration_app-2.8.0/core_user_registration_app/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:11.611687 core_user_registration_app-2.8.0/core_user_registration_app/permissions/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:07.000000 core_user_registration_app-2.8.0/core_user_registration_app/permissions/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      190 2024-03-12 19:07:07.000000 core_user_registration_app-2.8.0/core_user_registration_app/permissions/rights.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1596 2024-03-12 19:07:07.000000 core_user_registration_app-2.8.0/core_user_registration_app/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:10.517233 core_user_registration_app-2.8.0/core_user_registration_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:10.566054 core_user_registration_app-2.8.0/core_user_registration_app/static/core_user_registration_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:10.526184 core_user_registration_app-2.8.0/core_user_registration_app/static/core_user_registration_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:11.684970 core_user_registration_app-2.8.0/core_user_registration_app/static/core_user_registration_app/admin/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      211 2024-03-12 19:07:07.000000 core_user_registration_app-2.8.0/core_user_registration_app/static/core_user_registration_app/admin/js/view_meta.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       83 2024-03-12 19:07:07.000000 core_user_registration_app-2.8.0/core_user_registration_app/static/core_user_registration_app/admin/js/view_meta.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:10.538863 core_user_registration_app-2.8.0/core_user_registration_app/static/core_user_registration_app/common/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:10.542765 core_user_registration_app-2.8.0/core_user_registration_app/static/core_user_registration_app/common/js/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:11.734188 core_user_registration_app-2.8.0/core_user_registration_app/static/core_user_registration_app/common/js/templates/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      660 2024-03-12 19:07:07.000000 core_user_registration_app-2.8.0/core_user_registration_app/static/core_user_registration_app/common/js/templates/set_current.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      107 2024-03-12 19:07:07.000000 core_user_registration_app-2.8.0/core_user_registration_app/static/core_user_registration_app/common/js/templates/set_current.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:11.777485 core_user_registration_app-2.8.0/core_user_registration_app/static/core_user_registration_app/common/js/templates/versions/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      662 2024-03-12 19:07:07.000000 core_user_registration_app-2.8.0/core_user_registration_app/static/core_user_registration_app/common/js/templates/versions/set_current.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      125 2024-03-12 19:07:07.000000 core_user_registration_app-2.8.0/core_user_registration_app/static/core_user_registration_app/common/js/templates/versions/set_current.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:10.575660 core_user_registration_app-2.8.0/core_user_registration_app/static/core_user_registration_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:11.904531 core_user_registration_app-2.8.0/core_user_registration_app/static/core_user_registration_app/user/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      934 2024-03-12 19:07:07.000000 core_user_registration_app-2.8.0/core_user_registration_app/static/core_user_registration_app/user/js/autosave.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      100 2024-03-12 19:07:07.000000 core_user_registration_app-2.8.0/core_user_registration_app/static/core_user_registration_app/user/js/autosave.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      756 2024-03-12 19:07:07.000000 core_user_registration_app-2.8.0/core_user_registration_app/static/core_user_registration_app/user/js/report_data.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       89 2024-03-12 19:07:07.000000 core_user_registration_app-2.8.0/core_user_registration_app/static/core_user_registration_app/user/js/report_data.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1049 2024-03-12 19:07:07.000000 core_user_registration_app-2.8.0/core_user_registration_app/static/core_user_registration_app/user/js/save_data.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       68 2024-03-12 19:07:07.000000 core_user_registration_app-2.8.0/core_user_registration_app/static/core_user_registration_app/user/js/save_data.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:11.928643 core_user_registration_app-2.8.0/core_user_registration_app/static/core_user_registration_app/user/xsd/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      559 2024-03-12 19:07:07.000000 core_user_registration_app-2.8.0/core_user_registration_app/static/core_user_registration_app/user/xsd/user.xsd
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:11.977132 core_user_registration_app-2.8.0/core_user_registration_app/system/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:07.000000 core_user_registration_app-2.8.0/core_user_registration_app/system/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2013 2024-03-12 19:07:07.000000 core_user_registration_app-2.8.0/core_user_registration_app/system/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1541 2024-03-12 19:07:07.000000 core_user_registration_app-2.8.0/core_user_registration_app/tasks.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:10.601827 core_user_registration_app-2.8.0/core_user_registration_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:10.634637 core_user_registration_app-2.8.0/core_user_registration_app/templates/core_user_registration_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:12.007178 core_user_registration_app-2.8.0/core_user_registration_app/templates/core_user_registration_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:12.033901 core_user_registration_app-2.8.0/core_user_registration_app/templates/core_user_registration_app/admin/account_requests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1860 2024-03-12 19:07:07.000000 core_user_registration_app-2.8.0/core_user_registration_app/templates/core_user_registration_app/admin/account_requests/pending.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:12.077511 core_user_registration_app-2.8.0/core_user_registration_app/templates/core_user_registration_app/admin/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:12.101284 core_user_registration_app-2.8.0/core_user_registration_app/templates/core_user_registration_app/admin/templates/list/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1812 2024-03-12 19:07:07.000000 core_user_registration_app-2.8.0/core_user_registration_app/templates/core_user_registration_app/admin/templates/list/available.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      514 2024-03-12 19:07:07.000000 core_user_registration_app-2.8.0/core_user_registration_app/templates/core_user_registration_app/admin/templates/list.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:12.124397 core_user_registration_app-2.8.0/core_user_registration_app/templates/core_user_registration_app/admin/templates/versions/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3404 2024-03-12 19:07:07.000000 core_user_registration_app-2.8.0/core_user_registration_app/templates/core_user_registration_app/admin/templates/versions/available.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      615 2024-03-12 19:07:07.000000 core_user_registration_app-2.8.0/core_user_registration_app/templates/core_user_registration_app/admin/templates/versions.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      338 2024-03-12 19:07:07.000000 core_user_registration_app-2.8.0/core_user_registration_app/templates/core_user_registration_app/admin/user_requests.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:12.170807 core_user_registration_app-2.8.0/core_user_registration_app/templates/core_user_registration_app/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1015 2024-03-12 19:07:07.000000 core_user_registration_app-2.8.0/core_user_registration_app/templates/core_user_registration_app/user/account_creation.html
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     1288 2024-03-12 19:07:07.000000 core_user_registration_app-2.8.0/core_user_registration_app/templates/core_user_registration_app/user/request_new_account.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1636 2024-03-12 19:07:07.000000 core_user_registration_app-2.8.0/core_user_registration_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:12.195555 core_user_registration_app-2.8.0/core_user_registration_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:07.000000 core_user_registration_app-2.8.0/core_user_registration_app/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:12.264779 core_user_registration_app-2.8.0/core_user_registration_app/views/admin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:07.000000 core_user_registration_app-2.8.0/core_user_registration_app/views/admin/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1592 2024-03-12 19:07:07.000000 core_user_registration_app-2.8.0/core_user_registration_app/views/admin/ajax.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14677 2024-03-12 19:07:07.000000 core_user_registration_app-2.8.0/core_user_registration_app/views/admin/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:12.377871 core_user_registration_app-2.8.0/core_user_registration_app/views/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:07.000000 core_user_registration_app-2.8.0/core_user_registration_app/views/user/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5566 2024-03-12 19:07:07.000000 core_user_registration_app-2.8.0/core_user_registration_app/views/user/ajax.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7456 2024-03-12 19:07:07.000000 core_user_registration_app-2.8.0/core_user_registration_app/views/user/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:11.120216 core_user_registration_app-2.8.0/core_user_registration_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1068 2024-03-12 19:07:09.000000 core_user_registration_app-2.8.0/core_user_registration_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5520 2024-03-12 19:07:10.000000 core_user_registration_app-2.8.0/core_user_registration_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2024-03-12 19:07:09.000000 core_user_registration_app-2.8.0/core_user_registration_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       36 2024-03-12 19:07:09.000000 core_user_registration_app-2.8.0/core_user_registration_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       33 2024-03-12 19:07:09.000000 core_user_registration_app-2.8.0/core_user_registration_app.egg-info/top_level.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      170 2024-03-12 19:07:07.000000 core_user_registration_app-2.8.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       91 2024-03-12 19:07:07.000000 core_user_registration_app-2.8.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       36 2024-03-12 19:07:07.000000 core_user_registration_app-2.8.0/requirements.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2024-03-12 19:07:12.959560 core_user_registration_app-2.8.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      939 2024-03-12 19:07:07.000000 core_user_registration_app-2.8.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:12.439305 core_user_registration_app-2.8.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:07.000000 core_user_registration_app-2.8.0/tests/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:12.457749 core_user_registration_app-2.8.0/tests/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:07.000000 core_user_registration_app-2.8.0/tests/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:12.501663 core_user_registration_app-2.8.0/tests/components/account_request_metadata/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:07.000000 core_user_registration_app-2.8.0/tests/components/account_request_metadata/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2900 2024-03-12 19:07:07.000000 core_user_registration_app-2.8.0/tests/components/account_request_metadata/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:12.520246 core_user_registration_app-2.8.0/tests/components/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:07.000000 core_user_registration_app-2.8.0/tests/components/user/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:12.565139 core_user_registration_app-2.8.0/tests/components/user/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:07.000000 core_user_registration_app-2.8.0/tests/components/user/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1119 2024-03-12 19:07:07.000000 core_user_registration_app-2.8.0/tests/components/user/fixtures/fixtures.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:12.630405 core_user_registration_app-2.8.0/tests/components/user_data_structure/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:07.000000 core_user_registration_app-2.8.0/tests/components/user_data_structure/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:12.670331 core_user_registration_app-2.8.0/tests/components/user_data_structure/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:07.000000 core_user_registration_app-2.8.0/tests/components/user_data_structure/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2347 2024-03-12 19:07:07.000000 core_user_registration_app-2.8.0/tests/components/user_data_structure/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7919 2024-03-12 19:07:07.000000 core_user_registration_app-2.8.0/tests/components/user_data_structure/test_int_access_control.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3204 2024-03-12 19:07:07.000000 core_user_registration_app-2.8.0/tests/components/user_data_structure/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:12.732082 core_user_registration_app-2.8.0/tests/components/user_metadata/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:07.000000 core_user_registration_app-2.8.0/tests/components/user_metadata/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:12.774383 core_user_registration_app-2.8.0/tests/components/user_metadata/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:07.000000 core_user_registration_app-2.8.0/tests/components/user_metadata/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4816 2024-03-12 19:07:08.000000 core_user_registration_app-2.8.0/tests/components/user_metadata/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4649 2024-03-12 19:07:08.000000 core_user_registration_app-2.8.0/tests/components/user_metadata/test_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3486 2024-03-12 19:07:08.000000 core_user_registration_app-2.8.0/tests/components/user_metadata/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:12.838480 core_user_registration_app-2.8.0/tests/components/user_template_version_manager/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:08.000000 core_user_registration_app-2.8.0/tests/components/user_template_version_manager/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:12.881706 core_user_registration_app-2.8.0/tests/components/user_template_version_manager/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:08.000000 core_user_registration_app-2.8.0/tests/components/user_template_version_manager/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2475 2024-03-12 19:07:08.000000 core_user_registration_app-2.8.0/tests/components/user_template_version_manager/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8929 2024-03-12 19:07:08.000000 core_user_registration_app-2.8.0/tests/components/user_template_version_manager/test_int_access_control.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2103 2024-03-12 19:07:08.000000 core_user_registration_app-2.8.0/tests/test_settings.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2134 2024-03-12 19:07:08.000000 core_user_registration_app-2.8.0/tests/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:12.901859 core_user_registration_app-2.8.0/tests/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:08.000000 core_user_registration_app-2.8.0/tests/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:12.926317 core_user_registration_app-2.8.0/tests/views/ajax/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:07:08.000000 core_user_registration_app-2.8.0/tests/views/ajax/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:25.227946 core_user_registration_app-2.9.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2024-05-13 16:12:18.000000 core_user_registration_app-2.9.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      185 2024-05-13 16:12:18.000000 core_user_registration_app-2.9.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1068 2024-05-13 16:12:25.221932 core_user_registration_app-2.9.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      586 2024-05-13 16:12:18.000000 core_user_registration_app-2.9.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:23.214030 core_user_registration_app-2.9.0/core_user_registration_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       89 2024-05-13 16:12:18.000000 core_user_registration_app-2.9.0/core_user_registration_app/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:23.357041 core_user_registration_app-2.9.0/core_user_registration_app/access_control/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:18.000000 core_user_registration_app-2.9.0/core_user_registration_app/access_control/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3113 2024-05-13 16:12:18.000000 core_user_registration_app-2.9.0/core_user_registration_app/access_control/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2683 2024-05-13 16:12:19.000000 core_user_registration_app-2.9.0/core_user_registration_app/admin.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      516 2024-05-13 16:12:19.000000 core_user_registration_app-2.9.0/core_user_registration_app/apps.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:23.378809 core_user_registration_app-2.9.0/core_user_registration_app/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:19.000000 core_user_registration_app-2.9.0/core_user_registration_app/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:23.505349 core_user_registration_app-2.9.0/core_user_registration_app/components/account_request_metadata/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:19.000000 core_user_registration_app-2.9.0/core_user_registration_app/components/account_request_metadata/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2833 2024-05-13 16:12:19.000000 core_user_registration_app-2.9.0/core_user_registration_app/components/account_request_metadata/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      721 2024-05-13 16:12:19.000000 core_user_registration_app-2.9.0/core_user_registration_app/components/account_request_metadata/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:23.565401 core_user_registration_app-2.9.0/core_user_registration_app/components/user_data_structure/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:19.000000 core_user_registration_app-2.9.0/core_user_registration_app/components/user_data_structure/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2624 2024-05-13 16:12:19.000000 core_user_registration_app-2.9.0/core_user_registration_app/components/user_data_structure/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5373 2024-05-13 16:12:19.000000 core_user_registration_app-2.9.0/core_user_registration_app/components/user_data_structure/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:23.624933 core_user_registration_app-2.9.0/core_user_registration_app/components/user_metadata/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:19.000000 core_user_registration_app-2.9.0/core_user_registration_app/components/user_metadata/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1566 2024-05-13 16:12:19.000000 core_user_registration_app-2.9.0/core_user_registration_app/components/user_metadata/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3149 2024-05-13 16:12:19.000000 core_user_registration_app-2.9.0/core_user_registration_app/components/user_metadata/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:23.704852 core_user_registration_app-2.9.0/core_user_registration_app/components/user_template_version_manager/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:19.000000 core_user_registration_app-2.9.0/core_user_registration_app/components/user_template_version_manager/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1299 2024-05-13 16:12:19.000000 core_user_registration_app-2.9.0/core_user_registration_app/components/user_template_version_manager/access_control.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3416 2024-05-13 16:12:19.000000 core_user_registration_app-2.9.0/core_user_registration_app/components/user_template_version_manager/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2628 2024-05-13 16:12:19.000000 core_user_registration_app-2.9.0/core_user_registration_app/components/user_template_version_manager/models.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5603 2024-05-13 16:12:19.000000 core_user_registration_app-2.9.0/core_user_registration_app/discover.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      514 2024-05-13 16:12:19.000000 core_user_registration_app-2.9.0/core_user_registration_app/menus.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:23.782365 core_user_registration_app-2.9.0/core_user_registration_app/migrations/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7426 2024-05-13 16:12:19.000000 core_user_registration_app-2.9.0/core_user_registration_app/migrations/0001_initial.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      418 2024-05-13 16:12:19.000000 core_user_registration_app-2.9.0/core_user_registration_app/migrations/0002_template_formats.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      876 2024-05-13 16:12:19.000000 core_user_registration_app-2.9.0/core_user_registration_app/migrations/0003_init_data.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:19.000000 core_user_registration_app-2.9.0/core_user_registration_app/migrations/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      642 2024-05-13 16:12:19.000000 core_user_registration_app-2.9.0/core_user_registration_app/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:23.830713 core_user_registration_app-2.9.0/core_user_registration_app/permissions/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:19.000000 core_user_registration_app-2.9.0/core_user_registration_app/permissions/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      190 2024-05-13 16:12:19.000000 core_user_registration_app-2.9.0/core_user_registration_app/permissions/rights.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1583 2024-05-13 16:12:19.000000 core_user_registration_app-2.9.0/core_user_registration_app/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:22.607981 core_user_registration_app-2.9.0/core_user_registration_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:22.647991 core_user_registration_app-2.9.0/core_user_registration_app/static/core_user_registration_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:22.616302 core_user_registration_app-2.9.0/core_user_registration_app/static/core_user_registration_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:23.880089 core_user_registration_app-2.9.0/core_user_registration_app/static/core_user_registration_app/admin/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      211 2024-05-13 16:12:19.000000 core_user_registration_app-2.9.0/core_user_registration_app/static/core_user_registration_app/admin/js/view_meta.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       83 2024-05-13 16:12:19.000000 core_user_registration_app-2.9.0/core_user_registration_app/static/core_user_registration_app/admin/js/view_meta.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:22.630705 core_user_registration_app-2.9.0/core_user_registration_app/static/core_user_registration_app/common/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:22.634734 core_user_registration_app-2.9.0/core_user_registration_app/static/core_user_registration_app/common/js/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:23.930315 core_user_registration_app-2.9.0/core_user_registration_app/static/core_user_registration_app/common/js/templates/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      660 2024-05-13 16:12:19.000000 core_user_registration_app-2.9.0/core_user_registration_app/static/core_user_registration_app/common/js/templates/set_current.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      107 2024-05-13 16:12:19.000000 core_user_registration_app-2.9.0/core_user_registration_app/static/core_user_registration_app/common/js/templates/set_current.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:23.971970 core_user_registration_app-2.9.0/core_user_registration_app/static/core_user_registration_app/common/js/templates/versions/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      662 2024-05-13 16:12:19.000000 core_user_registration_app-2.9.0/core_user_registration_app/static/core_user_registration_app/common/js/templates/versions/set_current.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      125 2024-05-13 16:12:19.000000 core_user_registration_app-2.9.0/core_user_registration_app/static/core_user_registration_app/common/js/templates/versions/set_current.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:22.657851 core_user_registration_app-2.9.0/core_user_registration_app/static/core_user_registration_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:24.091691 core_user_registration_app-2.9.0/core_user_registration_app/static/core_user_registration_app/user/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      934 2024-05-13 16:12:19.000000 core_user_registration_app-2.9.0/core_user_registration_app/static/core_user_registration_app/user/js/autosave.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      100 2024-05-13 16:12:19.000000 core_user_registration_app-2.9.0/core_user_registration_app/static/core_user_registration_app/user/js/autosave.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      756 2024-05-13 16:12:19.000000 core_user_registration_app-2.9.0/core_user_registration_app/static/core_user_registration_app/user/js/report_data.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       89 2024-05-13 16:12:19.000000 core_user_registration_app-2.9.0/core_user_registration_app/static/core_user_registration_app/user/js/report_data.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1049 2024-05-13 16:12:19.000000 core_user_registration_app-2.9.0/core_user_registration_app/static/core_user_registration_app/user/js/save_data.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       68 2024-05-13 16:12:19.000000 core_user_registration_app-2.9.0/core_user_registration_app/static/core_user_registration_app/user/js/save_data.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:24.111923 core_user_registration_app-2.9.0/core_user_registration_app/static/core_user_registration_app/user/xsd/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      559 2024-05-13 16:12:19.000000 core_user_registration_app-2.9.0/core_user_registration_app/static/core_user_registration_app/user/xsd/user.xsd
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:24.155144 core_user_registration_app-2.9.0/core_user_registration_app/system/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:19.000000 core_user_registration_app-2.9.0/core_user_registration_app/system/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1999 2024-05-13 16:12:19.000000 core_user_registration_app-2.9.0/core_user_registration_app/system/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1541 2024-05-13 16:12:19.000000 core_user_registration_app-2.9.0/core_user_registration_app/tasks.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:22.676581 core_user_registration_app-2.9.0/core_user_registration_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:22.735158 core_user_registration_app-2.9.0/core_user_registration_app/templates/core_user_registration_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:24.194806 core_user_registration_app-2.9.0/core_user_registration_app/templates/core_user_registration_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:24.216030 core_user_registration_app-2.9.0/core_user_registration_app/templates/core_user_registration_app/admin/account_requests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1860 2024-05-13 16:12:19.000000 core_user_registration_app-2.9.0/core_user_registration_app/templates/core_user_registration_app/admin/account_requests/pending.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:24.273637 core_user_registration_app-2.9.0/core_user_registration_app/templates/core_user_registration_app/admin/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:24.293931 core_user_registration_app-2.9.0/core_user_registration_app/templates/core_user_registration_app/admin/templates/list/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1812 2024-05-13 16:12:19.000000 core_user_registration_app-2.9.0/core_user_registration_app/templates/core_user_registration_app/admin/templates/list/available.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      514 2024-05-13 16:12:19.000000 core_user_registration_app-2.9.0/core_user_registration_app/templates/core_user_registration_app/admin/templates/list.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:24.315500 core_user_registration_app-2.9.0/core_user_registration_app/templates/core_user_registration_app/admin/templates/versions/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3404 2024-05-13 16:12:19.000000 core_user_registration_app-2.9.0/core_user_registration_app/templates/core_user_registration_app/admin/templates/versions/available.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      615 2024-05-13 16:12:19.000000 core_user_registration_app-2.9.0/core_user_registration_app/templates/core_user_registration_app/admin/templates/versions.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      338 2024-05-13 16:12:19.000000 core_user_registration_app-2.9.0/core_user_registration_app/templates/core_user_registration_app/admin/user_requests.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:24.357859 core_user_registration_app-2.9.0/core_user_registration_app/templates/core_user_registration_app/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1015 2024-05-13 16:12:19.000000 core_user_registration_app-2.9.0/core_user_registration_app/templates/core_user_registration_app/user/account_creation.html
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     1288 2024-05-13 16:12:19.000000 core_user_registration_app-2.9.0/core_user_registration_app/templates/core_user_registration_app/user/request_new_account.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1636 2024-05-13 16:12:19.000000 core_user_registration_app-2.9.0/core_user_registration_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:24.391094 core_user_registration_app-2.9.0/core_user_registration_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:19.000000 core_user_registration_app-2.9.0/core_user_registration_app/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:24.463141 core_user_registration_app-2.9.0/core_user_registration_app/views/admin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:19.000000 core_user_registration_app-2.9.0/core_user_registration_app/views/admin/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1592 2024-05-13 16:12:19.000000 core_user_registration_app-2.9.0/core_user_registration_app/views/admin/ajax.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14677 2024-05-13 16:12:19.000000 core_user_registration_app-2.9.0/core_user_registration_app/views/admin/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:24.535310 core_user_registration_app-2.9.0/core_user_registration_app/views/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:19.000000 core_user_registration_app-2.9.0/core_user_registration_app/views/user/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5553 2024-05-13 16:12:19.000000 core_user_registration_app-2.9.0/core_user_registration_app/views/user/ajax.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7456 2024-05-13 16:12:19.000000 core_user_registration_app-2.9.0/core_user_registration_app/views/user/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:23.314025 core_user_registration_app-2.9.0/core_user_registration_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1068 2024-05-13 16:12:21.000000 core_user_registration_app-2.9.0/core_user_registration_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5632 2024-05-13 16:12:22.000000 core_user_registration_app-2.9.0/core_user_registration_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2024-05-13 16:12:21.000000 core_user_registration_app-2.9.0/core_user_registration_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       36 2024-05-13 16:12:21.000000 core_user_registration_app-2.9.0/core_user_registration_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       33 2024-05-13 16:12:21.000000 core_user_registration_app-2.9.0/core_user_registration_app.egg-info/top_level.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      170 2024-05-13 16:12:19.000000 core_user_registration_app-2.9.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      121 2024-05-13 16:12:19.000000 core_user_registration_app-2.9.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       36 2024-05-13 16:12:19.000000 core_user_registration_app-2.9.0/requirements.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2024-05-13 16:12:25.230418 core_user_registration_app-2.9.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      939 2024-05-13 16:12:19.000000 core_user_registration_app-2.9.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:24.602912 core_user_registration_app-2.9.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:19.000000 core_user_registration_app-2.9.0/tests/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:24.626331 core_user_registration_app-2.9.0/tests/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:19.000000 core_user_registration_app-2.9.0/tests/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:24.675287 core_user_registration_app-2.9.0/tests/components/account_request_metadata/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:19.000000 core_user_registration_app-2.9.0/tests/components/account_request_metadata/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2900 2024-05-13 16:12:19.000000 core_user_registration_app-2.9.0/tests/components/account_request_metadata/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:24.700009 core_user_registration_app-2.9.0/tests/components/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:19.000000 core_user_registration_app-2.9.0/tests/components/user/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:24.753929 core_user_registration_app-2.9.0/tests/components/user/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:19.000000 core_user_registration_app-2.9.0/tests/components/user/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1119 2024-05-13 16:12:20.000000 core_user_registration_app-2.9.0/tests/components/user/fixtures/fixtures.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:24.827073 core_user_registration_app-2.9.0/tests/components/user_data_structure/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:20.000000 core_user_registration_app-2.9.0/tests/components/user_data_structure/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:24.872062 core_user_registration_app-2.9.0/tests/components/user_data_structure/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:20.000000 core_user_registration_app-2.9.0/tests/components/user_data_structure/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2347 2024-05-13 16:12:20.000000 core_user_registration_app-2.9.0/tests/components/user_data_structure/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7919 2024-05-13 16:12:20.000000 core_user_registration_app-2.9.0/tests/components/user_data_structure/test_int_access_control.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3204 2024-05-13 16:12:20.000000 core_user_registration_app-2.9.0/tests/components/user_data_structure/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:24.938320 core_user_registration_app-2.9.0/tests/components/user_metadata/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:20.000000 core_user_registration_app-2.9.0/tests/components/user_metadata/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:24.988822 core_user_registration_app-2.9.0/tests/components/user_metadata/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:20.000000 core_user_registration_app-2.9.0/tests/components/user_metadata/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4816 2024-05-13 16:12:20.000000 core_user_registration_app-2.9.0/tests/components/user_metadata/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4649 2024-05-13 16:12:20.000000 core_user_registration_app-2.9.0/tests/components/user_metadata/test_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3486 2024-05-13 16:12:20.000000 core_user_registration_app-2.9.0/tests/components/user_metadata/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:25.044070 core_user_registration_app-2.9.0/tests/components/user_template_version_manager/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:20.000000 core_user_registration_app-2.9.0/tests/components/user_template_version_manager/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:25.091616 core_user_registration_app-2.9.0/tests/components/user_template_version_manager/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:20.000000 core_user_registration_app-2.9.0/tests/components/user_template_version_manager/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2475 2024-05-13 16:12:20.000000 core_user_registration_app-2.9.0/tests/components/user_template_version_manager/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8929 2024-05-13 16:12:20.000000 core_user_registration_app-2.9.0/tests/components/user_template_version_manager/test_int_access_control.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:25.136992 core_user_registration_app-2.9.0/tests/discover/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:20.000000 core_user_registration_app-2.9.0/tests/discover/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2713 2024-05-13 16:12:20.000000 core_user_registration_app-2.9.0/tests/discover/tests_unit.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2161 2024-05-13 16:12:20.000000 core_user_registration_app-2.9.0/tests/test_settings.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2134 2024-05-13 16:12:20.000000 core_user_registration_app-2.9.0/tests/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:25.158889 core_user_registration_app-2.9.0/tests/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:20.000000 core_user_registration_app-2.9.0/tests/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:25.187143 core_user_registration_app-2.9.0/tests/views/ajax/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:20.000000 core_user_registration_app-2.9.0/tests/views/ajax/__init__.py
```

### Comparing `core_user_registration_app-2.8.0/LICENSE.md` & `core_user_registration_app-2.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.8.0/PKG-INFO` & `core_user_registration_app-2.9.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_user_registration_app
-Version: 2.8.0
+Version: 2.9.0
 Summary: User registration module for the core project
 Home-page: https://github.com/usnistgov/core_user_registration_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: core_user_registration_app
         ==========================
```

### Comparing `core_user_registration_app-2.8.0/README.rst` & `core_user_registration_app-2.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.8.0/core_user_registration_app/access_control/api.py` & `core_user_registration_app-2.9.0/core_user_registration_app/access_control/api.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.8.0/core_user_registration_app/admin.py` & `core_user_registration_app-2.9.0/core_user_registration_app/admin.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.8.0/core_user_registration_app/components/account_request_metadata/api.py` & `core_user_registration_app-2.9.0/core_user_registration_app/components/account_request_metadata/api.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.8.0/core_user_registration_app/components/account_request_metadata/models.py` & `core_user_registration_app-2.9.0/core_user_registration_app/components/account_request_metadata/models.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.8.0/core_user_registration_app/components/user_data_structure/api.py` & `core_user_registration_app-2.9.0/core_user_registration_app/components/user_data_structure/api.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.8.0/core_user_registration_app/components/user_data_structure/models.py` & `core_user_registration_app-2.9.0/core_user_registration_app/components/user_data_structure/models.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.8.0/core_user_registration_app/components/user_metadata/api.py` & `core_user_registration_app-2.9.0/core_user_registration_app/components/user_metadata/api.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.8.0/core_user_registration_app/components/user_metadata/models.py` & `core_user_registration_app-2.9.0/core_user_registration_app/components/user_metadata/models.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.8.0/core_user_registration_app/components/user_template_version_manager/access_control.py` & `core_user_registration_app-2.9.0/core_user_registration_app/components/user_template_version_manager/access_control.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.8.0/core_user_registration_app/components/user_template_version_manager/api.py` & `core_user_registration_app-2.9.0/core_user_registration_app/components/user_template_version_manager/api.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.8.0/core_user_registration_app/components/user_template_version_manager/models.py` & `core_user_registration_app-2.9.0/core_user_registration_app/components/user_template_version_manager/models.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.8.0/core_user_registration_app/discover.py` & `core_user_registration_app-2.9.0/core_user_registration_app/discover.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,68 +2,112 @@
 """
 import logging
 from os.path import join
 
 from django.contrib.auth.models import Group, Permission
 from django.contrib.staticfiles import finders
 from django.core.exceptions import ObjectDoesNotExist
+from django.db.migrations.exceptions import BadMigrationError
 from django_celery_beat.models import CrontabSchedule, PeriodicTask
 
 import core_main_app.permissions.rights as main_rights
 import core_user_registration_app.permissions.rights as registration_rights
 from core_main_app.commons import exceptions
+from core_main_app.components.template_xsl_rendering import (
+    api as template_xsl_rendering_api,
+)
 from core_main_app.components.xsl_transformation import (
     api as xslt_transformation_api,
 )
 from core_main_app.components.xsl_transformation.models import (
     XslTransformation,
 )
-from core_main_app.system import api as system_api
-from core_main_app.utils.file import read_file_content
-from core_user_registration_app.components.user_template_version_manager import (
-    api as user_version_manager_api,
-)
-from core_user_registration_app.settings import (
-    REGISTRY_XSD_USER_FILENAME,
-    REGISTRY_XSD_USER_FILEPATH,
-)
-from core_user_registration_app.settings import (
-    XSL_FOLDER_PATH,
-    LIST_XSL_FILENAME,
-    DETAIL_XSL_FILENAME,
+from core_main_app.utils import file as file_utils
+from core_user_registration_app import settings as user_registration_settings
+from core_user_registration_app.components.user_template_version_manager.models import (
+    UserTemplateVersionManager,
 )
 from core_user_registration_app.system import api as registry_system_api
 from core_user_registration_app.tasks import delete_user_data_structure
 
 logger = logging.getLogger(__name__)
 
 
 def init_registration_app():
     """Init the registry. Add the registry template.
 
     Returns:
 
     """
-
-    try:
-        # Init scheduled tasks
-        _init_periodic_tasks()
-        # Add template
-        _add_user_template()
-        # Init the permissions
-        _init_permissions()
-        # Init the xslt
-        _init_xslt()
-    except Exception as e:
-        logger.error(
-            "Impossible to init the registration app: {0}".format(str(e))
+    # Check if data were previously inserted
+    if UserTemplateVersionManager.objects.count() > 0:
+        logger.warning("The database is not empty. Skipping migration.")
+        return
+
+    # Check if settings are set
+    if (
+        not user_registration_settings.REGISTRY_XSD_USER_FILEPATH
+        or not user_registration_settings.REGISTRY_XSD_USER_FILENAME
+        or not user_registration_settings.XSL_FOLDER_PATH
+        or not user_registration_settings.LIST_XSL_FILENAME
+        or not user_registration_settings.DETAIL_XSL_FILENAME
+    ):
+        raise BadMigrationError(
+            "Please configure the REGISTRY_XSD_USER_FILENAME "
+            "and REGISTRY_XSD_USER_FILEPATH, "
+            "XSL_FOLDER_PATH, LIST_XSL_FILENAME and DETAIL_XSL_FILENAME "
+            "setting in your project."
+        )
+
+    # Load files
+    default_xsd_path = finders.find(
+        user_registration_settings.REGISTRY_XSD_USER_FILEPATH
+    )
+    list_xslt_path = finders.find(
+        join(
+            user_registration_settings.XSL_FOLDER_PATH,
+            user_registration_settings.LIST_XSL_FILENAME,
         )
+    )
+    detail_xslt_path = finders.find(
+        join(
+            user_registration_settings.XSL_FOLDER_PATH,
+            user_registration_settings.DETAIL_XSL_FILENAME,
+        )
+    )
+    if not default_xsd_path or not list_xslt_path or not detail_xslt_path:
+        raise BadMigrationError(
+            "A file required for loading data was not found."
+        )
+
+    # Read files
+    xsd_data = file_utils.read_file_content(default_xsd_path)
+
+    # Create User template
+    user_template_vm = registry_system_api.insert_registry_user_schema(
+        user_registration_settings.REGISTRY_XSD_USER_FILENAME, xsd_data
+    )
+    # Save list and detail XSLT
+    list_xslt = _get_or_create_xslt(
+        list_xslt_path, user_registration_settings.LIST_XSL_FILENAME
+    )
+    detail_xslt = _get_or_create_xslt(
+        detail_xslt_path, user_registration_settings.DETAIL_XSL_FILENAME
+    )
+
+    # Bind XSLT to template
+    template_xsl_rendering_api.add_or_delete(
+        template=user_template_vm.current_version,
+        list_xslt=list_xslt,
+        default_detail_xslt=detail_xslt,
+        list_detail_xslt=[detail_xslt],
+    )
 
 
-def _init_permissions():
+def init_permissions():
     """Initialization of groups and permissions."""
     try:
         # Get or Create the default group
         anonymous, created = Group.objects.get_or_create(
             name=main_rights.ANONYMOUS_GROUP
         )
 
@@ -81,130 +125,38 @@
             register_view_data_save_repo_perm,
         )
 
     except Exception as e:
         logger.error("Impossible to init register permissions: %s" % str(e))
 
 
-def _add_user_template():
-    """Add the registry template.
-
-    Returns:
-
-    """
-    xsd_filepath = REGISTRY_XSD_USER_FILEPATH
-    xsd_filename = REGISTRY_XSD_USER_FILENAME
-    if xsd_filename == "":
-        raise Exception(
-            "Please configure the REGISTRY_XSD_USER_FILENAME setting in your project."
-        )
-    if xsd_filepath == "":
-        raise Exception(
-            "Please configure the REGISTRY_XSD_USER_FILEPATH setting in your project."
-        )
-    try:
-        registry_system_api.get_active_global_version_manager_by_title(
-            xsd_filename
-        )
-    except exceptions.DoesNotExist:
-        default_xsd_path = finders.find(xsd_filepath)
-        xsd_data = read_file_content(default_xsd_path)
-        registry_system_api.insert_registry_user_schema(xsd_filename, xsd_data)
-    except Exception as e:
-        logger.error("Impossible to add the template: {0}".format(str(e)))
-
-
-def _init_xslt():
-    """Init the XSLTs. Add XSLTs and the binding with the user template.
-
-    Returns:
-
-    """
-    try:
-        # Get or create template
-        template_version_manager = (
-            user_version_manager_api.get_default_version_manager()
-        )
-        # Get or create XSLTs
-        list_xslt = _get_or_create_xslt(LIST_XSL_FILENAME)
-        default_detail_xslt = _get_or_create_xslt(DETAIL_XSL_FILENAME)
-        list_detail_xslt = [default_detail_xslt]
-        # Create binding between template and XSLTs if does not exist
-        _bind_template_xslt(
-            template_version_manager[0].current,
-            list_xslt,
-            default_detail_xslt,
-            list_detail_xslt,
-        )
-    except Exception as e:
-        print("ERROR : Impossible to init the XSLTs. " + str(e))
-
-
-def _get_or_create_xslt(filename):
-    """Get or create an xslt.
+def _get_or_create_xslt(file_path, filename):
+    """Get or create a xslt.
 
     Args:
-        filename: XSLT filename.
+        file_path: XSLT filename.
 
     Returns:
         XSLT.
 
     """
     try:
         return xslt_transformation_api.get_by_name(filename)
-    except exceptions.ApiError:
-        # Get XSLT.
-        list_xslt_path = finders.find(join(XSL_FOLDER_PATH, filename))
+    except exceptions.DoesNotExist:
+        logger.info(f"XSLT {filename} not found, creating it now.")
         # Read content.
-        list_xsl_data = read_file_content(list_xslt_path)
+        xsl_data = file_utils.read_file_content(file_path)
         # Create the XSLT.
         list_xslt = XslTransformation(
-            name=filename, filename=filename, content=list_xsl_data
+            name=filename, filename=filename, content=xsl_data
         )
         return xslt_transformation_api.upsert(list_xslt)
-    except Exception as e:
-        raise Exception(
-            "Impossible to add the xslt {0} : {1} ".format(filename, str(e))
-        )
-
-
-def _bind_template_xslt(
-    template_id, list_xslt, default_detail_xslt, list_detail_xslt
-):
-    """Bind the registry template with the XSLTs.
-
-    Args:
-        template_id: Registry template id.
-        list_xslt: List XSLT.
-        default_detail_xslt: Detail XSLT.
-        list_detail_xslt:
-
-    Returns:
-
-    """
-    from core_main_app.components.template_xsl_rendering import (
-        api as template_xsl_rendering_api,
-    )
-
-    try:
-        template_xsl_rendering_api.get_by_template_id(template_id)
-    except exceptions.DoesNotExist:
-        template_xsl_rendering_api.add_or_delete(
-            template=system_api.get_template_by_id(template_id),
-            list_xslt=list_xslt,
-            default_detail_xslt=default_detail_xslt,
-            list_detail_xslt=list_detail_xslt,
-        )
-    except Exception as e:
-        raise Exception(
-            "Impossible to bind the template with XSLTs : " + str(e)
-        )
 
 
-def _init_periodic_tasks():
+def init_periodic_tasks():
     """Create periodic tasks for the app and add them to a crontab schedule"""
     schedule, _ = CrontabSchedule.objects.get_or_create(
         minute="*",
     )
     try:
         PeriodicTask.objects.get(name=delete_user_data_structure.__name__)
     except ObjectDoesNotExist:
```

### Comparing `core_user_registration_app-2.8.0/core_user_registration_app/menus.py` & `core_user_registration_app-2.9.0/core_user_registration_app/menus.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.8.0/core_user_registration_app/migrations/0001_initial.py` & `core_user_registration_app-2.9.0/core_user_registration_app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.8.0/core_user_registration_app/models.py` & `core_user_registration_app-2.9.0/core_user_registration_app/models.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.8.0/core_user_registration_app/settings.py` & `core_user_registration_app-2.9.0/core_user_registration_app/settings.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 """
 Django settings for core_user_registration_app project.
 
 Generated by 'django-admin startproject' using Django 1.11.
 
 For more information on this file, see
-https://docs.djangoproject.com/en/1.11/topics/settings/
+https://docs.djangoproject.com/en/4.2/topics/settings/
 
 For the full list of settings and their values, see
-https://docs.djangoproject.com/en/1.11/ref/settings/
+https://docs.djangoproject.com/en/4.2/ref/settings/
 """
 
 from os.path import join
 
 from django.conf import settings
 
 if not settings.configured:
     settings.configure()
 
 REGISTRY_XSD_FILENAME = getattr(settings, "REGISTRY_XSD_FILENAME", "")
 """ str: Registry xsd filename used for the initialisation.
 """
 
 XSL_FOLDER_PATH = getattr(
-    settings, "XSL_FOLDER_PATH", "core_explore_keyword_registry_app/xsl"
+    settings, "XSL_FOLDER_PATH", "core_main_registry_app/xsl"
 )
 """ str: Xsl folder path used for the initialisation.
 """
 
 LIST_XSL_FILENAME = getattr(settings, "LIST_XSL_FILENAME", "registry-list.xsl")
 """" str : List xsl filename used for the initialisation.
 """
```

### Comparing `core_user_registration_app-2.8.0/core_user_registration_app/static/core_user_registration_app/common/js/templates/set_current.js` & `core_user_registration_app-2.9.0/core_user_registration_app/static/core_user_registration_app/common/js/templates/set_current.js`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.8.0/core_user_registration_app/static/core_user_registration_app/common/js/templates/versions/set_current.js` & `core_user_registration_app-2.9.0/core_user_registration_app/static/core_user_registration_app/common/js/templates/versions/set_current.js`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.8.0/core_user_registration_app/static/core_user_registration_app/user/js/autosave.js` & `core_user_registration_app-2.9.0/core_user_registration_app/static/core_user_registration_app/user/js/autosave.js`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.8.0/core_user_registration_app/static/core_user_registration_app/user/js/report_data.js` & `core_user_registration_app-2.9.0/core_user_registration_app/static/core_user_registration_app/user/js/report_data.js`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.8.0/core_user_registration_app/static/core_user_registration_app/user/js/save_data.js` & `core_user_registration_app-2.9.0/core_user_registration_app/static/core_user_registration_app/user/js/save_data.js`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.8.0/core_user_registration_app/static/core_user_registration_app/user/xsd/user.xsd` & `core_user_registration_app-2.9.0/core_user_registration_app/static/core_user_registration_app/user/xsd/user.xsd`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.8.0/core_user_registration_app/system/api.py` & `core_user_registration_app-2.9.0/core_user_registration_app/system/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,14 @@
 
 
 def get_active_global_version_manager_by_title(version_manager_title):
     """Return all active Version Managers with user set to None.
 
     Args:
         version_manager_title:
-        _cls:
 
     Returns:
 
     """
     return (
         UserTemplateVersionManager.get_active_global_version_manager_by_title(
             version_manager_title
```

### Comparing `core_user_registration_app-2.8.0/core_user_registration_app/tasks.py` & `core_user_registration_app-2.9.0/core_user_registration_app/tasks.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.8.0/core_user_registration_app/templates/core_user_registration_app/admin/account_requests/pending.html` & `core_user_registration_app-2.9.0/core_user_registration_app/templates/core_user_registration_app/admin/account_requests/pending.html`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.8.0/core_user_registration_app/templates/core_user_registration_app/admin/templates/list/available.html` & `core_user_registration_app-2.9.0/core_user_registration_app/templates/core_user_registration_app/admin/templates/list/available.html`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.8.0/core_user_registration_app/templates/core_user_registration_app/admin/templates/list.html` & `core_user_registration_app-2.9.0/core_user_registration_app/templates/core_user_registration_app/admin/templates/list.html`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.8.0/core_user_registration_app/templates/core_user_registration_app/admin/templates/versions/available.html` & `core_user_registration_app-2.9.0/core_user_registration_app/templates/core_user_registration_app/admin/templates/versions/available.html`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.8.0/core_user_registration_app/templates/core_user_registration_app/admin/templates/versions.html` & `core_user_registration_app-2.9.0/core_user_registration_app/templates/core_user_registration_app/admin/templates/versions.html`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.8.0/core_user_registration_app/templates/core_user_registration_app/user/account_creation.html` & `core_user_registration_app-2.9.0/core_user_registration_app/templates/core_user_registration_app/user/account_creation.html`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.8.0/core_user_registration_app/templates/core_user_registration_app/user/request_new_account.html` & `core_user_registration_app-2.9.0/core_user_registration_app/templates/core_user_registration_app/user/request_new_account.html`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.8.0/core_user_registration_app/urls.py` & `core_user_registration_app-2.9.0/core_user_registration_app/urls.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.8.0/core_user_registration_app/views/admin/ajax.py` & `core_user_registration_app-2.9.0/core_user_registration_app/views/admin/ajax.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.8.0/core_user_registration_app/views/admin/views.py` & `core_user_registration_app-2.9.0/core_user_registration_app/views/admin/views.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.8.0/core_user_registration_app/views/user/ajax.py` & `core_user_registration_app-2.9.0/core_user_registration_app/views/user/ajax.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,15 +76,15 @@
             data_api.upsert(data, request.user)
             # insert Metadata reference in account request
             account_request_metadata_api.insert_metadata(
                 request.user, account_request_metadata_id, data
             )
             user_data_structure_api.delete(user_data_structure, request.user)
             messages.add_message(
-                request, messages.SUCCESS, "User metadata saved with success."
+                request, messages.SUCCESS, "User metadata saved."
             )
     except Exception as e:
         message = str(e).replace('"', "'")
         return HttpResponseBadRequest(
             message, content_type="application/javascript"
         )
```

### Comparing `core_user_registration_app-2.8.0/core_user_registration_app/views/user/views.py` & `core_user_registration_app-2.9.0/core_user_registration_app/views/user/views.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.8.0/core_user_registration_app.egg-info/PKG-INFO` & `core_user_registration_app-2.9.0/core_user_registration_app.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-user-registration-app
-Version: 2.8.0
+Version: 2.9.0
 Summary: User registration module for the core project
 Home-page: https://github.com/usnistgov/core_user_registration_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: core_user_registration_app
         ==========================
```

### Comparing `core_user_registration_app-2.8.0/core_user_registration_app.egg-info/SOURCES.txt` & `core_user_registration_app-2.9.0/core_user_registration_app.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 core_user_registration_app/components/user_metadata/models.py
 core_user_registration_app/components/user_template_version_manager/__init__.py
 core_user_registration_app/components/user_template_version_manager/access_control.py
 core_user_registration_app/components/user_template_version_manager/api.py
 core_user_registration_app/components/user_template_version_manager/models.py
 core_user_registration_app/migrations/0001_initial.py
 core_user_registration_app/migrations/0002_template_formats.py
+core_user_registration_app/migrations/0003_init_data.py
 core_user_registration_app/migrations/__init__.py
 core_user_registration_app/permissions/__init__.py
 core_user_registration_app/permissions/rights.py
 core_user_registration_app/static/core_user_registration_app/admin/js/view_meta.js
 core_user_registration_app/static/core_user_registration_app/admin/js/view_meta.raw.js
 core_user_registration_app/static/core_user_registration_app/common/js/templates/set_current.js
 core_user_registration_app/static/core_user_registration_app/common/js/templates/set_current.raw.js
@@ -89,9 +90,11 @@
 tests/components/user_metadata/test_unit.py
 tests/components/user_metadata/fixtures/__init__.py
 tests/components/user_metadata/fixtures/fixtures.py
 tests/components/user_template_version_manager/__init__.py
 tests/components/user_template_version_manager/test_int_access_control.py
 tests/components/user_template_version_manager/fixtures/__init__.py
 tests/components/user_template_version_manager/fixtures/fixtures.py
+tests/discover/__init__.py
+tests/discover/tests_unit.py
 tests/views/__init__.py
 tests/views/ajax/__init__.py
```

### Comparing `core_user_registration_app-2.8.0/setup.py` & `core_user_registration_app-2.9.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_user_registration_app",
-    version="2.8.0",
+    version="2.9.0",
     description="User registration module for the core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_user_registration_app",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `core_user_registration_app-2.8.0/tests/components/account_request_metadata/tests_unit.py` & `core_user_registration_app-2.9.0/tests/components/account_request_metadata/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.8.0/tests/components/user/fixtures/fixtures.py` & `core_user_registration_app-2.9.0/tests/components/user/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.8.0/tests/components/user_data_structure/fixtures/fixtures.py` & `core_user_registration_app-2.9.0/tests/components/user_data_structure/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.8.0/tests/components/user_data_structure/test_int_access_control.py` & `core_user_registration_app-2.9.0/tests/components/user_data_structure/test_int_access_control.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.8.0/tests/components/user_data_structure/tests_unit.py` & `core_user_registration_app-2.9.0/tests/components/user_data_structure/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.8.0/tests/components/user_metadata/fixtures/fixtures.py` & `core_user_registration_app-2.9.0/tests/components/user_metadata/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.8.0/tests/components/user_metadata/test_int.py` & `core_user_registration_app-2.9.0/tests/components/user_metadata/test_int.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.8.0/tests/components/user_metadata/test_unit.py` & `core_user_registration_app-2.9.0/tests/components/user_metadata/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.8.0/tests/components/user_template_version_manager/fixtures/fixtures.py` & `core_user_registration_app-2.9.0/tests/components/user_template_version_manager/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.8.0/tests/components/user_template_version_manager/test_int_access_control.py` & `core_user_registration_app-2.9.0/tests/components/user_template_version_manager/test_int_access_control.py`

 * *Files identical despite different names*

### Comparing `core_user_registration_app-2.8.0/tests/test_settings.py` & `core_user_registration_app-2.9.0/tests/test_settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     "django.contrib.sites",
     "django.contrib.staticfiles",
     # Extra apps
     "captcha",
     "django_celery_beat",
     # Local apps
     "core_main_app",
+    "core_main_registry_app",
     "core_website_app",
     "core_parser_app",
     "core_curate_app",
     "core_user_registration_app",
     "tests",
 ]
 
@@ -71,7 +72,9 @@
 CUSTOM_NAME = "Curator"
 ENABLE_SAML2_SSO_AUTH = False
 CELERYBEAT_SCHEDULER = "django_celery_beat.schedulers:DatabaseScheduler"
 
 CAN_ANONYMOUS_ACCESS_PUBLIC_DOCUMENT = False
 MONGODB_INDEXING = False
 MONGODB_ASYNC_SAVE = False
+
+CELERY_ALWAYS_EAGER = True
```

### Comparing `core_user_registration_app-2.8.0/tests/urls.py` & `core_user_registration_app-2.9.0/tests/urls.py`

 * *Files identical despite different names*

