# Comparing `tmp/core_main_registry_app-2.8.0.tar.gz` & `tmp/core_main_registry_app-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_main_registry_app-2.8.0.tar", last modified: Tue Mar 12 19:03:42 2024, max compression
+gzip compressed data, was "core_main_registry_app-2.9.0.tar", last modified: Mon May 13 16:08:48 2024, max compression
```

## Comparing `core_main_registry_app-2.8.0.tar` & `core_main_registry_app-2.9.0.tar`

### file list

```diff
@@ -1,204 +1,210 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:42.535217 core_main_registry_app-2.8.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2024-03-12 19:03:33.000000 core_main_registry_app-2.8.0/LICENSE.md
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      177 2024-03-12 19:03:33.000000 core_main_registry_app-2.8.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2045 2024-03-12 19:03:42.528607 core_main_registry_app-2.8.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1275 2024-03-12 19:03:33.000000 core_main_registry_app-2.8.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:39.767898 core_main_registry_app-2.8.0/core_main_registry_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       99 2024-03-12 19:03:33.000000 core_main_registry_app-2.8.0/core_main_registry_app/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5232 2024-03-12 19:03:34.000000 core_main_registry_app-2.8.0/core_main_registry_app/admin.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      539 2024-03-12 19:03:34.000000 core_main_registry_app-2.8.0/core_main_registry_app/apps.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:39.894587 core_main_registry_app-2.8.0/core_main_registry_app/commons/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:34.000000 core_main_registry_app-2.8.0/core_main_registry_app/commons/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      168 2024-03-12 19:03:34.000000 core_main_registry_app-2.8.0/core_main_registry_app/commons/constants.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:39.913824 core_main_registry_app-2.8.0/core_main_registry_app/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:34.000000 core_main_registry_app-2.8.0/core_main_registry_app/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:39.986353 core_main_registry_app-2.8.0/core_main_registry_app/components/category/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:34.000000 core_main_registry_app-2.8.0/core_main_registry_app/components/category/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1843 2024-03-12 19:03:34.000000 core_main_registry_app-2.8.0/core_main_registry_app/components/category/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3721 2024-03-12 19:03:34.000000 core_main_registry_app-2.8.0/core_main_registry_app/components/category/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:40.066861 core_main_registry_app-2.8.0/core_main_registry_app/components/custom_resource/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:34.000000 core_main_registry_app-2.8.0/core_main_registry_app/components/custom_resource/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      478 2024-03-12 19:03:34.000000 core_main_registry_app-2.8.0/core_main_registry_app/components/custom_resource/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7731 2024-03-12 19:03:34.000000 core_main_registry_app-2.8.0/core_main_registry_app/components/custom_resource/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4505 2024-03-12 19:03:34.000000 core_main_registry_app-2.8.0/core_main_registry_app/components/custom_resource/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:40.128848 core_main_registry_app-2.8.0/core_main_registry_app/components/data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:34.000000 core_main_registry_app-2.8.0/core_main_registry_app/components/data/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      515 2024-03-12 19:03:34.000000 core_main_registry_app-2.8.0/core_main_registry_app/components/data/access_control.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3069 2024-03-12 19:03:34.000000 core_main_registry_app-2.8.0/core_main_registry_app/components/data/api.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:40.189041 core_main_registry_app-2.8.0/core_main_registry_app/components/refinement/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:34.000000 core_main_registry_app-2.8.0/core_main_registry_app/components/refinement/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1463 2024-03-12 19:03:34.000000 core_main_registry_app-2.8.0/core_main_registry_app/components/refinement/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2488 2024-03-12 19:03:34.000000 core_main_registry_app-2.8.0/core_main_registry_app/components/refinement/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:40.232583 core_main_registry_app-2.8.0/core_main_registry_app/components/template/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:34.000000 core_main_registry_app-2.8.0/core_main_registry_app/components/template/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      881 2024-03-12 19:03:34.000000 core_main_registry_app-2.8.0/core_main_registry_app/components/template/api.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:40.275420 core_main_registry_app-2.8.0/core_main_registry_app/components/version_manager/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:34.000000 core_main_registry_app-2.8.0/core_main_registry_app/components/version_manager/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      749 2024-03-12 19:03:34.000000 core_main_registry_app-2.8.0/core_main_registry_app/components/version_manager/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      360 2024-03-12 19:03:34.000000 core_main_registry_app-2.8.0/core_main_registry_app/constants.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3751 2024-03-12 19:03:34.000000 core_main_registry_app-2.8.0/core_main_registry_app/discover.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      671 2024-03-12 19:03:34.000000 core_main_registry_app-2.8.0/core_main_registry_app/menus.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:40.327772 core_main_registry_app-2.8.0/core_main_registry_app/migrations/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5740 2024-03-12 19:03:34.000000 core_main_registry_app-2.8.0/core_main_registry_app/migrations/0001_initial.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:34.000000 core_main_registry_app-2.8.0/core_main_registry_app/migrations/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       80 2024-03-12 19:03:34.000000 core_main_registry_app-2.8.0/core_main_registry_app/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:40.381675 core_main_registry_app-2.8.0/core_main_registry_app/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:34.000000 core_main_registry_app-2.8.0/core_main_registry_app/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:40.425318 core_main_registry_app-2.8.0/core_main_registry_app/rest/data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:34.000000 core_main_registry_app-2.8.0/core_main_registry_app/rest/data/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3243 2024-03-12 19:03:34.000000 core_main_registry_app-2.8.0/core_main_registry_app/rest/data/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:40.471757 core_main_registry_app-2.8.0/core_main_registry_app/rest/template_version_manager/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:34.000000 core_main_registry_app-2.8.0/core_main_registry_app/rest/template_version_manager/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      784 2024-03-12 19:03:34.000000 core_main_registry_app-2.8.0/core_main_registry_app/rest/template_version_manager/views.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    12516 2024-03-12 19:03:34.000000 core_main_registry_app-2.8.0/core_main_registry_app/rest/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:40.535389 core_main_registry_app-2.8.0/core_main_registry_app/rest/workspace/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:34.000000 core_main_registry_app-2.8.0/core_main_registry_app/rest/workspace/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      824 2024-03-12 19:03:34.000000 core_main_registry_app-2.8.0/core_main_registry_app/rest/workspace/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      432 2024-03-12 19:03:34.000000 core_main_registry_app-2.8.0/core_main_registry_app/rest/workspace/views.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1149 2024-03-12 19:03:34.000000 core_main_registry_app-2.8.0/core_main_registry_app/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:39.086750 core_main_registry_app-2.8.0/core_main_registry_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:39.169609 core_main_registry_app-2.8.0/core_main_registry_app/static/core_main_registry_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:39.096890 core_main_registry_app-2.8.0/core_main_registry_app/static/core_main_registry_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:39.101464 core_main_registry_app-2.8.0/core_main_registry_app/static/core_main_registry_app/admin/js/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:40.573096 core_main_registry_app-2.8.0/core_main_registry_app/static/core_main_registry_app/admin/js/templates/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      111 2024-03-12 19:03:34.000000 core_main_registry_app-2.8.0/core_main_registry_app/static/core_main_registry_app/admin/js/templates/sort.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:40.594934 core_main_registry_app-2.8.0/core_main_registry_app/static/core_main_registry_app/json/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4331 2024-03-12 19:03:34.000000 core_main_registry_app-2.8.0/core_main_registry_app/static/core_main_registry_app/json/custom_registry.json
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:39.139268 core_main_registry_app-2.8.0/core_main_registry_app/static/core_main_registry_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:39.156367 core_main_registry_app-2.8.0/core_main_registry_app/static/core_main_registry_app/user/css/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:40.625162 core_main_registry_app-2.8.0/core_main_registry_app/static/core_main_registry_app/user/css/fancytree/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      388 2024-03-12 19:03:34.000000 core_main_registry_app-2.8.0/core_main_registry_app/static/core_main_registry_app/user/css/fancytree/fancytree.custom.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:40.668987 core_main_registry_app-2.8.0/core_main_registry_app/static/core_main_registry_app/user/css/resource_banner/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      980 2024-03-12 19:03:34.000000 core_main_registry_app-2.8.0/core_main_registry_app/static/core_main_registry_app/user/css/resource_banner/resource_banner.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      327 2024-03-12 19:03:34.000000 core_main_registry_app-2.8.0/core_main_registry_app/static/core_main_registry_app/user/css/resource_banner/selection.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:40.689143 core_main_registry_app-2.8.0/core_main_registry_app/static/core_main_registry_app/xsd/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)   188155 2024-03-12 19:03:34.000000 core_main_registry_app-2.8.0/core_main_registry_app/static/core_main_registry_app/xsd/res-md.xsd
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:40.714912 core_main_registry_app-2.8.0/core_main_registry_app/static/core_main_registry_app/xsl/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5704 2024-03-12 19:03:34.000000 core_main_registry_app-2.8.0/core_main_registry_app/static/core_main_registry_app/xsl/xml2html.xsl
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:40.756712 core_main_registry_app-2.8.0/core_main_registry_app/system/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:34.000000 core_main_registry_app-2.8.0/core_main_registry_app/system/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2769 2024-03-12 19:03:34.000000 core_main_registry_app-2.8.0/core_main_registry_app/system/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      426 2024-03-12 19:03:34.000000 core_main_registry_app-2.8.0/core_main_registry_app/tasks.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:39.193203 core_main_registry_app-2.8.0/core_main_registry_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:39.235525 core_main_registry_app-2.8.0/core_main_registry_app/templates/core_main_registry_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:39.222301 core_main_registry_app-2.8.0/core_main_registry_app/templates/core_main_registry_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:40.965282 core_main_registry_app-2.8.0/core_main_registry_app/templates/core_main_registry_app/admin/custom_registry/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      338 2024-03-12 19:03:34.000000 core_main_registry_app-2.8.0/core_main_registry_app/templates/core_main_registry_app/admin/custom_registry/list.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      925 2024-03-12 19:03:34.000000 core_main_registry_app-2.8.0/core_main_registry_app/templates/core_main_registry_app/admin/custom_registry/table.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:40.989879 core_main_registry_app-2.8.0/core_main_registry_app/templates/core_main_registry_app/admin/custom_registry/upload/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       60 2024-03-12 19:03:34.000000 core_main_registry_app-2.8.0/core_main_registry_app/templates/core_main_registry_app/admin/custom_registry/upload/base.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      181 2024-03-12 19:03:34.000000 core_main_registry_app-2.8.0/core_main_registry_app/templates/core_main_registry_app/admin/custom_registry/upload.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:41.031596 core_main_registry_app-2.8.0/core_main_registry_app/templates/core_main_registry_app/admin/data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      384 2024-03-12 19:03:34.000000 core_main_registry_app-2.8.0/core_main_registry_app/templates/core_main_registry_app/admin/data/detail.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      319 2024-03-12 19:03:34.000000 core_main_registry_app-2.8.0/core_main_registry_app/templates/core_main_registry_app/admin/data/view_data.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:41.051321 core_main_registry_app-2.8.0/core_main_registry_app/templates/core_main_registry_app/admin/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:41.074419 core_main_registry_app-2.8.0/core_main_registry_app/templates/core_main_registry_app/admin/templates/list/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2382 2024-03-12 19:03:34.000000 core_main_registry_app-2.8.0/core_main_registry_app/templates/core_main_registry_app/admin/templates/list/available.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      510 2024-03-12 19:03:34.000000 core_main_registry_app-2.8.0/core_main_registry_app/templates/core_main_registry_app/admin/templates/list.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:41.105215 core_main_registry_app-2.8.0/core_main_registry_app/templates/core_main_registry_app/resource_banner/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      815 2024-03-12 19:03:34.000000 core_main_registry_app-2.8.0/core_main_registry_app/templates/core_main_registry_app/resource_banner/resource_banner.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5783 2024-03-12 19:03:34.000000 core_main_registry_app-2.8.0/core_main_registry_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:41.128911 core_main_registry_app-2.8.0/core_main_registry_app/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:34.000000 core_main_registry_app-2.8.0/core_main_registry_app/utils/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:41.173108 core_main_registry_app-2.8.0/core_main_registry_app/utils/fancytree/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:34.000000 core_main_registry_app-2.8.0/core_main_registry_app/utils/fancytree/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10322 2024-03-12 19:03:34.000000 core_main_registry_app-2.8.0/core_main_registry_app/utils/fancytree/widget.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:41.218584 core_main_registry_app-2.8.0/core_main_registry_app/utils/menu/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:34.000000 core_main_registry_app-2.8.0/core_main_registry_app/utils/menu/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      560 2024-03-12 19:03:34.000000 core_main_registry_app-2.8.0/core_main_registry_app/utils/menu/menu_utils.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:41.299871 core_main_registry_app-2.8.0/core_main_registry_app/utils/refinement/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:34.000000 core_main_registry_app-2.8.0/core_main_registry_app/utils/refinement/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6124 2024-03-12 19:03:34.000000 core_main_registry_app-2.8.0/core_main_registry_app/utils/refinement/mongo_query.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2776 2024-03-12 19:03:34.000000 core_main_registry_app-2.8.0/core_main_registry_app/utils/refinement/refinement.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:41.359281 core_main_registry_app-2.8.0/core_main_registry_app/utils/refinement/tools/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:34.000000 core_main_registry_app-2.8.0/core_main_registry_app/utils/refinement/tools/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3577 2024-03-12 19:03:35.000000 core_main_registry_app-2.8.0/core_main_registry_app/utils/refinement/tools/tree.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9709 2024-03-12 19:03:35.000000 core_main_registry_app-2.8.0/core_main_registry_app/utils/refinement/tools/xsd_refinements.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1032 2024-03-12 19:03:35.000000 core_main_registry_app-2.8.0/core_main_registry_app/utils/refinement/watch.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:41.403313 core_main_registry_app-2.8.0/core_main_registry_app/utils/role/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:35.000000 core_main_registry_app-2.8.0/core_main_registry_app/utils/role/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      553 2024-03-12 19:03:35.000000 core_main_registry_app-2.8.0/core_main_registry_app/utils/role/extraction.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:41.423793 core_main_registry_app-2.8.0/core_main_registry_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:35.000000 core_main_registry_app-2.8.0/core_main_registry_app/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:41.491519 core_main_registry_app-2.8.0/core_main_registry_app/views/admin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:35.000000 core_main_registry_app-2.8.0/core_main_registry_app/views/admin/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      310 2024-03-12 19:03:35.000000 core_main_registry_app-2.8.0/core_main_registry_app/views/admin/forms.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7295 2024-03-12 19:03:35.000000 core_main_registry_app-2.8.0/core_main_registry_app/views/admin/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:39.853271 core_main_registry_app-2.8.0/core_main_registry_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2045 2024-03-12 19:03:38.000000 core_main_registry_app-2.8.0/core_main_registry_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6263 2024-03-12 19:03:38.000000 core_main_registry_app-2.8.0/core_main_registry_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2024-03-12 19:03:38.000000 core_main_registry_app-2.8.0/core_main_registry_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      103 2024-03-12 19:03:38.000000 core_main_registry_app-2.8.0/core_main_registry_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       29 2024-03-12 19:03:38.000000 core_main_registry_app-2.8.0/core_main_registry_app.egg-info/top_level.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2024-03-12 19:03:35.000000 core_main_registry_app-2.8.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       53 2024-03-12 19:03:35.000000 core_main_registry_app-2.8.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       49 2024-03-12 19:03:35.000000 core_main_registry_app-2.8.0/requirements.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2024-03-12 19:03:42.537762 core_main_registry_app-2.8.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1413 2024-03-12 19:03:35.000000 core_main_registry_app-2.8.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:41.603488 core_main_registry_app-2.8.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:35.000000 core_main_registry_app-2.8.0/tests/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:41.628372 core_main_registry_app-2.8.0/tests/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:35.000000 core_main_registry_app-2.8.0/tests/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:41.680308 core_main_registry_app-2.8.0/tests/components/category/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:35.000000 core_main_registry_app-2.8.0/tests/components/category/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5376 2024-03-12 19:03:35.000000 core_main_registry_app-2.8.0/tests/components/category/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:41.743004 core_main_registry_app-2.8.0/tests/components/custom_resource/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:35.000000 core_main_registry_app-2.8.0/tests/components/custom_resource/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:41.787329 core_main_registry_app-2.8.0/tests/components/custom_resource/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:35.000000 core_main_registry_app-2.8.0/tests/components/custom_resource/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5245 2024-03-12 19:03:35.000000 core_main_registry_app-2.8.0/tests/components/custom_resource/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14360 2024-03-12 19:03:35.000000 core_main_registry_app-2.8.0/tests/components/custom_resource/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14727 2024-03-12 19:03:35.000000 core_main_registry_app-2.8.0/tests/components/custom_resource/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:41.830899 core_main_registry_app-2.8.0/tests/components/data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:35.000000 core_main_registry_app-2.8.0/tests/components/data/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:41.878468 core_main_registry_app-2.8.0/tests/components/data/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:35.000000 core_main_registry_app-2.8.0/tests/components/data/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2996 2024-03-12 19:03:35.000000 core_main_registry_app-2.8.0/tests/components/data/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4813 2024-03-12 19:03:35.000000 core_main_registry_app-2.8.0/tests/components/data/tests_int.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:41.924471 core_main_registry_app-2.8.0/tests/components/refinement/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:35.000000 core_main_registry_app-2.8.0/tests/components/refinement/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4487 2024-03-12 19:03:35.000000 core_main_registry_app-2.8.0/tests/components/refinement/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:41.947066 core_main_registry_app-2.8.0/tests/components/template_version_manager/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:35.000000 core_main_registry_app-2.8.0/tests/components/template_version_manager/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:41.997416 core_main_registry_app-2.8.0/tests/components/template_version_manager/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:35.000000 core_main_registry_app-2.8.0/tests/components/template_version_manager/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2182 2024-03-12 19:03:35.000000 core_main_registry_app-2.8.0/tests/components/template_version_manager/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      539 2024-03-12 19:03:35.000000 core_main_registry_app-2.8.0/tests/mocks.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:42.019870 core_main_registry_app-2.8.0/tests/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:35.000000 core_main_registry_app-2.8.0/tests/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:42.071258 core_main_registry_app-2.8.0/tests/rest/data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:35.000000 core_main_registry_app-2.8.0/tests/rest/data/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5430 2024-03-12 19:03:35.000000 core_main_registry_app-2.8.0/tests/rest/data/tests_permissions.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:42.135063 core_main_registry_app-2.8.0/tests/rest/template_version_manager/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:35.000000 core_main_registry_app-2.8.0/tests/rest/template_version_manager/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3008 2024-03-12 19:03:35.000000 core_main_registry_app-2.8.0/tests/rest/template_version_manager/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2135 2024-03-12 19:03:35.000000 core_main_registry_app-2.8.0/tests/rest/template_version_manager/tests_permission.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:42.180745 core_main_registry_app-2.8.0/tests/rest/urls/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:35.000000 core_main_registry_app-2.8.0/tests/rest/urls/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      501 2024-03-12 19:03:35.000000 core_main_registry_app-2.8.0/tests/rest/urls/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:42.200167 core_main_registry_app-2.8.0/tests/rest/workspace/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:35.000000 core_main_registry_app-2.8.0/tests/rest/workspace/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:42.242609 core_main_registry_app-2.8.0/tests/rest/workspace/serializers/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:35.000000 core_main_registry_app-2.8.0/tests/rest/workspace/serializers/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1514 2024-03-12 19:03:35.000000 core_main_registry_app-2.8.0/tests/rest/workspace/serializers/tests_unit.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1085 2024-03-12 19:03:35.000000 core_main_registry_app-2.8.0/tests/test_menus.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1918 2024-03-12 19:03:35.000000 core_main_registry_app-2.8.0/tests/test_settings.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      194 2024-03-12 19:03:35.000000 core_main_registry_app-2.8.0/tests/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:42.263458 core_main_registry_app-2.8.0/tests/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:35.000000 core_main_registry_app-2.8.0/tests/utils/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:42.289192 core_main_registry_app-2.8.0/tests/utils/fancytree/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:35.000000 core_main_registry_app-2.8.0/tests/utils/fancytree/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:42.338559 core_main_registry_app-2.8.0/tests/utils/fancytree/widget/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:35.000000 core_main_registry_app-2.8.0/tests/utils/fancytree/widget/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      717 2024-03-12 19:03:35.000000 core_main_registry_app-2.8.0/tests/utils/fancytree/widget/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:42.385341 core_main_registry_app-2.8.0/tests/utils/role/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:35.000000 core_main_registry_app-2.8.0/tests/utils/role/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      761 2024-03-12 19:03:35.000000 core_main_registry_app-2.8.0/tests/utils/role/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:42.408965 core_main_registry_app-2.8.0/tests/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:35.000000 core_main_registry_app-2.8.0/tests/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:42.435599 core_main_registry_app-2.8.0/tests/views/admin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:35.000000 core_main_registry_app-2.8.0/tests/views/admin/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:42.507070 core_main_registry_app-2.8.0/tests/views/admin/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:35.000000 core_main_registry_app-2.8.0/tests/views/admin/views/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4418 2024-03-12 19:03:35.000000 core_main_registry_app-2.8.0/tests/views/admin/views/test_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5686 2024-03-12 19:03:35.000000 core_main_registry_app-2.8.0/tests/views/admin/views/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:48.915053 core_main_registry_app-2.9.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2024-05-13 16:08:40.000000 core_main_registry_app-2.9.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      177 2024-05-13 16:08:40.000000 core_main_registry_app-2.9.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2045 2024-05-13 16:08:48.909233 core_main_registry_app-2.9.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1275 2024-05-13 16:08:40.000000 core_main_registry_app-2.9.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:46.277151 core_main_registry_app-2.9.0/core_main_registry_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       99 2024-05-13 16:08:40.000000 core_main_registry_app-2.9.0/core_main_registry_app/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5232 2024-05-13 16:08:40.000000 core_main_registry_app-2.9.0/core_main_registry_app/admin.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      605 2024-05-13 16:08:40.000000 core_main_registry_app-2.9.0/core_main_registry_app/apps.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:46.458696 core_main_registry_app-2.9.0/core_main_registry_app/commons/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:40.000000 core_main_registry_app-2.9.0/core_main_registry_app/commons/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      168 2024-05-13 16:08:40.000000 core_main_registry_app-2.9.0/core_main_registry_app/commons/constants.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:46.482860 core_main_registry_app-2.9.0/core_main_registry_app/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:40.000000 core_main_registry_app-2.9.0/core_main_registry_app/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:46.551306 core_main_registry_app-2.9.0/core_main_registry_app/components/category/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:40.000000 core_main_registry_app-2.9.0/core_main_registry_app/components/category/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1843 2024-05-13 16:08:40.000000 core_main_registry_app-2.9.0/core_main_registry_app/components/category/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3721 2024-05-13 16:08:40.000000 core_main_registry_app-2.9.0/core_main_registry_app/components/category/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:46.624605 core_main_registry_app-2.9.0/core_main_registry_app/components/custom_resource/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:40.000000 core_main_registry_app-2.9.0/core_main_registry_app/components/custom_resource/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      478 2024-05-13 16:08:40.000000 core_main_registry_app-2.9.0/core_main_registry_app/components/custom_resource/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7221 2024-05-13 16:08:40.000000 core_main_registry_app-2.9.0/core_main_registry_app/components/custom_resource/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4505 2024-05-13 16:08:40.000000 core_main_registry_app-2.9.0/core_main_registry_app/components/custom_resource/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:46.676833 core_main_registry_app-2.9.0/core_main_registry_app/components/data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:40.000000 core_main_registry_app-2.9.0/core_main_registry_app/components/data/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      515 2024-05-13 16:08:40.000000 core_main_registry_app-2.9.0/core_main_registry_app/components/data/access_control.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3069 2024-05-13 16:08:40.000000 core_main_registry_app-2.9.0/core_main_registry_app/components/data/api.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:46.734468 core_main_registry_app-2.9.0/core_main_registry_app/components/refinement/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:41.000000 core_main_registry_app-2.9.0/core_main_registry_app/components/refinement/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1463 2024-05-13 16:08:41.000000 core_main_registry_app-2.9.0/core_main_registry_app/components/refinement/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2488 2024-05-13 16:08:41.000000 core_main_registry_app-2.9.0/core_main_registry_app/components/refinement/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:46.768108 core_main_registry_app-2.9.0/core_main_registry_app/components/template/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:41.000000 core_main_registry_app-2.9.0/core_main_registry_app/components/template/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      881 2024-05-13 16:08:41.000000 core_main_registry_app-2.9.0/core_main_registry_app/components/template/api.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:46.804436 core_main_registry_app-2.9.0/core_main_registry_app/components/version_manager/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:41.000000 core_main_registry_app-2.9.0/core_main_registry_app/components/version_manager/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      749 2024-05-13 16:08:41.000000 core_main_registry_app-2.9.0/core_main_registry_app/components/version_manager/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      360 2024-05-13 16:08:41.000000 core_main_registry_app-2.9.0/core_main_registry_app/constants.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4951 2024-05-13 16:08:41.000000 core_main_registry_app-2.9.0/core_main_registry_app/discover.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      671 2024-05-13 16:08:41.000000 core_main_registry_app-2.9.0/core_main_registry_app/menus.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:46.848256 core_main_registry_app-2.9.0/core_main_registry_app/migrations/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5740 2024-05-13 16:08:41.000000 core_main_registry_app-2.9.0/core_main_registry_app/migrations/0001_initial.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      568 2024-05-13 16:08:41.000000 core_main_registry_app-2.9.0/core_main_registry_app/migrations/0002_init_data.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:41.000000 core_main_registry_app-2.9.0/core_main_registry_app/migrations/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       80 2024-05-13 16:08:41.000000 core_main_registry_app-2.9.0/core_main_registry_app/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:46.889146 core_main_registry_app-2.9.0/core_main_registry_app/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:41.000000 core_main_registry_app-2.9.0/core_main_registry_app/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:46.928457 core_main_registry_app-2.9.0/core_main_registry_app/rest/data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:41.000000 core_main_registry_app-2.9.0/core_main_registry_app/rest/data/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3243 2024-05-13 16:08:41.000000 core_main_registry_app-2.9.0/core_main_registry_app/rest/data/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:46.967448 core_main_registry_app-2.9.0/core_main_registry_app/rest/template_version_manager/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:41.000000 core_main_registry_app-2.9.0/core_main_registry_app/rest/template_version_manager/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      784 2024-05-13 16:08:41.000000 core_main_registry_app-2.9.0/core_main_registry_app/rest/template_version_manager/views.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    12516 2024-05-13 16:08:41.000000 core_main_registry_app-2.9.0/core_main_registry_app/rest/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:47.024489 core_main_registry_app-2.9.0/core_main_registry_app/rest/workspace/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:41.000000 core_main_registry_app-2.9.0/core_main_registry_app/rest/workspace/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      824 2024-05-13 16:08:41.000000 core_main_registry_app-2.9.0/core_main_registry_app/rest/workspace/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      432 2024-05-13 16:08:41.000000 core_main_registry_app-2.9.0/core_main_registry_app/rest/workspace/views.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1614 2024-05-13 16:08:41.000000 core_main_registry_app-2.9.0/core_main_registry_app/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:45.617958 core_main_registry_app-2.9.0/core_main_registry_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:45.668074 core_main_registry_app-2.9.0/core_main_registry_app/static/core_main_registry_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:45.624779 core_main_registry_app-2.9.0/core_main_registry_app/static/core_main_registry_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:45.628177 core_main_registry_app-2.9.0/core_main_registry_app/static/core_main_registry_app/admin/js/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:47.064957 core_main_registry_app-2.9.0/core_main_registry_app/static/core_main_registry_app/admin/js/templates/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      111 2024-05-13 16:08:41.000000 core_main_registry_app-2.9.0/core_main_registry_app/static/core_main_registry_app/admin/js/templates/sort.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:47.084160 core_main_registry_app-2.9.0/core_main_registry_app/static/core_main_registry_app/json/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4331 2024-05-13 16:08:41.000000 core_main_registry_app-2.9.0/core_main_registry_app/static/core_main_registry_app/json/custom_registry.json
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:45.644853 core_main_registry_app-2.9.0/core_main_registry_app/static/core_main_registry_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:45.653648 core_main_registry_app-2.9.0/core_main_registry_app/static/core_main_registry_app/user/css/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:47.106806 core_main_registry_app-2.9.0/core_main_registry_app/static/core_main_registry_app/user/css/fancytree/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      388 2024-05-13 16:08:41.000000 core_main_registry_app-2.9.0/core_main_registry_app/static/core_main_registry_app/user/css/fancytree/fancytree.custom.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:47.141053 core_main_registry_app-2.9.0/core_main_registry_app/static/core_main_registry_app/user/css/resource_banner/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      980 2024-05-13 16:08:41.000000 core_main_registry_app-2.9.0/core_main_registry_app/static/core_main_registry_app/user/css/resource_banner/resource_banner.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      327 2024-05-13 16:08:41.000000 core_main_registry_app-2.9.0/core_main_registry_app/static/core_main_registry_app/user/css/resource_banner/selection.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:47.158710 core_main_registry_app-2.9.0/core_main_registry_app/static/core_main_registry_app/xsd/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)   188155 2024-05-13 16:08:41.000000 core_main_registry_app-2.9.0/core_main_registry_app/static/core_main_registry_app/xsd/res-md.xsd
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:47.217072 core_main_registry_app-2.9.0/core_main_registry_app/static/core_main_registry_app/xsl/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6861 2024-05-13 16:08:41.000000 core_main_registry_app-2.9.0/core_main_registry_app/static/core_main_registry_app/xsl/registry-detail.xsl
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4230 2024-05-13 16:08:41.000000 core_main_registry_app-2.9.0/core_main_registry_app/static/core_main_registry_app/xsl/registry-list.xsl
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5704 2024-05-13 16:08:41.000000 core_main_registry_app-2.9.0/core_main_registry_app/static/core_main_registry_app/xsl/xml2html.xsl
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:47.252996 core_main_registry_app-2.9.0/core_main_registry_app/system/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:41.000000 core_main_registry_app-2.9.0/core_main_registry_app/system/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2769 2024-05-13 16:08:41.000000 core_main_registry_app-2.9.0/core_main_registry_app/system/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      426 2024-05-13 16:08:41.000000 core_main_registry_app-2.9.0/core_main_registry_app/tasks.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:45.699913 core_main_registry_app-2.9.0/core_main_registry_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:45.734909 core_main_registry_app-2.9.0/core_main_registry_app/templates/core_main_registry_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:45.724121 core_main_registry_app-2.9.0/core_main_registry_app/templates/core_main_registry_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:47.322389 core_main_registry_app-2.9.0/core_main_registry_app/templates/core_main_registry_app/admin/custom_registry/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      338 2024-05-13 16:08:41.000000 core_main_registry_app-2.9.0/core_main_registry_app/templates/core_main_registry_app/admin/custom_registry/list.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      925 2024-05-13 16:08:41.000000 core_main_registry_app-2.9.0/core_main_registry_app/templates/core_main_registry_app/admin/custom_registry/table.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:47.340697 core_main_registry_app-2.9.0/core_main_registry_app/templates/core_main_registry_app/admin/custom_registry/upload/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       60 2024-05-13 16:08:41.000000 core_main_registry_app-2.9.0/core_main_registry_app/templates/core_main_registry_app/admin/custom_registry/upload/base.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      181 2024-05-13 16:08:41.000000 core_main_registry_app-2.9.0/core_main_registry_app/templates/core_main_registry_app/admin/custom_registry/upload.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:47.374452 core_main_registry_app-2.9.0/core_main_registry_app/templates/core_main_registry_app/admin/data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      384 2024-05-13 16:08:41.000000 core_main_registry_app-2.9.0/core_main_registry_app/templates/core_main_registry_app/admin/data/detail.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      319 2024-05-13 16:08:41.000000 core_main_registry_app-2.9.0/core_main_registry_app/templates/core_main_registry_app/admin/data/view_data.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:47.391756 core_main_registry_app-2.9.0/core_main_registry_app/templates/core_main_registry_app/admin/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:47.409563 core_main_registry_app-2.9.0/core_main_registry_app/templates/core_main_registry_app/admin/templates/list/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2382 2024-05-13 16:08:41.000000 core_main_registry_app-2.9.0/core_main_registry_app/templates/core_main_registry_app/admin/templates/list/available.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      510 2024-05-13 16:08:41.000000 core_main_registry_app-2.9.0/core_main_registry_app/templates/core_main_registry_app/admin/templates/list.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:47.429368 core_main_registry_app-2.9.0/core_main_registry_app/templates/core_main_registry_app/resource_banner/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      815 2024-05-13 16:08:41.000000 core_main_registry_app-2.9.0/core_main_registry_app/templates/core_main_registry_app/resource_banner/resource_banner.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5783 2024-05-13 16:08:41.000000 core_main_registry_app-2.9.0/core_main_registry_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:47.446833 core_main_registry_app-2.9.0/core_main_registry_app/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:41.000000 core_main_registry_app-2.9.0/core_main_registry_app/utils/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:47.488528 core_main_registry_app-2.9.0/core_main_registry_app/utils/fancytree/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:41.000000 core_main_registry_app-2.9.0/core_main_registry_app/utils/fancytree/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10322 2024-05-13 16:08:41.000000 core_main_registry_app-2.9.0/core_main_registry_app/utils/fancytree/widget.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:47.530022 core_main_registry_app-2.9.0/core_main_registry_app/utils/menu/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:41.000000 core_main_registry_app-2.9.0/core_main_registry_app/utils/menu/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      560 2024-05-13 16:08:41.000000 core_main_registry_app-2.9.0/core_main_registry_app/utils/menu/menu_utils.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:47.628613 core_main_registry_app-2.9.0/core_main_registry_app/utils/refinement/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:41.000000 core_main_registry_app-2.9.0/core_main_registry_app/utils/refinement/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6124 2024-05-13 16:08:41.000000 core_main_registry_app-2.9.0/core_main_registry_app/utils/refinement/mongo_query.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2773 2024-05-13 16:08:41.000000 core_main_registry_app-2.9.0/core_main_registry_app/utils/refinement/refinement.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:47.707399 core_main_registry_app-2.9.0/core_main_registry_app/utils/refinement/tools/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:41.000000 core_main_registry_app-2.9.0/core_main_registry_app/utils/refinement/tools/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3577 2024-05-13 16:08:41.000000 core_main_registry_app-2.9.0/core_main_registry_app/utils/refinement/tools/tree.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9709 2024-05-13 16:08:41.000000 core_main_registry_app-2.9.0/core_main_registry_app/utils/refinement/tools/xsd_refinements.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1032 2024-05-13 16:08:41.000000 core_main_registry_app-2.9.0/core_main_registry_app/utils/refinement/watch.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:47.743970 core_main_registry_app-2.9.0/core_main_registry_app/utils/role/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:41.000000 core_main_registry_app-2.9.0/core_main_registry_app/utils/role/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      553 2024-05-13 16:08:41.000000 core_main_registry_app-2.9.0/core_main_registry_app/utils/role/extraction.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:47.761637 core_main_registry_app-2.9.0/core_main_registry_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:41.000000 core_main_registry_app-2.9.0/core_main_registry_app/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:47.838222 core_main_registry_app-2.9.0/core_main_registry_app/views/admin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:41.000000 core_main_registry_app-2.9.0/core_main_registry_app/views/admin/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      310 2024-05-13 16:08:41.000000 core_main_registry_app-2.9.0/core_main_registry_app/views/admin/forms.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7295 2024-05-13 16:08:41.000000 core_main_registry_app-2.9.0/core_main_registry_app/views/admin/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:46.411437 core_main_registry_app-2.9.0/core_main_registry_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2045 2024-05-13 16:08:44.000000 core_main_registry_app-2.9.0/core_main_registry_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6523 2024-05-13 16:08:45.000000 core_main_registry_app-2.9.0/core_main_registry_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2024-05-13 16:08:44.000000 core_main_registry_app-2.9.0/core_main_registry_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      103 2024-05-13 16:08:44.000000 core_main_registry_app-2.9.0/core_main_registry_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       29 2024-05-13 16:08:44.000000 core_main_registry_app-2.9.0/core_main_registry_app.egg-info/top_level.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2024-05-13 16:08:41.000000 core_main_registry_app-2.9.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       53 2024-05-13 16:08:41.000000 core_main_registry_app-2.9.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       49 2024-05-13 16:08:41.000000 core_main_registry_app-2.9.0/requirements.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2024-05-13 16:08:48.917603 core_main_registry_app-2.9.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1413 2024-05-13 16:08:41.000000 core_main_registry_app-2.9.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:47.946003 core_main_registry_app-2.9.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:42.000000 core_main_registry_app-2.9.0/tests/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:47.966520 core_main_registry_app-2.9.0/tests/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:42.000000 core_main_registry_app-2.9.0/tests/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:48.036830 core_main_registry_app-2.9.0/tests/components/category/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:42.000000 core_main_registry_app-2.9.0/tests/components/category/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5568 2024-05-13 16:08:42.000000 core_main_registry_app-2.9.0/tests/components/category/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:48.101292 core_main_registry_app-2.9.0/tests/components/custom_resource/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:42.000000 core_main_registry_app-2.9.0/tests/components/custom_resource/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:48.146671 core_main_registry_app-2.9.0/tests/components/custom_resource/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:42.000000 core_main_registry_app-2.9.0/tests/components/custom_resource/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5245 2024-05-13 16:08:42.000000 core_main_registry_app-2.9.0/tests/components/custom_resource/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14360 2024-05-13 16:08:42.000000 core_main_registry_app-2.9.0/tests/components/custom_resource/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14691 2024-05-13 16:08:42.000000 core_main_registry_app-2.9.0/tests/components/custom_resource/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:48.215894 core_main_registry_app-2.9.0/tests/components/data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:42.000000 core_main_registry_app-2.9.0/tests/components/data/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:48.256030 core_main_registry_app-2.9.0/tests/components/data/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:42.000000 core_main_registry_app-2.9.0/tests/components/data/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2996 2024-05-13 16:08:42.000000 core_main_registry_app-2.9.0/tests/components/data/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4813 2024-05-13 16:08:42.000000 core_main_registry_app-2.9.0/tests/components/data/tests_int.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:48.302625 core_main_registry_app-2.9.0/tests/components/refinement/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:42.000000 core_main_registry_app-2.9.0/tests/components/refinement/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4639 2024-05-13 16:08:42.000000 core_main_registry_app-2.9.0/tests/components/refinement/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:48.322042 core_main_registry_app-2.9.0/tests/components/template_version_manager/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:42.000000 core_main_registry_app-2.9.0/tests/components/template_version_manager/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:48.363135 core_main_registry_app-2.9.0/tests/components/template_version_manager/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:42.000000 core_main_registry_app-2.9.0/tests/components/template_version_manager/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2182 2024-05-13 16:08:42.000000 core_main_registry_app-2.9.0/tests/components/template_version_manager/fixtures/fixtures.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:48.413599 core_main_registry_app-2.9.0/tests/discover/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:42.000000 core_main_registry_app-2.9.0/tests/discover/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5274 2024-05-13 16:08:42.000000 core_main_registry_app-2.9.0/tests/discover/tests_unit.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      539 2024-05-13 16:08:42.000000 core_main_registry_app-2.9.0/tests/mocks.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:48.435350 core_main_registry_app-2.9.0/tests/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:42.000000 core_main_registry_app-2.9.0/tests/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:48.476367 core_main_registry_app-2.9.0/tests/rest/data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:42.000000 core_main_registry_app-2.9.0/tests/rest/data/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5430 2024-05-13 16:08:42.000000 core_main_registry_app-2.9.0/tests/rest/data/tests_permissions.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:48.535206 core_main_registry_app-2.9.0/tests/rest/template_version_manager/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:42.000000 core_main_registry_app-2.9.0/tests/rest/template_version_manager/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3008 2024-05-13 16:08:42.000000 core_main_registry_app-2.9.0/tests/rest/template_version_manager/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2135 2024-05-13 16:08:42.000000 core_main_registry_app-2.9.0/tests/rest/template_version_manager/tests_permission.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:48.575722 core_main_registry_app-2.9.0/tests/rest/urls/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:42.000000 core_main_registry_app-2.9.0/tests/rest/urls/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      501 2024-05-13 16:08:42.000000 core_main_registry_app-2.9.0/tests/rest/urls/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:48.596318 core_main_registry_app-2.9.0/tests/rest/workspace/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:42.000000 core_main_registry_app-2.9.0/tests/rest/workspace/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:48.642808 core_main_registry_app-2.9.0/tests/rest/workspace/serializers/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:42.000000 core_main_registry_app-2.9.0/tests/rest/workspace/serializers/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1514 2024-05-13 16:08:42.000000 core_main_registry_app-2.9.0/tests/rest/workspace/serializers/tests_unit.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1085 2024-05-13 16:08:42.000000 core_main_registry_app-2.9.0/tests/test_menus.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2190 2024-05-13 16:08:42.000000 core_main_registry_app-2.9.0/tests/test_settings.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      194 2024-05-13 16:08:42.000000 core_main_registry_app-2.9.0/tests/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:48.665417 core_main_registry_app-2.9.0/tests/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:42.000000 core_main_registry_app-2.9.0/tests/utils/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:48.691823 core_main_registry_app-2.9.0/tests/utils/fancytree/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:42.000000 core_main_registry_app-2.9.0/tests/utils/fancytree/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:48.738670 core_main_registry_app-2.9.0/tests/utils/fancytree/widget/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:42.000000 core_main_registry_app-2.9.0/tests/utils/fancytree/widget/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      717 2024-05-13 16:08:42.000000 core_main_registry_app-2.9.0/tests/utils/fancytree/widget/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:48.778988 core_main_registry_app-2.9.0/tests/utils/role/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:42.000000 core_main_registry_app-2.9.0/tests/utils/role/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      761 2024-05-13 16:08:42.000000 core_main_registry_app-2.9.0/tests/utils/role/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:48.796877 core_main_registry_app-2.9.0/tests/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:42.000000 core_main_registry_app-2.9.0/tests/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:48.827237 core_main_registry_app-2.9.0/tests/views/admin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:42.000000 core_main_registry_app-2.9.0/tests/views/admin/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:48.892243 core_main_registry_app-2.9.0/tests/views/admin/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:08:42.000000 core_main_registry_app-2.9.0/tests/views/admin/views/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4418 2024-05-13 16:08:42.000000 core_main_registry_app-2.9.0/tests/views/admin/views/test_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5686 2024-05-13 16:08:42.000000 core_main_registry_app-2.9.0/tests/views/admin/views/test_unit.py
```

### Comparing `core_main_registry_app-2.8.0/LICENSE.md` & `core_main_registry_app-2.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.8.0/PKG-INFO` & `core_main_registry_app-2.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_main_registry_app
-Version: 2.8.0
+Version: 2.9.0
 Summary: Main functionalities for the registry project
 Home-page: https://github.com/usnistgov/core_main_registry_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: Core Main Registry App
         ======================
```

### Comparing `core_main_registry_app-2.8.0/README.rst` & `core_main_registry_app-2.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.8.0/core_main_registry_app/admin.py` & `core_main_registry_app-2.9.0/core_main_registry_app/admin.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.8.0/core_main_registry_app/components/category/api.py` & `core_main_registry_app-2.9.0/core_main_registry_app/components/category/api.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.8.0/core_main_registry_app/components/category/models.py` & `core_main_registry_app-2.9.0/core_main_registry_app/components/category/models.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.8.0/core_main_registry_app/components/custom_resource/api.py` & `core_main_registry_app-2.9.0/core_main_registry_app/components/custom_resource/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-""" Custom Resource model
+""" Custom Resource api
 """
 import logging
 
 from django.conf import settings
 
 from core_main_app.commons import exceptions as exceptions
 from core_main_app.components.template import api as template_api
@@ -24,37 +24,47 @@
     """Parse the data to create custom resources and save them.
 
     Args:
      data: dict
      current_template:
     Returns:
     """
-
-    for key in data.keys():
-        resource = data[key]
-
-        custom_resource = CustomResource(template=current_template)
-
-        if _is_type_all(resource):
-            custom_resource = _create_custom_resource_type_all(
-                custom_resource, resource, key
-            )
-            # TODO: make sure only one type = 'all' ?
-        else:
-            custom_resource = _create_custom_resource(
-                custom_resource, resource, key
-            )
-
+    # Build list of custom resources from data
+    custom_resources_list = get_resources_from_dict(data)
+    # Save custom resources
+    for custom_resource in custom_resources_list:
+        custom_resource.template = current_template
         try:
-            _check_curate(custom_resource)
             custom_resource.save()
         except Exception as exception:
             raise exceptions.ModelError(str(exception))
 
 
+def get_resources_from_dict(resource_dict):
+    """Get list of custom resources from dictionary
+
+    Args:
+        resource_dict:
+
+    Returns:
+
+    """
+    # Initialize list
+    custom_resources_list = list()
+    # Create Custom Resources
+    for key in resource_dict.keys():
+        resource = resource_dict[key]
+        custom_resource = CustomResource()
+        custom_resources_list.append(
+            _create_custom_resource(custom_resource, resource, key)
+        )
+    # Return list of custom resources
+    return custom_resources_list
+
+
 def _check_curate(custom_resource):
     """Check if we have all information from configuration file for curate.
 
     Args:
         custom_resource:
     Returns:
     """
@@ -68,29 +78,14 @@
     ):
         raise exceptions.ModelError(
             "Curate app is installed. "
             "You need url key, role choice and role type configured in configuration file."
         )
 
 
-def _get_value(dict, key):
-    """Get the value from the dict with the key.
-
-    Args:
-     dict:
-     key:
-    Returns:
-    """
-    try:
-        return dict[key]
-    except Exception:
-        logger.warning("The key %s is missing from the JSON file.", str(key))
-        return None
-
-
 def _is_custom_resource_type_resource(custom_resource):
     """Is the custom resource a resource.
 
     Args:
         custom_resource:
     Returns:
     """
@@ -106,52 +101,38 @@
     """
     try:
         return resource["type"] == CUSTOM_RESOURCE_TYPE.ALL.value
     except Exception:
         raise exceptions.ModelError("The configuration file is not valid.")
 
 
-def _create_custom_resource_type_all(custom_resource, resource, key):
-    """Create a custom resource for 'all resource'.
-
-    Args:
-     custom_resource:
-     resource:
-    Returns:
-    """
-    custom_resource.type = CUSTOM_RESOURCE_TYPE.ALL.value
-    custom_resource.name_in_schema = key
-    custom_resource.title = _get_value(resource, "title")
-    custom_resource.icon = _get_value(resource, "icon")
-    custom_resource.display_icon = _get_value(resource, "display_icon")
-    custom_resource.icon_color = _get_value(resource, "icon_color")
-    custom_resource.sort = _get_value(resource, "sort")
-    return custom_resource
-
-
 def _create_custom_resource(custom_resource, resource, key):
     """Create a custom resource.
 
     Args:
      custom_resource:
      resource:
      key:
     Returns:
     """
-    custom_resource.type = CUSTOM_RESOURCE_TYPE.RESOURCE.value
+    if _is_type_all(resource):
+        custom_resource.type = CUSTOM_RESOURCE_TYPE.ALL.value
+    else:
+        custom_resource.type = CUSTOM_RESOURCE_TYPE.RESOURCE.value
+        custom_resource.role_choice = resource.get("role_choice", None)
+        custom_resource.role_type = resource.get("role_type", None)
+        custom_resource.description = resource.get("description", None)
+        custom_resource.refinements = resource.get("refinements", None)
     custom_resource.name_in_schema = key
-    custom_resource.title = _get_value(resource, "title")
-    custom_resource.description = _get_value(resource, "description")
-    custom_resource.icon = _get_value(resource, "icon")
-    custom_resource.icon_color = _get_value(resource, "icon_color")
-    custom_resource.display_icon = _get_value(resource, "display_icon")
-    custom_resource.role_choice = _get_value(resource, "role_choice")
-    custom_resource.role_type = _get_value(resource, "role_type")
-    custom_resource.sort = _get_value(resource, "sort")
-    custom_resource.refinements = _get_value(resource, "refinements")
+    custom_resource.title = resource.get("title", None)
+    custom_resource.icon = resource.get("icon", None)
+    custom_resource.icon_color = resource.get("icon_color", None)
+    custom_resource.display_icon = resource.get("display_icon", None)
+    custom_resource.sort = resource.get("sort", None)
+    _check_curate(custom_resource)
     return custom_resource
 
 
 def get_all_by_template(template):
     """Return all custom resource by template.
 
     Args:
```

### Comparing `core_main_registry_app-2.8.0/core_main_registry_app/components/custom_resource/models.py` & `core_main_registry_app-2.9.0/core_main_registry_app/components/custom_resource/models.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.8.0/core_main_registry_app/components/data/access_control.py` & `core_main_registry_app-2.9.0/core_main_registry_app/components/data/access_control.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.8.0/core_main_registry_app/components/data/api.py` & `core_main_registry_app-2.9.0/core_main_registry_app/components/data/api.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.8.0/core_main_registry_app/components/refinement/api.py` & `core_main_registry_app-2.9.0/core_main_registry_app/components/refinement/api.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.8.0/core_main_registry_app/components/refinement/models.py` & `core_main_registry_app-2.9.0/core_main_registry_app/components/refinement/models.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.8.0/core_main_registry_app/components/template/api.py` & `core_main_registry_app-2.9.0/core_main_registry_app/components/template/api.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.8.0/core_main_registry_app/components/version_manager/api.py` & `core_main_registry_app-2.9.0/core_main_registry_app/components/version_manager/api.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.8.0/core_main_registry_app/menus.py` & `core_main_registry_app-2.9.0/core_main_registry_app/menus.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.8.0/core_main_registry_app/migrations/0001_initial.py` & `core_main_registry_app-2.9.0/core_main_registry_app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.8.0/core_main_registry_app/rest/data/views.py` & `core_main_registry_app-2.9.0/core_main_registry_app/rest/data/views.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.8.0/core_main_registry_app/rest/template_version_manager/views.py` & `core_main_registry_app-2.9.0/core_main_registry_app/rest/template_version_manager/views.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.8.0/core_main_registry_app/rest/urls.py` & `core_main_registry_app-2.9.0/core_main_registry_app/rest/urls.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.8.0/core_main_registry_app/rest/workspace/serializers.py` & `core_main_registry_app-2.9.0/core_main_registry_app/rest/workspace/serializers.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.8.0/core_main_registry_app/settings.py` & `core_main_registry_app-2.9.0/core_main_registry_app/settings.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,26 +14,42 @@
     settings,
     "REGISTRY_XSD_FILEPATH",
     join("core_main_registry_app", "xsd", "res-md.xsd"),
 )
 """ str: Registry xsd path used for the initialisation.
 """
 
-REGISTRY_XSD_FILENAME = getattr(settings, "REGISTRY_XSD_FILENAME", "")
+REGISTRY_XSD_FILENAME = getattr(settings, "REGISTRY_XSD_FILENAME", "res-md")
 """ str: Registry xsd filename used for the initialisation.
 """
 
 CUSTOM_REGISTRY_FILE_PATH = getattr(
     settings,
     "CUSTOM_REGISTRY_FILE_PATH",
     join("core_main_registry_app", "json", "custom_registry.json"),
 )
 """ str: Custom registry configuration file path used for the initialisation.
 """
 
+XSL_FOLDER_PATH = getattr(
+    settings, "XSL_FOLDER_PATH", join("core_main_registry_app", "xsl")
+)
+""" str: Xsl folder path used for the initialisation.
+"""
+
+LIST_XSL_FILENAME = getattr(settings, "LIST_XSL_FILENAME", "registry-list.xsl")
+"""" str : List xsl filename used for the initialisation.
+"""
+
+DETAIL_XSL_FILENAME = getattr(
+    settings, "DETAIL_XSL_FILENAME", "registry-detail.xsl"
+)
+"""  str : Detail xsl filename used for the initialisation.
+"""
+
 ENABLE_BLOB_ENDPOINTS = getattr(settings, "ENABLE_BLOB_ENDPOINTS", False)
 """ bool: Enable blob api and user views for blob management.
 """
 
 ALLOW_MULTIPLE_SCHEMAS = getattr(settings, "ALLOW_MULTIPLE_SCHEMAS", False)
 """ bool: Enable the use of multiple schemas in the registry.
 """
```

### Comparing `core_main_registry_app-2.8.0/core_main_registry_app/static/core_main_registry_app/json/custom_registry.json` & `core_main_registry_app-2.9.0/core_main_registry_app/static/core_main_registry_app/json/custom_registry.json`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.8.0/core_main_registry_app/static/core_main_registry_app/user/css/resource_banner/resource_banner.css` & `core_main_registry_app-2.9.0/core_main_registry_app/static/core_main_registry_app/user/css/resource_banner/resource_banner.css`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.8.0/core_main_registry_app/static/core_main_registry_app/xsd/res-md.xsd` & `core_main_registry_app-2.9.0/core_main_registry_app/static/core_main_registry_app/xsd/res-md.xsd`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.8.0/core_main_registry_app/static/core_main_registry_app/xsl/xml2html.xsl` & `core_main_registry_app-2.9.0/core_main_registry_app/static/core_main_registry_app/xsl/xml2html.xsl`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.8.0/core_main_registry_app/system/api.py` & `core_main_registry_app-2.9.0/core_main_registry_app/system/api.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.8.0/core_main_registry_app/templates/core_main_registry_app/admin/custom_registry/table.html` & `core_main_registry_app-2.9.0/core_main_registry_app/templates/core_main_registry_app/admin/custom_registry/table.html`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.8.0/core_main_registry_app/templates/core_main_registry_app/admin/templates/list/available.html` & `core_main_registry_app-2.9.0/core_main_registry_app/templates/core_main_registry_app/admin/templates/list/available.html`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.8.0/core_main_registry_app/templates/core_main_registry_app/resource_banner/resource_banner.html` & `core_main_registry_app-2.9.0/core_main_registry_app/templates/core_main_registry_app/resource_banner/resource_banner.html`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.8.0/core_main_registry_app/urls.py` & `core_main_registry_app-2.9.0/core_main_registry_app/urls.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.8.0/core_main_registry_app/utils/fancytree/widget.py` & `core_main_registry_app-2.9.0/core_main_registry_app/utils/fancytree/widget.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.8.0/core_main_registry_app/utils/menu/menu_utils.py` & `core_main_registry_app-2.9.0/core_main_registry_app/utils/menu/menu_utils.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.8.0/core_main_registry_app/utils/refinement/mongo_query.py` & `core_main_registry_app-2.9.0/core_main_registry_app/utils/refinement/mongo_query.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.8.0/core_main_registry_app/utils/refinement/refinement.py` & `core_main_registry_app-2.9.0/core_main_registry_app/utils/refinement/refinement.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,11 +88,11 @@
         parent = category_api.create_and_save(
             name=key.title,
             path=key.path,
             value=value,
             parent=parent,
             refinement=refinement,
         )
-        # For each children.
+        # For each child.
         for key, value in sorted(leaves.items()):
             # Create sub categories.
             _create_sub_categories(key, value, refinement, parent=parent)
```

### Comparing `core_main_registry_app-2.8.0/core_main_registry_app/utils/refinement/tools/tree.py` & `core_main_registry_app-2.9.0/core_main_registry_app/utils/refinement/tools/tree.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.8.0/core_main_registry_app/utils/refinement/tools/xsd_refinements.py` & `core_main_registry_app-2.9.0/core_main_registry_app/utils/refinement/tools/xsd_refinements.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.8.0/core_main_registry_app/utils/refinement/watch.py` & `core_main_registry_app-2.9.0/core_main_registry_app/utils/refinement/watch.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.8.0/core_main_registry_app/utils/role/extraction.py` & `core_main_registry_app-2.9.0/core_main_registry_app/utils/role/extraction.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.8.0/core_main_registry_app/views/admin/views.py` & `core_main_registry_app-2.9.0/core_main_registry_app/views/admin/views.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.8.0/core_main_registry_app.egg-info/PKG-INFO` & `core_main_registry_app-2.9.0/core_main_registry_app.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-main-registry-app
-Version: 2.8.0
+Version: 2.9.0
 Summary: Main functionalities for the registry project
 Home-page: https://github.com/usnistgov/core_main_registry_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: Core Main Registry App
         ======================
```

### Comparing `core_main_registry_app-2.8.0/core_main_registry_app.egg-info/SOURCES.txt` & `core_main_registry_app-2.9.0/core_main_registry_app.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 core_main_registry_app/components/refinement/api.py
 core_main_registry_app/components/refinement/models.py
 core_main_registry_app/components/template/__init__.py
 core_main_registry_app/components/template/api.py
 core_main_registry_app/components/version_manager/__init__.py
 core_main_registry_app/components/version_manager/api.py
 core_main_registry_app/migrations/0001_initial.py
+core_main_registry_app/migrations/0002_init_data.py
 core_main_registry_app/migrations/__init__.py
 core_main_registry_app/rest/__init__.py
 core_main_registry_app/rest/urls.py
 core_main_registry_app/rest/data/__init__.py
 core_main_registry_app/rest/data/views.py
 core_main_registry_app/rest/template_version_manager/__init__.py
 core_main_registry_app/rest/template_version_manager/views.py
@@ -53,14 +54,16 @@
 core_main_registry_app/rest/workspace/views.py
 core_main_registry_app/static/core_main_registry_app/admin/js/templates/sort.raw.js
 core_main_registry_app/static/core_main_registry_app/json/custom_registry.json
 core_main_registry_app/static/core_main_registry_app/user/css/fancytree/fancytree.custom.css
 core_main_registry_app/static/core_main_registry_app/user/css/resource_banner/resource_banner.css
 core_main_registry_app/static/core_main_registry_app/user/css/resource_banner/selection.css
 core_main_registry_app/static/core_main_registry_app/xsd/res-md.xsd
+core_main_registry_app/static/core_main_registry_app/xsl/registry-detail.xsl
+core_main_registry_app/static/core_main_registry_app/xsl/registry-list.xsl
 core_main_registry_app/static/core_main_registry_app/xsl/xml2html.xsl
 core_main_registry_app/system/__init__.py
 core_main_registry_app/system/api.py
 core_main_registry_app/templates/core_main_registry_app/admin/custom_registry/list.html
 core_main_registry_app/templates/core_main_registry_app/admin/custom_registry/table.html
 core_main_registry_app/templates/core_main_registry_app/admin/custom_registry/upload.html
 core_main_registry_app/templates/core_main_registry_app/admin/custom_registry/upload/base.html
@@ -105,14 +108,16 @@
 tests/components/data/fixtures/__init__.py
 tests/components/data/fixtures/fixtures.py
 tests/components/refinement/__init__.py
 tests/components/refinement/tests_unit.py
 tests/components/template_version_manager/__init__.py
 tests/components/template_version_manager/fixtures/__init__.py
 tests/components/template_version_manager/fixtures/fixtures.py
+tests/discover/__init__.py
+tests/discover/tests_unit.py
 tests/rest/__init__.py
 tests/rest/data/__init__.py
 tests/rest/data/tests_permissions.py
 tests/rest/template_version_manager/__init__.py
 tests/rest/template_version_manager/tests_int.py
 tests/rest/template_version_manager/tests_permission.py
 tests/rest/urls/__init__.py
```

### Comparing `core_main_registry_app-2.8.0/setup.py` & `core_main_registry_app-2.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_main_registry_app",
-    version="2.8.0",
+    version="2.9.0",
     description="Main functionalities for the registry project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_main_registry_app",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `core_main_registry_app-2.8.0/tests/components/category/tests_unit.py` & `core_main_registry_app-2.9.0/tests/components/category/tests_unit.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,29 +35,32 @@
 
 
 class TestCategoryGetAllFilteredByRefinementId(TestCase):
     """
     Test Category Get All Filtered By Refinement Id
     """
 
-    def test_category_get_all_filtered_by_refinement_id_returns_empty_list(
+    def test_category_get_all_filtered_by_refinement_id_returns_list_of_categories(
         self,
     ):
-        """test_category_get_all_filtered_by_refinement_id_returns_empty_list"""
+        """test_category_get_all_filtered_by_refinement_id_returns_list_of_categories"""
         # Act
         result = category_api.get_all_filtered_by_refinement_id(1)
         # Assert
-        self.assertEqual(len(result), 0)
+        for obj in list(result):
+            self.assertTrue(isinstance(obj, Category))
 
     def test_category_get_all_filtered_by_refinement_id_returns_list(self):
         """test_category_get_all_filtered_by_refinement_id_returns_list"""
         # Arrange
         category = create_category()
         # Act
-        result = category_api.get_all_filtered_by_refinement_id(1)
+        result = category_api.get_all_filtered_by_refinement_id(
+            category.refinement.id
+        )
         # Assert
         self.assertEqual(len(result), 1)
         self.assertTrue(category in result)
 
 
 class TestCategoryGetById(TestCase):
     """
@@ -81,29 +84,29 @@
 
 
 class TestCategoryGetAll(TestCase):
     """
     Test Category Get All
     """
 
-    def test_category_get_all_returns_empty_list(self):
-        """test_category_get_all_returns_empty_list"""
+    def test_category_get_all_returns_list_of_categories(self):
+        """test_category_get_all_returns_list_of_categories"""
         # Act
         result = category_api.get_all()
         # Assert
-        self.assertEqual(len(result), 0)
+        for obj in list(result):
+            self.assertTrue(isinstance(obj, Category))
 
     def test_category_get_all_returns_list(self):
         """test_category_get_all_returns_list"""
         # Arrange
         category = create_category()
         # Act
         result = category_api.get_all()
         # Assert
-        self.assertEqual(len(result), 1)
         self.assertTrue(category in result)
 
 
 class TestCategoryGetAllCategoriesIdsFromNameAndRefinementId(TestCase):
     """
     Test Category Get All Categories Ids From Name And Refinement Id
     """
@@ -119,19 +122,19 @@
             )
 
     def test_category_get_all_categories_ids_from_name_and_refinement_id_returns_list(
         self,
     ):
         """test_category_get_all_categories_ids_from_name_and_refinement_id_returns_list"""
         # Arrange
-        create_category()
+        category = create_category()
         # Act
         result = (
             category_api.get_all_categories_ids_from_name_and_refinement_id(
-                "Category", 1
+                "Category", category.refinement.id
             )
         )
         # Assert
         self.assertEqual(len(result), 1)
 
 
 class TestCategoryGetAllCategoriesIdsByParentSlugAndRefinementId(TestCase):
@@ -150,18 +153,18 @@
             )
 
     def test_get_all_categories_ids_by_parent_slug_and_refinement_id_returns_list(
         self,
     ):
         """test_get_all_categories_ids_by_parent_slug_and_refinement_id_returns_list"""
         # Arrange
-        create_category()
+        category = create_category()
         # Act
         result = category_api.get_all_categories_ids_by_parent_slug_and_refinement_id(
-            "", 1
+            "", category.refinement.id
         )
         # Assert
         self.assertEqual(len(result), 1)
 
 
 def create_category():
     """create_refinement
```

### Comparing `core_main_registry_app-2.8.0/tests/components/custom_resource/fixtures/fixtures.py` & `core_main_registry_app-2.9.0/tests/components/custom_resource/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.8.0/tests/components/custom_resource/tests_int.py` & `core_main_registry_app-2.9.0/tests/components/custom_resource/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.8.0/tests/components/custom_resource/tests_unit.py` & `core_main_registry_app-2.9.0/tests/components/custom_resource/tests_unit.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,51 +30,51 @@
 
     fixture = fixtureCustomResource
 
     def test_create_all_resource_custom_resource_return_type_all(self):
         """test_create_all_resource_custom_resource_return_type_all"""
         # Act
         key = "all_resource"
-        custom_resource = custom_resource_api._create_custom_resource_type_all(
+        custom_resource = custom_resource_api._create_custom_resource(
             self.fixture.create_custom_resource(),
             self.fixture.get_dict_custom_resource_all_resource()[key],
             key,
         )
         # Assert
         self.assertEqual(custom_resource.type, CUSTOM_RESOURCE_TYPE.ALL.value)
 
     def test_create_all_resource_custom_resource_return_icon(self):
         """test_create_all_resource_custom_resource_return_icon"""
         # Act
         key = "all_resource"
-        custom_resource = custom_resource_api._create_custom_resource_type_all(
+        custom_resource = custom_resource_api._create_custom_resource(
             self.fixture.create_custom_resource(),
             self.fixture.get_dict_custom_resource_all_resource()[key],
             key,
         )
         # Assert
         self.assertEqual(custom_resource.icon, "fa-globe")
 
     def test_create_all_resource_custom_resource_return_icon_color(self):
         """test_create_all_resource_custom_resource_return_icon_color"""
         # Act
         key = "all_resource"
-        custom_resource = custom_resource_api._create_custom_resource_type_all(
+        custom_resource = custom_resource_api._create_custom_resource(
             self.fixture.create_custom_resource(),
             self.fixture.get_dict_custom_resource_all_resource()[key],
             key,
         )
         # Assert
         self.assertEqual(custom_resource.icon_color, "#557EB9")
 
     def test_create_all_resource_custom_resource_return_sort(self):
         """test_create_all_resource_custom_resource_return_sort"""
         # Act
         key = "all_resource"
-        custom_resource = custom_resource_api._create_custom_resource_type_all(
+        custom_resource = custom_resource_api._create_custom_resource(
             self.fixture.create_custom_resource(),
             self.fixture.get_dict_custom_resource_all_resource()[key],
             key,
         )
         # Assert
         self.assertEqual(custom_resource.sort, 0)
```

### Comparing `core_main_registry_app-2.8.0/tests/components/data/fixtures/fixtures.py` & `core_main_registry_app-2.9.0/tests/components/data/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.8.0/tests/components/data/tests_int.py` & `core_main_registry_app-2.9.0/tests/components/data/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.8.0/tests/components/refinement/tests_unit.py` & `core_main_registry_app-2.9.0/tests/components/refinement/tests_unit.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,32 +26,34 @@
 
 
 class TestRefinementGetAll(TestCase):
     """
     Test Refinement Get All
     """
 
-    def test_refinement_get_all_refinement_returns_empty_list(self):
-        """test_get_all_refinements_returns_empty_list"""
+    def test_refinement_get_all_refinements_returns_list_of_refinements(self):
+        """test_refinement_get_all_refinements_returns_list_of_refinements"""
         # Act
         result = refinement_api.get_all()
         # Assert
 
-        self.assertEqual(len(result), 0)
+        for obj in list(result):
+            self.assertTrue(isinstance(obj, Refinement))
 
     def test_refinement_get_all_refinement_returns_list(self):
         """test_get_all_refinements_returns_empty_list"""
         # Arrange
+        refinement_count = Refinement.objects.count()
         refinement_1 = create_refinement()
         refinement_2 = create_refinement()
         # Act
         result = refinement_api.get_all()
         # Assert
 
-        self.assertEqual(len(result), 2)
+        self.assertEqual(len(result), refinement_count + 2)
         self.assertTrue(refinement_1 in result)
         self.assertTrue(refinement_2 in result)
 
 
 class TestRefinementGetAllFilteredByTemplateHash(TestCase):
     """
     Test Refinement Get All Filtered By Template Hash
```

### Comparing `core_main_registry_app-2.8.0/tests/components/template_version_manager/fixtures/fixtures.py` & `core_main_registry_app-2.9.0/tests/components/template_version_manager/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.8.0/tests/mocks.py` & `core_main_registry_app-2.9.0/tests/mocks.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.8.0/tests/rest/data/tests_permissions.py` & `core_main_registry_app-2.9.0/tests/rest/data/tests_permissions.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.8.0/tests/rest/template_version_manager/tests_int.py` & `core_main_registry_app-2.9.0/tests/rest/template_version_manager/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.8.0/tests/rest/template_version_manager/tests_permission.py` & `core_main_registry_app-2.9.0/tests/rest/template_version_manager/tests_permission.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.8.0/tests/rest/workspace/serializers/tests_unit.py` & `core_main_registry_app-2.9.0/tests/rest/workspace/serializers/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.8.0/tests/test_menus.py` & `core_main_registry_app-2.9.0/tests/test_menus.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.8.0/tests/test_settings.py` & `core_main_registry_app-2.9.0/tests/test_settings.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """ Tests Settings
 """
+import os
 
 SECRET_KEY = "fake-key"
 
 INSTALLED_APPS = [
     # Django apps
     "django.contrib.admin",
     "django.contrib.auth",
@@ -68,7 +69,18 @@
 MONGODB_ASYNC_SAVE = False
 ENABLE_SAML2_SSO_AUTH = False
 ALLOW_MULTIPLE_SCHEMAS = True
 
 DEFAULT_AUTO_FIELD = "django.db.models.BigAutoField"
 CUSTOM_NAME = "NMRR"
 ROOT_URLCONF = "tests.urls"
+
+
+REGISTRY_XSD_FILEPATH = os.path.join(
+    "core_main_registry_app", "xsd", "res-md.xsd"
+)
+REGISTRY_XSD_FILENAME = "res-md.xsd"
+CUSTOM_REGISTRY_FILE_PATH = os.path.join(
+    "core_main_registry_app", "json", "custom_registry.json"
+)
+
+CELERY_ALWAYS_EAGER = True
```

### Comparing `core_main_registry_app-2.8.0/tests/utils/fancytree/widget/tests_unit.py` & `core_main_registry_app-2.9.0/tests/utils/fancytree/widget/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.8.0/tests/utils/role/tests_unit.py` & `core_main_registry_app-2.9.0/tests/utils/role/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.8.0/tests/views/admin/views/test_int.py` & `core_main_registry_app-2.9.0/tests/views/admin/views/test_int.py`

 * *Files identical despite different names*

### Comparing `core_main_registry_app-2.8.0/tests/views/admin/views/test_unit.py` & `core_main_registry_app-2.9.0/tests/views/admin/views/test_unit.py`

 * *Files identical despite different names*

