# Comparing `tmp/core_composer_app-2.8.0.tar.gz` & `tmp/core_composer_app-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_composer_app-2.8.0.tar", last modified: Tue Mar 12 18:57:19 2024, max compression
+gzip compressed data, was "core_composer_app-2.9.0.tar", last modified: Mon May 13 16:02:23 2024, max compression
```

## Comparing `core_composer_app-2.8.0.tar` & `core_composer_app-2.9.0.tar`

### file list

```diff
@@ -1,200 +1,200 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:19.872072 core_composer_app-2.8.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2024-03-12 18:56:41.000000 core_composer_app-2.8.0/LICENSE.md
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      142 2024-03-12 18:56:41.000000 core_composer_app-2.8.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1038 2024-03-12 18:57:19.865997 core_composer_app-2.8.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      548 2024-03-12 18:56:41.000000 core_composer_app-2.8.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:06.991680 core_composer_app-2.8.0/core_composer_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      105 2024-03-12 18:56:41.000000 core_composer_app-2.8.0/core_composer_app/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3401 2024-03-12 18:56:41.000000 core_composer_app-2.8.0/core_composer_app/admin.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      494 2024-03-12 18:56:41.000000 core_composer_app-2.8.0/core_composer_app/apps.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:09.012625 core_composer_app-2.8.0/core_composer_app/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:56:41.000000 core_composer_app-2.8.0/core_composer_app/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:09.076553 core_composer_app-2.8.0/core_composer_app/components/bucket/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:56:41.000000 core_composer_app-2.8.0/core_composer_app/components/bucket/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2542 2024-03-12 18:56:41.000000 core_composer_app-2.8.0/core_composer_app/components/bucket/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2390 2024-03-12 18:56:41.000000 core_composer_app-2.8.0/core_composer_app/components/bucket/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:09.150899 core_composer_app-2.8.0/core_composer_app/components/type/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:56:41.000000 core_composer_app-2.8.0/core_composer_app/components/type/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      346 2024-03-12 18:56:41.000000 core_composer_app-2.8.0/core_composer_app/components/type/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1466 2024-03-12 18:56:41.000000 core_composer_app-2.8.0/core_composer_app/components/type/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1040 2024-03-12 18:56:41.000000 core_composer_app-2.8.0/core_composer_app/components/type/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:09.233064 core_composer_app-2.8.0/core_composer_app/components/type_version_manager/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:56:41.000000 core_composer_app-2.8.0/core_composer_app/components/type_version_manager/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      355 2024-03-12 18:56:41.000000 core_composer_app-2.8.0/core_composer_app/components/type_version_manager/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3877 2024-03-12 18:56:41.000000 core_composer_app-2.8.0/core_composer_app/components/type_version_manager/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2375 2024-03-12 18:56:41.000000 core_composer_app-2.8.0/core_composer_app/components/type_version_manager/models.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      630 2024-03-12 18:56:41.000000 core_composer_app-2.8.0/core_composer_app/menus.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:09.272569 core_composer_app-2.8.0/core_composer_app/migrations/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3384 2024-03-12 18:56:41.000000 core_composer_app-2.8.0/core_composer_app/migrations/0001_initial.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:56:41.000000 core_composer_app-2.8.0/core_composer_app/migrations/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      777 2024-03-12 18:56:41.000000 core_composer_app-2.8.0/core_composer_app/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:09.348870 core_composer_app-2.8.0/core_composer_app/permissions/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:56:41.000000 core_composer_app-2.8.0/core_composer_app/permissions/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1295 2024-03-12 18:56:41.000000 core_composer_app-2.8.0/core_composer_app/permissions/discover.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      191 2024-03-12 18:56:41.000000 core_composer_app-2.8.0/core_composer_app/permissions/rights.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:09.395734 core_composer_app-2.8.0/core_composer_app/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:56:41.000000 core_composer_app-2.8.0/core_composer_app/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:09.457917 core_composer_app-2.8.0/core_composer_app/rest/bucket/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:56:41.000000 core_composer_app-2.8.0/core_composer_app/rest/bucket/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1680 2024-03-12 18:56:41.000000 core_composer_app-2.8.0/core_composer_app/rest/bucket/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10151 2024-03-12 18:56:41.000000 core_composer_app-2.8.0/core_composer_app/rest/bucket/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:09.542050 core_composer_app-2.8.0/core_composer_app/rest/type_version_manager/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:56:41.000000 core_composer_app-2.8.0/core_composer_app/rest/type_version_manager/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5479 2024-03-12 18:56:41.000000 core_composer_app-2.8.0/core_composer_app/rest/type_version_manager/abstract_views.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2390 2024-03-12 18:56:41.000000 core_composer_app-2.8.0/core_composer_app/rest/type_version_manager/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3366 2024-03-12 18:56:41.000000 core_composer_app-2.8.0/core_composer_app/rest/type_version_manager/views.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3225 2024-03-12 18:56:41.000000 core_composer_app-2.8.0/core_composer_app/rest/urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      121 2024-03-12 18:56:41.000000 core_composer_app-2.8.0/core_composer_app/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:56:55.727388 core_composer_app-2.8.0/core_composer_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:56:55.768900 core_composer_app-2.8.0/core_composer_app/static/core_composer_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:56:55.736784 core_composer_app-2.8.0/core_composer_app/static/core_composer_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:09.594807 core_composer_app-2.8.0/core_composer_app/static/core_composer_app/admin/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      753 2024-03-12 18:56:41.000000 core_composer_app-2.8.0/core_composer_app/static/core_composer_app/admin/js/bucket.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       80 2024-03-12 18:56:41.000000 core_composer_app-2.8.0/core_composer_app/static/core_composer_app/admin/js/bucket.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:56:55.749245 core_composer_app-2.8.0/core_composer_app/static/core_composer_app/admin/js/types/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:09.661951 core_composer_app-2.8.0/core_composer_app/static/core_composer_app/admin/js/types/upload/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      983 2024-03-12 18:56:41.000000 core_composer_app-2.8.0/core_composer_app/static/core_composer_app/admin/js/types/upload/dependencies.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       98 2024-03-12 18:56:41.000000 core_composer_app-2.8.0/core_composer_app/static/core_composer_app/admin/js/types/upload/dependencies.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      143 2024-03-12 18:56:41.000000 core_composer_app-2.8.0/core_composer_app/static/core_composer_app/admin/js/types/upload/dependency_resolver.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:56:55.760589 core_composer_app-2.8.0/core_composer_app/static/core_composer_app/common/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:09.690002 core_composer_app-2.8.0/core_composer_app/static/core_composer_app/common/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      122 2024-03-12 18:56:41.000000 core_composer_app-2.8.0/core_composer_app/static/core_composer_app/common/css/bucket.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:56:55.794311 core_composer_app-2.8.0/core_composer_app/static/core_composer_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:09.756273 core_composer_app-2.8.0/core_composer_app/static/core_composer_app/user/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      532 2024-03-12 18:56:41.000000 core_composer_app-2.8.0/core_composer_app/static/core_composer_app/user/css/menu.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       56 2024-03-12 18:56:41.000000 core_composer_app-2.8.0/core_composer_app/static/core_composer_app/user/css/style.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       64 2024-03-12 18:56:41.000000 core_composer_app-2.8.0/core_composer_app/static/core_composer_app/user/css/xsd_tree.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:09.851486 core_composer_app-2.8.0/core_composer_app/static/core_composer_app/user/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3532 2024-03-12 18:56:41.000000 core_composer_app-2.8.0/core_composer_app/static/core_composer_app/user/js/build_template.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      713 2024-03-12 18:56:41.000000 core_composer_app-2.8.0/core_composer_app/static/core_composer_app/user/js/build_template.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10778 2024-03-12 18:56:41.000000 core_composer_app-2.8.0/core_composer_app/static/core_composer_app/user/js/menus.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1043 2024-03-12 18:56:41.000000 core_composer_app-2.8.0/core_composer_app/static/core_composer_app/user/js/xpath.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      444 2024-03-12 18:56:41.000000 core_composer_app-2.8.0/core_composer_app/static/core_composer_app/user/js/xsd_tree.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:09.873328 core_composer_app-2.8.0/core_composer_app/static/core_composer_app/user/xsd/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      202 2024-03-12 18:56:41.000000 core_composer_app-2.8.0/core_composer_app/static/core_composer_app/user/xsd/new_base_template.xsd
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:09.893925 core_composer_app-2.8.0/core_composer_app/static/core_composer_app/user/xsl/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4750 2024-03-12 18:56:41.000000 core_composer_app-2.8.0/core_composer_app/static/core_composer_app/user/xsl/xsd2html.xsl
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:56:55.811434 core_composer_app-2.8.0/core_composer_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:56:55.854221 core_composer_app-2.8.0/core_composer_app/templates/core_composer_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:56:55.836542 core_composer_app-2.8.0/core_composer_app/templates/core_composer_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:15.776801 core_composer_app-2.8.0/core_composer_app/templates/core_composer_app/admin/buckets/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      168 2024-03-12 18:56:41.000000 core_composer_app-2.8.0/core_composer_app/templates/core_composer_app/admin/buckets/add.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1022 2024-03-12 18:56:41.000000 core_composer_app-2.8.0/core_composer_app/templates/core_composer_app/admin/buckets/add_content.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      348 2024-03-12 18:56:41.000000 core_composer_app-2.8.0/core_composer_app/templates/core_composer_app/admin/buckets/edit.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1221 2024-03-12 18:56:41.000000 core_composer_app-2.8.0/core_composer_app/templates/core_composer_app/admin/buckets/edit_content.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:15.799750 core_composer_app-2.8.0/core_composer_app/templates/core_composer_app/admin/buckets/list/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1429 2024-03-12 18:56:41.000000 core_composer_app-2.8.0/core_composer_app/templates/core_composer_app/admin/buckets/list/available.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      165 2024-03-12 18:56:41.000000 core_composer_app-2.8.0/core_composer_app/templates/core_composer_app/admin/buckets/list.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:15.821855 core_composer_app-2.8.0/core_composer_app/templates/core_composer_app/admin/buckets/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      664 2024-03-12 18:56:42.000000 core_composer_app-2.8.0/core_composer_app/templates/core_composer_app/admin/buckets/modals/delete.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:15.882334 core_composer_app-2.8.0/core_composer_app/templates/core_composer_app/admin/types/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:15.923877 core_composer_app-2.8.0/core_composer_app/templates/core_composer_app/admin/types/list/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2066 2024-03-12 18:56:42.000000 core_composer_app-2.8.0/core_composer_app/templates/core_composer_app/admin/types/list/available.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1120 2024-03-12 18:56:42.000000 core_composer_app-2.8.0/core_composer_app/templates/core_composer_app/admin/types/list/disabled.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      228 2024-03-12 18:56:42.000000 core_composer_app-2.8.0/core_composer_app/templates/core_composer_app/admin/types/list.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       58 2024-03-12 18:56:42.000000 core_composer_app-2.8.0/core_composer_app/templates/core_composer_app/admin/types/upload.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:15.965916 core_composer_app-2.8.0/core_composer_app/templates/core_composer_app/admin/types/versions/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1411 2024-03-12 18:56:42.000000 core_composer_app-2.8.0/core_composer_app/templates/core_composer_app/admin/types/versions/available.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       68 2024-03-12 18:56:42.000000 core_composer_app-2.8.0/core_composer_app/templates/core_composer_app/admin/types/versions/disabled.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      360 2024-03-12 18:56:42.000000 core_composer_app-2.8.0/core_composer_app/templates/core_composer_app/admin/types/versions.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:16.008699 core_composer_app-2.8.0/core_composer_app/templates/core_composer_app/user/
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     1301 2024-03-12 18:56:42.000000 core_composer_app-2.8.0/core_composer_app/templates/core_composer_app/user/build_template.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:16.053332 core_composer_app-2.8.0/core_composer_app/templates/core_composer_app/user/builder/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      889 2024-03-12 18:56:42.000000 core_composer_app-2.8.0/core_composer_app/templates/core_composer_app/user/builder/list_types.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:16.111873 core_composer_app-2.8.0/core_composer_app/templates/core_composer_app/user/builder/menus/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      276 2024-03-12 18:56:42.000000 core_composer_app-2.8.0/core_composer_app/templates/core_composer_app/user/builder/menus/element.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      126 2024-03-12 18:56:42.000000 core_composer_app-2.8.0/core_composer_app/templates/core_composer_app/user/builder/menus/element_root.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      198 2024-03-12 18:56:42.000000 core_composer_app-2.8.0/core_composer_app/templates/core_composer_app/user/builder/menus/sequence.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:17.560781 core_composer_app-2.8.0/core_composer_app/templates/core_composer_app/user/builder/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      767 2024-03-12 18:56:42.000000 core_composer_app-2.8.0/core_composer_app/templates/core_composer_app/user/builder/modals/change_type.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      639 2024-03-12 18:56:42.000000 core_composer_app-2.8.0/core_composer_app/templates/core_composer_app/user/builder/modals/delete_element.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      819 2024-03-12 18:56:42.000000 core_composer_app-2.8.0/core_composer_app/templates/core_composer_app/user/builder/modals/element_name.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      525 2024-03-12 18:56:42.000000 core_composer_app-2.8.0/core_composer_app/templates/core_composer_app/user/builder/modals/errors.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1291 2024-03-12 18:56:42.000000 core_composer_app-2.8.0/core_composer_app/templates/core_composer_app/user/builder/modals/insert_element.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1186 2024-03-12 18:56:42.000000 core_composer_app-2.8.0/core_composer_app/templates/core_composer_app/user/builder/modals/occurrences.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      676 2024-03-12 18:56:42.000000 core_composer_app-2.8.0/core_composer_app/templates/core_composer_app/user/builder/modals/root_type_name.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:56:42.000000 core_composer_app-2.8.0/core_composer_app/templates/core_composer_app/user/builder/modals/save_success.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      723 2024-03-12 18:56:42.000000 core_composer_app-2.8.0/core_composer_app/templates/core_composer_app/user/builder/modals/save_template.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      705 2024-03-12 18:56:42.000000 core_composer_app-2.8.0/core_composer_app/templates/core_composer_app/user/builder/modals/save_type.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      384 2024-03-12 18:56:42.000000 core_composer_app-2.8.0/core_composer_app/templates/core_composer_app/user/builder/new_element.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2031 2024-03-12 18:56:42.000000 core_composer_app-2.8.0/core_composer_app/templates/core_composer_app/user/index.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:17.585174 core_composer_app-2.8.0/core_composer_app/templates/core_composer_app/user/list/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      275 2024-03-12 18:56:42.000000 core_composer_app-2.8.0/core_composer_app/templates/core_composer_app/user/list/list.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:17.606907 core_composer_app-2.8.0/core_composer_app/templates/core_composer_app/user/types/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:18.881060 core_composer_app-2.8.0/core_composer_app/templates/core_composer_app/user/types/versions/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      325 2024-03-12 18:56:42.000000 core_composer_app-2.8.0/core_composer_app/templates/core_composer_app/user/types/versions/available.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      262 2024-03-12 18:56:42.000000 core_composer_app-2.8.0/core_composer_app/templates/core_composer_app/user/types/versions.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2529 2024-03-12 18:56:42.000000 core_composer_app-2.8.0/core_composer_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:18.926868 core_composer_app-2.8.0/core_composer_app/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:56:42.000000 core_composer_app-2.8.0/core_composer_app/utils/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    16675 2024-03-12 18:56:42.000000 core_composer_app-2.8.0/core_composer_app/utils/xml.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:18.950013 core_composer_app-2.8.0/core_composer_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:56:42.000000 core_composer_app-2.8.0/core_composer_app/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:19.036478 core_composer_app-2.8.0/core_composer_app/views/admin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:56:42.000000 core_composer_app-2.8.0/core_composer_app/views/admin/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3892 2024-03-12 18:56:42.000000 core_composer_app-2.8.0/core_composer_app/views/admin/ajax.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2157 2024-03-12 18:56:42.000000 core_composer_app-2.8.0/core_composer_app/views/admin/forms.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    17258 2024-03-12 18:56:42.000000 core_composer_app-2.8.0/core_composer_app/views/admin/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:19.100139 core_composer_app-2.8.0/core_composer_app/views/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:56:42.000000 core_composer_app-2.8.0/core_composer_app/views/user/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    17198 2024-03-12 18:56:42.000000 core_composer_app-2.8.0/core_composer_app/views/user/ajax.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9936 2024-03-12 18:56:42.000000 core_composer_app-2.8.0/core_composer_app/views/user/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:07.078506 core_composer_app-2.8.0/core_composer_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1038 2024-03-12 18:56:54.000000 core_composer_app-2.8.0/core_composer_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7003 2024-03-12 18:56:55.000000 core_composer_app-2.8.0/core_composer_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2024-03-12 18:56:54.000000 core_composer_app-2.8.0/core_composer_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       67 2024-03-12 18:56:54.000000 core_composer_app-2.8.0/core_composer_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       29 2024-03-12 18:56:54.000000 core_composer_app-2.8.0/core_composer_app.egg-info/top_level.txt
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:19.173061 core_composer_app-2.8.0/docs/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:56:42.000000 core_composer_app-2.8.0/docs/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11283 2024-03-12 18:56:42.000000 core_composer_app-2.8.0/docs/conf.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      289 2024-03-12 18:56:42.000000 core_composer_app-2.8.0/docs/conf_urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2024-03-12 18:56:43.000000 core_composer_app-2.8.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       21 2024-03-12 18:56:43.000000 core_composer_app-2.8.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2024-03-12 18:57:19.874712 core_composer_app-2.8.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1408 2024-03-12 18:56:43.000000 core_composer_app-2.8.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:19.218859 core_composer_app-2.8.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:56:43.000000 core_composer_app-2.8.0/tests/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:19.240433 core_composer_app-2.8.0/tests/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:56:43.000000 core_composer_app-2.8.0/tests/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:19.289136 core_composer_app-2.8.0/tests/components/bucket/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:56:43.000000 core_composer_app-2.8.0/tests/components/bucket/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:19.336344 core_composer_app-2.8.0/tests/components/bucket/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:56:43.000000 core_composer_app-2.8.0/tests/components/bucket/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1047 2024-03-12 18:56:43.000000 core_composer_app-2.8.0/tests/components/bucket/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7227 2024-03-12 18:56:43.000000 core_composer_app-2.8.0/tests/components/bucket/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:19.378731 core_composer_app-2.8.0/tests/components/type/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:56:43.000000 core_composer_app-2.8.0/tests/components/type/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5623 2024-03-12 18:56:43.000000 core_composer_app-2.8.0/tests/components/type/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:19.441101 core_composer_app-2.8.0/tests/components/type_version_manager/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:56:43.000000 core_composer_app-2.8.0/tests/components/type_version_manager/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:19.483097 core_composer_app-2.8.0/tests/components/type_version_manager/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:56:43.000000 core_composer_app-2.8.0/tests/components/type_version_manager/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4419 2024-03-12 18:56:43.000000 core_composer_app-2.8.0/tests/components/type_version_manager/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    20898 2024-03-12 18:56:43.000000 core_composer_app-2.8.0/tests/components/type_version_manager/tests_int_access_control.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14720 2024-03-12 18:56:43.000000 core_composer_app-2.8.0/tests/components/type_version_manager/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:19.504213 core_composer_app-2.8.0/tests/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:56:43.000000 core_composer_app-2.8.0/tests/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:19.571699 core_composer_app-2.8.0/tests/rest/bucket/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:56:43.000000 core_composer_app-2.8.0/tests/rest/bucket/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    13700 2024-03-12 18:56:43.000000 core_composer_app-2.8.0/tests/rest/bucket/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10519 2024-03-12 18:56:43.000000 core_composer_app-2.8.0/tests/rest/bucket/tests_permission.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:19.633620 core_composer_app-2.8.0/tests/rest/type_version_manager/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:56:43.000000 core_composer_app-2.8.0/tests/rest/type_version_manager/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14878 2024-03-12 18:56:43.000000 core_composer_app-2.8.0/tests/rest/type_version_manager/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9582 2024-03-12 18:56:43.000000 core_composer_app-2.8.0/tests/rest/type_version_manager/tests_permission.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1582 2024-03-12 18:56:43.000000 core_composer_app-2.8.0/tests/test_settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:19.681494 core_composer_app-2.8.0/tests/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:56:43.000000 core_composer_app-2.8.0/tests/utils/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8032 2024-03-12 18:56:43.000000 core_composer_app-2.8.0/tests/utils/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:19.704245 core_composer_app-2.8.0/tests/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:56:43.000000 core_composer_app-2.8.0/tests/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:19.733069 core_composer_app-2.8.0/tests/views/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:56:43.000000 core_composer_app-2.8.0/tests/views/user/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:19.802977 core_composer_app-2.8.0/tests/views/user/ajax/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:56:43.000000 core_composer_app-2.8.0/tests/views/user/ajax/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11311 2024-03-12 18:56:43.000000 core_composer_app-2.8.0/tests/views/user/ajax/tests_permissions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    22448 2024-03-12 18:56:43.000000 core_composer_app-2.8.0/tests/views/user/ajax/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:19.847611 core_composer_app-2.8.0/tests/views/user/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:56:43.000000 core_composer_app-2.8.0/tests/views/user/views/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7141 2024-03-12 18:56:43.000000 core_composer_app-2.8.0/tests/views/user/views/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:23.760677 core_composer_app-2.9.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2024-05-13 16:01:51.000000 core_composer_app-2.9.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      142 2024-05-13 16:01:51.000000 core_composer_app-2.9.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1038 2024-05-13 16:02:23.754697 core_composer_app-2.9.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      548 2024-05-13 16:01:52.000000 core_composer_app-2.9.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:20.831971 core_composer_app-2.9.0/core_composer_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      105 2024-05-13 16:01:52.000000 core_composer_app-2.9.0/core_composer_app/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3401 2024-05-13 16:01:52.000000 core_composer_app-2.9.0/core_composer_app/admin.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      494 2024-05-13 16:01:52.000000 core_composer_app-2.9.0/core_composer_app/apps.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:20.972599 core_composer_app-2.9.0/core_composer_app/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:01:52.000000 core_composer_app-2.9.0/core_composer_app/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:21.049042 core_composer_app-2.9.0/core_composer_app/components/bucket/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:01:52.000000 core_composer_app-2.9.0/core_composer_app/components/bucket/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2542 2024-05-13 16:01:52.000000 core_composer_app-2.9.0/core_composer_app/components/bucket/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2390 2024-05-13 16:01:52.000000 core_composer_app-2.9.0/core_composer_app/components/bucket/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:21.158838 core_composer_app-2.9.0/core_composer_app/components/type/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:01:52.000000 core_composer_app-2.9.0/core_composer_app/components/type/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      346 2024-05-13 16:01:52.000000 core_composer_app-2.9.0/core_composer_app/components/type/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1466 2024-05-13 16:01:52.000000 core_composer_app-2.9.0/core_composer_app/components/type/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1040 2024-05-13 16:01:52.000000 core_composer_app-2.9.0/core_composer_app/components/type/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:21.242698 core_composer_app-2.9.0/core_composer_app/components/type_version_manager/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:01:52.000000 core_composer_app-2.9.0/core_composer_app/components/type_version_manager/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      355 2024-05-13 16:01:52.000000 core_composer_app-2.9.0/core_composer_app/components/type_version_manager/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3877 2024-05-13 16:01:52.000000 core_composer_app-2.9.0/core_composer_app/components/type_version_manager/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2375 2024-05-13 16:01:53.000000 core_composer_app-2.9.0/core_composer_app/components/type_version_manager/models.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      630 2024-05-13 16:01:53.000000 core_composer_app-2.9.0/core_composer_app/menus.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:21.286494 core_composer_app-2.9.0/core_composer_app/migrations/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3384 2024-05-13 16:01:53.000000 core_composer_app-2.9.0/core_composer_app/migrations/0001_initial.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:01:53.000000 core_composer_app-2.9.0/core_composer_app/migrations/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      777 2024-05-13 16:01:53.000000 core_composer_app-2.9.0/core_composer_app/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:21.352661 core_composer_app-2.9.0/core_composer_app/permissions/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:01:53.000000 core_composer_app-2.9.0/core_composer_app/permissions/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1295 2024-05-13 16:01:53.000000 core_composer_app-2.9.0/core_composer_app/permissions/discover.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      191 2024-05-13 16:01:53.000000 core_composer_app-2.9.0/core_composer_app/permissions/rights.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:21.396489 core_composer_app-2.9.0/core_composer_app/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:01:53.000000 core_composer_app-2.9.0/core_composer_app/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:21.478030 core_composer_app-2.9.0/core_composer_app/rest/bucket/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:01:53.000000 core_composer_app-2.9.0/core_composer_app/rest/bucket/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1680 2024-05-13 16:01:53.000000 core_composer_app-2.9.0/core_composer_app/rest/bucket/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10151 2024-05-13 16:01:53.000000 core_composer_app-2.9.0/core_composer_app/rest/bucket/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:21.561644 core_composer_app-2.9.0/core_composer_app/rest/type_version_manager/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:01:53.000000 core_composer_app-2.9.0/core_composer_app/rest/type_version_manager/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5479 2024-05-13 16:01:53.000000 core_composer_app-2.9.0/core_composer_app/rest/type_version_manager/abstract_views.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2390 2024-05-13 16:01:53.000000 core_composer_app-2.9.0/core_composer_app/rest/type_version_manager/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3366 2024-05-13 16:01:53.000000 core_composer_app-2.9.0/core_composer_app/rest/type_version_manager/views.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3225 2024-05-13 16:01:53.000000 core_composer_app-2.9.0/core_composer_app/rest/urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      121 2024-05-13 16:01:53.000000 core_composer_app-2.9.0/core_composer_app/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:20.108723 core_composer_app-2.9.0/core_composer_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:20.155581 core_composer_app-2.9.0/core_composer_app/static/core_composer_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:20.116175 core_composer_app-2.9.0/core_composer_app/static/core_composer_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:21.630512 core_composer_app-2.9.0/core_composer_app/static/core_composer_app/admin/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      753 2024-05-13 16:01:53.000000 core_composer_app-2.9.0/core_composer_app/static/core_composer_app/admin/js/bucket.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       80 2024-05-13 16:01:53.000000 core_composer_app-2.9.0/core_composer_app/static/core_composer_app/admin/js/bucket.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:20.135615 core_composer_app-2.9.0/core_composer_app/static/core_composer_app/admin/js/types/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:21.689783 core_composer_app-2.9.0/core_composer_app/static/core_composer_app/admin/js/types/upload/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      983 2024-05-13 16:01:53.000000 core_composer_app-2.9.0/core_composer_app/static/core_composer_app/admin/js/types/upload/dependencies.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       98 2024-05-13 16:01:53.000000 core_composer_app-2.9.0/core_composer_app/static/core_composer_app/admin/js/types/upload/dependencies.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      143 2024-05-13 16:01:53.000000 core_composer_app-2.9.0/core_composer_app/static/core_composer_app/admin/js/types/upload/dependency_resolver.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:20.148777 core_composer_app-2.9.0/core_composer_app/static/core_composer_app/common/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:21.734262 core_composer_app-2.9.0/core_composer_app/static/core_composer_app/common/css/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      122 2024-05-13 16:02:03.000000 core_composer_app-2.9.0/core_composer_app/static/core_composer_app/common/css/bucket.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:20.179355 core_composer_app-2.9.0/core_composer_app/static/core_composer_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:21.796372 core_composer_app-2.9.0/core_composer_app/static/core_composer_app/user/css/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      532 2024-05-13 16:02:03.000000 core_composer_app-2.9.0/core_composer_app/static/core_composer_app/user/css/menu.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       56 2024-05-13 16:02:03.000000 core_composer_app-2.9.0/core_composer_app/static/core_composer_app/user/css/style.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       64 2024-05-13 16:02:03.000000 core_composer_app-2.9.0/core_composer_app/static/core_composer_app/user/css/xsd_tree.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:21.954612 core_composer_app-2.9.0/core_composer_app/static/core_composer_app/user/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3532 2024-05-13 16:02:03.000000 core_composer_app-2.9.0/core_composer_app/static/core_composer_app/user/js/build_template.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      713 2024-05-13 16:02:03.000000 core_composer_app-2.9.0/core_composer_app/static/core_composer_app/user/js/build_template.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10778 2024-05-13 16:02:03.000000 core_composer_app-2.9.0/core_composer_app/static/core_composer_app/user/js/menus.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1043 2024-05-13 16:02:03.000000 core_composer_app-2.9.0/core_composer_app/static/core_composer_app/user/js/xpath.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      444 2024-05-13 16:02:03.000000 core_composer_app-2.9.0/core_composer_app/static/core_composer_app/user/js/xsd_tree.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:21.976412 core_composer_app-2.9.0/core_composer_app/static/core_composer_app/user/xsd/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      202 2024-05-13 16:02:03.000000 core_composer_app-2.9.0/core_composer_app/static/core_composer_app/user/xsd/new_base_template.xsd
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:21.996766 core_composer_app-2.9.0/core_composer_app/static/core_composer_app/user/xsl/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4750 2024-05-13 16:02:03.000000 core_composer_app-2.9.0/core_composer_app/static/core_composer_app/user/xsl/xsd2html.xsl
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:20.218706 core_composer_app-2.9.0/core_composer_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:20.298561 core_composer_app-2.9.0/core_composer_app/templates/core_composer_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:20.282809 core_composer_app-2.9.0/core_composer_app/templates/core_composer_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:22.171049 core_composer_app-2.9.0/core_composer_app/templates/core_composer_app/admin/buckets/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      168 2024-05-13 16:02:03.000000 core_composer_app-2.9.0/core_composer_app/templates/core_composer_app/admin/buckets/add.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1022 2024-05-13 16:02:03.000000 core_composer_app-2.9.0/core_composer_app/templates/core_composer_app/admin/buckets/add_content.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      348 2024-05-13 16:02:03.000000 core_composer_app-2.9.0/core_composer_app/templates/core_composer_app/admin/buckets/edit.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1221 2024-05-13 16:02:03.000000 core_composer_app-2.9.0/core_composer_app/templates/core_composer_app/admin/buckets/edit_content.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:22.191274 core_composer_app-2.9.0/core_composer_app/templates/core_composer_app/admin/buckets/list/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1429 2024-05-13 16:02:03.000000 core_composer_app-2.9.0/core_composer_app/templates/core_composer_app/admin/buckets/list/available.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      165 2024-05-13 16:02:03.000000 core_composer_app-2.9.0/core_composer_app/templates/core_composer_app/admin/buckets/list.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:22.227640 core_composer_app-2.9.0/core_composer_app/templates/core_composer_app/admin/buckets/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      664 2024-05-13 16:02:03.000000 core_composer_app-2.9.0/core_composer_app/templates/core_composer_app/admin/buckets/modals/delete.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:22.284959 core_composer_app-2.9.0/core_composer_app/templates/core_composer_app/admin/types/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:22.337762 core_composer_app-2.9.0/core_composer_app/templates/core_composer_app/admin/types/list/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2066 2024-05-13 16:02:04.000000 core_composer_app-2.9.0/core_composer_app/templates/core_composer_app/admin/types/list/available.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1120 2024-05-13 16:02:04.000000 core_composer_app-2.9.0/core_composer_app/templates/core_composer_app/admin/types/list/disabled.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      228 2024-05-13 16:02:03.000000 core_composer_app-2.9.0/core_composer_app/templates/core_composer_app/admin/types/list.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       58 2024-05-13 16:02:04.000000 core_composer_app-2.9.0/core_composer_app/templates/core_composer_app/admin/types/upload.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:22.376143 core_composer_app-2.9.0/core_composer_app/templates/core_composer_app/admin/types/versions/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1411 2024-05-13 16:02:04.000000 core_composer_app-2.9.0/core_composer_app/templates/core_composer_app/admin/types/versions/available.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       68 2024-05-13 16:02:04.000000 core_composer_app-2.9.0/core_composer_app/templates/core_composer_app/admin/types/versions/disabled.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      360 2024-05-13 16:02:04.000000 core_composer_app-2.9.0/core_composer_app/templates/core_composer_app/admin/types/versions.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:22.412439 core_composer_app-2.9.0/core_composer_app/templates/core_composer_app/user/
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     1301 2024-05-13 16:02:04.000000 core_composer_app-2.9.0/core_composer_app/templates/core_composer_app/user/build_template.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:22.454015 core_composer_app-2.9.0/core_composer_app/templates/core_composer_app/user/builder/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      889 2024-05-13 16:02:04.000000 core_composer_app-2.9.0/core_composer_app/templates/core_composer_app/user/builder/list_types.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:22.523054 core_composer_app-2.9.0/core_composer_app/templates/core_composer_app/user/builder/menus/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      276 2024-05-13 16:02:04.000000 core_composer_app-2.9.0/core_composer_app/templates/core_composer_app/user/builder/menus/element.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      126 2024-05-13 16:02:04.000000 core_composer_app-2.9.0/core_composer_app/templates/core_composer_app/user/builder/menus/element_root.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      198 2024-05-13 16:02:04.000000 core_composer_app-2.9.0/core_composer_app/templates/core_composer_app/user/builder/menus/sequence.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:22.693453 core_composer_app-2.9.0/core_composer_app/templates/core_composer_app/user/builder/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      767 2024-05-13 16:02:04.000000 core_composer_app-2.9.0/core_composer_app/templates/core_composer_app/user/builder/modals/change_type.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      639 2024-05-13 16:02:04.000000 core_composer_app-2.9.0/core_composer_app/templates/core_composer_app/user/builder/modals/delete_element.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      819 2024-05-13 16:02:04.000000 core_composer_app-2.9.0/core_composer_app/templates/core_composer_app/user/builder/modals/element_name.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      525 2024-05-13 16:02:04.000000 core_composer_app-2.9.0/core_composer_app/templates/core_composer_app/user/builder/modals/errors.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1291 2024-05-13 16:02:04.000000 core_composer_app-2.9.0/core_composer_app/templates/core_composer_app/user/builder/modals/insert_element.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1186 2024-05-13 16:02:04.000000 core_composer_app-2.9.0/core_composer_app/templates/core_composer_app/user/builder/modals/occurrences.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      676 2024-05-13 16:02:04.000000 core_composer_app-2.9.0/core_composer_app/templates/core_composer_app/user/builder/modals/root_type_name.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:04.000000 core_composer_app-2.9.0/core_composer_app/templates/core_composer_app/user/builder/modals/save_success.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      723 2024-05-13 16:02:04.000000 core_composer_app-2.9.0/core_composer_app/templates/core_composer_app/user/builder/modals/save_template.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      705 2024-05-13 16:02:04.000000 core_composer_app-2.9.0/core_composer_app/templates/core_composer_app/user/builder/modals/save_type.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      384 2024-05-13 16:02:04.000000 core_composer_app-2.9.0/core_composer_app/templates/core_composer_app/user/builder/new_element.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2031 2024-05-13 16:02:04.000000 core_composer_app-2.9.0/core_composer_app/templates/core_composer_app/user/index.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:22.713644 core_composer_app-2.9.0/core_composer_app/templates/core_composer_app/user/list/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      275 2024-05-13 16:02:04.000000 core_composer_app-2.9.0/core_composer_app/templates/core_composer_app/user/list/list.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:22.733790 core_composer_app-2.9.0/core_composer_app/templates/core_composer_app/user/types/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:22.754094 core_composer_app-2.9.0/core_composer_app/templates/core_composer_app/user/types/versions/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      325 2024-05-13 16:02:04.000000 core_composer_app-2.9.0/core_composer_app/templates/core_composer_app/user/types/versions/available.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      262 2024-05-13 16:02:04.000000 core_composer_app-2.9.0/core_composer_app/templates/core_composer_app/user/types/versions.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2529 2024-05-13 16:02:04.000000 core_composer_app-2.9.0/core_composer_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:22.802984 core_composer_app-2.9.0/core_composer_app/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:04.000000 core_composer_app-2.9.0/core_composer_app/utils/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    16675 2024-05-13 16:02:04.000000 core_composer_app-2.9.0/core_composer_app/utils/xml.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:22.824481 core_composer_app-2.9.0/core_composer_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:04.000000 core_composer_app-2.9.0/core_composer_app/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:22.904795 core_composer_app-2.9.0/core_composer_app/views/admin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:04.000000 core_composer_app-2.9.0/core_composer_app/views/admin/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3879 2024-05-13 16:02:04.000000 core_composer_app-2.9.0/core_composer_app/views/admin/ajax.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2157 2024-05-13 16:02:04.000000 core_composer_app-2.9.0/core_composer_app/views/admin/forms.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    17258 2024-05-13 16:02:04.000000 core_composer_app-2.9.0/core_composer_app/views/admin/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:22.978813 core_composer_app-2.9.0/core_composer_app/views/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:04.000000 core_composer_app-2.9.0/core_composer_app/views/user/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    17130 2024-05-13 16:02:04.000000 core_composer_app-2.9.0/core_composer_app/views/user/ajax.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9936 2024-05-13 16:02:04.000000 core_composer_app-2.9.0/core_composer_app/views/user/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:20.951836 core_composer_app-2.9.0/core_composer_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1038 2024-05-13 16:02:19.000000 core_composer_app-2.9.0/core_composer_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7003 2024-05-13 16:02:19.000000 core_composer_app-2.9.0/core_composer_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2024-05-13 16:02:19.000000 core_composer_app-2.9.0/core_composer_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       67 2024-05-13 16:02:19.000000 core_composer_app-2.9.0/core_composer_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       29 2024-05-13 16:02:19.000000 core_composer_app-2.9.0/core_composer_app.egg-info/top_level.txt
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:23.041920 core_composer_app-2.9.0/docs/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:04.000000 core_composer_app-2.9.0/docs/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11283 2024-05-13 16:02:05.000000 core_composer_app-2.9.0/docs/conf.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      289 2024-05-13 16:02:05.000000 core_composer_app-2.9.0/docs/conf_urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2024-05-13 16:02:15.000000 core_composer_app-2.9.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       21 2024-05-13 16:02:15.000000 core_composer_app-2.9.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2024-05-13 16:02:23.762718 core_composer_app-2.9.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1408 2024-05-13 16:02:15.000000 core_composer_app-2.9.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:23.097549 core_composer_app-2.9.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:15.000000 core_composer_app-2.9.0/tests/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:23.119185 core_composer_app-2.9.0/tests/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:15.000000 core_composer_app-2.9.0/tests/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:23.179634 core_composer_app-2.9.0/tests/components/bucket/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:15.000000 core_composer_app-2.9.0/tests/components/bucket/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:23.217007 core_composer_app-2.9.0/tests/components/bucket/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:15.000000 core_composer_app-2.9.0/tests/components/bucket/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1047 2024-05-13 16:02:16.000000 core_composer_app-2.9.0/tests/components/bucket/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7227 2024-05-13 16:02:16.000000 core_composer_app-2.9.0/tests/components/bucket/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:23.254937 core_composer_app-2.9.0/tests/components/type/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:16.000000 core_composer_app-2.9.0/tests/components/type/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5623 2024-05-13 16:02:16.000000 core_composer_app-2.9.0/tests/components/type/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:23.310897 core_composer_app-2.9.0/tests/components/type_version_manager/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:16.000000 core_composer_app-2.9.0/tests/components/type_version_manager/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:23.359654 core_composer_app-2.9.0/tests/components/type_version_manager/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:16.000000 core_composer_app-2.9.0/tests/components/type_version_manager/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4419 2024-05-13 16:02:16.000000 core_composer_app-2.9.0/tests/components/type_version_manager/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    20898 2024-05-13 16:02:16.000000 core_composer_app-2.9.0/tests/components/type_version_manager/tests_int_access_control.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14720 2024-05-13 16:02:16.000000 core_composer_app-2.9.0/tests/components/type_version_manager/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:23.377801 core_composer_app-2.9.0/tests/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:16.000000 core_composer_app-2.9.0/tests/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:23.462626 core_composer_app-2.9.0/tests/rest/bucket/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:16.000000 core_composer_app-2.9.0/tests/rest/bucket/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    13700 2024-05-13 16:02:16.000000 core_composer_app-2.9.0/tests/rest/bucket/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10519 2024-05-13 16:02:16.000000 core_composer_app-2.9.0/tests/rest/bucket/tests_permission.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:23.524232 core_composer_app-2.9.0/tests/rest/type_version_manager/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:16.000000 core_composer_app-2.9.0/tests/rest/type_version_manager/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14878 2024-05-13 16:02:16.000000 core_composer_app-2.9.0/tests/rest/type_version_manager/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9582 2024-05-13 16:02:16.000000 core_composer_app-2.9.0/tests/rest/type_version_manager/tests_permission.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1582 2024-05-13 16:02:16.000000 core_composer_app-2.9.0/tests/test_settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:23.580413 core_composer_app-2.9.0/tests/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:16.000000 core_composer_app-2.9.0/tests/utils/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8032 2024-05-13 16:02:16.000000 core_composer_app-2.9.0/tests/utils/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:23.601768 core_composer_app-2.9.0/tests/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:16.000000 core_composer_app-2.9.0/tests/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:23.624051 core_composer_app-2.9.0/tests/views/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:16.000000 core_composer_app-2.9.0/tests/views/user/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:23.680248 core_composer_app-2.9.0/tests/views/user/ajax/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:16.000000 core_composer_app-2.9.0/tests/views/user/ajax/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11311 2024-05-13 16:02:16.000000 core_composer_app-2.9.0/tests/views/user/ajax/tests_permissions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    22448 2024-05-13 16:02:16.000000 core_composer_app-2.9.0/tests/views/user/ajax/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:23.716374 core_composer_app-2.9.0/tests/views/user/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:16.000000 core_composer_app-2.9.0/tests/views/user/views/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7141 2024-05-13 16:02:16.000000 core_composer_app-2.9.0/tests/views/user/views/tests_unit.py
```

### Comparing `core_composer_app-2.8.0/LICENSE.md` & `core_composer_app-2.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.8.0/PKG-INFO` & `core_composer_app-2.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_composer_app
-Version: 2.8.0
+Version: 2.9.0
 Summary: Template and type composer for the curator core project
 Home-page: https://github.com/usnistgov/core_composer_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: =================
         Core Composer App
```

### Comparing `core_composer_app-2.8.0/README.rst` & `core_composer_app-2.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.8.0/core_composer_app/admin.py` & `core_composer_app-2.9.0/core_composer_app/admin.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.8.0/core_composer_app/components/bucket/api.py` & `core_composer_app-2.9.0/core_composer_app/components/bucket/api.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.8.0/core_composer_app/components/bucket/models.py` & `core_composer_app-2.9.0/core_composer_app/components/bucket/models.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.8.0/core_composer_app/components/type/api.py` & `core_composer_app-2.9.0/core_composer_app/components/type/api.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.8.0/core_composer_app/components/type/models.py` & `core_composer_app-2.9.0/core_composer_app/components/type/models.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.8.0/core_composer_app/components/type_version_manager/api.py` & `core_composer_app-2.9.0/core_composer_app/components/type_version_manager/api.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.8.0/core_composer_app/components/type_version_manager/models.py` & `core_composer_app-2.9.0/core_composer_app/components/type_version_manager/models.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.8.0/core_composer_app/menus.py` & `core_composer_app-2.9.0/core_composer_app/menus.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.8.0/core_composer_app/migrations/0001_initial.py` & `core_composer_app-2.9.0/core_composer_app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.8.0/core_composer_app/models.py` & `core_composer_app-2.9.0/core_composer_app/models.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.8.0/core_composer_app/permissions/discover.py` & `core_composer_app-2.9.0/core_composer_app/permissions/discover.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.8.0/core_composer_app/rest/bucket/serializers.py` & `core_composer_app-2.9.0/core_composer_app/rest/bucket/serializers.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.8.0/core_composer_app/rest/bucket/views.py` & `core_composer_app-2.9.0/core_composer_app/rest/bucket/views.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.8.0/core_composer_app/rest/type_version_manager/abstract_views.py` & `core_composer_app-2.9.0/core_composer_app/rest/type_version_manager/abstract_views.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.8.0/core_composer_app/rest/type_version_manager/serializers.py` & `core_composer_app-2.9.0/core_composer_app/rest/type_version_manager/serializers.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.8.0/core_composer_app/rest/type_version_manager/views.py` & `core_composer_app-2.9.0/core_composer_app/rest/type_version_manager/views.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.8.0/core_composer_app/rest/urls.py` & `core_composer_app-2.9.0/core_composer_app/rest/urls.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.8.0/core_composer_app/static/core_composer_app/admin/js/bucket.js` & `core_composer_app-2.9.0/core_composer_app/static/core_composer_app/admin/js/bucket.js`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.8.0/core_composer_app/static/core_composer_app/admin/js/types/upload/dependencies.js` & `core_composer_app-2.9.0/core_composer_app/static/core_composer_app/admin/js/types/upload/dependencies.js`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.8.0/core_composer_app/static/core_composer_app/user/css/menu.css` & `core_composer_app-2.9.0/core_composer_app/static/core_composer_app/user/css/menu.css`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.8.0/core_composer_app/static/core_composer_app/user/js/build_template.js` & `core_composer_app-2.9.0/core_composer_app/static/core_composer_app/user/js/build_template.js`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.8.0/core_composer_app/static/core_composer_app/user/js/build_template.raw.js` & `core_composer_app-2.9.0/core_composer_app/static/core_composer_app/user/js/build_template.raw.js`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.8.0/core_composer_app/static/core_composer_app/user/js/menus.js` & `core_composer_app-2.9.0/core_composer_app/static/core_composer_app/user/js/menus.js`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.8.0/core_composer_app/static/core_composer_app/user/js/xpath.js` & `core_composer_app-2.9.0/core_composer_app/static/core_composer_app/user/js/xpath.js`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.8.0/core_composer_app/static/core_composer_app/user/xsl/xsd2html.xsl` & `core_composer_app-2.9.0/core_composer_app/static/core_composer_app/user/xsl/xsd2html.xsl`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.8.0/core_composer_app/templates/core_composer_app/admin/buckets/add_content.html` & `core_composer_app-2.9.0/core_composer_app/templates/core_composer_app/admin/buckets/add_content.html`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.8.0/core_composer_app/templates/core_composer_app/admin/buckets/edit_content.html` & `core_composer_app-2.9.0/core_composer_app/templates/core_composer_app/admin/buckets/edit_content.html`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.8.0/core_composer_app/templates/core_composer_app/admin/buckets/list/available.html` & `core_composer_app-2.9.0/core_composer_app/templates/core_composer_app/admin/buckets/list/available.html`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.8.0/core_composer_app/templates/core_composer_app/admin/buckets/modals/delete.html` & `core_composer_app-2.9.0/core_composer_app/templates/core_composer_app/admin/buckets/modals/delete.html`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.8.0/core_composer_app/templates/core_composer_app/admin/types/list/available.html` & `core_composer_app-2.9.0/core_composer_app/templates/core_composer_app/admin/types/list/available.html`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.8.0/core_composer_app/templates/core_composer_app/admin/types/list/disabled.html` & `core_composer_app-2.9.0/core_composer_app/templates/core_composer_app/admin/types/list/disabled.html`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.8.0/core_composer_app/templates/core_composer_app/admin/types/versions/available.html` & `core_composer_app-2.9.0/core_composer_app/templates/core_composer_app/admin/types/versions/available.html`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.8.0/core_composer_app/templates/core_composer_app/user/build_template.html` & `core_composer_app-2.9.0/core_composer_app/templates/core_composer_app/user/build_template.html`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.8.0/core_composer_app/templates/core_composer_app/user/builder/list_types.html` & `core_composer_app-2.9.0/core_composer_app/templates/core_composer_app/user/builder/list_types.html`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.8.0/core_composer_app/templates/core_composer_app/user/builder/modals/change_type.html` & `core_composer_app-2.9.0/core_composer_app/templates/core_composer_app/user/builder/modals/change_type.html`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.8.0/core_composer_app/templates/core_composer_app/user/builder/modals/delete_element.html` & `core_composer_app-2.9.0/core_composer_app/templates/core_composer_app/user/builder/modals/delete_element.html`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.8.0/core_composer_app/templates/core_composer_app/user/builder/modals/element_name.html` & `core_composer_app-2.9.0/core_composer_app/templates/core_composer_app/user/builder/modals/element_name.html`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.8.0/core_composer_app/templates/core_composer_app/user/builder/modals/errors.html` & `core_composer_app-2.9.0/core_composer_app/templates/core_composer_app/user/builder/modals/errors.html`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.8.0/core_composer_app/templates/core_composer_app/user/builder/modals/insert_element.html` & `core_composer_app-2.9.0/core_composer_app/templates/core_composer_app/user/builder/modals/insert_element.html`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.8.0/core_composer_app/templates/core_composer_app/user/builder/modals/occurrences.html` & `core_composer_app-2.9.0/core_composer_app/templates/core_composer_app/user/builder/modals/occurrences.html`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.8.0/core_composer_app/templates/core_composer_app/user/builder/modals/root_type_name.html` & `core_composer_app-2.9.0/core_composer_app/templates/core_composer_app/user/builder/modals/root_type_name.html`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.8.0/core_composer_app/templates/core_composer_app/user/builder/modals/save_template.html` & `core_composer_app-2.9.0/core_composer_app/templates/core_composer_app/user/builder/modals/save_template.html`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.8.0/core_composer_app/templates/core_composer_app/user/builder/modals/save_type.html` & `core_composer_app-2.9.0/core_composer_app/templates/core_composer_app/user/builder/modals/save_type.html`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.8.0/core_composer_app/templates/core_composer_app/user/index.html` & `core_composer_app-2.9.0/core_composer_app/templates/core_composer_app/user/index.html`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.8.0/core_composer_app/urls.py` & `core_composer_app-2.9.0/core_composer_app/urls.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.8.0/core_composer_app/utils/xml.py` & `core_composer_app-2.9.0/core_composer_app/utils/xml.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.8.0/core_composer_app/views/admin/ajax.py` & `core_composer_app-2.9.0/core_composer_app/views/admin/ajax.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,15 @@
 
 class EditBucketView(EditObjectModalView):
     """Edit Bucket View"""
 
     form_class = EditBucketForm
     model = Bucket
     success_url = reverse_lazy("core-admin:core_composer_app_buckets")
-    success_message = "Label edited with success."
+    success_message = "Label edited."
 
     def _save(self, form):
         """_save
 
         Args:
             form
```

### Comparing `core_composer_app-2.8.0/core_composer_app/views/admin/forms.py` & `core_composer_app-2.9.0/core_composer_app/views/admin/forms.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.8.0/core_composer_app/views/admin/views.py` & `core_composer_app-2.9.0/core_composer_app/views/admin/views.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.8.0/core_composer_app/views/user/ajax.py` & `core_composer_app-2.9.0/core_composer_app/views/user/ajax.py`

 * *Files 1% similar despite different names*

```diff
@@ -393,17 +393,15 @@
         except ValidationError:
             return HttpResponseBadRequest(
                 "Title must not be empty or only whitespaces."
             )
         except Exception as exception:
             return _error_response(escape(str(exception)))
 
-        messages.add_message(
-            request, messages.SUCCESS, "Template succesfully saved."
-        )
+        messages.add_message(request, messages.SUCCESS, "Template saved.")
         return HttpResponse(
             json.dumps(response_dict), content_type="application/javascript"
         )
     except Exception as exception:
         return HttpResponseBadRequest(
             escape(str(exception)), content_type="application/javascript"
         )
@@ -494,17 +492,15 @@
         except ValidationError:
             return HttpResponseBadRequest(
                 "Title must not be empty or only whitespaces."
             )
         except Exception as exception:
             return _error_response(escape(str(exception)))
 
-        messages.add_message(
-            request, messages.SUCCESS, "Type succesfully saved."
-        )
+        messages.add_message(request, messages.SUCCESS, "Type saved.")
         return HttpResponse(
             json.dumps(response_dict), content_type="application/javascript"
         )
     except Exception as exception:
         return HttpResponseBadRequest(
             escape(str(exception)), content_type="application/javascript"
         )
```

### Comparing `core_composer_app-2.8.0/core_composer_app/views/user/views.py` & `core_composer_app-2.9.0/core_composer_app/views/user/views.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.8.0/core_composer_app.egg-info/PKG-INFO` & `core_composer_app-2.9.0/core_composer_app.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-composer-app
-Version: 2.8.0
+Version: 2.9.0
 Summary: Template and type composer for the curator core project
 Home-page: https://github.com/usnistgov/core_composer_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: =================
         Core Composer App
```

### Comparing `core_composer_app-2.8.0/core_composer_app.egg-info/SOURCES.txt` & `core_composer_app-2.9.0/core_composer_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.8.0/docs/conf.py` & `core_composer_app-2.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.8.0/setup.py` & `core_composer_app-2.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_composer_app",
-    version="2.8.0",
+    version="2.9.0",
     description="Template and type composer for the curator core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_composer_app",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `core_composer_app-2.8.0/tests/components/bucket/fixtures/fixtures.py` & `core_composer_app-2.9.0/tests/components/bucket/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.8.0/tests/components/bucket/tests_unit.py` & `core_composer_app-2.9.0/tests/components/bucket/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.8.0/tests/components/type/tests_unit.py` & `core_composer_app-2.9.0/tests/components/type/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.8.0/tests/components/type_version_manager/fixtures/fixtures.py` & `core_composer_app-2.9.0/tests/components/type_version_manager/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.8.0/tests/components/type_version_manager/tests_int_access_control.py` & `core_composer_app-2.9.0/tests/components/type_version_manager/tests_int_access_control.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.8.0/tests/components/type_version_manager/tests_unit.py` & `core_composer_app-2.9.0/tests/components/type_version_manager/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.8.0/tests/rest/bucket/tests_int.py` & `core_composer_app-2.9.0/tests/rest/bucket/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.8.0/tests/rest/bucket/tests_permission.py` & `core_composer_app-2.9.0/tests/rest/bucket/tests_permission.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.8.0/tests/rest/type_version_manager/tests_int.py` & `core_composer_app-2.9.0/tests/rest/type_version_manager/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.8.0/tests/rest/type_version_manager/tests_permission.py` & `core_composer_app-2.9.0/tests/rest/type_version_manager/tests_permission.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.8.0/tests/test_settings.py` & `core_composer_app-2.9.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.8.0/tests/utils/tests_unit.py` & `core_composer_app-2.9.0/tests/utils/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.8.0/tests/views/user/ajax/tests_permissions.py` & `core_composer_app-2.9.0/tests/views/user/ajax/tests_permissions.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.8.0/tests/views/user/ajax/tests_unit.py` & `core_composer_app-2.9.0/tests/views/user/ajax/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_composer_app-2.8.0/tests/views/user/views/tests_unit.py` & `core_composer_app-2.9.0/tests/views/user/views/tests_unit.py`

 * *Files identical despite different names*

