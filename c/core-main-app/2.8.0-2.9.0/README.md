# Comparing `tmp/core_main_app-2.8.0.tar.gz` & `tmp/core_main_app-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_main_app-2.8.0.tar", last modified: Tue Mar 12 19:03:13 2024, max compression
+gzip compressed data, was "core_main_app-2.9.0.tar", last modified: Mon May 13 16:52:51 2024, max compression
```

## Comparing `core_main_app-2.8.0.tar` & `core_main_app-2.9.0.tar`

### file list

```diff
@@ -1,954 +1,954 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:13.195784 core_main_app-2.8.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2024-03-12 19:02:24.000000 core_main_app-2.8.0/LICENSE.md
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      219 2024-03-12 19:02:24.000000 core_main_app-2.8.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9924 2024-03-12 19:03:13.188018 core_main_app-2.8.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7529 2024-03-12 19:02:24.000000 core_main_app-2.8.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:52.725135 core_main_app-2.8.0/core_main_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       81 2024-03-12 19:02:24.000000 core_main_app-2.8.0/core_main_app/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:52.939142 core_main_app-2.8.0/core_main_app/access_control/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:24.000000 core_main_app-2.8.0/core_main_app/access_control/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11259 2024-03-12 19:02:24.000000 core_main_app-2.8.0/core_main_app/access_control/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      628 2024-03-12 19:02:24.000000 core_main_app-2.8.0/core_main_app/access_control/decorators.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      197 2024-03-12 19:02:24.000000 core_main_app-2.8.0/core_main_app/access_control/exceptions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1825 2024-03-12 19:02:24.000000 core_main_app-2.8.0/core_main_app/access_control/utils.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7058 2024-03-12 19:02:24.000000 core_main_app-2.8.0/core_main_app/admin.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1360 2024-03-12 19:02:24.000000 core_main_app-2.8.0/core_main_app/apps.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:53.056307 core_main_app-2.8.0/core_main_app/commons/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:24.000000 core_main_app-2.8.0/core_main_app/commons/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      919 2024-03-12 19:02:24.000000 core_main_app-2.8.0/core_main_app/commons/constants.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       62 2024-03-12 19:02:24.000000 core_main_app-2.8.0/core_main_app/commons/enums.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4743 2024-03-12 19:02:24.000000 core_main_app-2.8.0/core_main_app/commons/exceptions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       82 2024-03-12 19:02:24.000000 core_main_app-2.8.0/core_main_app/commons/regex.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      332 2024-03-12 19:02:24.000000 core_main_app-2.8.0/core_main_app/commons/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9144 2024-03-12 19:02:24.000000 core_main_app-2.8.0/core_main_app/commons/validators.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:53.076010 core_main_app-2.8.0/core_main_app/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:24.000000 core_main_app-2.8.0/core_main_app/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:53.131693 core_main_app-2.8.0/core_main_app/components/abstract_data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:24.000000 core_main_app-2.8.0/core_main_app/components/abstract_data/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4731 2024-03-12 19:02:24.000000 core_main_app-2.8.0/core_main_app/components/abstract_data/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:53.233532 core_main_app-2.8.0/core_main_app/components/blob/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:24.000000 core_main_app-2.8.0/core_main_app/components/blob/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2923 2024-03-12 19:02:24.000000 core_main_app-2.8.0/core_main_app/components/blob/access_control.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      315 2024-03-12 19:02:24.000000 core_main_app-2.8.0/core_main_app/components/blob/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3676 2024-03-12 19:02:24.000000 core_main_app-2.8.0/core_main_app/components/blob/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4077 2024-03-12 19:02:24.000000 core_main_app-2.8.0/core_main_app/components/blob/models.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      442 2024-03-12 19:02:24.000000 core_main_app-2.8.0/core_main_app/components/blob/utils.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:53.358276 core_main_app-2.8.0/core_main_app/components/data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:24.000000 core_main_app-2.8.0/core_main_app/components/data/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4687 2024-03-12 19:02:24.000000 core_main_app-2.8.0/core_main_app/components/data/access_control.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5523 2024-03-12 19:02:24.000000 core_main_app-2.8.0/core_main_app/components/data/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9946 2024-03-12 19:02:24.000000 core_main_app-2.8.0/core_main_app/components/data/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8346 2024-03-12 19:02:24.000000 core_main_app-2.8.0/core_main_app/components/data/models.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11291 2024-03-12 19:02:24.000000 core_main_app-2.8.0/core_main_app/components/data/tasks.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:53.399020 core_main_app-2.8.0/core_main_app/components/group/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:24.000000 core_main_app-2.8.0/core_main_app/components/group/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1982 2024-03-12 19:02:24.000000 core_main_app-2.8.0/core_main_app/components/group/api.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:53.484230 core_main_app-2.8.0/core_main_app/components/lock/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:24.000000 core_main_app-2.8.0/core_main_app/components/lock/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      330 2024-03-12 19:02:24.000000 core_main_app-2.8.0/core_main_app/components/lock/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2570 2024-03-12 19:02:24.000000 core_main_app-2.8.0/core_main_app/components/lock/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2665 2024-03-12 19:02:24.000000 core_main_app-2.8.0/core_main_app/components/lock/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:53.552121 core_main_app-2.8.0/core_main_app/components/mongo/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:24.000000 core_main_app-2.8.0/core_main_app/components/mongo/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1041 2024-03-12 19:02:24.000000 core_main_app-2.8.0/core_main_app/components/mongo/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11665 2024-03-12 19:02:24.000000 core_main_app-2.8.0/core_main_app/components/mongo/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:53.648096 core_main_app-2.8.0/core_main_app/components/template/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:24.000000 core_main_app-2.8.0/core_main_app/components/template/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4599 2024-03-12 19:02:24.000000 core_main_app-2.8.0/core_main_app/components/template/access_control.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      362 2024-03-12 19:02:24.000000 core_main_app-2.8.0/core_main_app/components/template/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5561 2024-03-12 19:02:24.000000 core_main_app-2.8.0/core_main_app/components/template/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8014 2024-03-12 19:02:24.000000 core_main_app-2.8.0/core_main_app/components/template/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:53.752088 core_main_app-2.8.0/core_main_app/components/template_version_manager/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:24.000000 core_main_app-2.8.0/core_main_app/components/template_version_manager/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2690 2024-03-12 19:02:24.000000 core_main_app-2.8.0/core_main_app/components/template_version_manager/access_control.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      507 2024-03-12 19:02:24.000000 core_main_app-2.8.0/core_main_app/components/template_version_manager/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8166 2024-03-12 19:02:24.000000 core_main_app-2.8.0/core_main_app/components/template_version_manager/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4720 2024-03-12 19:02:24.000000 core_main_app-2.8.0/core_main_app/components/template_version_manager/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:53.827387 core_main_app-2.8.0/core_main_app/components/template_xsl_rendering/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:24.000000 core_main_app-2.8.0/core_main_app/components/template_xsl_rendering/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      338 2024-03-12 19:02:24.000000 core_main_app-2.8.0/core_main_app/components/template_xsl_rendering/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6892 2024-03-12 19:02:24.000000 core_main_app-2.8.0/core_main_app/components/template_xsl_rendering/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3435 2024-03-12 19:02:24.000000 core_main_app-2.8.0/core_main_app/components/template_xsl_rendering/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:53.872200 core_main_app-2.8.0/core_main_app/components/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:24.000000 core_main_app-2.8.0/core_main_app/components/user/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2470 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/components/user/api.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:53.968772 core_main_app-2.8.0/core_main_app/components/user_preferences/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/components/user_preferences/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1835 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/components/user_preferences/access_control.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      486 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/components/user_preferences/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1000 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/components/user_preferences/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1392 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/components/user_preferences/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:54.065266 core_main_app-2.8.0/core_main_app/components/version_manager/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/components/version_manager/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4884 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/components/version_manager/access_control.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3744 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/components/version_manager/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3248 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/components/version_manager/models.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      550 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/components/version_manager/utils.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:54.122132 core_main_app-2.8.0/core_main_app/components/web_page/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/components/web_page/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1280 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/components/web_page/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1097 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/components/web_page/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:54.162990 core_main_app-2.8.0/core_main_app/components/web_page_login/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/components/web_page_login/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      809 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/components/web_page_login/api.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:54.263800 core_main_app-2.8.0/core_main_app/components/workspace/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/components/workspace/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2493 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/components/workspace/access_control.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      372 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/components/workspace/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    16858 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/components/workspace/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5695 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/components/workspace/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:54.340248 core_main_app-2.8.0/core_main_app/components/xsl_transformation/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/components/xsl_transformation/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      366 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/components/xsl_transformation/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2542 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/components/xsl_transformation/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4469 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/components/xsl_transformation/models.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1791 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/menus.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:54.384152 core_main_app-2.8.0/core_main_app/middleware/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/middleware/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1378 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/middleware/timezone.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:54.556417 core_main_app-2.8.0/core_main_app/migrations/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    16483 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/migrations/0001_initial.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      751 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/migrations/0002_site_update.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1880 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/migrations/0003_psql_full_text.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      823 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/migrations/0004_template_ordering.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      474 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/migrations/0005_template_dependencies.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      655 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/migrations/0006_blob_metadata.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1372 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/migrations/0007_user_preferences.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      440 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/migrations/0008_blob_ordering.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      828 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/migrations/0009_template_formats.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/migrations/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      733 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:54.654255 core_main_app-2.8.0/core_main_app/permissions/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/permissions/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6351 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/permissions/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3152 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/permissions/discover.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      644 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/permissions/rights.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      230 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/permissions/utils.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:54.719807 core_main_app-2.8.0/core_main_app/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:54.782000 core_main_app-2.8.0/core_main_app/rest/blob/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/rest/blob/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4747 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/rest/blob/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    19770 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/rest/blob/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:54.913290 core_main_app-2.8.0/core_main_app/rest/data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/rest/data/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8239 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/rest/data/abstract_views.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2261 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/rest/data/admin_serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4201 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/rest/data/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    38308 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/rest/data/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:54.957577 core_main_app-2.8.0/core_main_app/rest/group/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/rest/group/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      293 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/rest/group/serializers.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:54.998790 core_main_app-2.8.0/core_main_app/rest/mongo_data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/rest/mongo_data/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1989 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/rest/mongo_data/serializers.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:55.075327 core_main_app-2.8.0/core_main_app/rest/template/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/rest/template/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      907 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/rest/template/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5344 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/rest/template/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:55.166275 core_main_app-2.8.0/core_main_app/rest/template_version_manager/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/rest/template_version_manager/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    13930 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/rest/template_version_manager/abstract_views.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2858 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/rest/template_version_manager/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      587 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/rest/template_version_manager/utils.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    12279 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/rest/template_version_manager/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:55.248907 core_main_app-2.8.0/core_main_app/rest/template_xsl_rendering/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/rest/template_xsl_rendering/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1168 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/rest/template_xsl_rendering/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14418 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/rest/template_xsl_rendering/views.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14537 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/rest/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:55.320256 core_main_app-2.8.0/core_main_app/rest/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/rest/user/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1157 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/rest/user/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      709 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/rest/user/views.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2468 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/rest/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:55.391988 core_main_app-2.8.0/core_main_app/rest/web_page/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/rest/web_page/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1042 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/rest/web_page/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4688 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/rest/web_page/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:55.455268 core_main_app-2.8.0/core_main_app/rest/workspace/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/rest/workspace/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      894 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/rest/workspace/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    23314 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/rest/workspace/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:55.521743 core_main_app-2.8.0/core_main_app/rest/xsl_transformation/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/rest/xsl_transformation/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1437 2024-03-12 19:02:25.000000 core_main_app-2.8.0/core_main_app/rest/xsl_transformation/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8160 2024-03-12 19:02:26.000000 core_main_app-2.8.0/core_main_app/rest/xsl_transformation/views.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9027 2024-03-12 19:02:26.000000 core_main_app-2.8.0/core_main_app/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:50.981891 core_main_app-2.8.0/core_main_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:51.220117 core_main_app-2.8.0/core_main_app/static/core_main_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:51.039114 core_main_app-2.8.0/core_main_app/static/core_main_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:51.014205 core_main_app-2.8.0/core_main_app/static/core_main_app/admin/_theme/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:55.616834 core_main_app-2.8.0/core_main_app/static/core_main_app/admin/_theme/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      251 2024-03-12 19:02:26.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/admin/_theme/css/additional.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    47539 2024-03-12 19:02:26.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/admin/_theme/css/skins.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)   110978 2024-03-12 19:02:26.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/admin/_theme/css/theme.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:55.738949 core_main_app-2.8.0/core_main_app/static/core_main_app/admin/_theme/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    22937 2024-03-12 19:02:26.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/admin/_theme/js/app.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      578 2024-03-12 19:02:26.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/admin/_theme/js/menu.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:55.778182 core_main_app-2.8.0/core_main_app/static/core_main_app/admin/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1575 2024-03-12 19:02:26.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/admin/css/data_migration.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       81 2024-03-12 19:02:26.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/admin/css/permissions.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:55.795726 core_main_app-2.8.0/core_main_app/static/core_main_app/admin/css/templates_xslt/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1363 2024-03-12 19:02:26.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/admin/css/templates_xslt/form.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:55.815918 core_main_app-2.8.0/core_main_app/static/core_main_app/admin/css/web_page/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       31 2024-03-12 19:02:26.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/admin/css/web_page/style.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:55.836913 core_main_app-2.8.0/core_main_app/static/core_main_app/admin/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1232 2024-03-12 19:02:26.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/admin/js/display_permissions.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:55.876003 core_main_app-2.8.0/core_main_app/static/core_main_app/admin/js/templates/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    30064 2024-03-12 19:02:26.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/admin/js/templates/data_migration.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      594 2024-03-12 19:02:26.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/admin/js/templates/data_migration.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:55.933295 core_main_app-2.8.0/core_main_app/static/core_main_app/admin/js/templates/upload/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1334 2024-03-12 19:02:26.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/admin/js/templates/upload/dependencies.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       94 2024-03-12 19:02:26.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/admin/js/templates/upload/dependencies.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      139 2024-03-12 19:02:26.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/admin/js/templates/upload/dependency_resolver.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:55.954737 core_main_app-2.8.0/core_main_app/static/core_main_app/admin/js/templates_xslt/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1395 2024-03-12 19:02:26.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/admin/js/templates_xslt/detail_xslt.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:51.188425 core_main_app-2.8.0/core_main_app/static/core_main_app/common/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:56.201582 core_main_app-2.8.0/core_main_app/static/core_main_app/common/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2236 2024-03-12 19:02:26.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/common/css/XMLTree.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      121 2024-03-12 19:02:26.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/common/css/bootstrap5.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       68 2024-03-12 19:02:26.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/common/css/buttons.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      146 2024-03-12 19:02:26.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/common/css/detail.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      177 2024-03-12 19:02:26.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/common/css/fields.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      132 2024-03-12 19:02:26.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/common/css/highlight.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       92 2024-03-12 19:02:26.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/common/css/loading-spinner.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1332 2024-03-12 19:02:26.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/common/css/messages.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:56.226189 core_main_app-2.8.0/core_main_app/static/core_main_app/common/css/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      102 2024-03-12 19:02:26.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/common/css/modals/download.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      317 2024-03-12 19:02:26.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/common/css/select.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      392 2024-03-12 19:02:26.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/common/css/share_link.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      940 2024-03-12 19:02:26.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/common/css/switch.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      486 2024-03-12 19:02:26.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/common/css/table.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:56.249073 core_main_app-2.8.0/core_main_app/static/core_main_app/common/css/template/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       59 2024-03-12 19:02:26.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/common/css/template/template_ordering.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      189 2024-03-12 19:02:26.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/common/css/word-wrap.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:56.268411 core_main_app-2.8.0/core_main_app/static/core_main_app/common/css/workspace/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      333 2024-03-12 19:02:26.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/common/css/workspace/table.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:56.325052 core_main_app-2.8.0/core_main_app/static/core_main_app/common/img/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      246 2024-03-12 19:02:26.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/common/img/collapse.png
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      253 2024-03-12 19:02:26.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/common/img/expand.png
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:56.528572 core_main_app-2.8.0/core_main_app/static/core_main_app/common/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      335 2024-03-12 19:02:26.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/common/js/XMLTree.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      247 2024-03-12 19:02:26.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/common/js/backtoprevious.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1828 2024-03-12 19:02:26.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/common/js/csrf.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      192 2024-03-12 19:02:26.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/common/js/data_detail.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      531 2024-03-12 19:02:26.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/common/js/debounce.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      787 2024-03-12 19:02:26.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/common/js/elementViewport.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      413 2024-03-12 19:02:26.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/common/js/leave_notice.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      966 2024-03-12 19:02:26.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/common/js/loading_spinner.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2274 2024-03-12 19:02:26.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/common/js/messages.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:56.665660 core_main_app-2.8.0/core_main_app/static/core_main_app/common/js/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1292 2024-03-12 19:02:26.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/common/js/modals/add.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1136 2024-03-12 19:02:26.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/common/js/modals/delete.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      491 2024-03-12 19:02:26.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/common/js/modals/download.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      188 2024-03-12 19:02:26.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/common/js/modals/download.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1257 2024-03-12 19:02:26.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/common/js/modals/edit.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      439 2024-03-12 19:02:26.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/common/js/modals/error_page_modal.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:56.706344 core_main_app-2.8.0/core_main_app/static/core_main_app/common/js/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:56.751994 core_main_app-2.8.0/core_main_app/static/core_main_app/common/js/templates/list/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:56.793173 core_main_app-2.8.0/core_main_app/static/core_main_app/common/js/templates/list/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1086 2024-03-12 19:02:26.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/common/js/templates/list/modals/disable.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      125 2024-03-12 19:02:26.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/common/js/templates/list/modals/disable.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      663 2024-03-12 19:02:26.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/common/js/templates/list/restore.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      124 2024-03-12 19:02:26.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/common/js/templates/list/restore.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1495 2024-03-12 19:02:26.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/common/js/templates/sort.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      217 2024-03-12 19:02:26.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/common/js/templates/sort.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:56.870350 core_main_app-2.8.0/core_main_app/static/core_main_app/common/js/templates/versions/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:56.909939 core_main_app-2.8.0/core_main_app/static/core_main_app/common/js/templates/versions/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1029 2024-03-12 19:02:26.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/common/js/templates/versions/modals/disable.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      108 2024-03-12 19:02:26.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/common/js/templates/versions/modals/disable.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      537 2024-03-12 19:02:26.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/common/js/templates/versions/restore.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      107 2024-03-12 19:02:26.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/common/js/templates/versions/restore.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      662 2024-03-12 19:02:27.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/common/js/templates/versions/set_current.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      111 2024-03-12 19:02:27.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/common/js/templates/versions/set_current.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      189 2024-03-12 19:02:27.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/common/js/tooltip.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:51.176681 core_main_app-2.8.0/core_main_app/static/core_main_app/common/js/xslt/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:51.182074 core_main_app-2.8.0/core_main_app/static/core_main_app/common/js/xslt/list/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:57.007001 core_main_app-2.8.0/core_main_app/static/core_main_app/common/js/xslt/list/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      859 2024-03-12 19:02:27.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/common/js/xslt/list/modals/delete.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       64 2024-03-12 19:02:27.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/common/js/xslt/list/modals/delete.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1012 2024-03-12 19:02:27.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/common/js/xslt/list/modals/edit.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       60 2024-03-12 19:02:27.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/common/js/xslt/list/modals/edit.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:57.031042 core_main_app-2.8.0/core_main_app/static/core_main_app/common/xsl/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1763 2024-03-12 19:02:27.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/common/xsl/xml2html.xsl
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:51.201694 core_main_app-2.8.0/core_main_app/static/core_main_app/libs/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:51.206453 core_main_app-2.8.0/core_main_app/static/core_main_app/libs/jquery-ui/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:57.137494 core_main_app-2.8.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:57.260859 core_main_app-2.8.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7006 2024-03-12 19:02:27.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_444444_256x240.png
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7074 2024-03-12 19:02:27.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_555555_256x240.png
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4676 2024-03-12 19:02:27.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_777620_256x240.png
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7013 2024-03-12 19:02:27.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_777777_256x240.png
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4632 2024-03-12 19:02:27.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_cc0000_256x240.png
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6313 2024-03-12 19:02:27.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_ffffff_256x240.png
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    37326 2024-03-12 19:02:27.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/jquery-ui.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)   520714 2024-03-12 19:02:27.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/jquery-ui.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    18705 2024-03-12 19:02:27.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/jquery-ui.structure.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    18671 2024-03-12 19:02:27.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/jquery-ui.theme.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:51.232057 core_main_app-2.8.0/core_main_app/static/core_main_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:57.325055 core_main_app-2.8.0/core_main_app/static/core_main_app/user/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       32 2024-03-12 19:02:27.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/user/css/login.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       63 2024-03-12 19:02:27.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/user/css/registration.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      576 2024-03-12 19:02:27.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/user/css/text-editor.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:57.347679 core_main_app-2.8.0/core_main_app/static/core_main_app/user/js/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:57.407274 core_main_app-2.8.0/core_main_app/static/core_main_app/user/js/blob/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1505 2024-03-12 19:02:27.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/user/js/blob/blob_metadata.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      217 2024-03-12 19:02:27.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/user/js/blob/blob_metadata.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      119 2024-03-12 19:02:27.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/user/js/blob/detail.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:57.467283 core_main_app-2.8.0/core_main_app/static/core_main_app/user/js/data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      618 2024-03-12 19:02:27.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/user/js/data/change_display.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      120 2024-03-12 19:02:27.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/user/js/data/change_display.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      158 2024-03-12 19:02:27.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/user/js/data/detail.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:57.541096 core_main_app-2.8.0/core_main_app/static/core_main_app/user/js/login/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      768 2024-03-12 19:02:27.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/user/js/login/message.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       52 2024-03-12 19:02:27.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/user/js/login/message.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1315 2024-03-12 19:02:27.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/user/js/sharing_modal.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:57.630848 core_main_app-2.8.0/core_main_app/static/core_main_app/user/js/text_editor/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      234 2024-03-12 19:02:27.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/user/js/text_editor/data_text_editor.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      120 2024-03-12 19:02:27.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/user/js/text_editor/monaco-editor-loader.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       73 2024-03-12 19:02:27.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/user/js/text_editor/template_text_editor.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10276 2024-03-12 19:02:27.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/user/js/text_editor/text_editor.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:57.800605 core_main_app-2.8.0/core_main_app/static/core_main_app/user/js/workspaces/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1800 2024-03-12 19:02:27.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/user/js/workspaces/add_group.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      160 2024-03-12 19:02:27.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/user/js/workspaces/add_group.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1723 2024-03-12 19:02:27.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/user/js/workspaces/add_user.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      156 2024-03-12 19:02:27.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/user/js/workspaces/add_user.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1138 2024-03-12 19:02:27.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/user/js/workspaces/create_workspace.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       73 2024-03-12 19:02:27.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/user/js/workspaces/create_workspace.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      515 2024-03-12 19:02:27.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/user/js/workspaces/init.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       43 2024-03-12 19:02:27.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/user/js/workspaces/init.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:51.272934 core_main_app-2.8.0/core_main_app/static/core_main_app/user/js/workspaces/list/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:58.032699 core_main_app-2.8.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      187 2024-03-12 19:02:27.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/assign_blob_workspace.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      187 2024-03-12 19:02:27.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/assign_data_workspace.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1587 2024-03-12 19:02:27.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/assign_workspace.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1360 2024-03-12 19:02:27.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/remove_rights.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       60 2024-03-12 19:02:27.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/remove_rights.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      807 2024-03-12 19:02:27.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/set_private.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       96 2024-03-12 19:02:27.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/set_private.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      822 2024-03-12 19:02:27.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/set_public.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       94 2024-03-12 19:02:27.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/set_public.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1728 2024-03-12 19:02:27.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/switch_right.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      144 2024-03-12 19:02:27.000000 core_main_app-2.8.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/switch_right.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:58.079723 core_main_app-2.8.0/core_main_app/system/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:27.000000 core_main_app-2.8.0/core_main_app/system/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2767 2024-03-12 19:02:27.000000 core_main_app-2.8.0/core_main_app/system/api.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:58.125708 core_main_app-2.8.0/core_main_app/system/blob/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:27.000000 core_main_app-2.8.0/core_main_app/system/blob/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      233 2024-03-12 19:02:27.000000 core_main_app-2.8.0/core_main_app/system/blob/api.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:58.148872 core_main_app-2.8.0/core_main_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:51.597988 core_main_app-2.8.0/core_main_app/templates/core_main_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:51.340613 core_main_app-2.8.0/core_main_app/templates/core_main_app/_render/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:58.193755 core_main_app-2.8.0/core_main_app/templates/core_main_app/_render/admin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1302 2024-03-12 19:02:27.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/_render/admin/app_wrapper.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:58.269770 core_main_app-2.8.0/core_main_app/templates/core_main_app/_render/admin/theme/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2405 2024-03-12 19:02:27.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/_render/admin/theme/base.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      324 2024-03-12 19:02:27.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/_render/admin/theme/footer.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1110 2024-03-12 19:02:27.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/_render/admin/theme/header.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3513 2024-03-12 19:02:27.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/_render/admin/theme/menu.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:58.341670 core_main_app-2.8.0/core_main_app/templates/core_main_app/_render/admin/theme/tools/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      726 2024-03-12 19:02:27.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/_render/admin/theme/tools/box.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:27.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/_render/admin/theme/tools/form.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1034 2024-03-12 19:02:27.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/_render/admin/theme/tools/modal.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      283 2024-03-12 19:02:27.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/_render/admin/theme/tools/section.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:58.400080 core_main_app-2.8.0/core_main_app/templates/core_main_app/_render/common/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2352 2024-03-12 19:02:27.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/_render/common/base_css.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1558 2024-03-12 19:02:27.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/_render/common/base_js.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1675 2024-03-12 19:02:27.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/_render/common/messages.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:58.459899 core_main_app-2.8.0/core_main_app/templates/core_main_app/_render/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1974 2024-03-12 19:02:27.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/_render/user/app_wrapper.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      902 2024-03-12 19:02:27.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/_render/user/default.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1867 2024-03-12 19:02:28.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/_render/user/theme_base.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:58.545443 core_main_app-2.8.0/core_main_app/templates/core_main_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:58.626862 core_main_app-2.8.0/core_main_app/templates/core_main_app/admin/blob/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      312 2024-03-12 19:02:28.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/admin/blob/detail.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      359 2024-03-12 19:02:28.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/admin/blob/detail_box.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      323 2024-03-12 19:02:28.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/admin/blob/detail_metadata.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      367 2024-03-12 19:02:28.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/admin/blob/detail_metadata_box.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:51.370445 core_main_app-2.8.0/core_main_app/templates/core_main_app/admin/commons/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:58.675572 core_main_app-2.8.0/core_main_app/templates/core_main_app/admin/commons/errors/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      401 2024-03-12 19:02:28.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/admin/commons/errors/errors.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      254 2024-03-12 19:02:28.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/admin/commons/errors/errors_wrapper.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:58.720929 core_main_app-2.8.0/core_main_app/templates/core_main_app/admin/commons/upload/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      795 2024-03-12 19:02:28.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/admin/commons/upload/form.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      313 2024-03-12 19:02:28.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/admin/commons/upload/upload.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      103 2024-03-12 19:02:28.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/admin/dashboard.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:58.765382 core_main_app-2.8.0/core_main_app/templates/core_main_app/admin/data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      311 2024-03-12 19:02:28.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/admin/data/detail.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      383 2024-03-12 19:02:28.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/admin/data/detail_box.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1598 2024-03-12 19:02:28.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/admin/dependency_resolver.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      211 2024-03-12 19:02:28.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/admin/list_dependencies.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:58.841906 core_main_app-2.8.0/core_main_app/templates/core_main_app/admin/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:58.864039 core_main_app-2.8.0/core_main_app/templates/core_main_app/admin/templates/data_migration/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8123 2024-03-12 19:02:28.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/admin/templates/data_migration/templates_list.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      289 2024-03-12 19:02:28.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/admin/templates/data_migration.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:58.912258 core_main_app-2.8.0/core_main_app/templates/core_main_app/admin/templates/list/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2705 2024-03-12 19:02:28.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/admin/templates/list/available.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      830 2024-03-12 19:02:28.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/admin/templates/list/disabled.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:58.935714 core_main_app-2.8.0/core_main_app/templates/core_main_app/admin/templates/list/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      926 2024-03-12 19:02:28.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/admin/templates/list/modals/disable.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      542 2024-03-12 19:02:28.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/admin/templates/list.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:58.959423 core_main_app-2.8.0/core_main_app/templates/core_main_app/admin/templates/upload/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      399 2024-03-12 19:02:28.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/admin/templates/upload/base.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      166 2024-03-12 19:02:28.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/admin/templates/upload.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:59.003013 core_main_app-2.8.0/core_main_app/templates/core_main_app/admin/templates/versions/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3746 2024-03-12 19:02:28.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/admin/templates/versions/available.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1182 2024-03-12 19:02:28.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/admin/templates/versions/disabled.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:59.031262 core_main_app-2.8.0/core_main_app/templates/core_main_app/admin/templates/versions/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      840 2024-03-12 19:02:28.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/admin/templates/versions/modals/disable.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      677 2024-03-12 19:02:28.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/admin/templates/versions.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:59.055050 core_main_app-2.8.0/core_main_app/templates/core_main_app/admin/templates_xslt/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:59.077005 core_main_app-2.8.0/core_main_app/templates/core_main_app/admin/templates_xslt/main/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5044 2024-03-12 19:02:28.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/admin/templates_xslt/main/form.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      393 2024-03-12 19:02:28.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/admin/templates_xslt/main.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      860 2024-03-12 19:02:28.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/admin/upload_template.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:59.155421 core_main_app-2.8.0/core_main_app/templates/core_main_app/admin/web_page/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      166 2024-03-12 19:02:28.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/admin/web_page/login_page.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      905 2024-03-12 19:02:28.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/admin/web_page/main.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      387 2024-03-12 19:02:28.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/admin/web_page/web_page.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      375 2024-03-12 19:02:28.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/admin/web_page/web_page_unavailable.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:59.179059 core_main_app-2.8.0/core_main_app/templates/core_main_app/admin/workspaces/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      234 2024-03-12 19:02:28.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/admin/workspaces/edit_rights.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:59.215842 core_main_app-2.8.0/core_main_app/templates/core_main_app/admin/xslt/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:59.239272 core_main_app-2.8.0/core_main_app/templates/core_main_app/admin/xslt/list/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1337 2024-03-12 19:02:28.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/admin/xslt/list/table.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      323 2024-03-12 19:02:28.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/admin/xslt/list.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:59.262812 core_main_app-2.8.0/core_main_app/templates/core_main_app/admin/xslt/upload/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       61 2024-03-12 19:02:28.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/admin/xslt/upload/base.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      161 2024-03-12 19:02:28.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/admin/xslt/upload.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:51.562787 core_main_app-2.8.0/core_main_app/templates/core_main_app/common/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:59.352839 core_main_app-2.8.0/core_main_app/templates/core_main_app/common/blob/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      823 2024-03-12 19:02:28.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/common/blob/detail_blob.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2165 2024-03-12 19:02:28.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/common/blob/detail_metadata.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1321 2024-03-12 19:02:28.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/common/blob/tools_blob.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      682 2024-03-12 19:02:28.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/common/blob/tools_metadata.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:59.454141 core_main_app-2.8.0/core_main_app/templates/core_main_app/common/buttons/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      194 2024-03-12 19:02:28.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/common/buttons/add.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      253 2024-03-12 19:02:28.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/common/buttons/back_to_previous.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      194 2024-03-12 19:02:28.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/common/buttons/delete.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      190 2024-03-12 19:02:28.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/common/buttons/edit.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      104 2024-03-12 19:02:28.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/common/buttons/go_to.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:59.516828 core_main_app-2.8.0/core_main_app/templates/core_main_app/common/commons/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      189 2024-03-12 19:02:28.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/common/commons/error.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       97 2024-03-12 19:02:28.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/common/commons/form.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      167 2024-03-12 19:02:28.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/common/commons/form_delete.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:59.558869 core_main_app-2.8.0/core_main_app/templates/core_main_app/common/commons/upload/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      679 2024-03-12 19:02:28.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/common/commons/upload/form.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      313 2024-03-12 19:02:28.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/common/commons/upload/upload.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:59.603411 core_main_app-2.8.0/core_main_app/templates/core_main_app/common/data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      759 2024-03-12 19:02:28.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/common/data/detail_data.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2486 2024-03-12 19:02:28.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/common/data/tools_data.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:59.626274 core_main_app-2.8.0/core_main_app/templates/core_main_app/common/defender/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       90 2024-03-12 19:02:28.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/common/defender/error.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:59.765188 core_main_app-2.8.0/core_main_app/templates/core_main_app/common/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      576 2024-03-12 19:02:28.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/common/modals/add_page_modal.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      750 2024-03-12 19:02:28.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/common/modals/create_data_modal.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      601 2024-03-12 19:02:28.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/common/modals/delete_page_modal.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1197 2024-03-12 19:02:28.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/common/modals/download-options.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      580 2024-03-12 19:02:28.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/common/modals/edit_page_modal.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      429 2024-03-12 19:02:28.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/common/modals/error_page_modal.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:59.788382 core_main_app-2.8.0/core_main_app/templates/core_main_app/common/pagination/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3008 2024-03-12 19:02:28.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/common/pagination/data_source_pagination.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:59.812360 core_main_app-2.8.0/core_main_app/templates/core_main_app/common/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:59.857534 core_main_app-2.8.0/core_main_app/templates/core_main_app/common/templates/list/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1625 2024-03-12 19:02:28.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/common/templates/list/available.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      801 2024-03-12 19:02:28.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/common/templates/list/disabled.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:59.900961 core_main_app-2.8.0/core_main_app/templates/core_main_app/common/templates/list/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      918 2024-03-12 19:02:28.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/common/templates/list/modals/disable.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      854 2024-03-12 19:02:28.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/common/templates/list/modals/edit.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:59.924219 core_main_app-2.8.0/core_main_app/templates/core_main_app/common/templates/versions/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2367 2024-03-12 19:02:28.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/common/templates/versions/available.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:59.947853 core_main_app-2.8.0/core_main_app/templates/core_main_app/common/templates/versions/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      775 2024-03-12 19:02:29.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/common/templates/versions/modals/disable.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      265 2024-03-12 19:02:28.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/common/templates/versions.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:59.972797 core_main_app-2.8.0/core_main_app/templates/core_main_app/common/templates_xslt/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:59.997512 core_main_app-2.8.0/core_main_app/templates/core_main_app/common/templates_xslt/main/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1263 2024-03-12 19:02:29.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/common/templates_xslt/main/form.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      428 2024-03-12 19:02:29.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/common/templates_xslt/main.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:00.041672 core_main_app-2.8.0/core_main_app/templates/core_main_app/common/xslt/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:00.064974 core_main_app-2.8.0/core_main_app/templates/core_main_app/common/xslt/list/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:00.107388 core_main_app-2.8.0/core_main_app/templates/core_main_app/common/xslt/list/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      677 2024-03-12 19:02:29.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/common/xslt/list/modals/delete.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1234 2024-03-12 19:02:29.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/common/xslt/list/modals/edit.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1248 2024-03-12 19:02:29.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/common/xslt/list/table.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      255 2024-03-12 19:02:29.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/common/xslt/list.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:00.130924 core_main_app-2.8.0/core_main_app/templates/core_main_app/common/xslt/upload/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       62 2024-03-12 19:02:29.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/common/xslt/upload/base.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      163 2024-03-12 19:02:29.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/common/xslt/upload.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:00.177734 core_main_app-2.8.0/core_main_app/templates/core_main_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:00.220211 core_main_app-2.8.0/core_main_app/templates/core_main_app/user/blob/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      295 2024-03-12 19:02:29.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/user/blob/detail.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      338 2024-03-12 19:02:29.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/user/blob/detail_metadata.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:51.618897 core_main_app-2.8.0/core_main_app/templates/core_main_app/user/blob/list/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:00.308841 core_main_app-2.8.0/core_main_app/templates/core_main_app/user/blob/list/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      689 2024-03-12 19:02:29.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/user/blob/list/modals/add_metadata.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      231 2024-03-12 19:02:29.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/user/blob/list/modals/add_metadata_form.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      686 2024-03-12 19:02:29.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/user/blob/list/modals/file_upload.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      148 2024-03-12 19:02:29.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/user/blob/list/modals/file_upload_form.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:00.333075 core_main_app-2.8.0/core_main_app/templates/core_main_app/user/data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      483 2024-03-12 19:02:29.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/user/data/detail.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      139 2024-03-12 19:02:29.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/user/homepage.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:00.376056 core_main_app-2.8.0/core_main_app/templates/core_main_app/user/login/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2408 2024-03-12 19:02:29.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/user/login/main.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:00.398657 core_main_app-2.8.0/core_main_app/templates/core_main_app/user/login/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      534 2024-03-12 19:02:29.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/user/login/modals/login_message.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      340 2024-03-12 19:02:29.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/user/login/saml2_error.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:00.516348 core_main_app-2.8.0/core_main_app/templates/core_main_app/user/registration/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      171 2024-03-12 19:02:29.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/user/registration/password_reset_complete.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      491 2024-03-12 19:02:29.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/user/registration/password_reset_confirm.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      600 2024-03-12 19:02:29.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/user/registration/password_reset_done.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      362 2024-03-12 19:02:29.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/user/registration/password_reset_email.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      281 2024-03-12 19:02:29.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/user/registration/password_reset_form.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       14 2024-03-12 19:02:29.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/user/registration/password_reset_subject.txt
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:00.538544 core_main_app-2.8.0/core_main_app/templates/core_main_app/user/sharing/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      274 2024-03-12 19:02:29.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/user/sharing/button.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:00.578677 core_main_app-2.8.0/core_main_app/templates/core_main_app/user/sharing/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      504 2024-03-12 19:02:29.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/user/sharing/modals/multi-link.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1132 2024-03-12 19:02:29.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/user/sharing/modals/single-link.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:00.620304 core_main_app-2.8.0/core_main_app/templates/core_main_app/user/template/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      453 2024-03-12 19:02:29.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/user/template/list_body.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2024-03-12 19:02:29.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/user/template/list_header.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:00.647960 core_main_app-2.8.0/core_main_app/templates/core_main_app/user/text_editor/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4486 2024-03-12 19:02:29.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/user/text_editor/text_editor.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      757 2024-03-12 19:02:29.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/user/timezone.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:00.670880 core_main_app-2.8.0/core_main_app/templates/core_main_app/user/workspaces/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1186 2024-03-12 19:02:29.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/user/workspaces/edit_rights.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:00.712072 core_main_app-2.8.0/core_main_app/templates/core_main_app/user/workspaces/list/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1622 2024-03-12 19:02:29.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/user/workspaces/list/create_workspace.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1882 2024-03-12 19:02:29.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/user/workspaces/list/edit_rights_table.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:00.908944 core_main_app-2.8.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1747 2024-03-12 19:02:29.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/add_group.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      222 2024-03-12 19:02:29.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/add_group_form.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1725 2024-03-12 19:02:29.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/add_user.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      219 2024-03-12 19:02:29.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/add_user_form.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      945 2024-03-12 19:02:29.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/assign_workspace.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      411 2024-03-12 19:02:29.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/assign_workspace_form.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1264 2024-03-12 19:02:29.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/remove_rights.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1183 2024-03-12 19:02:29.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/set_private.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1191 2024-03-12 19:02:29.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/set_public.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      981 2024-03-12 19:02:29.000000 core_main_app-2.8.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/switch_right.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      147 2024-03-12 19:02:29.000000 core_main_app-2.8.0/core_main_app/templates/theme.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:01.137295 core_main_app-2.8.0/core_main_app/templatetags/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:29.000000 core_main_app-2.8.0/core_main_app/templatetags/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      686 2024-03-12 19:02:29.000000 core_main_app-2.8.0/core_main_app/templatetags/auth_extras.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1690 2024-03-12 19:02:29.000000 core_main_app-2.8.0/core_main_app/templatetags/blob_tags.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      367 2024-03-12 19:02:29.000000 core_main_app-2.8.0/core_main_app/templatetags/dict_key_extras.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      487 2024-03-12 19:02:29.000000 core_main_app-2.8.0/core_main_app/templatetags/format_json.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      514 2024-03-12 19:02:29.000000 core_main_app-2.8.0/core_main_app/templatetags/get_attribute.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      598 2024-03-12 19:02:29.000000 core_main_app-2.8.0/core_main_app/templatetags/include_static.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1124 2024-03-12 19:02:29.000000 core_main_app-2.8.0/core_main_app/templatetags/json_date.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      509 2024-03-12 19:02:29.000000 core_main_app-2.8.0/core_main_app/templatetags/parse_date.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      640 2024-03-12 19:02:29.000000 core_main_app-2.8.0/core_main_app/templatetags/stripjs.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      316 2024-03-12 19:02:29.000000 core_main_app-2.8.0/core_main_app/templatetags/timestamptags.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3319 2024-03-12 19:02:29.000000 core_main_app-2.8.0/core_main_app/templatetags/xsl_transform_tag.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4975 2024-03-12 19:02:29.000000 core_main_app-2.8.0/core_main_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:01.486084 core_main_app-2.8.0/core_main_app/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:29.000000 core_main_app-2.8.0/core_main_app/utils/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:01.544251 core_main_app-2.8.0/core_main_app/utils/admin_site/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:29.000000 core_main_app-2.8.0/core_main_app/utils/admin_site/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1233 2024-03-12 19:02:29.000000 core_main_app-2.8.0/core_main_app/utils/admin_site/model_admin_class.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      379 2024-03-12 19:02:29.000000 core_main_app-2.8.0/core_main_app/utils/admin_site/view_only_admin.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2447 2024-03-12 19:02:29.000000 core_main_app-2.8.0/core_main_app/utils/blob_downloader.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      405 2024-03-12 19:02:29.000000 core_main_app-2.8.0/core_main_app/utils/boolean.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1137 2024-03-12 19:02:29.000000 core_main_app-2.8.0/core_main_app/utils/checksum.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1966 2024-03-12 19:02:29.000000 core_main_app-2.8.0/core_main_app/utils/custom_context_processors.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:01.582594 core_main_app-2.8.0/core_main_app/utils/databases/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:29.000000 core_main_app-2.8.0/core_main_app/utils/databases/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      627 2024-03-12 19:02:29.000000 core_main_app-2.8.0/core_main_app/utils/databases/backend.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:01.614728 core_main_app-2.8.0/core_main_app/utils/databases/mongo/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      574 2024-03-12 19:02:29.000000 core_main_app-2.8.0/core_main_app/utils/databases/mongo/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      873 2024-03-12 19:02:29.000000 core_main_app-2.8.0/core_main_app/utils/databases/mongo/pymongo_database.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      286 2024-03-12 19:02:29.000000 core_main_app-2.8.0/core_main_app/utils/datetime.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9575 2024-03-12 19:02:29.000000 core_main_app-2.8.0/core_main_app/utils/decorators.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      449 2024-03-12 19:02:29.000000 core_main_app-2.8.0/core_main_app/utils/dict.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4473 2024-03-12 19:02:29.000000 core_main_app-2.8.0/core_main_app/utils/file.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      377 2024-03-12 19:02:29.000000 core_main_app-2.8.0/core_main_app/utils/group.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:01.683286 core_main_app-2.8.0/core_main_app/utils/integration_tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/utils/integration_tests/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      262 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/utils/integration_tests/fixture_interface.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1651 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/utils/integration_tests/integration_base_test_case.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1031 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/utils/integration_tests/integration_base_transaction_test_case.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4219 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/utils/json_utils.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      318 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/utils/labels.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:01.721883 core_main_app-2.8.0/core_main_app/utils/logger/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/utils/logger/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1762 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/utils/logger/logger_utils.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      438 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/utils/markdown_parser.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      956 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/utils/migrations.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:01.764159 core_main_app-2.8.0/core_main_app/utils/notifications/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/utils/notifications/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3448 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/utils/notifications/mail.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:01.804780 core_main_app-2.8.0/core_main_app/utils/notifications/tasks/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/utils/notifications/tasks/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2566 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/utils/notifications/tasks/task_mail.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:01.824288 core_main_app-2.8.0/core_main_app/utils/pagination/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/utils/pagination/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:01.866803 core_main_app-2.8.0/core_main_app/utils/pagination/django_paginator/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/utils/pagination/django_paginator/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      773 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/utils/pagination/django_paginator/results_paginator.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:01.909528 core_main_app-2.8.0/core_main_app/utils/pagination/mongoengine_paginator/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/utils/pagination/mongoengine_paginator/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1109 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/utils/pagination/mongoengine_paginator/paginator.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:02.041042 core_main_app-2.8.0/core_main_app/utils/pagination/rest_framework_paginator/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/utils/pagination/rest_framework_paginator/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      525 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/utils/pagination/rest_framework_paginator/pagination.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1108 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/utils/pagination/rest_framework_paginator/rest_framework_paginator.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      458 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/utils/parser.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:02.084317 core_main_app-2.8.0/core_main_app/utils/query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/utils/query/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      145 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/utils/query/constants.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:02.150731 core_main_app-2.8.0/core_main_app/utils/query/mongo/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/utils/query/mongo/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14676 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/utils/query/mongo/prepare.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3095 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/utils/query/mongo/query_builder.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:02.225793 core_main_app-2.8.0/core_main_app/utils/raw_query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/utils/raw_query/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1622 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/utils/raw_query/common.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3901 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/utils/raw_query/django_raw_query.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2134 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/utils/raw_query/mongo_raw_query.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3182 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/utils/rendering.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:02.316717 core_main_app-2.8.0/core_main_app/utils/requests_utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/utils/requests_utils/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      568 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/utils/requests_utils/access_control.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1663 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/utils/requests_utils/requests_utils.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2054 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/utils/requests_utils/ssl.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:02.397339 core_main_app-2.8.0/core_main_app/utils/resolvers/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/utils/resolvers/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1184 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/utils/resolvers/requests_resolver.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1072 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/utils/resolvers/resolver_utils.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      194 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/utils/resolvers/xsd_uri_resolvers.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:02.448530 core_main_app-2.8.0/core_main_app/utils/routers/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/utils/routers/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      786 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/utils/routers/db_router.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:02.488555 core_main_app-2.8.0/core_main_app/utils/saml2/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/utils/saml2/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8886 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/utils/saml2/utils.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1857 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/utils/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:02.540604 core_main_app-2.8.0/core_main_app/utils/storage/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/utils/storage/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3523 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/utils/storage/gridfs_storage.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1791 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/utils/storage/storage.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:02.591390 core_main_app-2.8.0/core_main_app/utils/tests_tools/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      853 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/utils/tests_tools/MockUser.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5344 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/utils/tests_tools/RequestMock.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/utils/tests_tools/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:02.614011 core_main_app-2.8.0/core_main_app/utils/tests_tools/databases/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/utils/tests_tools/databases/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:02.670791 core_main_app-2.8.0/core_main_app/utils/tests_tools/databases/mongo/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/utils/tests_tools/databases/mongo/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1690 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/utils/tests_tools/databases/mongo/mongoengine_database.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3654 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/utils/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:02.743808 core_main_app-2.8.0/core_main_app/utils/validation/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/utils/validation/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1162 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/utils/validation/regex_validation.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      644 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/utils/validation/xpath_validation.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:02.792355 core_main_app-2.8.0/core_main_app/utils/view_builders/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/utils/view_builders/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6818 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/utils/view_builders/data.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    15550 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/utils/xml.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:02.852234 core_main_app-2.8.0/core_main_app/utils/xsd_flattener/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/utils/xsd_flattener/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2094 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/utils/xsd_flattener/xsd_flattener_database_url.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1000 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/utils/xsd_flattener/xsd_flattener_requests_url.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:02.875207 core_main_app-2.8.0/core_main_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:02.955063 core_main_app-2.8.0/core_main_app/views/admin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/views/admin/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4302 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/views/admin/ajax.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:02.982836 core_main_app-2.8.0/core_main_app/views/admin/commons/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/views/admin/commons/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:03.027578 core_main_app-2.8.0/core_main_app/views/admin/commons/upload/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/views/admin/commons/upload/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      439 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/views/admin/commons/upload/forms.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5702 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/views/admin/forms.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    21702 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/views/admin/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:03.114149 core_main_app-2.8.0/core_main_app/views/common/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/views/common/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7236 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/views/common/ajax.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      459 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/views/common/forms.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    43264 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/views/common/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:03.196462 core_main_app-2.8.0/core_main_app/views/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/views/user/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    21825 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/views/user/ajax.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6400 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/views/user/forms.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11091 2024-03-12 19:02:30.000000 core_main_app-2.8.0/core_main_app/views/user/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:52.823794 core_main_app-2.8.0/core_main_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9924 2024-03-12 19:02:45.000000 core_main_app-2.8.0/core_main_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    35867 2024-03-12 19:02:50.000000 core_main_app-2.8.0/core_main_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2024-03-12 19:02:45.000000 core_main_app-2.8.0/core_main_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      491 2024-03-12 19:02:45.000000 core_main_app-2.8.0/core_main_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       25 2024-03-12 19:02:45.000000 core_main_app-2.8.0/core_main_app.egg-info/top_level.txt
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:03.260844 core_main_app-2.8.0/docs/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:31.000000 core_main_app-2.8.0/docs/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11121 2024-03-12 19:02:31.000000 core_main_app-2.8.0/docs/conf.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      278 2024-03-12 19:02:31.000000 core_main_app-2.8.0/docs/conf_urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      170 2024-03-12 19:02:37.000000 core_main_app-2.8.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       18 2024-03-12 19:02:37.000000 core_main_app-2.8.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       91 2024-03-12 19:02:37.000000 core_main_app-2.8.0/requirements.dev.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       20 2024-03-12 19:02:37.000000 core_main_app-2.8.0/requirements.mongo.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      340 2024-03-12 19:02:37.000000 core_main_app-2.8.0/requirements.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2024-03-12 19:03:13.199531 core_main_app-2.8.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2104 2024-03-12 19:02:37.000000 core_main_app-2.8.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:03.376957 core_main_app-2.8.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:37.000000 core_main_app-2.8.0/tests/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:03.419189 core_main_app-2.8.0/tests/access_control/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:37.000000 core_main_app-2.8.0/tests/access_control/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:03.460545 core_main_app-2.8.0/tests/access_control/api/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:37.000000 core_main_app-2.8.0/tests/access_control/api/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1126 2024-03-12 19:02:37.000000 core_main_app-2.8.0/tests/access_control/api/tests_unit.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3415 2024-03-12 19:02:37.000000 core_main_app-2.8.0/tests/access_control/tests_access_control.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:03.516599 core_main_app-2.8.0/tests/access_control/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:37.000000 core_main_app-2.8.0/tests/access_control/utils/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6858 2024-03-12 19:02:37.000000 core_main_app-2.8.0/tests/access_control/utils/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:03.537278 core_main_app-2.8.0/tests/commons/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:37.000000 core_main_app-2.8.0/tests/commons/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:03.582389 core_main_app-2.8.0/tests/commons/exceptions/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:37.000000 core_main_app-2.8.0/tests/commons/exceptions/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1254 2024-03-12 19:02:37.000000 core_main_app-2.8.0/tests/commons/exceptions/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:03.625986 core_main_app-2.8.0/tests/commons/validators/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:37.000000 core_main_app-2.8.0/tests/commons/validators/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4324 2024-03-12 19:02:37.000000 core_main_app-2.8.0/tests/commons/validators/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:03.649868 core_main_app-2.8.0/tests/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:37.000000 core_main_app-2.8.0/tests/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:03.740586 core_main_app-2.8.0/tests/components/blob/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:37.000000 core_main_app-2.8.0/tests/components/blob/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:03.781950 core_main_app-2.8.0/tests/components/blob/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:37.000000 core_main_app-2.8.0/tests/components/blob/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3165 2024-03-12 19:02:37.000000 core_main_app-2.8.0/tests/components/blob/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6398 2024-03-12 19:02:37.000000 core_main_app-2.8.0/tests/components/blob/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    38881 2024-03-12 19:02:37.000000 core_main_app-2.8.0/tests/components/blob/tests_int_access_control.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2353 2024-03-12 19:02:37.000000 core_main_app-2.8.0/tests/components/blob/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:03.891425 core_main_app-2.8.0/tests/components/data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:37.000000 core_main_app-2.8.0/tests/components/data/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:03.938567 core_main_app-2.8.0/tests/components/data/access_control/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:37.000000 core_main_app-2.8.0/tests/components/data/access_control/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2716 2024-03-12 19:02:37.000000 core_main_app-2.8.0/tests/components/data/access_control/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:03.982623 core_main_app-2.8.0/tests/components/data/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:37.000000 core_main_app-2.8.0/tests/components/data/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    28106 2024-03-12 19:02:37.000000 core_main_app-2.8.0/tests/components/data/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    69360 2024-03-12 19:02:37.000000 core_main_app-2.8.0/tests/components/data/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    83957 2024-03-12 19:02:37.000000 core_main_app-2.8.0/tests/components/data/tests_int_access_control.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3730 2024-03-12 19:02:37.000000 core_main_app-2.8.0/tests/components/data/tests_int_ordering.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    40552 2024-03-12 19:02:37.000000 core_main_app-2.8.0/tests/components/data/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:04.034116 core_main_app-2.8.0/tests/components/group/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:37.000000 core_main_app-2.8.0/tests/components/group/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:04.098035 core_main_app-2.8.0/tests/components/group/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:37.000000 core_main_app-2.8.0/tests/components/group/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      570 2024-03-12 19:02:37.000000 core_main_app-2.8.0/tests/components/group/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      879 2024-03-12 19:02:37.000000 core_main_app-2.8.0/tests/components/group/fixtures/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4760 2024-03-12 19:02:37.000000 core_main_app-2.8.0/tests/components/group/tests_int.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:04.160755 core_main_app-2.8.0/tests/components/lock/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:37.000000 core_main_app-2.8.0/tests/components/lock/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4153 2024-03-12 19:02:37.000000 core_main_app-2.8.0/tests/components/lock/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2440 2024-03-12 19:02:37.000000 core_main_app-2.8.0/tests/components/lock/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:04.226494 core_main_app-2.8.0/tests/components/mongo_data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:37.000000 core_main_app-2.8.0/tests/components/mongo_data/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    75687 2024-03-12 19:02:37.000000 core_main_app-2.8.0/tests/components/mongo_data/tests_int_access_control.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5423 2024-03-12 19:02:37.000000 core_main_app-2.8.0/tests/components/mongo_data/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:04.293094 core_main_app-2.8.0/tests/components/template/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:37.000000 core_main_app-2.8.0/tests/components/template/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:04.337085 core_main_app-2.8.0/tests/components/template/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:37.000000 core_main_app-2.8.0/tests/components/template/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2081 2024-03-12 19:02:37.000000 core_main_app-2.8.0/tests/components/template/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    46022 2024-03-12 19:02:37.000000 core_main_app-2.8.0/tests/components/template/tests_int_access_control.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10648 2024-03-12 19:02:37.000000 core_main_app-2.8.0/tests/components/template/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:04.395254 core_main_app-2.8.0/tests/components/template_version_manager/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:37.000000 core_main_app-2.8.0/tests/components/template_version_manager/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:04.435833 core_main_app-2.8.0/tests/components/template_version_manager/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:38.000000 core_main_app-2.8.0/tests/components/template_version_manager/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6479 2024-03-12 19:02:38.000000 core_main_app-2.8.0/tests/components/template_version_manager/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    54686 2024-03-12 19:02:38.000000 core_main_app-2.8.0/tests/components/template_version_manager/tests_int_access_control.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    20410 2024-03-12 19:02:38.000000 core_main_app-2.8.0/tests/components/template_version_manager/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:04.493251 core_main_app-2.8.0/tests/components/template_xsl_rendering/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:38.000000 core_main_app-2.8.0/tests/components/template_xsl_rendering/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:04.534160 core_main_app-2.8.0/tests/components/template_xsl_rendering/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:38.000000 core_main_app-2.8.0/tests/components/template_xsl_rendering/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3269 2024-03-12 19:02:38.000000 core_main_app-2.8.0/tests/components/template_xsl_rendering/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7896 2024-03-12 19:02:38.000000 core_main_app-2.8.0/tests/components/template_xsl_rendering/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9565 2024-03-12 19:02:38.000000 core_main_app-2.8.0/tests/components/template_xsl_rendering/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:04.575250 core_main_app-2.8.0/tests/components/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:38.000000 core_main_app-2.8.0/tests/components/user/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:04.636534 core_main_app-2.8.0/tests/components/user/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:38.000000 core_main_app-2.8.0/tests/components/user/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1552 2024-03-12 19:02:38.000000 core_main_app-2.8.0/tests/components/user/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1429 2024-03-12 19:02:38.000000 core_main_app-2.8.0/tests/components/user/fixtures/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7733 2024-03-12 19:02:38.000000 core_main_app-2.8.0/tests/components/user/tests_int.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:04.807897 core_main_app-2.8.0/tests/components/user_preferences/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:38.000000 core_main_app-2.8.0/tests/components/user_preferences/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:04.859483 core_main_app-2.8.0/tests/components/user_preferences/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:38.000000 core_main_app-2.8.0/tests/components/user_preferences/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1302 2024-03-12 19:02:38.000000 core_main_app-2.8.0/tests/components/user_preferences/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3912 2024-03-12 19:02:38.000000 core_main_app-2.8.0/tests/components/user_preferences/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11726 2024-03-12 19:02:38.000000 core_main_app-2.8.0/tests/components/user_preferences/tests_int_access_control.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6563 2024-03-12 19:02:38.000000 core_main_app-2.8.0/tests/components/user_preferences/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:04.923504 core_main_app-2.8.0/tests/components/version_manager/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:38.000000 core_main_app-2.8.0/tests/components/version_manager/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    61614 2024-03-12 19:02:38.000000 core_main_app-2.8.0/tests/components/version_manager/tests_int_access_control.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9899 2024-03-12 19:02:38.000000 core_main_app-2.8.0/tests/components/version_manager/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:04.968336 core_main_app-2.8.0/tests/components/web_page/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:38.000000 core_main_app-2.8.0/tests/components/web_page/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4846 2024-03-12 19:02:38.000000 core_main_app-2.8.0/tests/components/web_page/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:05.023980 core_main_app-2.8.0/tests/components/web_page_login/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:38.000000 core_main_app-2.8.0/tests/components/web_page_login/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3905 2024-03-12 19:02:38.000000 core_main_app-2.8.0/tests/components/web_page_login/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:05.070257 core_main_app-2.8.0/tests/components/workspace/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:38.000000 core_main_app-2.8.0/tests/components/workspace/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:05.132456 core_main_app-2.8.0/tests/components/workspace/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:38.000000 core_main_app-2.8.0/tests/components/workspace/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1235 2024-03-12 19:02:38.000000 core_main_app-2.8.0/tests/components/workspace/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      919 2024-03-12 19:02:38.000000 core_main_app-2.8.0/tests/components/workspace/fixtures/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7478 2024-03-12 19:02:38.000000 core_main_app-2.8.0/tests/components/workspace/tests_int.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:05.175637 core_main_app-2.8.0/tests/components/xsl_transformation/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:38.000000 core_main_app-2.8.0/tests/components/xsl_transformation/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    12828 2024-03-12 19:02:38.000000 core_main_app-2.8.0/tests/components/xsl_transformation/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:05.239140 core_main_app-2.8.0/tests/middleware/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:38.000000 core_main_app-2.8.0/tests/middleware/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3431 2024-03-12 19:02:38.000000 core_main_app-2.8.0/tests/middleware/tests_unit.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      356 2024-03-12 19:02:38.000000 core_main_app-2.8.0/tests/mocks.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:05.283678 core_main_app-2.8.0/tests/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:38.000000 core_main_app-2.8.0/tests/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:05.378143 core_main_app-2.8.0/tests/rest/blob/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:38.000000 core_main_app-2.8.0/tests/rest/blob/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:05.598114 core_main_app-2.8.0/tests/rest/blob/serializers/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:38.000000 core_main_app-2.8.0/tests/rest/blob/serializers/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4251 2024-03-12 19:02:38.000000 core_main_app-2.8.0/tests/rest/blob/serializers/tests_unit.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    31044 2024-03-12 19:02:38.000000 core_main_app-2.8.0/tests/rest/blob/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    26694 2024-03-12 19:02:38.000000 core_main_app-2.8.0/tests/rest/blob/tests_permissions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       36 2024-03-12 19:02:38.000000 core_main_app-2.8.0/tests/rest/blob/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:07.800532 core_main_app-2.8.0/tests/rest/data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:38.000000 core_main_app-2.8.0/tests/rest/data/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    49596 2024-03-12 19:02:38.000000 core_main_app-2.8.0/tests/rest/data/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    37874 2024-03-12 19:02:38.000000 core_main_app-2.8.0/tests/rest/data/tests_permissions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    30805 2024-03-12 19:02:38.000000 core_main_app-2.8.0/tests/rest/data/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:09.813826 core_main_app-2.8.0/tests/rest/template/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:38.000000 core_main_app-2.8.0/tests/rest/template/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2518 2024-03-12 19:02:38.000000 core_main_app-2.8.0/tests/rest/template/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5026 2024-03-12 19:02:38.000000 core_main_app-2.8.0/tests/rest/template/tests_permission.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6295 2024-03-12 19:02:38.000000 core_main_app-2.8.0/tests/rest/template/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:11.287801 core_main_app-2.8.0/tests/rest/template_version_manager/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:38.000000 core_main_app-2.8.0/tests/rest/template_version_manager/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    45015 2024-03-12 19:02:38.000000 core_main_app-2.8.0/tests/rest/template_version_manager/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    41433 2024-03-12 19:02:38.000000 core_main_app-2.8.0/tests/rest/template_version_manager/tests_permission.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5606 2024-03-12 19:02:38.000000 core_main_app-2.8.0/tests/rest/template_version_manager/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:11.351648 core_main_app-2.8.0/tests/rest/template_xsl_rendering/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:38.000000 core_main_app-2.8.0/tests/rest/template_xsl_rendering/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11418 2024-03-12 19:02:38.000000 core_main_app-2.8.0/tests/rest/template_xsl_rendering/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    13879 2024-03-12 19:02:38.000000 core_main_app-2.8.0/tests/rest/template_xsl_rendering/tests_permissions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3610 2024-03-12 19:02:38.000000 core_main_app-2.8.0/tests/rest/tests_views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:11.430779 core_main_app-2.8.0/tests/rest/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:38.000000 core_main_app-2.8.0/tests/rest/user/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1737 2024-03-12 19:02:38.000000 core_main_app-2.8.0/tests/rest/user/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3137 2024-03-12 19:02:38.000000 core_main_app-2.8.0/tests/rest/user/tests_permissions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      886 2024-03-12 19:02:38.000000 core_main_app-2.8.0/tests/rest/user/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:11.476740 core_main_app-2.8.0/tests/rest/web_page/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:38.000000 core_main_app-2.8.0/tests/rest/web_page/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6164 2024-03-12 19:02:38.000000 core_main_app-2.8.0/tests/rest/web_page/tests_permission.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:11.542122 core_main_app-2.8.0/tests/rest/workspace/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:38.000000 core_main_app-2.8.0/tests/rest/workspace/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    71809 2024-03-12 19:02:38.000000 core_main_app-2.8.0/tests/rest/workspace/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    48644 2024-03-12 19:02:38.000000 core_main_app-2.8.0/tests/rest/workspace/tests_permissions.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:11.624565 core_main_app-2.8.0/tests/rest/xsl_transformation/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:38.000000 core_main_app-2.8.0/tests/rest/xsl_transformation/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:11.667732 core_main_app-2.8.0/tests/rest/xsl_transformation/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:38.000000 core_main_app-2.8.0/tests/rest/xsl_transformation/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1283 2024-03-12 19:02:38.000000 core_main_app-2.8.0/tests/rest/xsl_transformation/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11618 2024-03-12 19:02:39.000000 core_main_app-2.8.0/tests/rest/xsl_transformation/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    12753 2024-03-12 19:02:39.000000 core_main_app-2.8.0/tests/rest/xsl_transformation/tests_permission.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4365 2024-03-12 19:02:39.000000 core_main_app-2.8.0/tests/rest/xsl_transformation/tests_unit.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      738 2024-03-12 19:02:39.000000 core_main_app-2.8.0/tests/rest_urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:11.708782 core_main_app-2.8.0/tests/system/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:39.000000 core_main_app-2.8.0/tests/system/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:11.729709 core_main_app-2.8.0/tests/system/blob/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:39.000000 core_main_app-2.8.0/tests/system/blob/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:11.778830 core_main_app-2.8.0/tests/system/blob/api/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:39.000000 core_main_app-2.8.0/tests/system/blob/api/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      935 2024-03-12 19:02:39.000000 core_main_app-2.8.0/tests/system/blob/api/tests_unit.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7830 2024-03-12 19:02:39.000000 core_main_app-2.8.0/tests/system/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:11.887640 core_main_app-2.8.0/tests/templatetags/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:39.000000 core_main_app-2.8.0/tests/templatetags/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:11.933218 core_main_app-2.8.0/tests/templatetags/auth_extras/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:39.000000 core_main_app-2.8.0/tests/templatetags/auth_extras/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1576 2024-03-12 19:02:39.000000 core_main_app-2.8.0/tests/templatetags/auth_extras/tests_unit.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1946 2024-03-12 19:02:39.000000 core_main_app-2.8.0/tests/templatetags/test_blob_tags.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      530 2024-03-12 19:02:39.000000 core_main_app-2.8.0/tests/templatetags/test_format_json.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1364 2024-03-12 19:02:39.000000 core_main_app-2.8.0/tests/templatetags/test_get_attribute.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1486 2024-03-12 19:02:39.000000 core_main_app-2.8.0/tests/templatetags/test_parse_date.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2883 2024-03-12 19:02:39.000000 core_main_app-2.8.0/tests/test_settings.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      293 2024-03-12 19:02:39.000000 core_main_app-2.8.0/tests/test_settings_sqlite3.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4310 2024-03-12 19:02:39.000000 core_main_app-2.8.0/tests/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:12.134515 core_main_app-2.8.0/tests/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:39.000000 core_main_app-2.8.0/tests/utils/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:12.178107 core_main_app-2.8.0/tests/utils/checksum/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:39.000000 core_main_app-2.8.0/tests/utils/checksum/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1294 2024-03-12 19:02:39.000000 core_main_app-2.8.0/tests/utils/checksum/tests_checksum.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:12.225476 core_main_app-2.8.0/tests/utils/dict/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:39.000000 core_main_app-2.8.0/tests/utils/dict/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      712 2024-03-12 19:02:39.000000 core_main_app-2.8.0/tests/utils/dict/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:12.272342 core_main_app-2.8.0/tests/utils/json_utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:39.000000 core_main_app-2.8.0/tests/utils/json_utils/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7501 2024-03-12 19:02:39.000000 core_main_app-2.8.0/tests/utils/json_utils/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:12.314933 core_main_app-2.8.0/tests/utils/migrations/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:39.000000 core_main_app-2.8.0/tests/utils/migrations/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1664 2024-03-12 19:02:39.000000 core_main_app-2.8.0/tests/utils/migrations/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:12.335672 core_main_app-2.8.0/tests/utils/query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:39.000000 core_main_app-2.8.0/tests/utils/query/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:12.385620 core_main_app-2.8.0/tests/utils/query/mongo/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:39.000000 core_main_app-2.8.0/tests/utils/query/mongo/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9855 2024-03-12 19:02:39.000000 core_main_app-2.8.0/tests/utils/query/mongo/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:12.433598 core_main_app-2.8.0/tests/utils/requests_utls/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:39.000000 core_main_app-2.8.0/tests/utils/requests_utls/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1436 2024-03-12 19:02:39.000000 core_main_app-2.8.0/tests/utils/requests_utls/tests_ssl.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:12.477368 core_main_app-2.8.0/tests/utils/routers/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:39.000000 core_main_app-2.8.0/tests/utils/routers/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1620 2024-03-12 19:02:39.000000 core_main_app-2.8.0/tests/utils/routers/tests_db_router.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:12.521969 core_main_app-2.8.0/tests/utils/settings/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:39.000000 core_main_app-2.8.0/tests/utils/settings/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4447 2024-03-12 19:02:39.000000 core_main_app-2.8.0/tests/utils/settings/tests_unit.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      902 2024-03-12 19:02:39.000000 core_main_app-2.8.0/tests/utils/test_unit_apps.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      772 2024-03-12 19:02:39.000000 core_main_app-2.8.0/tests/utils/test_unit_urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4010 2024-03-12 19:02:39.000000 core_main_app-2.8.0/tests/utils/tests_int_blob_downloader.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7757 2024-03-12 19:02:39.000000 core_main_app-2.8.0/tests/utils/tests_int_file.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2368 2024-03-12 19:02:39.000000 core_main_app-2.8.0/tests/utils/tests_unit_admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1726 2024-03-12 19:02:39.000000 core_main_app-2.8.0/tests/utils/tests_unit_boolean.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      402 2024-03-12 19:02:39.000000 core_main_app-2.8.0/tests/utils/tests_unit_parser.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11988 2024-03-12 19:02:39.000000 core_main_app-2.8.0/tests/utils/tests_unit_xml_operation.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5194 2024-03-12 19:02:39.000000 core_main_app-2.8.0/tests/utils/tests_view_data.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:12.579707 core_main_app-2.8.0/tests/utils/validation/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:39.000000 core_main_app-2.8.0/tests/utils/validation/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1318 2024-03-12 19:02:39.000000 core_main_app-2.8.0/tests/utils/validation/tests_unit_validation.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:12.640905 core_main_app-2.8.0/tests/utils/xsd_flattener/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:39.000000 core_main_app-2.8.0/tests/utils/xsd_flattener/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4358 2024-03-12 19:02:39.000000 core_main_app-2.8.0/tests/utils/xsd_flattener/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:12.725974 core_main_app-2.8.0/tests/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:39.000000 core_main_app-2.8.0/tests/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:12.747308 core_main_app-2.8.0/tests/views/admin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:39.000000 core_main_app-2.8.0/tests/views/admin/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:12.794826 core_main_app-2.8.0/tests/views/admin/ajax/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:39.000000 core_main_app-2.8.0/tests/views/admin/ajax/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      662 2024-03-12 19:02:39.000000 core_main_app-2.8.0/tests/views/admin/ajax/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:12.850530 core_main_app-2.8.0/tests/views/admin/forms/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:39.000000 core_main_app-2.8.0/tests/views/admin/forms/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1691 2024-03-12 19:02:39.000000 core_main_app-2.8.0/tests/views/admin/forms/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:12.894500 core_main_app-2.8.0/tests/views/admin/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:39.000000 core_main_app-2.8.0/tests/views/admin/views/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1336 2024-03-12 19:02:39.000000 core_main_app-2.8.0/tests/views/admin/views/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:12.926667 core_main_app-2.8.0/tests/views/common/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:39.000000 core_main_app-2.8.0/tests/views/common/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:12.994653 core_main_app-2.8.0/tests/views/common/ajax/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:39.000000 core_main_app-2.8.0/tests/views/common/ajax/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6717 2024-03-12 19:02:39.000000 core_main_app-2.8.0/tests/views/common/ajax/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:13.042964 core_main_app-2.8.0/tests/views/common/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:39.000000 core_main_app-2.8.0/tests/views/common/views/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11087 2024-03-12 19:02:39.000000 core_main_app-2.8.0/tests/views/common/views/test_unit.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6921 2024-03-12 19:02:39.000000 core_main_app-2.8.0/tests/views/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    81283 2024-03-12 19:02:39.000000 core_main_app-2.8.0/tests/views/tests_int_access_control.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1328 2024-03-12 19:02:39.000000 core_main_app-2.8.0/tests/views/tests_permissions.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:13.067897 core_main_app-2.8.0/tests/views/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:39.000000 core_main_app-2.8.0/tests/views/user/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:13.117919 core_main_app-2.8.0/tests/views/user/forms/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:40.000000 core_main_app-2.8.0/tests/views/user/forms/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2119 2024-03-12 19:02:40.000000 core_main_app-2.8.0/tests/views/user/forms/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:03:13.164546 core_main_app-2.8.0/tests/views/user/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:02:40.000000 core_main_app-2.8.0/tests/views/user/views/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9833 2024-03-12 19:02:40.000000 core_main_app-2.8.0/tests/views/user/views/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:51.409334 core_main_app-2.9.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2024-05-13 16:51:59.000000 core_main_app-2.9.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      219 2024-05-13 16:51:59.000000 core_main_app-2.9.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9924 2024-05-13 16:52:51.403128 core_main_app-2.9.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7529 2024-05-13 16:51:59.000000 core_main_app-2.9.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:31.373394 core_main_app-2.9.0/core_main_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       81 2024-05-13 16:51:59.000000 core_main_app-2.9.0/core_main_app/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:31.591218 core_main_app-2.9.0/core_main_app/access_control/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:51:59.000000 core_main_app-2.9.0/core_main_app/access_control/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11259 2024-05-13 16:51:59.000000 core_main_app-2.9.0/core_main_app/access_control/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      628 2024-05-13 16:51:59.000000 core_main_app-2.9.0/core_main_app/access_control/decorators.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      197 2024-05-13 16:51:59.000000 core_main_app-2.9.0/core_main_app/access_control/exceptions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1825 2024-05-13 16:51:59.000000 core_main_app-2.9.0/core_main_app/access_control/utils.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7058 2024-05-13 16:51:59.000000 core_main_app-2.9.0/core_main_app/admin.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1485 2024-05-13 16:51:59.000000 core_main_app-2.9.0/core_main_app/apps.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:31.735460 core_main_app-2.9.0/core_main_app/commons/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:51:59.000000 core_main_app-2.9.0/core_main_app/commons/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      919 2024-05-13 16:51:59.000000 core_main_app-2.9.0/core_main_app/commons/constants.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       62 2024-05-13 16:51:59.000000 core_main_app-2.9.0/core_main_app/commons/enums.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4743 2024-05-13 16:51:59.000000 core_main_app-2.9.0/core_main_app/commons/exceptions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       82 2024-05-13 16:51:59.000000 core_main_app-2.9.0/core_main_app/commons/regex.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      332 2024-05-13 16:51:59.000000 core_main_app-2.9.0/core_main_app/commons/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9144 2024-05-13 16:51:59.000000 core_main_app-2.9.0/core_main_app/commons/validators.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:31.758198 core_main_app-2.9.0/core_main_app/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:51:59.000000 core_main_app-2.9.0/core_main_app/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:31.803645 core_main_app-2.9.0/core_main_app/components/abstract_data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:51:59.000000 core_main_app-2.9.0/core_main_app/components/abstract_data/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4731 2024-05-13 16:51:59.000000 core_main_app-2.9.0/core_main_app/components/abstract_data/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:31.936585 core_main_app-2.9.0/core_main_app/components/blob/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:51:59.000000 core_main_app-2.9.0/core_main_app/components/blob/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2923 2024-05-13 16:51:59.000000 core_main_app-2.9.0/core_main_app/components/blob/access_control.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      315 2024-05-13 16:51:59.000000 core_main_app-2.9.0/core_main_app/components/blob/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3676 2024-05-13 16:51:59.000000 core_main_app-2.9.0/core_main_app/components/blob/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4077 2024-05-13 16:51:59.000000 core_main_app-2.9.0/core_main_app/components/blob/models.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      442 2024-05-13 16:51:59.000000 core_main_app-2.9.0/core_main_app/components/blob/utils.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:32.078504 core_main_app-2.9.0/core_main_app/components/data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:51:59.000000 core_main_app-2.9.0/core_main_app/components/data/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4687 2024-05-13 16:51:59.000000 core_main_app-2.9.0/core_main_app/components/data/access_control.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5583 2024-05-13 16:51:59.000000 core_main_app-2.9.0/core_main_app/components/data/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9946 2024-05-13 16:51:59.000000 core_main_app-2.9.0/core_main_app/components/data/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8346 2024-05-13 16:51:59.000000 core_main_app-2.9.0/core_main_app/components/data/models.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11291 2024-05-13 16:51:59.000000 core_main_app-2.9.0/core_main_app/components/data/tasks.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:32.126652 core_main_app-2.9.0/core_main_app/components/group/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:51:59.000000 core_main_app-2.9.0/core_main_app/components/group/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1982 2024-05-13 16:51:59.000000 core_main_app-2.9.0/core_main_app/components/group/api.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:32.213508 core_main_app-2.9.0/core_main_app/components/lock/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:51:59.000000 core_main_app-2.9.0/core_main_app/components/lock/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      330 2024-05-13 16:52:00.000000 core_main_app-2.9.0/core_main_app/components/lock/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2570 2024-05-13 16:52:00.000000 core_main_app-2.9.0/core_main_app/components/lock/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2665 2024-05-13 16:52:00.000000 core_main_app-2.9.0/core_main_app/components/lock/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:32.313517 core_main_app-2.9.0/core_main_app/components/mongo/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:00.000000 core_main_app-2.9.0/core_main_app/components/mongo/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1041 2024-05-13 16:52:00.000000 core_main_app-2.9.0/core_main_app/components/mongo/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11665 2024-05-13 16:52:00.000000 core_main_app-2.9.0/core_main_app/components/mongo/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:32.439381 core_main_app-2.9.0/core_main_app/components/template/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:00.000000 core_main_app-2.9.0/core_main_app/components/template/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4599 2024-05-13 16:52:00.000000 core_main_app-2.9.0/core_main_app/components/template/access_control.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      362 2024-05-13 16:52:00.000000 core_main_app-2.9.0/core_main_app/components/template/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5561 2024-05-13 16:52:00.000000 core_main_app-2.9.0/core_main_app/components/template/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8014 2024-05-13 16:52:00.000000 core_main_app-2.9.0/core_main_app/components/template/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:32.548138 core_main_app-2.9.0/core_main_app/components/template_version_manager/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:00.000000 core_main_app-2.9.0/core_main_app/components/template_version_manager/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2690 2024-05-13 16:52:00.000000 core_main_app-2.9.0/core_main_app/components/template_version_manager/access_control.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      507 2024-05-13 16:52:00.000000 core_main_app-2.9.0/core_main_app/components/template_version_manager/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8166 2024-05-13 16:52:00.000000 core_main_app-2.9.0/core_main_app/components/template_version_manager/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4720 2024-05-13 16:52:00.000000 core_main_app-2.9.0/core_main_app/components/template_version_manager/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:32.645588 core_main_app-2.9.0/core_main_app/components/template_xsl_rendering/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:00.000000 core_main_app-2.9.0/core_main_app/components/template_xsl_rendering/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      338 2024-05-13 16:52:00.000000 core_main_app-2.9.0/core_main_app/components/template_xsl_rendering/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6722 2024-05-13 16:52:00.000000 core_main_app-2.9.0/core_main_app/components/template_xsl_rendering/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3435 2024-05-13 16:52:00.000000 core_main_app-2.9.0/core_main_app/components/template_xsl_rendering/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:32.694415 core_main_app-2.9.0/core_main_app/components/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:00.000000 core_main_app-2.9.0/core_main_app/components/user/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2470 2024-05-13 16:52:00.000000 core_main_app-2.9.0/core_main_app/components/user/api.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:32.802526 core_main_app-2.9.0/core_main_app/components/user_preferences/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:00.000000 core_main_app-2.9.0/core_main_app/components/user_preferences/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1835 2024-05-13 16:52:00.000000 core_main_app-2.9.0/core_main_app/components/user_preferences/access_control.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      486 2024-05-13 16:52:00.000000 core_main_app-2.9.0/core_main_app/components/user_preferences/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1000 2024-05-13 16:52:00.000000 core_main_app-2.9.0/core_main_app/components/user_preferences/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1392 2024-05-13 16:52:00.000000 core_main_app-2.9.0/core_main_app/components/user_preferences/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:32.899113 core_main_app-2.9.0/core_main_app/components/version_manager/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:00.000000 core_main_app-2.9.0/core_main_app/components/version_manager/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4884 2024-05-13 16:52:00.000000 core_main_app-2.9.0/core_main_app/components/version_manager/access_control.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3744 2024-05-13 16:52:00.000000 core_main_app-2.9.0/core_main_app/components/version_manager/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3248 2024-05-13 16:52:00.000000 core_main_app-2.9.0/core_main_app/components/version_manager/models.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      550 2024-05-13 16:52:00.000000 core_main_app-2.9.0/core_main_app/components/version_manager/utils.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:32.961436 core_main_app-2.9.0/core_main_app/components/web_page/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:00.000000 core_main_app-2.9.0/core_main_app/components/web_page/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1280 2024-05-13 16:52:00.000000 core_main_app-2.9.0/core_main_app/components/web_page/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1097 2024-05-13 16:52:00.000000 core_main_app-2.9.0/core_main_app/components/web_page/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:33.007817 core_main_app-2.9.0/core_main_app/components/web_page_login/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:00.000000 core_main_app-2.9.0/core_main_app/components/web_page_login/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      809 2024-05-13 16:52:00.000000 core_main_app-2.9.0/core_main_app/components/web_page_login/api.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:33.110134 core_main_app-2.9.0/core_main_app/components/workspace/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:00.000000 core_main_app-2.9.0/core_main_app/components/workspace/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2493 2024-05-13 16:52:00.000000 core_main_app-2.9.0/core_main_app/components/workspace/access_control.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      372 2024-05-13 16:52:00.000000 core_main_app-2.9.0/core_main_app/components/workspace/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    16858 2024-05-13 16:52:00.000000 core_main_app-2.9.0/core_main_app/components/workspace/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5695 2024-05-13 16:52:00.000000 core_main_app-2.9.0/core_main_app/components/workspace/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:33.199961 core_main_app-2.9.0/core_main_app/components/xsl_transformation/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:00.000000 core_main_app-2.9.0/core_main_app/components/xsl_transformation/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      366 2024-05-13 16:52:00.000000 core_main_app-2.9.0/core_main_app/components/xsl_transformation/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2396 2024-05-13 16:52:00.000000 core_main_app-2.9.0/core_main_app/components/xsl_transformation/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4469 2024-05-13 16:52:00.000000 core_main_app-2.9.0/core_main_app/components/xsl_transformation/models.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1791 2024-05-13 16:52:00.000000 core_main_app-2.9.0/core_main_app/menus.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:33.264836 core_main_app-2.9.0/core_main_app/middleware/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:00.000000 core_main_app-2.9.0/core_main_app/middleware/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1378 2024-05-13 16:52:00.000000 core_main_app-2.9.0/core_main_app/middleware/timezone.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:33.452468 core_main_app-2.9.0/core_main_app/migrations/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    16483 2024-05-13 16:52:00.000000 core_main_app-2.9.0/core_main_app/migrations/0001_initial.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      751 2024-05-13 16:52:00.000000 core_main_app-2.9.0/core_main_app/migrations/0002_site_update.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1880 2024-05-13 16:52:00.000000 core_main_app-2.9.0/core_main_app/migrations/0003_psql_full_text.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      823 2024-05-13 16:52:00.000000 core_main_app-2.9.0/core_main_app/migrations/0004_template_ordering.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      474 2024-05-13 16:52:00.000000 core_main_app-2.9.0/core_main_app/migrations/0005_template_dependencies.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      655 2024-05-13 16:52:00.000000 core_main_app-2.9.0/core_main_app/migrations/0006_blob_metadata.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1372 2024-05-13 16:52:00.000000 core_main_app-2.9.0/core_main_app/migrations/0007_user_preferences.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      440 2024-05-13 16:52:00.000000 core_main_app-2.9.0/core_main_app/migrations/0008_blob_ordering.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      828 2024-05-13 16:52:00.000000 core_main_app-2.9.0/core_main_app/migrations/0009_template_formats.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:00.000000 core_main_app-2.9.0/core_main_app/migrations/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      706 2024-05-13 16:52:00.000000 core_main_app-2.9.0/core_main_app/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:33.546245 core_main_app-2.9.0/core_main_app/permissions/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:00.000000 core_main_app-2.9.0/core_main_app/permissions/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6351 2024-05-13 16:52:00.000000 core_main_app-2.9.0/core_main_app/permissions/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3243 2024-05-13 16:52:00.000000 core_main_app-2.9.0/core_main_app/permissions/discover.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      644 2024-05-13 16:52:00.000000 core_main_app-2.9.0/core_main_app/permissions/rights.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      230 2024-05-13 16:52:00.000000 core_main_app-2.9.0/core_main_app/permissions/utils.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:33.608783 core_main_app-2.9.0/core_main_app/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:00.000000 core_main_app-2.9.0/core_main_app/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:33.680351 core_main_app-2.9.0/core_main_app/rest/blob/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:00.000000 core_main_app-2.9.0/core_main_app/rest/blob/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4932 2024-05-13 16:52:00.000000 core_main_app-2.9.0/core_main_app/rest/blob/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    19770 2024-05-13 16:52:00.000000 core_main_app-2.9.0/core_main_app/rest/blob/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:33.779943 core_main_app-2.9.0/core_main_app/rest/data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:00.000000 core_main_app-2.9.0/core_main_app/rest/data/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8239 2024-05-13 16:52:00.000000 core_main_app-2.9.0/core_main_app/rest/data/abstract_views.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2261 2024-05-13 16:52:00.000000 core_main_app-2.9.0/core_main_app/rest/data/admin_serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4201 2024-05-13 16:52:01.000000 core_main_app-2.9.0/core_main_app/rest/data/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    38308 2024-05-13 16:52:01.000000 core_main_app-2.9.0/core_main_app/rest/data/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:33.827301 core_main_app-2.9.0/core_main_app/rest/group/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:01.000000 core_main_app-2.9.0/core_main_app/rest/group/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      293 2024-05-13 16:52:01.000000 core_main_app-2.9.0/core_main_app/rest/group/serializers.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:33.874101 core_main_app-2.9.0/core_main_app/rest/mongo_data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:01.000000 core_main_app-2.9.0/core_main_app/rest/mongo_data/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1989 2024-05-13 16:52:01.000000 core_main_app-2.9.0/core_main_app/rest/mongo_data/serializers.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:33.950385 core_main_app-2.9.0/core_main_app/rest/template/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:01.000000 core_main_app-2.9.0/core_main_app/rest/template/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      907 2024-05-13 16:52:01.000000 core_main_app-2.9.0/core_main_app/rest/template/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5344 2024-05-13 16:52:01.000000 core_main_app-2.9.0/core_main_app/rest/template/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:34.056683 core_main_app-2.9.0/core_main_app/rest/template_version_manager/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:01.000000 core_main_app-2.9.0/core_main_app/rest/template_version_manager/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    13930 2024-05-13 16:52:01.000000 core_main_app-2.9.0/core_main_app/rest/template_version_manager/abstract_views.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2858 2024-05-13 16:52:01.000000 core_main_app-2.9.0/core_main_app/rest/template_version_manager/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      587 2024-05-13 16:52:01.000000 core_main_app-2.9.0/core_main_app/rest/template_version_manager/utils.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    12279 2024-05-13 16:52:01.000000 core_main_app-2.9.0/core_main_app/rest/template_version_manager/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:34.138637 core_main_app-2.9.0/core_main_app/rest/template_xsl_rendering/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:01.000000 core_main_app-2.9.0/core_main_app/rest/template_xsl_rendering/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1117 2024-05-13 16:52:01.000000 core_main_app-2.9.0/core_main_app/rest/template_xsl_rendering/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14418 2024-05-13 16:52:01.000000 core_main_app-2.9.0/core_main_app/rest/template_xsl_rendering/views.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14537 2024-05-13 16:52:01.000000 core_main_app-2.9.0/core_main_app/rest/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:34.208108 core_main_app-2.9.0/core_main_app/rest/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:01.000000 core_main_app-2.9.0/core_main_app/rest/user/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1157 2024-05-13 16:52:01.000000 core_main_app-2.9.0/core_main_app/rest/user/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      709 2024-05-13 16:52:01.000000 core_main_app-2.9.0/core_main_app/rest/user/views.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2468 2024-05-13 16:52:01.000000 core_main_app-2.9.0/core_main_app/rest/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:34.286293 core_main_app-2.9.0/core_main_app/rest/web_page/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:01.000000 core_main_app-2.9.0/core_main_app/rest/web_page/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1042 2024-05-13 16:52:01.000000 core_main_app-2.9.0/core_main_app/rest/web_page/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4688 2024-05-13 16:52:01.000000 core_main_app-2.9.0/core_main_app/rest/web_page/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:34.638059 core_main_app-2.9.0/core_main_app/rest/workspace/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:01.000000 core_main_app-2.9.0/core_main_app/rest/workspace/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      894 2024-05-13 16:52:01.000000 core_main_app-2.9.0/core_main_app/rest/workspace/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    23314 2024-05-13 16:52:01.000000 core_main_app-2.9.0/core_main_app/rest/workspace/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:34.705621 core_main_app-2.9.0/core_main_app/rest/xsl_transformation/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:01.000000 core_main_app-2.9.0/core_main_app/rest/xsl_transformation/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1437 2024-05-13 16:52:01.000000 core_main_app-2.9.0/core_main_app/rest/xsl_transformation/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8160 2024-05-13 16:52:01.000000 core_main_app-2.9.0/core_main_app/rest/xsl_transformation/views.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9027 2024-05-13 16:52:01.000000 core_main_app-2.9.0/core_main_app/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:29.571121 core_main_app-2.9.0/core_main_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:29.788671 core_main_app-2.9.0/core_main_app/static/core_main_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:29.610721 core_main_app-2.9.0/core_main_app/static/core_main_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:29.588506 core_main_app-2.9.0/core_main_app/static/core_main_app/admin/_theme/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:34.779028 core_main_app-2.9.0/core_main_app/static/core_main_app/admin/_theme/css/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      251 2024-05-13 16:52:01.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/admin/_theme/css/additional.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    47539 2024-05-13 16:52:01.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/admin/_theme/css/skins.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)   110978 2024-05-13 16:52:01.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/admin/_theme/css/theme.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:34.822786 core_main_app-2.9.0/core_main_app/static/core_main_app/admin/_theme/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    22937 2024-05-13 16:52:01.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/admin/_theme/js/app.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      578 2024-05-13 16:52:01.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/admin/_theme/js/menu.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:34.859280 core_main_app-2.9.0/core_main_app/static/core_main_app/admin/css/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1575 2024-05-13 16:52:01.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/admin/css/data_migration.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       81 2024-05-13 16:52:01.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/admin/css/permissions.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:34.880230 core_main_app-2.9.0/core_main_app/static/core_main_app/admin/css/templates_xslt/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1363 2024-05-13 16:52:01.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/admin/css/templates_xslt/form.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:34.902101 core_main_app-2.9.0/core_main_app/static/core_main_app/admin/css/web_page/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       31 2024-05-13 16:52:01.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/admin/css/web_page/style.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:34.924221 core_main_app-2.9.0/core_main_app/static/core_main_app/admin/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1232 2024-05-13 16:52:01.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/admin/js/display_permissions.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:34.964291 core_main_app-2.9.0/core_main_app/static/core_main_app/admin/js/templates/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    30064 2024-05-13 16:52:01.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/admin/js/templates/data_migration.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      594 2024-05-13 16:52:01.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/admin/js/templates/data_migration.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:35.024913 core_main_app-2.9.0/core_main_app/static/core_main_app/admin/js/templates/upload/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1334 2024-05-13 16:52:01.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/admin/js/templates/upload/dependencies.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       94 2024-05-13 16:52:01.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/admin/js/templates/upload/dependencies.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      139 2024-05-13 16:52:01.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/admin/js/templates/upload/dependency_resolver.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:35.046795 core_main_app-2.9.0/core_main_app/static/core_main_app/admin/js/templates_xslt/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1395 2024-05-13 16:52:01.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/admin/js/templates_xslt/detail_xslt.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:29.740755 core_main_app-2.9.0/core_main_app/static/core_main_app/common/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:35.315970 core_main_app-2.9.0/core_main_app/static/core_main_app/common/css/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2236 2024-05-13 16:52:01.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/common/css/XMLTree.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      121 2024-05-13 16:52:01.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/common/css/bootstrap5.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       68 2024-05-13 16:52:01.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/common/css/buttons.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      180 2024-05-13 16:52:01.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/common/css/detail.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      177 2024-05-13 16:52:01.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/common/css/fields.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      132 2024-05-13 16:52:01.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/common/css/highlight.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       92 2024-05-13 16:52:01.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/common/css/loading-spinner.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1332 2024-05-13 16:52:01.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/common/css/messages.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:35.339331 core_main_app-2.9.0/core_main_app/static/core_main_app/common/css/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      102 2024-05-13 16:52:01.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/common/css/modals/download.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      317 2024-05-13 16:52:01.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/common/css/select.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      392 2024-05-13 16:52:01.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/common/css/share_link.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      940 2024-05-13 16:52:01.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/common/css/switch.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      486 2024-05-13 16:52:01.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/common/css/table.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:35.362725 core_main_app-2.9.0/core_main_app/static/core_main_app/common/css/template/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       59 2024-05-13 16:52:01.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/common/css/template/template_ordering.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      189 2024-05-13 16:52:01.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/common/css/word-wrap.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:35.386582 core_main_app-2.9.0/core_main_app/static/core_main_app/common/css/workspace/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      333 2024-05-13 16:52:01.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/common/css/workspace/table.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:35.427098 core_main_app-2.9.0/core_main_app/static/core_main_app/common/img/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      246 2024-05-13 16:52:01.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/common/img/collapse.png
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      253 2024-05-13 16:52:01.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/common/img/expand.png
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:35.638331 core_main_app-2.9.0/core_main_app/static/core_main_app/common/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      335 2024-05-13 16:52:01.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/common/js/XMLTree.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      247 2024-05-13 16:52:01.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/common/js/backtoprevious.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1828 2024-05-13 16:52:01.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/common/js/csrf.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      192 2024-05-13 16:52:01.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/common/js/data_detail.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      531 2024-05-13 16:52:02.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/common/js/debounce.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      787 2024-05-13 16:52:02.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/common/js/elementViewport.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      413 2024-05-13 16:52:02.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/common/js/leave_notice.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      966 2024-05-13 16:52:02.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/common/js/loading_spinner.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2274 2024-05-13 16:52:02.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/common/js/messages.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:35.758669 core_main_app-2.9.0/core_main_app/static/core_main_app/common/js/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1292 2024-05-13 16:52:02.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/common/js/modals/add.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1136 2024-05-13 16:52:02.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/common/js/modals/delete.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      491 2024-05-13 16:52:02.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/common/js/modals/download.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      188 2024-05-13 16:52:02.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/common/js/modals/download.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1257 2024-05-13 16:52:02.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/common/js/modals/edit.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      439 2024-05-13 16:52:02.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/common/js/modals/error_page_modal.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:35.799923 core_main_app-2.9.0/core_main_app/static/core_main_app/common/js/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:35.850377 core_main_app-2.9.0/core_main_app/static/core_main_app/common/js/templates/list/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:35.900128 core_main_app-2.9.0/core_main_app/static/core_main_app/common/js/templates/list/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1086 2024-05-13 16:52:02.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/common/js/templates/list/modals/disable.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      125 2024-05-13 16:52:02.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/common/js/templates/list/modals/disable.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      663 2024-05-13 16:52:02.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/common/js/templates/list/restore.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      124 2024-05-13 16:52:02.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/common/js/templates/list/restore.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1495 2024-05-13 16:52:02.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/common/js/templates/sort.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      217 2024-05-13 16:52:02.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/common/js/templates/sort.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:35.974169 core_main_app-2.9.0/core_main_app/static/core_main_app/common/js/templates/versions/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:36.031753 core_main_app-2.9.0/core_main_app/static/core_main_app/common/js/templates/versions/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1029 2024-05-13 16:52:02.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/common/js/templates/versions/modals/disable.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      108 2024-05-13 16:52:02.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/common/js/templates/versions/modals/disable.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      537 2024-05-13 16:52:02.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/common/js/templates/versions/restore.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      107 2024-05-13 16:52:02.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/common/js/templates/versions/restore.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      662 2024-05-13 16:52:02.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/common/js/templates/versions/set_current.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      111 2024-05-13 16:52:02.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/common/js/templates/versions/set_current.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      189 2024-05-13 16:52:02.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/common/js/tooltip.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:29.731313 core_main_app-2.9.0/core_main_app/static/core_main_app/common/js/xslt/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:29.735330 core_main_app-2.9.0/core_main_app/static/core_main_app/common/js/xslt/list/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:36.123122 core_main_app-2.9.0/core_main_app/static/core_main_app/common/js/xslt/list/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      859 2024-05-13 16:52:02.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/common/js/xslt/list/modals/delete.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       64 2024-05-13 16:52:02.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/common/js/xslt/list/modals/delete.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1012 2024-05-13 16:52:02.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/common/js/xslt/list/modals/edit.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       60 2024-05-13 16:52:02.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/common/js/xslt/list/modals/edit.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:36.145300 core_main_app-2.9.0/core_main_app/static/core_main_app/common/xsl/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1763 2024-05-13 16:52:02.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/common/xsl/xml2html.xsl
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:29.771894 core_main_app-2.9.0/core_main_app/static/core_main_app/libs/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:29.775842 core_main_app-2.9.0/core_main_app/static/core_main_app/libs/jquery-ui/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:36.242908 core_main_app-2.9.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:36.377446 core_main_app-2.9.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7006 2024-05-13 16:52:02.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_444444_256x240.png
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7074 2024-05-13 16:52:02.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_555555_256x240.png
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4676 2024-05-13 16:52:02.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_777620_256x240.png
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7013 2024-05-13 16:52:02.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_777777_256x240.png
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4632 2024-05-13 16:52:02.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_cc0000_256x240.png
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6313 2024-05-13 16:52:02.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_ffffff_256x240.png
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    37326 2024-05-13 16:52:02.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/jquery-ui.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)   520714 2024-05-13 16:52:02.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/jquery-ui.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    18705 2024-05-13 16:52:02.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/jquery-ui.structure.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    18671 2024-05-13 16:52:02.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/jquery-ui.theme.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:29.797971 core_main_app-2.9.0/core_main_app/static/core_main_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:36.444566 core_main_app-2.9.0/core_main_app/static/core_main_app/user/css/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       32 2024-05-13 16:52:02.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/user/css/login.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       63 2024-05-13 16:52:02.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/user/css/registration.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      576 2024-05-13 16:52:02.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/user/css/text-editor.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:36.466914 core_main_app-2.9.0/core_main_app/static/core_main_app/user/js/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:36.527237 core_main_app-2.9.0/core_main_app/static/core_main_app/user/js/blob/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1505 2024-05-13 16:52:02.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/user/js/blob/blob_metadata.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      217 2024-05-13 16:52:02.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/user/js/blob/blob_metadata.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      119 2024-05-13 16:52:02.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/user/js/blob/detail.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:36.623181 core_main_app-2.9.0/core_main_app/static/core_main_app/user/js/data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      618 2024-05-13 16:52:02.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/user/js/data/change_display.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      120 2024-05-13 16:52:02.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/user/js/data/change_display.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      158 2024-05-13 16:52:02.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/user/js/data/detail.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:36.664871 core_main_app-2.9.0/core_main_app/static/core_main_app/user/js/login/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      768 2024-05-13 16:52:02.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/user/js/login/message.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       52 2024-05-13 16:52:02.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/user/js/login/message.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1302 2024-05-13 16:52:02.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/user/js/sharing_modal.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:36.741544 core_main_app-2.9.0/core_main_app/static/core_main_app/user/js/text_editor/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      234 2024-05-13 16:52:02.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/user/js/text_editor/data_text_editor.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      120 2024-05-13 16:52:02.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/user/js/text_editor/monaco-editor-loader.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       73 2024-05-13 16:52:02.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/user/js/text_editor/template_text_editor.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10351 2024-05-13 16:52:02.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/user/js/text_editor/text_editor.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:36.894989 core_main_app-2.9.0/core_main_app/static/core_main_app/user/js/workspaces/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1800 2024-05-13 16:52:02.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/user/js/workspaces/add_group.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      160 2024-05-13 16:52:02.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/user/js/workspaces/add_group.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1723 2024-05-13 16:52:02.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/user/js/workspaces/add_user.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      156 2024-05-13 16:52:02.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/user/js/workspaces/add_user.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1138 2024-05-13 16:52:02.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/user/js/workspaces/create_workspace.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       73 2024-05-13 16:52:02.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/user/js/workspaces/create_workspace.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      515 2024-05-13 16:52:02.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/user/js/workspaces/init.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       43 2024-05-13 16:52:02.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/user/js/workspaces/init.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:29.842079 core_main_app-2.9.0/core_main_app/static/core_main_app/user/js/workspaces/list/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:37.106711 core_main_app-2.9.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      187 2024-05-13 16:52:02.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/assign_blob_workspace.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      187 2024-05-13 16:52:02.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/assign_data_workspace.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1587 2024-05-13 16:52:02.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/assign_workspace.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1360 2024-05-13 16:52:02.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/remove_rights.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       60 2024-05-13 16:52:02.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/remove_rights.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      807 2024-05-13 16:52:02.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/set_private.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       96 2024-05-13 16:52:02.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/set_private.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      822 2024-05-13 16:52:02.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/set_public.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       94 2024-05-13 16:52:03.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/set_public.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1728 2024-05-13 16:52:03.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/switch_right.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      144 2024-05-13 16:52:03.000000 core_main_app-2.9.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/switch_right.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:37.151129 core_main_app-2.9.0/core_main_app/system/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:03.000000 core_main_app-2.9.0/core_main_app/system/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2767 2024-05-13 16:52:03.000000 core_main_app-2.9.0/core_main_app/system/api.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:37.197280 core_main_app-2.9.0/core_main_app/system/blob/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:03.000000 core_main_app-2.9.0/core_main_app/system/blob/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      233 2024-05-13 16:52:03.000000 core_main_app-2.9.0/core_main_app/system/blob/api.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:37.223149 core_main_app-2.9.0/core_main_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:30.213287 core_main_app-2.9.0/core_main_app/templates/core_main_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:29.914543 core_main_app-2.9.0/core_main_app/templates/core_main_app/_render/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:37.251669 core_main_app-2.9.0/core_main_app/templates/core_main_app/_render/admin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1302 2024-05-13 16:52:03.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/_render/admin/app_wrapper.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:37.329914 core_main_app-2.9.0/core_main_app/templates/core_main_app/_render/admin/theme/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2405 2024-05-13 16:52:03.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/_render/admin/theme/base.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      324 2024-05-13 16:52:03.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/_render/admin/theme/footer.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1110 2024-05-13 16:52:03.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/_render/admin/theme/header.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3513 2024-05-13 16:52:03.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/_render/admin/theme/menu.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:37.412021 core_main_app-2.9.0/core_main_app/templates/core_main_app/_render/admin/theme/tools/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      726 2024-05-13 16:52:03.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/_render/admin/theme/tools/box.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:03.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/_render/admin/theme/tools/form.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1034 2024-05-13 16:52:03.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/_render/admin/theme/tools/modal.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      283 2024-05-13 16:52:03.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/_render/admin/theme/tools/section.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:37.488885 core_main_app-2.9.0/core_main_app/templates/core_main_app/_render/common/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2352 2024-05-13 16:52:03.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/_render/common/base_css.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1558 2024-05-13 16:52:03.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/_render/common/base_js.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1675 2024-05-13 16:52:03.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/_render/common/messages.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:37.545637 core_main_app-2.9.0/core_main_app/templates/core_main_app/_render/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1974 2024-05-13 16:52:03.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/_render/user/app_wrapper.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      902 2024-05-13 16:52:03.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/_render/user/default.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1867 2024-05-13 16:52:03.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/_render/user/theme_base.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:37.636547 core_main_app-2.9.0/core_main_app/templates/core_main_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:37.708145 core_main_app-2.9.0/core_main_app/templates/core_main_app/admin/blob/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      312 2024-05-13 16:52:03.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/admin/blob/detail.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      359 2024-05-13 16:52:03.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/admin/blob/detail_box.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      323 2024-05-13 16:52:03.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/admin/blob/detail_metadata.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      367 2024-05-13 16:52:03.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/admin/blob/detail_metadata_box.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:29.943970 core_main_app-2.9.0/core_main_app/templates/core_main_app/admin/commons/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:37.746091 core_main_app-2.9.0/core_main_app/templates/core_main_app/admin/commons/errors/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      401 2024-05-13 16:52:03.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/admin/commons/errors/errors.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      254 2024-05-13 16:52:03.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/admin/commons/errors/errors_wrapper.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:37.803000 core_main_app-2.9.0/core_main_app/templates/core_main_app/admin/commons/upload/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      795 2024-05-13 16:52:03.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/admin/commons/upload/form.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      313 2024-05-13 16:52:03.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/admin/commons/upload/upload.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      103 2024-05-13 16:52:03.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/admin/dashboard.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:37.839177 core_main_app-2.9.0/core_main_app/templates/core_main_app/admin/data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      311 2024-05-13 16:52:03.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/admin/data/detail.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      383 2024-05-13 16:52:03.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/admin/data/detail_box.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1598 2024-05-13 16:52:03.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/admin/dependency_resolver.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      211 2024-05-13 16:52:03.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/admin/list_dependencies.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:37.920090 core_main_app-2.9.0/core_main_app/templates/core_main_app/admin/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:37.943253 core_main_app-2.9.0/core_main_app/templates/core_main_app/admin/templates/data_migration/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8123 2024-05-13 16:52:03.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/admin/templates/data_migration/templates_list.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      289 2024-05-13 16:52:03.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/admin/templates/data_migration.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:37.981780 core_main_app-2.9.0/core_main_app/templates/core_main_app/admin/templates/list/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2705 2024-05-13 16:52:03.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/admin/templates/list/available.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      830 2024-05-13 16:52:03.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/admin/templates/list/disabled.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:38.002580 core_main_app-2.9.0/core_main_app/templates/core_main_app/admin/templates/list/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      926 2024-05-13 16:52:03.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/admin/templates/list/modals/disable.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      542 2024-05-13 16:52:03.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/admin/templates/list.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:38.022678 core_main_app-2.9.0/core_main_app/templates/core_main_app/admin/templates/upload/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      399 2024-05-13 16:52:03.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/admin/templates/upload/base.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      166 2024-05-13 16:52:03.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/admin/templates/upload.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:38.056727 core_main_app-2.9.0/core_main_app/templates/core_main_app/admin/templates/versions/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3746 2024-05-13 16:52:03.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/admin/templates/versions/available.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1182 2024-05-13 16:52:03.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/admin/templates/versions/disabled.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:38.076729 core_main_app-2.9.0/core_main_app/templates/core_main_app/admin/templates/versions/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      840 2024-05-13 16:52:03.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/admin/templates/versions/modals/disable.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      677 2024-05-13 16:52:03.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/admin/templates/versions.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:38.094899 core_main_app-2.9.0/core_main_app/templates/core_main_app/admin/templates_xslt/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:38.114004 core_main_app-2.9.0/core_main_app/templates/core_main_app/admin/templates_xslt/main/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5044 2024-05-13 16:52:03.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/admin/templates_xslt/main/form.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      393 2024-05-13 16:52:03.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/admin/templates_xslt/main.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      860 2024-05-13 16:52:03.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/admin/upload_template.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:38.208847 core_main_app-2.9.0/core_main_app/templates/core_main_app/admin/web_page/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      166 2024-05-13 16:52:03.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/admin/web_page/login_page.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      905 2024-05-13 16:52:03.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/admin/web_page/main.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      387 2024-05-13 16:52:03.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/admin/web_page/web_page.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      375 2024-05-13 16:52:03.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/admin/web_page/web_page_unavailable.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:38.241541 core_main_app-2.9.0/core_main_app/templates/core_main_app/admin/workspaces/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      234 2024-05-13 16:52:03.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/admin/workspaces/edit_rights.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:38.290126 core_main_app-2.9.0/core_main_app/templates/core_main_app/admin/xslt/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:38.311421 core_main_app-2.9.0/core_main_app/templates/core_main_app/admin/xslt/list/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1337 2024-05-13 16:52:03.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/admin/xslt/list/table.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      323 2024-05-13 16:52:03.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/admin/xslt/list.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:38.333845 core_main_app-2.9.0/core_main_app/templates/core_main_app/admin/xslt/upload/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       61 2024-05-13 16:52:03.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/admin/xslt/upload/base.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      161 2024-05-13 16:52:03.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/admin/xslt/upload.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:30.187767 core_main_app-2.9.0/core_main_app/templates/core_main_app/common/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:38.416495 core_main_app-2.9.0/core_main_app/templates/core_main_app/common/blob/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      823 2024-05-13 16:52:03.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/common/blob/detail_blob.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2165 2024-05-13 16:52:03.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/common/blob/detail_metadata.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1321 2024-05-13 16:52:03.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/common/blob/tools_blob.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      682 2024-05-13 16:52:03.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/common/blob/tools_metadata.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:38.507813 core_main_app-2.9.0/core_main_app/templates/core_main_app/common/buttons/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      194 2024-05-13 16:52:04.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/common/buttons/add.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      253 2024-05-13 16:52:04.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/common/buttons/back_to_previous.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      194 2024-05-13 16:52:04.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/common/buttons/delete.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      190 2024-05-13 16:52:04.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/common/buttons/edit.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      104 2024-05-13 16:52:04.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/common/buttons/go_to.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:38.562217 core_main_app-2.9.0/core_main_app/templates/core_main_app/common/commons/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      189 2024-05-13 16:52:04.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/common/commons/error.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       97 2024-05-13 16:52:04.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/common/commons/form.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      167 2024-05-13 16:52:04.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/common/commons/form_delete.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:38.605439 core_main_app-2.9.0/core_main_app/templates/core_main_app/common/commons/upload/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      679 2024-05-13 16:52:04.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/common/commons/upload/form.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      313 2024-05-13 16:52:04.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/common/commons/upload/upload.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:38.645134 core_main_app-2.9.0/core_main_app/templates/core_main_app/common/data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      759 2024-05-13 16:52:04.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/common/data/detail_data.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2486 2024-05-13 16:52:04.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/common/data/tools_data.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:38.666751 core_main_app-2.9.0/core_main_app/templates/core_main_app/common/defender/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       90 2024-05-13 16:52:04.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/common/defender/error.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:38.926898 core_main_app-2.9.0/core_main_app/templates/core_main_app/common/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      576 2024-05-13 16:52:04.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/common/modals/add_page_modal.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      750 2024-05-13 16:52:04.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/common/modals/create_data_modal.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      601 2024-05-13 16:52:04.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/common/modals/delete_page_modal.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1197 2024-05-13 16:52:04.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/common/modals/download-options.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      580 2024-05-13 16:52:04.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/common/modals/edit_page_modal.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      429 2024-05-13 16:52:04.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/common/modals/error_page_modal.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:38.949010 core_main_app-2.9.0/core_main_app/templates/core_main_app/common/pagination/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3008 2024-05-13 16:52:04.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/common/pagination/data_source_pagination.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:38.974235 core_main_app-2.9.0/core_main_app/templates/core_main_app/common/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:39.028579 core_main_app-2.9.0/core_main_app/templates/core_main_app/common/templates/list/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1625 2024-05-13 16:52:04.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/common/templates/list/available.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      801 2024-05-13 16:52:04.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/common/templates/list/disabled.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:39.065228 core_main_app-2.9.0/core_main_app/templates/core_main_app/common/templates/list/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      918 2024-05-13 16:52:04.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/common/templates/list/modals/disable.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      854 2024-05-13 16:52:04.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/common/templates/list/modals/edit.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:39.084097 core_main_app-2.9.0/core_main_app/templates/core_main_app/common/templates/versions/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2367 2024-05-13 16:52:04.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/common/templates/versions/available.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:39.104402 core_main_app-2.9.0/core_main_app/templates/core_main_app/common/templates/versions/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      775 2024-05-13 16:52:04.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/common/templates/versions/modals/disable.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      265 2024-05-13 16:52:04.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/common/templates/versions.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:39.124916 core_main_app-2.9.0/core_main_app/templates/core_main_app/common/templates_xslt/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:39.162197 core_main_app-2.9.0/core_main_app/templates/core_main_app/common/templates_xslt/main/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1263 2024-05-13 16:52:04.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/common/templates_xslt/main/form.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      428 2024-05-13 16:52:04.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/common/templates_xslt/main.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:39.201626 core_main_app-2.9.0/core_main_app/templates/core_main_app/common/xslt/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:39.225093 core_main_app-2.9.0/core_main_app/templates/core_main_app/common/xslt/list/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:39.277129 core_main_app-2.9.0/core_main_app/templates/core_main_app/common/xslt/list/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      677 2024-05-13 16:52:04.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/common/xslt/list/modals/delete.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1234 2024-05-13 16:52:04.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/common/xslt/list/modals/edit.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1248 2024-05-13 16:52:04.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/common/xslt/list/table.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      255 2024-05-13 16:52:04.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/common/xslt/list.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:39.298394 core_main_app-2.9.0/core_main_app/templates/core_main_app/common/xslt/upload/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       62 2024-05-13 16:52:04.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/common/xslt/upload/base.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      163 2024-05-13 16:52:04.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/common/xslt/upload.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:39.336483 core_main_app-2.9.0/core_main_app/templates/core_main_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:39.376772 core_main_app-2.9.0/core_main_app/templates/core_main_app/user/blob/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      295 2024-05-13 16:52:04.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/user/blob/detail.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      338 2024-05-13 16:52:04.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/user/blob/detail_metadata.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:30.232434 core_main_app-2.9.0/core_main_app/templates/core_main_app/user/blob/list/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:39.540260 core_main_app-2.9.0/core_main_app/templates/core_main_app/user/blob/list/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      689 2024-05-13 16:52:04.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/user/blob/list/modals/add_metadata.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      231 2024-05-13 16:52:04.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/user/blob/list/modals/add_metadata_form.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      686 2024-05-13 16:52:04.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/user/blob/list/modals/file_upload.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      148 2024-05-13 16:52:04.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/user/blob/list/modals/file_upload_form.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:39.562301 core_main_app-2.9.0/core_main_app/templates/core_main_app/user/data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      483 2024-05-13 16:52:04.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/user/data/detail.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      139 2024-05-13 16:52:04.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/user/homepage.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:39.605210 core_main_app-2.9.0/core_main_app/templates/core_main_app/user/login/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2408 2024-05-13 16:52:04.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/user/login/main.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:39.629391 core_main_app-2.9.0/core_main_app/templates/core_main_app/user/login/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      534 2024-05-13 16:52:04.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/user/login/modals/login_message.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      340 2024-05-13 16:52:04.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/user/login/saml2_error.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:39.802671 core_main_app-2.9.0/core_main_app/templates/core_main_app/user/registration/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      171 2024-05-13 16:52:04.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/user/registration/password_reset_complete.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      491 2024-05-13 16:52:04.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/user/registration/password_reset_confirm.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      600 2024-05-13 16:52:04.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/user/registration/password_reset_done.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      362 2024-05-13 16:52:04.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/user/registration/password_reset_email.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      281 2024-05-13 16:52:04.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/user/registration/password_reset_form.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       14 2024-05-13 16:52:04.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/user/registration/password_reset_subject.txt
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:39.826220 core_main_app-2.9.0/core_main_app/templates/core_main_app/user/sharing/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      274 2024-05-13 16:52:04.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/user/sharing/button.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:39.909758 core_main_app-2.9.0/core_main_app/templates/core_main_app/user/sharing/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      504 2024-05-13 16:52:04.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/user/sharing/modals/multi-link.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1132 2024-05-13 16:52:04.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/user/sharing/modals/single-link.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:39.951756 core_main_app-2.9.0/core_main_app/templates/core_main_app/user/template/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      453 2024-05-13 16:52:04.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/user/template/list_body.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2024-05-13 16:52:04.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/user/template/list_header.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:39.981903 core_main_app-2.9.0/core_main_app/templates/core_main_app/user/text_editor/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4894 2024-05-13 16:52:04.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/user/text_editor/text_editor.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      757 2024-05-13 16:52:04.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/user/timezone.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:40.003956 core_main_app-2.9.0/core_main_app/templates/core_main_app/user/workspaces/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1186 2024-05-13 16:52:04.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/user/workspaces/edit_rights.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:40.046438 core_main_app-2.9.0/core_main_app/templates/core_main_app/user/workspaces/list/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1622 2024-05-13 16:52:04.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/user/workspaces/list/create_workspace.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1882 2024-05-13 16:52:04.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/user/workspaces/list/edit_rights_table.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:40.265659 core_main_app-2.9.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1747 2024-05-13 16:52:05.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/add_group.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      222 2024-05-13 16:52:05.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/add_group_form.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1725 2024-05-13 16:52:05.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/add_user.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      219 2024-05-13 16:52:05.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/add_user_form.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      945 2024-05-13 16:52:05.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/assign_workspace.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      411 2024-05-13 16:52:05.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/assign_workspace_form.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1264 2024-05-13 16:52:05.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/remove_rights.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1183 2024-05-13 16:52:05.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/set_private.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1191 2024-05-13 16:52:05.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/set_public.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      981 2024-05-13 16:52:05.000000 core_main_app-2.9.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/switch_right.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      147 2024-05-13 16:52:05.000000 core_main_app-2.9.0/core_main_app/templates/theme.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:40.509446 core_main_app-2.9.0/core_main_app/templatetags/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:05.000000 core_main_app-2.9.0/core_main_app/templatetags/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      686 2024-05-13 16:52:05.000000 core_main_app-2.9.0/core_main_app/templatetags/auth_extras.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1690 2024-05-13 16:52:05.000000 core_main_app-2.9.0/core_main_app/templatetags/blob_tags.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      367 2024-05-13 16:52:05.000000 core_main_app-2.9.0/core_main_app/templatetags/dict_key_extras.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      487 2024-05-13 16:52:05.000000 core_main_app-2.9.0/core_main_app/templatetags/format_json.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      514 2024-05-13 16:52:05.000000 core_main_app-2.9.0/core_main_app/templatetags/get_attribute.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      598 2024-05-13 16:52:05.000000 core_main_app-2.9.0/core_main_app/templatetags/include_static.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1124 2024-05-13 16:52:05.000000 core_main_app-2.9.0/core_main_app/templatetags/json_date.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      509 2024-05-13 16:52:05.000000 core_main_app-2.9.0/core_main_app/templatetags/parse_date.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      640 2024-05-13 16:52:05.000000 core_main_app-2.9.0/core_main_app/templatetags/stripjs.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      316 2024-05-13 16:52:05.000000 core_main_app-2.9.0/core_main_app/templatetags/timestamptags.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3319 2024-05-13 16:52:05.000000 core_main_app-2.9.0/core_main_app/templatetags/xsl_transform_tag.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4975 2024-05-13 16:52:05.000000 core_main_app-2.9.0/core_main_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:40.882019 core_main_app-2.9.0/core_main_app/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:05.000000 core_main_app-2.9.0/core_main_app/utils/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:40.970206 core_main_app-2.9.0/core_main_app/utils/admin_site/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:05.000000 core_main_app-2.9.0/core_main_app/utils/admin_site/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1233 2024-05-13 16:52:05.000000 core_main_app-2.9.0/core_main_app/utils/admin_site/model_admin_class.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      379 2024-05-13 16:52:05.000000 core_main_app-2.9.0/core_main_app/utils/admin_site/view_only_admin.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2447 2024-05-13 16:52:05.000000 core_main_app-2.9.0/core_main_app/utils/blob_downloader.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      405 2024-05-13 16:52:05.000000 core_main_app-2.9.0/core_main_app/utils/boolean.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1137 2024-05-13 16:52:05.000000 core_main_app-2.9.0/core_main_app/utils/checksum.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1966 2024-05-13 16:52:05.000000 core_main_app-2.9.0/core_main_app/utils/custom_context_processors.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:41.012838 core_main_app-2.9.0/core_main_app/utils/databases/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:05.000000 core_main_app-2.9.0/core_main_app/utils/databases/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      627 2024-05-13 16:52:05.000000 core_main_app-2.9.0/core_main_app/utils/databases/backend.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:41.056803 core_main_app-2.9.0/core_main_app/utils/databases/mongo/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      574 2024-05-13 16:52:05.000000 core_main_app-2.9.0/core_main_app/utils/databases/mongo/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      873 2024-05-13 16:52:05.000000 core_main_app-2.9.0/core_main_app/utils/databases/mongo/pymongo_database.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      286 2024-05-13 16:52:05.000000 core_main_app-2.9.0/core_main_app/utils/datetime.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9575 2024-05-13 16:52:05.000000 core_main_app-2.9.0/core_main_app/utils/decorators.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      449 2024-05-13 16:52:05.000000 core_main_app-2.9.0/core_main_app/utils/dict.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4473 2024-05-13 16:52:05.000000 core_main_app-2.9.0/core_main_app/utils/file.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      377 2024-05-13 16:52:05.000000 core_main_app-2.9.0/core_main_app/utils/group.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:41.170132 core_main_app-2.9.0/core_main_app/utils/integration_tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:05.000000 core_main_app-2.9.0/core_main_app/utils/integration_tests/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      262 2024-05-13 16:52:05.000000 core_main_app-2.9.0/core_main_app/utils/integration_tests/fixture_interface.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1651 2024-05-13 16:52:05.000000 core_main_app-2.9.0/core_main_app/utils/integration_tests/integration_base_test_case.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1031 2024-05-13 16:52:05.000000 core_main_app-2.9.0/core_main_app/utils/integration_tests/integration_base_transaction_test_case.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4219 2024-05-13 16:52:05.000000 core_main_app-2.9.0/core_main_app/utils/json_utils.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      318 2024-05-13 16:52:05.000000 core_main_app-2.9.0/core_main_app/utils/labels.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:41.219627 core_main_app-2.9.0/core_main_app/utils/logger/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:05.000000 core_main_app-2.9.0/core_main_app/utils/logger/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1762 2024-05-13 16:52:05.000000 core_main_app-2.9.0/core_main_app/utils/logger/logger_utils.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      438 2024-05-13 16:52:05.000000 core_main_app-2.9.0/core_main_app/utils/markdown_parser.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      956 2024-05-13 16:52:05.000000 core_main_app-2.9.0/core_main_app/utils/migrations.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:41.266796 core_main_app-2.9.0/core_main_app/utils/notifications/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:05.000000 core_main_app-2.9.0/core_main_app/utils/notifications/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3448 2024-05-13 16:52:05.000000 core_main_app-2.9.0/core_main_app/utils/notifications/mail.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:41.312574 core_main_app-2.9.0/core_main_app/utils/notifications/tasks/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:05.000000 core_main_app-2.9.0/core_main_app/utils/notifications/tasks/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2566 2024-05-13 16:52:05.000000 core_main_app-2.9.0/core_main_app/utils/notifications/tasks/task_mail.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:41.334172 core_main_app-2.9.0/core_main_app/utils/pagination/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:05.000000 core_main_app-2.9.0/core_main_app/utils/pagination/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:41.379862 core_main_app-2.9.0/core_main_app/utils/pagination/django_paginator/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:05.000000 core_main_app-2.9.0/core_main_app/utils/pagination/django_paginator/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      773 2024-05-13 16:52:05.000000 core_main_app-2.9.0/core_main_app/utils/pagination/django_paginator/results_paginator.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:41.423492 core_main_app-2.9.0/core_main_app/utils/pagination/mongoengine_paginator/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:05.000000 core_main_app-2.9.0/core_main_app/utils/pagination/mongoengine_paginator/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1109 2024-05-13 16:52:05.000000 core_main_app-2.9.0/core_main_app/utils/pagination/mongoengine_paginator/paginator.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:41.482827 core_main_app-2.9.0/core_main_app/utils/pagination/rest_framework_paginator/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:05.000000 core_main_app-2.9.0/core_main_app/utils/pagination/rest_framework_paginator/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      525 2024-05-13 16:52:05.000000 core_main_app-2.9.0/core_main_app/utils/pagination/rest_framework_paginator/pagination.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1108 2024-05-13 16:52:05.000000 core_main_app-2.9.0/core_main_app/utils/pagination/rest_framework_paginator/rest_framework_paginator.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      458 2024-05-13 16:52:05.000000 core_main_app-2.9.0/core_main_app/utils/parser.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:41.541056 core_main_app-2.9.0/core_main_app/utils/query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:05.000000 core_main_app-2.9.0/core_main_app/utils/query/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      145 2024-05-13 16:52:05.000000 core_main_app-2.9.0/core_main_app/utils/query/constants.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:41.612035 core_main_app-2.9.0/core_main_app/utils/query/mongo/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:05.000000 core_main_app-2.9.0/core_main_app/utils/query/mongo/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14676 2024-05-13 16:52:05.000000 core_main_app-2.9.0/core_main_app/utils/query/mongo/prepare.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3095 2024-05-13 16:52:05.000000 core_main_app-2.9.0/core_main_app/utils/query/mongo/query_builder.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:41.697067 core_main_app-2.9.0/core_main_app/utils/raw_query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:05.000000 core_main_app-2.9.0/core_main_app/utils/raw_query/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1622 2024-05-13 16:52:05.000000 core_main_app-2.9.0/core_main_app/utils/raw_query/common.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3901 2024-05-13 16:52:05.000000 core_main_app-2.9.0/core_main_app/utils/raw_query/django_raw_query.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2134 2024-05-13 16:52:05.000000 core_main_app-2.9.0/core_main_app/utils/raw_query/mongo_raw_query.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3182 2024-05-13 16:52:05.000000 core_main_app-2.9.0/core_main_app/utils/rendering.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:41.791258 core_main_app-2.9.0/core_main_app/utils/requests_utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:06.000000 core_main_app-2.9.0/core_main_app/utils/requests_utils/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      568 2024-05-13 16:52:06.000000 core_main_app-2.9.0/core_main_app/utils/requests_utils/access_control.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1663 2024-05-13 16:52:06.000000 core_main_app-2.9.0/core_main_app/utils/requests_utils/requests_utils.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2054 2024-05-13 16:52:06.000000 core_main_app-2.9.0/core_main_app/utils/requests_utils/ssl.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:41.880981 core_main_app-2.9.0/core_main_app/utils/resolvers/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:06.000000 core_main_app-2.9.0/core_main_app/utils/resolvers/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1184 2024-05-13 16:52:06.000000 core_main_app-2.9.0/core_main_app/utils/resolvers/requests_resolver.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1072 2024-05-13 16:52:06.000000 core_main_app-2.9.0/core_main_app/utils/resolvers/resolver_utils.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      194 2024-05-13 16:52:06.000000 core_main_app-2.9.0/core_main_app/utils/resolvers/xsd_uri_resolvers.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:41.921541 core_main_app-2.9.0/core_main_app/utils/routers/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:06.000000 core_main_app-2.9.0/core_main_app/utils/routers/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      786 2024-05-13 16:52:06.000000 core_main_app-2.9.0/core_main_app/utils/routers/db_router.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:41.963672 core_main_app-2.9.0/core_main_app/utils/saml2/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:06.000000 core_main_app-2.9.0/core_main_app/utils/saml2/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8886 2024-05-13 16:52:06.000000 core_main_app-2.9.0/core_main_app/utils/saml2/utils.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1857 2024-05-13 16:52:06.000000 core_main_app-2.9.0/core_main_app/utils/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:42.047425 core_main_app-2.9.0/core_main_app/utils/storage/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:06.000000 core_main_app-2.9.0/core_main_app/utils/storage/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3523 2024-05-13 16:52:06.000000 core_main_app-2.9.0/core_main_app/utils/storage/gridfs_storage.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1791 2024-05-13 16:52:06.000000 core_main_app-2.9.0/core_main_app/utils/storage/storage.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:42.113033 core_main_app-2.9.0/core_main_app/utils/tests_tools/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      853 2024-05-13 16:52:06.000000 core_main_app-2.9.0/core_main_app/utils/tests_tools/MockUser.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5344 2024-05-13 16:52:06.000000 core_main_app-2.9.0/core_main_app/utils/tests_tools/RequestMock.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:06.000000 core_main_app-2.9.0/core_main_app/utils/tests_tools/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:42.140473 core_main_app-2.9.0/core_main_app/utils/tests_tools/databases/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:06.000000 core_main_app-2.9.0/core_main_app/utils/tests_tools/databases/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:42.208046 core_main_app-2.9.0/core_main_app/utils/tests_tools/databases/mongo/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:06.000000 core_main_app-2.9.0/core_main_app/utils/tests_tools/databases/mongo/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1690 2024-05-13 16:52:06.000000 core_main_app-2.9.0/core_main_app/utils/tests_tools/databases/mongo/mongoengine_database.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3654 2024-05-13 16:52:06.000000 core_main_app-2.9.0/core_main_app/utils/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:42.274038 core_main_app-2.9.0/core_main_app/utils/validation/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:06.000000 core_main_app-2.9.0/core_main_app/utils/validation/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1162 2024-05-13 16:52:06.000000 core_main_app-2.9.0/core_main_app/utils/validation/regex_validation.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      644 2024-05-13 16:52:06.000000 core_main_app-2.9.0/core_main_app/utils/validation/xpath_validation.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:42.321797 core_main_app-2.9.0/core_main_app/utils/view_builders/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:06.000000 core_main_app-2.9.0/core_main_app/utils/view_builders/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6818 2024-05-13 16:52:06.000000 core_main_app-2.9.0/core_main_app/utils/view_builders/data.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    15550 2024-05-13 16:52:06.000000 core_main_app-2.9.0/core_main_app/utils/xml.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:42.409114 core_main_app-2.9.0/core_main_app/utils/xsd_flattener/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:06.000000 core_main_app-2.9.0/core_main_app/utils/xsd_flattener/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2094 2024-05-13 16:52:06.000000 core_main_app-2.9.0/core_main_app/utils/xsd_flattener/xsd_flattener_database_url.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1000 2024-05-13 16:52:06.000000 core_main_app-2.9.0/core_main_app/utils/xsd_flattener/xsd_flattener_requests_url.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:42.431171 core_main_app-2.9.0/core_main_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:06.000000 core_main_app-2.9.0/core_main_app/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:42.514124 core_main_app-2.9.0/core_main_app/views/admin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:06.000000 core_main_app-2.9.0/core_main_app/views/admin/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4276 2024-05-13 16:52:06.000000 core_main_app-2.9.0/core_main_app/views/admin/ajax.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:42.536159 core_main_app-2.9.0/core_main_app/views/admin/commons/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:06.000000 core_main_app-2.9.0/core_main_app/views/admin/commons/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:42.595978 core_main_app-2.9.0/core_main_app/views/admin/commons/upload/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:06.000000 core_main_app-2.9.0/core_main_app/views/admin/commons/upload/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      439 2024-05-13 16:52:06.000000 core_main_app-2.9.0/core_main_app/views/admin/commons/upload/forms.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5702 2024-05-13 16:52:06.000000 core_main_app-2.9.0/core_main_app/views/admin/forms.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    21689 2024-05-13 16:52:06.000000 core_main_app-2.9.0/core_main_app/views/admin/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:42.676990 core_main_app-2.9.0/core_main_app/views/common/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:06.000000 core_main_app-2.9.0/core_main_app/views/common/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7223 2024-05-13 16:52:06.000000 core_main_app-2.9.0/core_main_app/views/common/ajax.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      459 2024-05-13 16:52:06.000000 core_main_app-2.9.0/core_main_app/views/common/forms.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    43369 2024-05-13 16:52:06.000000 core_main_app-2.9.0/core_main_app/views/common/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:42.768474 core_main_app-2.9.0/core_main_app/views/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:06.000000 core_main_app-2.9.0/core_main_app/views/user/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    21799 2024-05-13 16:52:06.000000 core_main_app-2.9.0/core_main_app/views/user/ajax.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6400 2024-05-13 16:52:06.000000 core_main_app-2.9.0/core_main_app/views/user/forms.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11091 2024-05-13 16:52:06.000000 core_main_app-2.9.0/core_main_app/views/user/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:31.490136 core_main_app-2.9.0/core_main_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9924 2024-05-13 16:52:23.000000 core_main_app-2.9.0/core_main_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    35867 2024-05-13 16:52:29.000000 core_main_app-2.9.0/core_main_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2024-05-13 16:52:23.000000 core_main_app-2.9.0/core_main_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      491 2024-05-13 16:52:23.000000 core_main_app-2.9.0/core_main_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       25 2024-05-13 16:52:23.000000 core_main_app-2.9.0/core_main_app.egg-info/top_level.txt
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:42.826023 core_main_app-2.9.0/docs/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:06.000000 core_main_app-2.9.0/docs/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11121 2024-05-13 16:52:07.000000 core_main_app-2.9.0/docs/conf.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      278 2024-05-13 16:52:07.000000 core_main_app-2.9.0/docs/conf_urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      170 2024-05-13 16:52:15.000000 core_main_app-2.9.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       18 2024-05-13 16:52:15.000000 core_main_app-2.9.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       91 2024-05-13 16:52:15.000000 core_main_app-2.9.0/requirements.dev.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       20 2024-05-13 16:52:15.000000 core_main_app-2.9.0/requirements.mongo.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      340 2024-05-13 16:52:15.000000 core_main_app-2.9.0/requirements.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2024-05-13 16:52:51.411849 core_main_app-2.9.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2104 2024-05-13 16:52:15.000000 core_main_app-2.9.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:42.946826 core_main_app-2.9.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:15.000000 core_main_app-2.9.0/tests/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:42.991058 core_main_app-2.9.0/tests/access_control/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:15.000000 core_main_app-2.9.0/tests/access_control/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:43.042739 core_main_app-2.9.0/tests/access_control/api/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:15.000000 core_main_app-2.9.0/tests/access_control/api/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1126 2024-05-13 16:52:15.000000 core_main_app-2.9.0/tests/access_control/api/tests_unit.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3415 2024-05-13 16:52:15.000000 core_main_app-2.9.0/tests/access_control/tests_access_control.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:43.087450 core_main_app-2.9.0/tests/access_control/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:15.000000 core_main_app-2.9.0/tests/access_control/utils/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6858 2024-05-13 16:52:15.000000 core_main_app-2.9.0/tests/access_control/utils/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:43.110315 core_main_app-2.9.0/tests/commons/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:15.000000 core_main_app-2.9.0/tests/commons/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:43.157087 core_main_app-2.9.0/tests/commons/exceptions/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:15.000000 core_main_app-2.9.0/tests/commons/exceptions/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1254 2024-05-13 16:52:16.000000 core_main_app-2.9.0/tests/commons/exceptions/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:43.204727 core_main_app-2.9.0/tests/commons/validators/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:16.000000 core_main_app-2.9.0/tests/commons/validators/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4324 2024-05-13 16:52:16.000000 core_main_app-2.9.0/tests/commons/validators/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:43.225937 core_main_app-2.9.0/tests/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:16.000000 core_main_app-2.9.0/tests/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:43.321816 core_main_app-2.9.0/tests/components/blob/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:16.000000 core_main_app-2.9.0/tests/components/blob/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:43.366284 core_main_app-2.9.0/tests/components/blob/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:16.000000 core_main_app-2.9.0/tests/components/blob/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3165 2024-05-13 16:52:16.000000 core_main_app-2.9.0/tests/components/blob/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6398 2024-05-13 16:52:16.000000 core_main_app-2.9.0/tests/components/blob/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    38881 2024-05-13 16:52:16.000000 core_main_app-2.9.0/tests/components/blob/tests_int_access_control.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2353 2024-05-13 16:52:16.000000 core_main_app-2.9.0/tests/components/blob/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:43.471445 core_main_app-2.9.0/tests/components/data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:16.000000 core_main_app-2.9.0/tests/components/data/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:43.513197 core_main_app-2.9.0/tests/components/data/access_control/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:16.000000 core_main_app-2.9.0/tests/components/data/access_control/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2716 2024-05-13 16:52:16.000000 core_main_app-2.9.0/tests/components/data/access_control/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:43.556004 core_main_app-2.9.0/tests/components/data/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:16.000000 core_main_app-2.9.0/tests/components/data/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    28106 2024-05-13 16:52:16.000000 core_main_app-2.9.0/tests/components/data/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    69360 2024-05-13 16:52:16.000000 core_main_app-2.9.0/tests/components/data/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    83957 2024-05-13 16:52:16.000000 core_main_app-2.9.0/tests/components/data/tests_int_access_control.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3730 2024-05-13 16:52:16.000000 core_main_app-2.9.0/tests/components/data/tests_int_ordering.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    40552 2024-05-13 16:52:16.000000 core_main_app-2.9.0/tests/components/data/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:43.601332 core_main_app-2.9.0/tests/components/group/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:16.000000 core_main_app-2.9.0/tests/components/group/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:43.663293 core_main_app-2.9.0/tests/components/group/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:16.000000 core_main_app-2.9.0/tests/components/group/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      570 2024-05-13 16:52:16.000000 core_main_app-2.9.0/tests/components/group/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      879 2024-05-13 16:52:16.000000 core_main_app-2.9.0/tests/components/group/fixtures/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4760 2024-05-13 16:52:16.000000 core_main_app-2.9.0/tests/components/group/tests_int.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:43.731190 core_main_app-2.9.0/tests/components/lock/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:16.000000 core_main_app-2.9.0/tests/components/lock/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4153 2024-05-13 16:52:16.000000 core_main_app-2.9.0/tests/components/lock/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2440 2024-05-13 16:52:16.000000 core_main_app-2.9.0/tests/components/lock/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:43.796092 core_main_app-2.9.0/tests/components/mongo_data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:16.000000 core_main_app-2.9.0/tests/components/mongo_data/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    75687 2024-05-13 16:52:16.000000 core_main_app-2.9.0/tests/components/mongo_data/tests_int_access_control.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5423 2024-05-13 16:52:16.000000 core_main_app-2.9.0/tests/components/mongo_data/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:43.858072 core_main_app-2.9.0/tests/components/template/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:16.000000 core_main_app-2.9.0/tests/components/template/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:43.902082 core_main_app-2.9.0/tests/components/template/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:16.000000 core_main_app-2.9.0/tests/components/template/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2081 2024-05-13 16:52:16.000000 core_main_app-2.9.0/tests/components/template/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    46022 2024-05-13 16:52:16.000000 core_main_app-2.9.0/tests/components/template/tests_int_access_control.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10648 2024-05-13 16:52:16.000000 core_main_app-2.9.0/tests/components/template/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:43.981199 core_main_app-2.9.0/tests/components/template_version_manager/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:16.000000 core_main_app-2.9.0/tests/components/template_version_manager/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:44.025184 core_main_app-2.9.0/tests/components/template_version_manager/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:16.000000 core_main_app-2.9.0/tests/components/template_version_manager/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6479 2024-05-13 16:52:16.000000 core_main_app-2.9.0/tests/components/template_version_manager/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    54686 2024-05-13 16:52:16.000000 core_main_app-2.9.0/tests/components/template_version_manager/tests_int_access_control.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    20410 2024-05-13 16:52:16.000000 core_main_app-2.9.0/tests/components/template_version_manager/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:44.086244 core_main_app-2.9.0/tests/components/template_xsl_rendering/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:16.000000 core_main_app-2.9.0/tests/components/template_xsl_rendering/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:44.130028 core_main_app-2.9.0/tests/components/template_xsl_rendering/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:16.000000 core_main_app-2.9.0/tests/components/template_xsl_rendering/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3269 2024-05-13 16:52:16.000000 core_main_app-2.9.0/tests/components/template_xsl_rendering/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7896 2024-05-13 16:52:16.000000 core_main_app-2.9.0/tests/components/template_xsl_rendering/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9565 2024-05-13 16:52:16.000000 core_main_app-2.9.0/tests/components/template_xsl_rendering/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:44.202684 core_main_app-2.9.0/tests/components/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:16.000000 core_main_app-2.9.0/tests/components/user/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:44.262718 core_main_app-2.9.0/tests/components/user/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:16.000000 core_main_app-2.9.0/tests/components/user/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1551 2024-05-13 16:52:16.000000 core_main_app-2.9.0/tests/components/user/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1429 2024-05-13 16:52:16.000000 core_main_app-2.9.0/tests/components/user/fixtures/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7733 2024-05-13 16:52:16.000000 core_main_app-2.9.0/tests/components/user/tests_int.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:45.546011 core_main_app-2.9.0/tests/components/user_preferences/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:16.000000 core_main_app-2.9.0/tests/components/user_preferences/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:46.604970 core_main_app-2.9.0/tests/components/user_preferences/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:16.000000 core_main_app-2.9.0/tests/components/user_preferences/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1302 2024-05-13 16:52:16.000000 core_main_app-2.9.0/tests/components/user_preferences/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3912 2024-05-13 16:52:16.000000 core_main_app-2.9.0/tests/components/user_preferences/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11726 2024-05-13 16:52:16.000000 core_main_app-2.9.0/tests/components/user_preferences/tests_int_access_control.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6563 2024-05-13 16:52:16.000000 core_main_app-2.9.0/tests/components/user_preferences/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:46.669344 core_main_app-2.9.0/tests/components/version_manager/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:16.000000 core_main_app-2.9.0/tests/components/version_manager/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    61614 2024-05-13 16:52:16.000000 core_main_app-2.9.0/tests/components/version_manager/tests_int_access_control.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9899 2024-05-13 16:52:16.000000 core_main_app-2.9.0/tests/components/version_manager/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:46.713531 core_main_app-2.9.0/tests/components/web_page/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:16.000000 core_main_app-2.9.0/tests/components/web_page/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4846 2024-05-13 16:52:16.000000 core_main_app-2.9.0/tests/components/web_page/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:46.758813 core_main_app-2.9.0/tests/components/web_page_login/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:16.000000 core_main_app-2.9.0/tests/components/web_page_login/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3905 2024-05-13 16:52:16.000000 core_main_app-2.9.0/tests/components/web_page_login/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:46.802791 core_main_app-2.9.0/tests/components/workspace/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:16.000000 core_main_app-2.9.0/tests/components/workspace/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:46.865186 core_main_app-2.9.0/tests/components/workspace/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:16.000000 core_main_app-2.9.0/tests/components/workspace/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1235 2024-05-13 16:52:16.000000 core_main_app-2.9.0/tests/components/workspace/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      968 2024-05-13 16:52:16.000000 core_main_app-2.9.0/tests/components/workspace/fixtures/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7006 2024-05-13 16:52:16.000000 core_main_app-2.9.0/tests/components/workspace/tests_int.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:48.861815 core_main_app-2.9.0/tests/components/xsl_transformation/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:17.000000 core_main_app-2.9.0/tests/components/xsl_transformation/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    12832 2024-05-13 16:52:17.000000 core_main_app-2.9.0/tests/components/xsl_transformation/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:48.903043 core_main_app-2.9.0/tests/middleware/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:17.000000 core_main_app-2.9.0/tests/middleware/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3431 2024-05-13 16:52:17.000000 core_main_app-2.9.0/tests/middleware/tests_unit.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      356 2024-05-13 16:52:17.000000 core_main_app-2.9.0/tests/mocks.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:48.955947 core_main_app-2.9.0/tests/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:17.000000 core_main_app-2.9.0/tests/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:49.052172 core_main_app-2.9.0/tests/rest/blob/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:17.000000 core_main_app-2.9.0/tests/rest/blob/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:49.094722 core_main_app-2.9.0/tests/rest/blob/serializers/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:17.000000 core_main_app-2.9.0/tests/rest/blob/serializers/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6224 2024-05-13 16:52:17.000000 core_main_app-2.9.0/tests/rest/blob/serializers/tests_unit.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    31044 2024-05-13 16:52:17.000000 core_main_app-2.9.0/tests/rest/blob/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    26694 2024-05-13 16:52:17.000000 core_main_app-2.9.0/tests/rest/blob/tests_permissions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       36 2024-05-13 16:52:17.000000 core_main_app-2.9.0/tests/rest/blob/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:49.188726 core_main_app-2.9.0/tests/rest/data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:17.000000 core_main_app-2.9.0/tests/rest/data/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    49596 2024-05-13 16:52:17.000000 core_main_app-2.9.0/tests/rest/data/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    37874 2024-05-13 16:52:17.000000 core_main_app-2.9.0/tests/rest/data/tests_permissions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    30805 2024-05-13 16:52:17.000000 core_main_app-2.9.0/tests/rest/data/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:49.295170 core_main_app-2.9.0/tests/rest/template/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:17.000000 core_main_app-2.9.0/tests/rest/template/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2518 2024-05-13 16:52:17.000000 core_main_app-2.9.0/tests/rest/template/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5026 2024-05-13 16:52:17.000000 core_main_app-2.9.0/tests/rest/template/tests_permission.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6295 2024-05-13 16:52:17.000000 core_main_app-2.9.0/tests/rest/template/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:49.434430 core_main_app-2.9.0/tests/rest/template_version_manager/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:17.000000 core_main_app-2.9.0/tests/rest/template_version_manager/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    45015 2024-05-13 16:52:17.000000 core_main_app-2.9.0/tests/rest/template_version_manager/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    41433 2024-05-13 16:52:17.000000 core_main_app-2.9.0/tests/rest/template_version_manager/tests_permission.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5606 2024-05-13 16:52:17.000000 core_main_app-2.9.0/tests/rest/template_version_manager/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:49.521454 core_main_app-2.9.0/tests/rest/template_xsl_rendering/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:17.000000 core_main_app-2.9.0/tests/rest/template_xsl_rendering/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11418 2024-05-13 16:52:17.000000 core_main_app-2.9.0/tests/rest/template_xsl_rendering/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    13879 2024-05-13 16:52:17.000000 core_main_app-2.9.0/tests/rest/template_xsl_rendering/tests_permissions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3610 2024-05-13 16:52:17.000000 core_main_app-2.9.0/tests/rest/tests_views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:49.607018 core_main_app-2.9.0/tests/rest/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:17.000000 core_main_app-2.9.0/tests/rest/user/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1737 2024-05-13 16:52:17.000000 core_main_app-2.9.0/tests/rest/user/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3137 2024-05-13 16:52:17.000000 core_main_app-2.9.0/tests/rest/user/tests_permissions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      886 2024-05-13 16:52:17.000000 core_main_app-2.9.0/tests/rest/user/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:49.674960 core_main_app-2.9.0/tests/rest/web_page/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:17.000000 core_main_app-2.9.0/tests/rest/web_page/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6164 2024-05-13 16:52:17.000000 core_main_app-2.9.0/tests/rest/web_page/tests_permission.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:49.740689 core_main_app-2.9.0/tests/rest/workspace/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:17.000000 core_main_app-2.9.0/tests/rest/workspace/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    72329 2024-05-13 16:52:17.000000 core_main_app-2.9.0/tests/rest/workspace/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    48644 2024-05-13 16:52:17.000000 core_main_app-2.9.0/tests/rest/workspace/tests_permissions.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:49.831884 core_main_app-2.9.0/tests/rest/xsl_transformation/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:17.000000 core_main_app-2.9.0/tests/rest/xsl_transformation/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:49.880221 core_main_app-2.9.0/tests/rest/xsl_transformation/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:17.000000 core_main_app-2.9.0/tests/rest/xsl_transformation/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1283 2024-05-13 16:52:17.000000 core_main_app-2.9.0/tests/rest/xsl_transformation/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11618 2024-05-13 16:52:17.000000 core_main_app-2.9.0/tests/rest/xsl_transformation/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    12753 2024-05-13 16:52:17.000000 core_main_app-2.9.0/tests/rest/xsl_transformation/tests_permission.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4365 2024-05-13 16:52:17.000000 core_main_app-2.9.0/tests/rest/xsl_transformation/tests_unit.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      738 2024-05-13 16:52:17.000000 core_main_app-2.9.0/tests/rest_urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:49.930711 core_main_app-2.9.0/tests/system/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:17.000000 core_main_app-2.9.0/tests/system/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:49.949591 core_main_app-2.9.0/tests/system/blob/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:17.000000 core_main_app-2.9.0/tests/system/blob/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:49.995419 core_main_app-2.9.0/tests/system/blob/api/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:17.000000 core_main_app-2.9.0/tests/system/blob/api/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      935 2024-05-13 16:52:17.000000 core_main_app-2.9.0/tests/system/blob/api/tests_unit.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7830 2024-05-13 16:52:17.000000 core_main_app-2.9.0/tests/system/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:50.108406 core_main_app-2.9.0/tests/templatetags/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:17.000000 core_main_app-2.9.0/tests/templatetags/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:50.169971 core_main_app-2.9.0/tests/templatetags/auth_extras/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:17.000000 core_main_app-2.9.0/tests/templatetags/auth_extras/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1576 2024-05-13 16:52:17.000000 core_main_app-2.9.0/tests/templatetags/auth_extras/tests_unit.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1946 2024-05-13 16:52:17.000000 core_main_app-2.9.0/tests/templatetags/test_blob_tags.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      530 2024-05-13 16:52:17.000000 core_main_app-2.9.0/tests/templatetags/test_format_json.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1364 2024-05-13 16:52:17.000000 core_main_app-2.9.0/tests/templatetags/test_get_attribute.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1486 2024-05-13 16:52:17.000000 core_main_app-2.9.0/tests/templatetags/test_parse_date.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2883 2024-05-13 16:52:17.000000 core_main_app-2.9.0/tests/test_settings.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      293 2024-05-13 16:52:17.000000 core_main_app-2.9.0/tests/test_settings_sqlite3.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4310 2024-05-13 16:52:17.000000 core_main_app-2.9.0/tests/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:50.381555 core_main_app-2.9.0/tests/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:17.000000 core_main_app-2.9.0/tests/utils/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:50.428207 core_main_app-2.9.0/tests/utils/checksum/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:17.000000 core_main_app-2.9.0/tests/utils/checksum/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1294 2024-05-13 16:52:17.000000 core_main_app-2.9.0/tests/utils/checksum/tests_checksum.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:50.486252 core_main_app-2.9.0/tests/utils/dict/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:17.000000 core_main_app-2.9.0/tests/utils/dict/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      712 2024-05-13 16:52:17.000000 core_main_app-2.9.0/tests/utils/dict/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:50.529773 core_main_app-2.9.0/tests/utils/json_utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:17.000000 core_main_app-2.9.0/tests/utils/json_utils/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7501 2024-05-13 16:52:17.000000 core_main_app-2.9.0/tests/utils/json_utils/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:50.572080 core_main_app-2.9.0/tests/utils/migrations/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:17.000000 core_main_app-2.9.0/tests/utils/migrations/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1664 2024-05-13 16:52:17.000000 core_main_app-2.9.0/tests/utils/migrations/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:50.593760 core_main_app-2.9.0/tests/utils/query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:18.000000 core_main_app-2.9.0/tests/utils/query/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:50.640703 core_main_app-2.9.0/tests/utils/query/mongo/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:18.000000 core_main_app-2.9.0/tests/utils/query/mongo/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9855 2024-05-13 16:52:18.000000 core_main_app-2.9.0/tests/utils/query/mongo/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:50.686761 core_main_app-2.9.0/tests/utils/requests_utls/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:18.000000 core_main_app-2.9.0/tests/utils/requests_utls/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1436 2024-05-13 16:52:18.000000 core_main_app-2.9.0/tests/utils/requests_utls/tests_ssl.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:50.731208 core_main_app-2.9.0/tests/utils/routers/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:18.000000 core_main_app-2.9.0/tests/utils/routers/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1620 2024-05-13 16:52:18.000000 core_main_app-2.9.0/tests/utils/routers/tests_db_router.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:50.773688 core_main_app-2.9.0/tests/utils/settings/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:18.000000 core_main_app-2.9.0/tests/utils/settings/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4447 2024-05-13 16:52:18.000000 core_main_app-2.9.0/tests/utils/settings/tests_unit.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      902 2024-05-13 16:52:18.000000 core_main_app-2.9.0/tests/utils/test_unit_apps.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      772 2024-05-13 16:52:18.000000 core_main_app-2.9.0/tests/utils/test_unit_urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4010 2024-05-13 16:52:18.000000 core_main_app-2.9.0/tests/utils/tests_int_blob_downloader.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7757 2024-05-13 16:52:18.000000 core_main_app-2.9.0/tests/utils/tests_int_file.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2368 2024-05-13 16:52:18.000000 core_main_app-2.9.0/tests/utils/tests_unit_admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1726 2024-05-13 16:52:18.000000 core_main_app-2.9.0/tests/utils/tests_unit_boolean.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      402 2024-05-13 16:52:18.000000 core_main_app-2.9.0/tests/utils/tests_unit_parser.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11988 2024-05-13 16:52:18.000000 core_main_app-2.9.0/tests/utils/tests_unit_xml_operation.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5194 2024-05-13 16:52:18.000000 core_main_app-2.9.0/tests/utils/tests_view_data.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:50.816522 core_main_app-2.9.0/tests/utils/validation/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:18.000000 core_main_app-2.9.0/tests/utils/validation/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1318 2024-05-13 16:52:18.000000 core_main_app-2.9.0/tests/utils/validation/tests_unit_validation.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:50.864815 core_main_app-2.9.0/tests/utils/xsd_flattener/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:18.000000 core_main_app-2.9.0/tests/utils/xsd_flattener/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4358 2024-05-13 16:52:18.000000 core_main_app-2.9.0/tests/utils/xsd_flattener/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:50.944985 core_main_app-2.9.0/tests/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:18.000000 core_main_app-2.9.0/tests/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:50.964815 core_main_app-2.9.0/tests/views/admin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:18.000000 core_main_app-2.9.0/tests/views/admin/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:51.009356 core_main_app-2.9.0/tests/views/admin/ajax/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:18.000000 core_main_app-2.9.0/tests/views/admin/ajax/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      662 2024-05-13 16:52:18.000000 core_main_app-2.9.0/tests/views/admin/ajax/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:51.052157 core_main_app-2.9.0/tests/views/admin/forms/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:18.000000 core_main_app-2.9.0/tests/views/admin/forms/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1691 2024-05-13 16:52:18.000000 core_main_app-2.9.0/tests/views/admin/forms/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:51.116785 core_main_app-2.9.0/tests/views/admin/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:18.000000 core_main_app-2.9.0/tests/views/admin/views/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1336 2024-05-13 16:52:18.000000 core_main_app-2.9.0/tests/views/admin/views/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:51.137230 core_main_app-2.9.0/tests/views/common/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:18.000000 core_main_app-2.9.0/tests/views/common/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:51.191926 core_main_app-2.9.0/tests/views/common/ajax/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:18.000000 core_main_app-2.9.0/tests/views/common/ajax/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6717 2024-05-13 16:52:18.000000 core_main_app-2.9.0/tests/views/common/ajax/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:51.240970 core_main_app-2.9.0/tests/views/common/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:18.000000 core_main_app-2.9.0/tests/views/common/views/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11087 2024-05-13 16:52:18.000000 core_main_app-2.9.0/tests/views/common/views/test_unit.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6921 2024-05-13 16:52:18.000000 core_main_app-2.9.0/tests/views/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    81283 2024-05-13 16:52:18.000000 core_main_app-2.9.0/tests/views/tests_int_access_control.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1328 2024-05-13 16:52:18.000000 core_main_app-2.9.0/tests/views/tests_permissions.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:51.262039 core_main_app-2.9.0/tests/views/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:18.000000 core_main_app-2.9.0/tests/views/user/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:51.336603 core_main_app-2.9.0/tests/views/user/forms/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:18.000000 core_main_app-2.9.0/tests/views/user/forms/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2119 2024-05-13 16:52:18.000000 core_main_app-2.9.0/tests/views/user/forms/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:51.382464 core_main_app-2.9.0/tests/views/user/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:52:18.000000 core_main_app-2.9.0/tests/views/user/views/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9833 2024-05-13 16:52:18.000000 core_main_app-2.9.0/tests/views/user/views/test_unit.py
```

### Comparing `core_main_app-2.8.0/LICENSE.md` & `core_main_app-2.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/PKG-INFO` & `core_main_app-2.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: core_main_app
-Version: 2.8.0
+Version: 2.9.0
 Summary: Main functionalities for the curator core project
 Home-page: https://github.com/usnistgov/core_main_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: =============
         Core Main App
```

### Comparing `core_main_app-2.8.0/README.rst` & `core_main_app-2.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/access_control/api.py` & `core_main_app-2.9.0/core_main_app/access_control/api.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/access_control/decorators.py` & `core_main_app-2.9.0/core_main_app/access_control/decorators.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/access_control/utils.py` & `core_main_app-2.9.0/core_main_app/access_control/utils.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/admin.py` & `core_main_app-2.9.0/core_main_app/admin.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/apps.py` & `core_main_app-2.9.0/core_main_app/apps.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,50 @@
 """ Apps file for setting core package when app is ready.
 """
-import sys
-
 from django.apps import AppConfig
 from django.conf import settings
+from django.db.models.signals import post_migrate
+
+
+def init_app(sender, **kwargs):
+    """Initialize app
+
+    Args:
+        sender:
+        **kwargs:
+
+    Returns:
+
+    """
+    from core_main_app.permissions import discover
+
+    discover.init_rules(sender.apps)
+    discover.create_public_workspace()
 
 
 class InitApp(AppConfig):
     """Core application settings."""
 
     verbose_name = "Core Main App"
 
     name = "core_main_app"
     """ :py:class:`str`: Package name
     """
 
     def ready(self):
-        from core_main_app.permissions import discover
         from core_main_app.settings import SSL_CERTIFICATES_DIR
         from core_main_app.utils.requests_utils.ssl import (
             check_ssl_certificates_dir_setting,
         )
+        from core_main_app.permissions import discover
 
-        """When the app is ready, run the discovery and init the indexes."""
-        if "migrate" not in sys.argv:
-            _check_settings()
-            check_ssl_certificates_dir_setting(SSL_CERTIFICATES_DIR)
-            discover.init_rules(self.apps)
-            discover.create_public_workspace()
-            discover.init_mongo_indexing()
+        _check_settings()
+        check_ssl_certificates_dir_setting(SSL_CERTIFICATES_DIR)
+        post_migrate.connect(init_app, sender=self)
+        discover.init_mongo_indexing()
 
 
 def _check_settings():
     """Check settings
 
     Returns:
```

### Comparing `core_main_app-2.8.0/core_main_app/commons/constants.py` & `core_main_app-2.9.0/core_main_app/commons/constants.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/commons/exceptions.py` & `core_main_app-2.9.0/core_main_app/commons/exceptions.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/commons/validators.py` & `core_main_app-2.9.0/core_main_app/commons/validators.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/components/abstract_data/models.py` & `core_main_app-2.9.0/core_main_app/components/abstract_data/models.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/components/blob/access_control.py` & `core_main_app-2.9.0/core_main_app/components/blob/access_control.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/components/blob/api.py` & `core_main_app-2.9.0/core_main_app/components/blob/api.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/components/blob/models.py` & `core_main_app-2.9.0/core_main_app/components/blob/models.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/components/data/access_control.py` & `core_main_app-2.9.0/core_main_app/components/data/access_control.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/components/data/admin_site.py` & `core_main_app-2.9.0/core_main_app/components/data/admin_site.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 from core_main_app.commons.exceptions import DoesNotExist
 from core_main_app.components.user import api as user_api
 from core_main_app.components.workspace import api as workspace_api
 from core_main_app.utils.admin_site.model_admin_class import (
     get_base_model_admin_class,
 )
+from core_main_app.utils.labels import get_data_label
 
 
 class UpdateActionForm(ActionForm):
     """Action form for data update"""
 
     user_id = ChoiceField(label="Owner:", required=False)
     workspace = ChoiceField(label="Workspace:", required=False)
@@ -90,15 +91,15 @@
             if settings.MONGODB_INDEXING:
                 from core_main_app.components.mongo.models import MongoData
 
                 MongoData.update_user_id_from_queryset(queryset, user_id)
             # Display success message
             model_admin.message_user(
                 request,
-                f"Successfully updated owner of {queryset.count()} Data",
+                f"Owner updated for {queryset.count()} {get_data_label()}.",
                 messages.SUCCESS,
             )
         # Check if workspace_id parameter provided
         if "workspace" in request.POST and request.POST["workspace"] != "":
             # Get workspace
             workspace = (
                 None
@@ -126,15 +127,15 @@
                 workspace_id = workspace.id if workspace else None
                 MongoData.update_workspace_id_from_queryset(
                     queryset, workspace_id
                 )
             # Display success message
             model_admin.message_user(
                 request,
-                f"Successfully updated workspace of {queryset.count()} Data",
+                f"Workspace updated for {queryset.count()} {get_data_label()}.",
                 messages.SUCCESS,
             )
     except DoesNotExist as ex:
         model_admin.message_user(request, str(ex), messages.ERROR)
     except Exception as ex:
         model_admin.message_user(request, str(ex), messages.ERROR)
```

### Comparing `core_main_app-2.8.0/core_main_app/components/data/api.py` & `core_main_app-2.9.0/core_main_app/components/data/api.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/components/data/models.py` & `core_main_app-2.9.0/core_main_app/components/data/models.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/components/data/tasks.py` & `core_main_app-2.9.0/core_main_app/components/data/tasks.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/components/group/api.py` & `core_main_app-2.9.0/core_main_app/components/group/api.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/components/lock/api.py` & `core_main_app-2.9.0/core_main_app/components/lock/api.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/components/lock/models.py` & `core_main_app-2.9.0/core_main_app/components/lock/models.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/components/mongo/api.py` & `core_main_app-2.9.0/core_main_app/components/mongo/api.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/components/mongo/models.py` & `core_main_app-2.9.0/core_main_app/components/mongo/models.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/components/template/access_control.py` & `core_main_app-2.9.0/core_main_app/components/template/access_control.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/components/template/api.py` & `core_main_app-2.9.0/core_main_app/components/template/api.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/components/template/models.py` & `core_main_app-2.9.0/core_main_app/components/template/models.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/components/template_version_manager/access_control.py` & `core_main_app-2.9.0/core_main_app/components/template_version_manager/access_control.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/components/template_version_manager/api.py` & `core_main_app-2.9.0/core_main_app/components/template_version_manager/api.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/components/template_version_manager/models.py` & `core_main_app-2.9.0/core_main_app/components/template_version_manager/models.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/components/template_xsl_rendering/api.py` & `core_main_app-2.9.0/core_main_app/components/template_xsl_rendering/api.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """ TemplateXslRendering API calls
 """
 import logging
 
-from core_main_app.commons.exceptions import ApiError
+from core_main_app.commons.exceptions import ApiError, DoesNotExist
 from core_main_app.components.template_xsl_rendering.models import (
     TemplateXslRendering,
 )
 from core_main_app.components.xsl_transformation import (
     api as xsl_transformation_api,
 )
 
@@ -43,15 +43,14 @@
 
     if need_to_be_kept:
         return upsert(
             template,
             list_xslt,
             default_detail_xslt,
             list_detail_xslt,
-            template_xsl_rendering_id,
         )
 
     try:
         if template_xsl_rendering_id:
             template_xsl_rendering = get_by_id(template_xsl_rendering_id)
             delete(template_xsl_rendering)
 
@@ -142,43 +141,38 @@
 
 
 def upsert(
     template,
     list_xslt,
     default_detail_xslt,
     list_detail_xslt,
-    template_xsl_rendering_id=None,
 ):
     """Update or create a XSL Template rendering object
 
     Args:
         template:
         list_xslt:
         default_detail_xslt:
         list_detail_xslt:
-        template_xsl_rendering_id:
 
     Returns:
         TemplateXSLRendering - The updated/created object.
     """
     try:
-        template_xsl_rendering = get_by_id(template_xsl_rendering_id)
+        template_xsl_rendering = get_by_template_id(template.id)
         template_xsl_rendering.list_xslt = list_xslt
         template_xsl_rendering.default_detail_xslt = default_detail_xslt
         template_xsl_rendering.list_detail_xslt.set(
             list_detail_xslt
             if list_detail_xslt
             else xsl_transformation_api.get_none()
         )
         template_xsl_rendering.save()
-    except Exception as exception:
-        logger.warning(
-            "Exception when saving TemplateXSLRendering object: %s"
-            % str(exception)
-        )
+    except DoesNotExist:
+        logger.info("TemplateXSLRendering not found, creating it now.")
         template_xsl_rendering = TemplateXslRendering(
             template=template,
             list_xslt=list_xslt,
             default_detail_xslt=default_detail_xslt,
         )
         template_xsl_rendering.save()
```

### Comparing `core_main_app-2.8.0/core_main_app/components/template_xsl_rendering/models.py` & `core_main_app-2.9.0/core_main_app/components/template_xsl_rendering/models.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/components/user/api.py` & `core_main_app-2.9.0/core_main_app/components/user/api.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/components/user_preferences/access_control.py` & `core_main_app-2.9.0/core_main_app/components/user_preferences/access_control.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/components/user_preferences/api.py` & `core_main_app-2.9.0/core_main_app/components/user_preferences/api.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/components/user_preferences/models.py` & `core_main_app-2.9.0/core_main_app/components/user_preferences/models.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/components/version_manager/access_control.py` & `core_main_app-2.9.0/core_main_app/components/version_manager/access_control.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/components/version_manager/api.py` & `core_main_app-2.9.0/core_main_app/components/version_manager/api.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/components/version_manager/models.py` & `core_main_app-2.9.0/core_main_app/components/version_manager/models.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/components/version_manager/utils.py` & `core_main_app-2.9.0/core_main_app/components/version_manager/utils.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/components/web_page/api.py` & `core_main_app-2.9.0/core_main_app/components/web_page/api.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/components/web_page/models.py` & `core_main_app-2.9.0/core_main_app/components/web_page/models.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/components/web_page_login/api.py` & `core_main_app-2.9.0/core_main_app/components/web_page_login/api.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/components/workspace/access_control.py` & `core_main_app-2.9.0/core_main_app/components/workspace/access_control.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/components/workspace/api.py` & `core_main_app-2.9.0/core_main_app/components/workspace/api.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/components/workspace/models.py` & `core_main_app-2.9.0/core_main_app/components/workspace/models.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/components/xsl_transformation/api.py` & `core_main_app-2.9.0/core_main_app/components/xsl_transformation/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,20 +9,15 @@
 
 
 def get_by_name(xslt_name):
     """Get an XSLT document.
 
     Returns:
     """
-    try:
-        return XslTransformation.get_by_name(xslt_name)
-    except Exception:
-        raise exceptions.ApiError(
-            "No transformation can be found with the given name"
-        )
+    return XslTransformation.get_by_name(xslt_name)
 
 
 def get_by_id(xslt_id):
     """Get an XSLT document by its id.
 
     Args:
         xslt_id: Id.
@@ -39,15 +34,15 @@
 
     Returns:
     """
     return XslTransformation.get_all()
 
 
 def upsert(xsl_transformation):
-    """Upsert an xsl_transformation.
+    """Upsert a xsl_transformation.
 
     Args:
         xsl_transformation: XslTransformation.
 
     Returns:
         XslTransformation instance.
```

### Comparing `core_main_app-2.8.0/core_main_app/components/xsl_transformation/models.py` & `core_main_app-2.9.0/core_main_app/components/xsl_transformation/models.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/menus.py` & `core_main_app-2.9.0/core_main_app/menus.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/middleware/timezone.py` & `core_main_app-2.9.0/core_main_app/middleware/timezone.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/migrations/0001_initial.py` & `core_main_app-2.9.0/core_main_app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/migrations/0002_site_update.py` & `core_main_app-2.9.0/core_main_app/migrations/0002_site_update.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/migrations/0003_psql_full_text.py` & `core_main_app-2.9.0/core_main_app/migrations/0003_psql_full_text.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/migrations/0004_template_ordering.py` & `core_main_app-2.9.0/core_main_app/migrations/0004_template_ordering.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/migrations/0006_blob_metadata.py` & `core_main_app-2.9.0/core_main_app/migrations/0006_blob_metadata.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/migrations/0007_user_preferences.py` & `core_main_app-2.9.0/core_main_app/migrations/0007_user_preferences.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/migrations/0009_template_formats.py` & `core_main_app-2.9.0/core_main_app/migrations/0009_template_formats.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/models.py` & `core_main_app-2.9.0/core_main_app/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from django.db import models
 
 from core_main_app.permissions import rights
 from core_main_app.permissions.utils import get_formatted_name
 
 
 class Main(models.Model):
-    """Main model containing several information:
+    """Main app model:
 
     Attributes:
         Meta.verbose_name (:py:class:`str`): Name of the app.
         Meta.permissions (:py:class:`list`): Default set of permissions bundled with the app.
     """
 
     class Meta:
```

### Comparing `core_main_app-2.8.0/core_main_app/permissions/api.py` & `core_main_app-2.9.0/core_main_app/permissions/api.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/permissions/discover.py` & `core_main_app-2.9.0/core_main_app/permissions/discover.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,24 +48,29 @@
     except Exception as exception:
         logger.error("Impossible to init the rules: %s", str(exception))
 
     logger.info("FINISH init rules.")
 
 
 def create_public_workspace():
-    """Create and save a public workspace for registry. It will also create permissions.
+    """Create and save a public workspace. It will also create permissions.
 
     Returns:
     """
-    logger.info("START create public workspace.")
-
-    # We need the app to be ready to access the Group model
     from core_main_app.components.workspace import api as workspace_api
     from core_main_app.commons import exceptions
 
+    logger.info("START create public workspace.")
+
+    if Workspace.objects.count() > 0:
+        logger.warning(
+            "The database is not empty. Skipping workspace initialization."
+        )
+        return
+
     try:
         try:
             # Test if global public workspace exists
             workspace_api.get_global_workspace()
         except exceptions.DoesNotExist:
             # Create workspace public global
             workspace_api.create_and_save(
```

### Comparing `core_main_app-2.8.0/core_main_app/permissions/rights.py` & `core_main_app-2.9.0/core_main_app/permissions/rights.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/rest/blob/serializers.py` & `core_main_app-2.9.0/core_main_app/rest/blob/serializers.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,14 +68,21 @@
 
         Returns:
 
         """
         if "core_linked_records_app" not in settings.INSTALLED_APPS:
             return None
 
+        from core_linked_records_app.components.pid_settings.models import (
+            PidSettings,
+        )
+
+        if not PidSettings.get().auto_set_pid:
+            return None
+
         from core_linked_records_app.system.blob import (
             api as linked_record_blob_system_api,
         )
         from core_linked_records_app.settings import (
             ID_PROVIDER_SYSTEM_NAME,
         )
```

### Comparing `core_main_app-2.8.0/core_main_app/rest/blob/views.py` & `core_main_app-2.9.0/core_main_app/rest/blob/views.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/rest/data/abstract_views.py` & `core_main_app-2.9.0/core_main_app/rest/data/abstract_views.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/rest/data/admin_serializers.py` & `core_main_app-2.9.0/core_main_app/rest/data/admin_serializers.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/rest/data/serializers.py` & `core_main_app-2.9.0/core_main_app/rest/data/serializers.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/rest/data/views.py` & `core_main_app-2.9.0/core_main_app/rest/data/views.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/rest/mongo_data/serializers.py` & `core_main_app-2.9.0/core_main_app/rest/mongo_data/serializers.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/rest/template/serializers.py` & `core_main_app-2.9.0/core_main_app/rest/template/serializers.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/rest/template/views.py` & `core_main_app-2.9.0/core_main_app/rest/template/views.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/rest/template_version_manager/abstract_views.py` & `core_main_app-2.9.0/core_main_app/rest/template_version_manager/abstract_views.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/rest/template_version_manager/serializers.py` & `core_main_app-2.9.0/core_main_app/rest/template_version_manager/serializers.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/rest/template_version_manager/utils.py` & `core_main_app-2.9.0/core_main_app/rest/template_version_manager/utils.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/rest/template_version_manager/views.py` & `core_main_app-2.9.0/core_main_app/rest/template_version_manager/views.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/rest/template_xsl_rendering/serializers.py` & `core_main_app-2.9.0/core_main_app/rest/template_xsl_rendering/serializers.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,9 +27,8 @@
         list_detail_xslt = validated_data.get("list_detail_xslt", None)
 
         return template_xsl_rendering_api.upsert(
             template,
             list_xslt,
             default_detail_xslt,
             list_detail_xslt,
-            template_xsl_rendering_id=instance.id,
         )
```

### Comparing `core_main_app-2.8.0/core_main_app/rest/template_xsl_rendering/views.py` & `core_main_app-2.9.0/core_main_app/rest/template_xsl_rendering/views.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/rest/urls.py` & `core_main_app-2.9.0/core_main_app/rest/urls.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/rest/user/serializers.py` & `core_main_app-2.9.0/core_main_app/rest/user/serializers.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/rest/user/views.py` & `core_main_app-2.9.0/core_main_app/rest/user/views.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/rest/views.py` & `core_main_app-2.9.0/core_main_app/rest/views.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/rest/web_page/serializers.py` & `core_main_app-2.9.0/core_main_app/rest/web_page/serializers.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/rest/web_page/views.py` & `core_main_app-2.9.0/core_main_app/rest/web_page/views.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/rest/workspace/serializers.py` & `core_main_app-2.9.0/core_main_app/rest/workspace/serializers.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/rest/workspace/views.py` & `core_main_app-2.9.0/core_main_app/rest/workspace/views.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/rest/xsl_transformation/serializers.py` & `core_main_app-2.9.0/core_main_app/rest/xsl_transformation/serializers.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/rest/xsl_transformation/views.py` & `core_main_app-2.9.0/core_main_app/rest/xsl_transformation/views.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/settings.py` & `core_main_app-2.9.0/core_main_app/settings.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/static/core_main_app/admin/_theme/css/skins.css` & `core_main_app-2.9.0/core_main_app/static/core_main_app/admin/_theme/css/skins.css`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/static/core_main_app/admin/_theme/css/theme.css` & `core_main_app-2.9.0/core_main_app/static/core_main_app/admin/_theme/css/theme.css`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/static/core_main_app/admin/_theme/js/app.js` & `core_main_app-2.9.0/core_main_app/static/core_main_app/admin/_theme/js/app.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/static/core_main_app/admin/_theme/js/menu.js` & `core_main_app-2.9.0/core_main_app/static/core_main_app/admin/_theme/js/menu.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/static/core_main_app/admin/css/data_migration.css` & `core_main_app-2.9.0/core_main_app/static/core_main_app/admin/css/data_migration.css`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/static/core_main_app/admin/css/templates_xslt/form.css` & `core_main_app-2.9.0/core_main_app/static/core_main_app/admin/css/templates_xslt/form.css`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/static/core_main_app/admin/js/display_permissions.js` & `core_main_app-2.9.0/core_main_app/static/core_main_app/admin/js/display_permissions.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/static/core_main_app/admin/js/templates/data_migration.js` & `core_main_app-2.9.0/core_main_app/static/core_main_app/admin/js/templates/data_migration.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/static/core_main_app/admin/js/templates/data_migration.raw.js` & `core_main_app-2.9.0/core_main_app/static/core_main_app/admin/js/templates/data_migration.raw.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/static/core_main_app/admin/js/templates/upload/dependencies.js` & `core_main_app-2.9.0/core_main_app/static/core_main_app/admin/js/templates/upload/dependencies.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/static/core_main_app/admin/js/templates_xslt/detail_xslt.js` & `core_main_app-2.9.0/core_main_app/static/core_main_app/admin/js/templates_xslt/detail_xslt.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/static/core_main_app/common/css/XMLTree.css` & `core_main_app-2.9.0/core_main_app/static/core_main_app/common/css/XMLTree.css`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/static/core_main_app/common/css/messages.css` & `core_main_app-2.9.0/core_main_app/static/core_main_app/common/css/messages.css`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/static/core_main_app/common/css/switch.css` & `core_main_app-2.9.0/core_main_app/static/core_main_app/common/css/switch.css`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/static/core_main_app/common/js/csrf.js` & `core_main_app-2.9.0/core_main_app/static/core_main_app/common/js/csrf.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/static/core_main_app/common/js/debounce.js` & `core_main_app-2.9.0/core_main_app/static/core_main_app/common/js/debounce.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/static/core_main_app/common/js/elementViewport.js` & `core_main_app-2.9.0/core_main_app/static/core_main_app/common/js/elementViewport.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/static/core_main_app/common/js/loading_spinner.js` & `core_main_app-2.9.0/core_main_app/static/core_main_app/common/js/loading_spinner.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/static/core_main_app/common/js/messages.js` & `core_main_app-2.9.0/core_main_app/static/core_main_app/common/js/messages.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/static/core_main_app/common/js/modals/add.js` & `core_main_app-2.9.0/core_main_app/static/core_main_app/common/js/modals/add.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/static/core_main_app/common/js/modals/delete.js` & `core_main_app-2.9.0/core_main_app/static/core_main_app/common/js/modals/delete.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/static/core_main_app/common/js/modals/edit.js` & `core_main_app-2.9.0/core_main_app/static/core_main_app/common/js/modals/edit.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/static/core_main_app/common/js/templates/list/modals/disable.js` & `core_main_app-2.9.0/core_main_app/static/core_main_app/common/js/templates/list/modals/disable.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/static/core_main_app/common/js/templates/list/restore.js` & `core_main_app-2.9.0/core_main_app/static/core_main_app/common/js/templates/list/restore.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/static/core_main_app/common/js/templates/sort.js` & `core_main_app-2.9.0/core_main_app/static/core_main_app/common/js/templates/sort.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/static/core_main_app/common/js/templates/versions/modals/disable.js` & `core_main_app-2.9.0/core_main_app/static/core_main_app/common/js/templates/versions/modals/disable.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/static/core_main_app/common/js/templates/versions/restore.js` & `core_main_app-2.9.0/core_main_app/static/core_main_app/common/js/templates/versions/restore.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/static/core_main_app/common/js/templates/versions/set_current.js` & `core_main_app-2.9.0/core_main_app/static/core_main_app/common/js/templates/versions/set_current.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/static/core_main_app/common/js/xslt/list/modals/delete.js` & `core_main_app-2.9.0/core_main_app/static/core_main_app/common/js/xslt/list/modals/delete.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/static/core_main_app/common/js/xslt/list/modals/edit.js` & `core_main_app-2.9.0/core_main_app/static/core_main_app/common/js/xslt/list/modals/edit.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/static/core_main_app/common/xsl/xml2html.xsl` & `core_main_app-2.9.0/core_main_app/static/core_main_app/common/xsl/xml2html.xsl`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_444444_256x240.png` & `core_main_app-2.9.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_444444_256x240.png`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_555555_256x240.png` & `core_main_app-2.9.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_555555_256x240.png`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_777620_256x240.png` & `core_main_app-2.9.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_777620_256x240.png`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_777777_256x240.png` & `core_main_app-2.9.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_777777_256x240.png`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_cc0000_256x240.png` & `core_main_app-2.9.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_cc0000_256x240.png`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_ffffff_256x240.png` & `core_main_app-2.9.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/jquery-ui.css` & `core_main_app-2.9.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/jquery-ui.js` & `core_main_app-2.9.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/jquery-ui.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/jquery-ui.structure.css` & `core_main_app-2.9.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/jquery-ui.structure.css`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/jquery-ui.theme.css` & `core_main_app-2.9.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/jquery-ui.theme.css`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/static/core_main_app/user/css/text-editor.css` & `core_main_app-2.9.0/core_main_app/static/core_main_app/user/css/text-editor.css`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/static/core_main_app/user/js/blob/blob_metadata.js` & `core_main_app-2.9.0/core_main_app/static/core_main_app/user/js/blob/blob_metadata.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/static/core_main_app/user/js/data/change_display.js` & `core_main_app-2.9.0/core_main_app/static/core_main_app/user/js/data/change_display.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/static/core_main_app/user/js/login/message.js` & `core_main_app-2.9.0/core_main_app/static/core_main_app/user/js/login/message.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/static/core_main_app/user/js/sharing_modal.js` & `core_main_app-2.9.0/core_main_app/static/core_main_app/user/js/sharing_modal.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -6,15 +6,15 @@
     /**
      * Copy the link on clipboard and close the modal
      */
     link.prop('disabled', false);
     link.focus();
     link.select();
     navigator.clipboard.writeText(link.val()).then(function() {
-        $.notify("URL copied to clipboard successfully!", "success");
+        $.notify("URL copied to clipboard!", "success");
     }, function() {
         $.notify("A problem has occurred while copying the Url.", "danger");
     });
     link.prop('disabled', true);
 };
 
 initSharingModal = function(sharingConfigurationFunction, sharingButtonId, sharingModalId,
```

### Comparing `core_main_app-2.8.0/core_main_app/static/core_main_app/user/js/text_editor/text_editor.js` & `core_main_app-2.9.0/core_main_app/static/core_main_app/user/js/text_editor/text_editor.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -71,14 +71,17 @@
 
 
     $('.btn.display').on('click', display);
     $('.btn.format').on('click', format);
     $('.btn.refresh').on('click', refresh);
     $('.btn.validate').on('click', validate);
     $('.btn.generate').on('click', generate);
+    $('#hide-alert').on('click', function() {
+        jqError.hide()
+    });
     $('.btn.save').on('click', function() {
         if (useModal) createDataModal();
         else save();
     });
 });
 
 /**
@@ -139,15 +142,15 @@
         error: function(data) {
             let dataContent = null;
             try {
                 dataContent = JSON.parse(data.responseText);
             } catch {
                 dataContent = data.responseText;
             }
-            jqError.html(
+            $("#error_message").html(
                 `<i class="fas fa-exclamation-triangle"></i> An error occurred while saving: ${buildErrorMessage(dataContent)}`
             );
             jqError.show();
         }
     }).always(function(data) {
         // get old button icon
         hideSpinner($(".save > i"), icon)
@@ -158,35 +161,35 @@
 
 /**
  * AJAX, to  format content
  */
 let format = function() {
     if (textEditor == "Monaco" && editorFormat == "JSON") {
         editor.getAction('editor.action.formatDocument').run();
-        $.notify("Document formatted successfully", "success");
+        $.notify("Document formatted ", "success");
     } else {
         jqError.hide();
         var icon = $(".format > i").attr("class");
         // Show loading spinner
         showSpinner($(".format > i"))
         $.ajax({
             url: textEditorUrl,
             type: "POST",
             data: {
                 'content': getContent(),
                 'action': 'format',
             },
             dataType: "json",
             success: function(data) {
-                $.notify("Document formatted successfully", "success");
+                $.notify("Document formatted ", "success");
                 if (editorFormat == "JSON") data = JSON.stringify(data, null, "  ")
                 setContent(data);
             },
             error: function(data) {
-                jqError.html('<i class="fas fa-exclamation-triangle"></i> ' + data.responseText);
+                $("#error_message").html('<i class="fas fa-exclamation-triangle"></i> ' + data.responseText);
                 jqError.show();
             }
         }).always(function(data) {
             // get old button icon
             hideSpinner($(".format > i"), icon)
             refreshLineNumbers();
         });
@@ -207,24 +210,24 @@
         data: {
             'content': getContent(),
             'action': 'validate',
             'template_id': templateID,
         },
         dataType: "json",
         success: function(data) {
-            $.notify("Content validated with success", "success");
+            $.notify("Content is valid.", "success");
         },
         error: function(data) {
             let dataContent = null;
             try {
                 dataContent = JSON.parse(data.responseText);
             } catch {
                 dataContent = data.responseText;
             }
-            jqError.html(
+            $("#error_message").html(
                 `<i class="fas fa-exclamation-triangle"></i> An error occurred at validation: ${buildErrorMessage(dataContent)}`
             );
             jqError.show();
         }
     }).always(function(data) {
         // get old button icon
         hideSpinner($(".validate > i"), icon)
@@ -258,15 +261,15 @@
         type: "post",
         success: function(data) {
             $.notify("Display updated.", "success");
             $(".tree").html(data.template)
 
         },
         error: function(data) {
-            jqError.html('<i class="fas fa-exclamation-triangle"></i> ' + data.responseText);
+            $("#error_message").html('<i class="fas fa-exclamation-triangle"></i> ' + data.responseText);
             jqError.show();
         }
     }).always(function(data) {
         // get old button icon
         hideSpinner(iconSelector, icon)
     });
 };
@@ -305,19 +308,19 @@
         data: {
             'content': getContent(),
             'template_id': templateID,
             'action': 'generate',
         },
         dataType: "json",
         success: function(data) {
-            $.notify("Document generated successfully", "success");
+            $.notify("Document generated.", "success");
             setContent(data);
         },
         error: function(data) {
-            jqError.html('<i class="fas fa-exclamation-triangle"></i> ' + data.responseText);
+            $("#error_message").html('<i class="fas fa-exclamation-triangle"></i> ' + data.responseText);
             jqError.show();
 
         }
     }).always(function(data) {
         // get old button icon
         hideSpinner($(".generate > i"), icon)
         // setup line numbers
```

### Comparing `core_main_app-2.8.0/core_main_app/static/core_main_app/user/js/workspaces/add_group.js` & `core_main_app-2.9.0/core_main_app/static/core_main_app/user/js/workspaces/add_group.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/static/core_main_app/user/js/workspaces/add_user.js` & `core_main_app-2.9.0/core_main_app/static/core_main_app/user/js/workspaces/add_user.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/static/core_main_app/user/js/workspaces/create_workspace.js` & `core_main_app-2.9.0/core_main_app/static/core_main_app/user/js/workspaces/create_workspace.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/static/core_main_app/user/js/workspaces/init.js` & `core_main_app-2.9.0/core_main_app/static/core_main_app/user/js/workspaces/init.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/assign_workspace.js` & `core_main_app-2.9.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/assign_workspace.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/remove_rights.js` & `core_main_app-2.9.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/remove_rights.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/set_private.js` & `core_main_app-2.9.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/set_private.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/set_public.js` & `core_main_app-2.9.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/set_public.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/switch_right.js` & `core_main_app-2.9.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/switch_right.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/system/api.py` & `core_main_app-2.9.0/core_main_app/system/api.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/templates/core_main_app/_render/admin/app_wrapper.html` & `core_main_app-2.9.0/core_main_app/templates/core_main_app/_render/admin/app_wrapper.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/templates/core_main_app/_render/admin/theme/base.html` & `core_main_app-2.9.0/core_main_app/templates/core_main_app/_render/admin/theme/base.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/templates/core_main_app/_render/admin/theme/header.html` & `core_main_app-2.9.0/core_main_app/templates/core_main_app/_render/admin/theme/header.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/templates/core_main_app/_render/admin/theme/menu.html` & `core_main_app-2.9.0/core_main_app/templates/core_main_app/_render/admin/theme/menu.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/templates/core_main_app/_render/admin/theme/tools/box.html` & `core_main_app-2.9.0/core_main_app/templates/core_main_app/_render/admin/theme/tools/box.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/templates/core_main_app/_render/admin/theme/tools/modal.html` & `core_main_app-2.9.0/core_main_app/templates/core_main_app/_render/admin/theme/tools/modal.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/templates/core_main_app/_render/common/base_css.html` & `core_main_app-2.9.0/core_main_app/templates/core_main_app/_render/common/base_css.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/templates/core_main_app/_render/common/base_js.html` & `core_main_app-2.9.0/core_main_app/templates/core_main_app/_render/common/base_js.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/templates/core_main_app/_render/common/messages.html` & `core_main_app-2.9.0/core_main_app/templates/core_main_app/_render/common/messages.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/templates/core_main_app/_render/user/app_wrapper.html` & `core_main_app-2.9.0/core_main_app/templates/core_main_app/_render/user/app_wrapper.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/templates/core_main_app/_render/user/default.html` & `core_main_app-2.9.0/core_main_app/templates/core_main_app/_render/user/default.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/templates/core_main_app/_render/user/theme_base.html` & `core_main_app-2.9.0/core_main_app/templates/core_main_app/_render/user/theme_base.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/templates/core_main_app/admin/commons/upload/form.html` & `core_main_app-2.9.0/core_main_app/templates/core_main_app/admin/commons/upload/form.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/templates/core_main_app/admin/dependency_resolver.html` & `core_main_app-2.9.0/core_main_app/templates/core_main_app/admin/dependency_resolver.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/templates/core_main_app/admin/templates/data_migration/templates_list.html` & `core_main_app-2.9.0/core_main_app/templates/core_main_app/admin/templates/data_migration/templates_list.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/templates/core_main_app/admin/templates/list/available.html` & `core_main_app-2.9.0/core_main_app/templates/core_main_app/admin/templates/list/available.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/templates/core_main_app/admin/templates/list/disabled.html` & `core_main_app-2.9.0/core_main_app/templates/core_main_app/admin/templates/list/disabled.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/templates/core_main_app/admin/templates/list/modals/disable.html` & `core_main_app-2.9.0/core_main_app/templates/core_main_app/admin/templates/list/modals/disable.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/templates/core_main_app/admin/templates/list.html` & `core_main_app-2.9.0/core_main_app/templates/core_main_app/admin/templates/list.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/templates/core_main_app/admin/templates/versions/available.html` & `core_main_app-2.9.0/core_main_app/templates/core_main_app/admin/templates/versions/available.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/templates/core_main_app/admin/templates/versions/disabled.html` & `core_main_app-2.9.0/core_main_app/templates/core_main_app/admin/templates/versions/disabled.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/templates/core_main_app/admin/templates/versions/modals/disable.html` & `core_main_app-2.9.0/core_main_app/templates/core_main_app/admin/templates/versions/modals/disable.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/templates/core_main_app/admin/templates/versions.html` & `core_main_app-2.9.0/core_main_app/templates/core_main_app/admin/templates/versions.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/templates/core_main_app/admin/templates_xslt/main/form.html` & `core_main_app-2.9.0/core_main_app/templates/core_main_app/admin/templates_xslt/main/form.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/templates/core_main_app/admin/upload_template.html` & `core_main_app-2.9.0/core_main_app/templates/core_main_app/admin/upload_template.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/templates/core_main_app/admin/web_page/main.html` & `core_main_app-2.9.0/core_main_app/templates/core_main_app/admin/web_page/main.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/templates/core_main_app/admin/xslt/list/table.html` & `core_main_app-2.9.0/core_main_app/templates/core_main_app/admin/xslt/list/table.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/templates/core_main_app/common/blob/detail_blob.html` & `core_main_app-2.9.0/core_main_app/templates/core_main_app/common/blob/detail_blob.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/templates/core_main_app/common/blob/detail_metadata.html` & `core_main_app-2.9.0/core_main_app/templates/core_main_app/common/blob/detail_metadata.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/templates/core_main_app/common/blob/tools_blob.html` & `core_main_app-2.9.0/core_main_app/templates/core_main_app/common/blob/tools_blob.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/templates/core_main_app/common/blob/tools_metadata.html` & `core_main_app-2.9.0/core_main_app/templates/core_main_app/common/blob/tools_metadata.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/templates/core_main_app/common/commons/upload/form.html` & `core_main_app-2.9.0/core_main_app/templates/core_main_app/common/commons/upload/form.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/templates/core_main_app/common/data/detail_data.html` & `core_main_app-2.9.0/core_main_app/templates/core_main_app/common/data/detail_data.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/templates/core_main_app/common/data/tools_data.html` & `core_main_app-2.9.0/core_main_app/templates/core_main_app/common/data/tools_data.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/templates/core_main_app/common/modals/add_page_modal.html` & `core_main_app-2.9.0/core_main_app/templates/core_main_app/common/modals/add_page_modal.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/templates/core_main_app/common/modals/create_data_modal.html` & `core_main_app-2.9.0/core_main_app/templates/core_main_app/common/modals/create_data_modal.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/templates/core_main_app/common/modals/delete_page_modal.html` & `core_main_app-2.9.0/core_main_app/templates/core_main_app/common/modals/delete_page_modal.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/templates/core_main_app/common/modals/download-options.html` & `core_main_app-2.9.0/core_main_app/templates/core_main_app/common/modals/download-options.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/templates/core_main_app/common/modals/edit_page_modal.html` & `core_main_app-2.9.0/core_main_app/templates/core_main_app/common/modals/edit_page_modal.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/templates/core_main_app/common/pagination/data_source_pagination.html` & `core_main_app-2.9.0/core_main_app/templates/core_main_app/common/pagination/data_source_pagination.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/templates/core_main_app/common/templates/list/available.html` & `core_main_app-2.9.0/core_main_app/templates/core_main_app/common/templates/list/available.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/templates/core_main_app/common/templates/list/disabled.html` & `core_main_app-2.9.0/core_main_app/templates/core_main_app/common/templates/list/disabled.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/templates/core_main_app/common/templates/list/modals/disable.html` & `core_main_app-2.9.0/core_main_app/templates/core_main_app/common/templates/list/modals/disable.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/templates/core_main_app/common/templates/list/modals/edit.html` & `core_main_app-2.9.0/core_main_app/templates/core_main_app/common/templates/list/modals/edit.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/templates/core_main_app/common/templates/versions/available.html` & `core_main_app-2.9.0/core_main_app/templates/core_main_app/common/templates/versions/available.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/templates/core_main_app/common/templates/versions/modals/disable.html` & `core_main_app-2.9.0/core_main_app/templates/core_main_app/common/templates/versions/modals/disable.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/templates/core_main_app/common/templates_xslt/main/form.html` & `core_main_app-2.9.0/core_main_app/templates/core_main_app/common/templates_xslt/main/form.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/templates/core_main_app/common/xslt/list/modals/delete.html` & `core_main_app-2.9.0/core_main_app/templates/core_main_app/common/xslt/list/modals/delete.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/templates/core_main_app/common/xslt/list/modals/edit.html` & `core_main_app-2.9.0/core_main_app/templates/core_main_app/common/xslt/list/modals/edit.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/templates/core_main_app/common/xslt/list/table.html` & `core_main_app-2.9.0/core_main_app/templates/core_main_app/common/xslt/list/table.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/templates/core_main_app/user/blob/list/modals/add_metadata.html` & `core_main_app-2.9.0/core_main_app/templates/core_main_app/user/blob/list/modals/add_metadata.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/templates/core_main_app/user/blob/list/modals/file_upload.html` & `core_main_app-2.9.0/core_main_app/templates/core_main_app/user/blob/list/modals/file_upload.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/templates/core_main_app/user/login/main.html` & `core_main_app-2.9.0/core_main_app/templates/core_main_app/user/login/main.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/templates/core_main_app/user/login/modals/login_message.html` & `core_main_app-2.9.0/core_main_app/templates/core_main_app/user/login/modals/login_message.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/templates/core_main_app/user/registration/password_reset_done.html` & `core_main_app-2.9.0/core_main_app/templates/core_main_app/user/registration/password_reset_done.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/templates/core_main_app/user/sharing/modals/single-link.html` & `core_main_app-2.9.0/core_main_app/templates/core_main_app/user/sharing/modals/single-link.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/templates/core_main_app/user/text_editor/text_editor.html` & `core_main_app-2.9.0/core_main_app/templates/core_main_app/user/text_editor/text_editor.html`

 * *Files 4% similar despite different names*

```diff
@@ -13,23 +13,32 @@
 <div id="switch-to-form" class="{% if BOOTSTRAP_VERSION|first == "4" %}float-right{% elif BOOTSTRAP_VERSION|first == "5"  %}float-end{% endif %} hidden">
     <button class="btn btn-secondary switch-to-form-editor"><i class="fas fa-circle-right"></i> Switch to Form Editor </button>
 </div>
 
 <h1>Title : {{data.name}}</h1>
 
 <div class="alert alert-danger m-2" style="display: none;" role="alert">
-    <i class="fas fa-exclamation-triangle"></i>
+    <button type="button" id="hide-alert" aria-label="Close"
+            {% if BOOTSTRAP_VERSION|first == "4" %}class="close"
+            {% elif BOOTSTRAP_VERSION|first == "5" %}class="btn-close float-end"
+            {% endif %} >
+            {% if BOOTSTRAP_VERSION|first == "4" %}
+                <span aria-hidden="true">&times;</span>
+            {% elif BOOTSTRAP_VERSION|first == "5" %}
+            {% endif %}
+        </button>
+    <div id="error_message"></div>
 </div>
 
 
 
 {% if data.TEXT_EDITOR_LIBRARY == "Monaco" %}
 <div>
-        <div id="data_content" class="hidden">{{data.content}}</div>
-        <div id="container" class="border rounded input"></div>
+<div id="data_content" class="hidden">{{data.content}}</div>
+<div id="container" class="border rounded input"></div>
 {% else %}
 <div class="row text-editor-font m-1">
     <div class="border {% if BOOTSTRAP_VERSION|first == "4" %}rounded-left{% elif BOOTSTRAP_VERSION|first == "5" %}rounded-start{% endif %} bg-light line-number"></div>
     <div class="border {% if BOOTSTRAP_VERSION|first == "4" %}rounded-right{% elif BOOTSTRAP_VERSION|first == "5" %}rounded-end{% endif %} input input-text-editor col" contenteditable="true">
         <pre class="content-highlight"><code>{{data.content}}</code></pre>
     </div>
```

### Comparing `core_main_app-2.8.0/core_main_app/templates/core_main_app/user/timezone.html` & `core_main_app-2.9.0/core_main_app/templates/core_main_app/user/timezone.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/templates/core_main_app/user/workspaces/edit_rights.html` & `core_main_app-2.9.0/core_main_app/templates/core_main_app/user/workspaces/edit_rights.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/templates/core_main_app/user/workspaces/list/create_workspace.html` & `core_main_app-2.9.0/core_main_app/templates/core_main_app/user/workspaces/list/create_workspace.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/templates/core_main_app/user/workspaces/list/edit_rights_table.html` & `core_main_app-2.9.0/core_main_app/templates/core_main_app/user/workspaces/list/edit_rights_table.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/add_group.html` & `core_main_app-2.9.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/add_group.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/add_user.html` & `core_main_app-2.9.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/add_user.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/assign_workspace.html` & `core_main_app-2.9.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/assign_workspace.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/remove_rights.html` & `core_main_app-2.9.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/remove_rights.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/set_private.html` & `core_main_app-2.9.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/set_private.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/set_public.html` & `core_main_app-2.9.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/set_public.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/switch_right.html` & `core_main_app-2.9.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/switch_right.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/templatetags/auth_extras.py` & `core_main_app-2.9.0/core_main_app/templatetags/auth_extras.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/templatetags/blob_tags.py` & `core_main_app-2.9.0/core_main_app/templatetags/blob_tags.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/templatetags/get_attribute.py` & `core_main_app-2.9.0/core_main_app/templatetags/get_attribute.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/templatetags/include_static.py` & `core_main_app-2.9.0/core_main_app/templatetags/include_static.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/templatetags/json_date.py` & `core_main_app-2.9.0/core_main_app/templatetags/json_date.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/templatetags/stripjs.py` & `core_main_app-2.9.0/core_main_app/templatetags/stripjs.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/templatetags/xsl_transform_tag.py` & `core_main_app-2.9.0/core_main_app/templatetags/xsl_transform_tag.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/urls.py` & `core_main_app-2.9.0/core_main_app/urls.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/utils/admin_site/model_admin_class.py` & `core_main_app-2.9.0/core_main_app/utils/admin_site/model_admin_class.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/utils/blob_downloader.py` & `core_main_app-2.9.0/core_main_app/utils/blob_downloader.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/utils/checksum.py` & `core_main_app-2.9.0/core_main_app/utils/checksum.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/utils/custom_context_processors.py` & `core_main_app-2.9.0/core_main_app/utils/custom_context_processors.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/utils/databases/backend.py` & `core_main_app-2.9.0/core_main_app/utils/databases/backend.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/utils/databases/mongo/__init__.py` & `core_main_app-2.9.0/core_main_app/utils/databases/mongo/__init__.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/utils/databases/mongo/pymongo_database.py` & `core_main_app-2.9.0/core_main_app/utils/databases/mongo/pymongo_database.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/utils/decorators.py` & `core_main_app-2.9.0/core_main_app/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/utils/file.py` & `core_main_app-2.9.0/core_main_app/utils/file.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/utils/integration_tests/integration_base_test_case.py` & `core_main_app-2.9.0/core_main_app/utils/integration_tests/integration_base_test_case.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/utils/integration_tests/integration_base_transaction_test_case.py` & `core_main_app-2.9.0/core_main_app/utils/integration_tests/integration_base_transaction_test_case.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/utils/json_utils.py` & `core_main_app-2.9.0/core_main_app/utils/json_utils.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/utils/logger/logger_utils.py` & `core_main_app-2.9.0/core_main_app/utils/logger/logger_utils.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/utils/migrations.py` & `core_main_app-2.9.0/core_main_app/utils/migrations.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/utils/notifications/mail.py` & `core_main_app-2.9.0/core_main_app/utils/notifications/mail.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/utils/notifications/tasks/task_mail.py` & `core_main_app-2.9.0/core_main_app/utils/notifications/tasks/task_mail.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/utils/pagination/django_paginator/results_paginator.py` & `core_main_app-2.9.0/core_main_app/utils/pagination/django_paginator/results_paginator.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/utils/pagination/mongoengine_paginator/paginator.py` & `core_main_app-2.9.0/core_main_app/utils/pagination/mongoengine_paginator/paginator.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/utils/pagination/rest_framework_paginator/pagination.py` & `core_main_app-2.9.0/core_main_app/utils/pagination/rest_framework_paginator/pagination.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/utils/pagination/rest_framework_paginator/rest_framework_paginator.py` & `core_main_app-2.9.0/core_main_app/utils/pagination/rest_framework_paginator/rest_framework_paginator.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/utils/query/mongo/prepare.py` & `core_main_app-2.9.0/core_main_app/utils/query/mongo/prepare.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/utils/query/mongo/query_builder.py` & `core_main_app-2.9.0/core_main_app/utils/query/mongo/query_builder.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/utils/raw_query/common.py` & `core_main_app-2.9.0/core_main_app/utils/raw_query/common.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/utils/raw_query/django_raw_query.py` & `core_main_app-2.9.0/core_main_app/utils/raw_query/django_raw_query.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/utils/raw_query/mongo_raw_query.py` & `core_main_app-2.9.0/core_main_app/utils/raw_query/mongo_raw_query.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/utils/rendering.py` & `core_main_app-2.9.0/core_main_app/utils/rendering.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/utils/requests_utils/access_control.py` & `core_main_app-2.9.0/core_main_app/utils/requests_utils/access_control.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/utils/requests_utils/requests_utils.py` & `core_main_app-2.9.0/core_main_app/utils/requests_utils/requests_utils.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/utils/requests_utils/ssl.py` & `core_main_app-2.9.0/core_main_app/utils/requests_utils/ssl.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/utils/resolvers/requests_resolver.py` & `core_main_app-2.9.0/core_main_app/utils/resolvers/requests_resolver.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/utils/resolvers/resolver_utils.py` & `core_main_app-2.9.0/core_main_app/utils/resolvers/resolver_utils.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/utils/routers/db_router.py` & `core_main_app-2.9.0/core_main_app/utils/routers/db_router.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/utils/saml2/utils.py` & `core_main_app-2.9.0/core_main_app/utils/saml2/utils.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/utils/settings.py` & `core_main_app-2.9.0/core_main_app/utils/settings.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/utils/storage/gridfs_storage.py` & `core_main_app-2.9.0/core_main_app/utils/storage/gridfs_storage.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/utils/storage/storage.py` & `core_main_app-2.9.0/core_main_app/utils/storage/storage.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/utils/tests_tools/MockUser.py` & `core_main_app-2.9.0/core_main_app/utils/tests_tools/MockUser.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/utils/tests_tools/RequestMock.py` & `core_main_app-2.9.0/core_main_app/utils/tests_tools/RequestMock.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/utils/tests_tools/databases/mongo/mongoengine_database.py` & `core_main_app-2.9.0/core_main_app/utils/tests_tools/databases/mongo/mongoengine_database.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/utils/urls.py` & `core_main_app-2.9.0/core_main_app/utils/urls.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/utils/validation/regex_validation.py` & `core_main_app-2.9.0/core_main_app/utils/validation/regex_validation.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/utils/validation/xpath_validation.py` & `core_main_app-2.9.0/core_main_app/utils/validation/xpath_validation.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/utils/view_builders/data.py` & `core_main_app-2.9.0/core_main_app/utils/view_builders/data.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/utils/xml.py` & `core_main_app-2.9.0/core_main_app/utils/xml.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/utils/xsd_flattener/xsd_flattener_database_url.py` & `core_main_app-2.9.0/core_main_app/utils/xsd_flattener/xsd_flattener_database_url.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/utils/xsd_flattener/xsd_flattener_requests_url.py` & `core_main_app-2.9.0/core_main_app/utils/xsd_flattener/xsd_flattener_requests_url.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/views/admin/ajax.py` & `core_main_app-2.9.0/core_main_app/views/admin/ajax.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,15 @@
 
 class EditXSLTView(EditObjectModalView):
     """Edit XSLT View"""
 
     form_class = EditXSLTForm
     model = XslTransformation
     success_url = reverse_lazy("core-admin:core_main_app_xslt")
-    success_message = "XSLT edited with success."
+    success_message = "XSLT edited."
 
     def _save(self, form):
         # Save treatment.
         try:
             xsl_transformation_api.upsert(self.object)
         except NotUniqueError:
             form.add_error(
@@ -133,13 +133,13 @@
 
 
 class DeleteXSLTView(DeleteObjectModalView):
     """Delete XSLT View"""
 
     model = XslTransformation
     success_url = reverse_lazy("core-admin:core_main_app_xslt")
-    success_message = "XSLT deleted with success."
+    success_message = "XSLT deleted."
     field_for_name = "name"
 
     def _delete(self, form):
         # Delete treatment.
         xsl_transformation_api.delete(self.object)
```

### Comparing `core_main_app-2.8.0/core_main_app/views/admin/forms.py` & `core_main_app-2.9.0/core_main_app/views/admin/forms.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/views/admin/views.py` & `core_main_app-2.9.0/core_main_app/views/admin/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -686,15 +686,15 @@
             if page is None:
                 page = WebPage(type=self.web_page_type, content=content)
             else:
                 page.content = content
 
             self.api.upsert(page)
             messages.add_message(
-                request, messages.SUCCESS, "Information saved with success."
+                request, messages.SUCCESS, "Information saved."
             )
 
             return redirect(reverse(self.post_redirect))
 
 
 @staff_member_required
 def data_migration(request):
```

### Comparing `core_main_app-2.8.0/core_main_app/views/common/ajax.py` & `core_main_app-2.9.0/core_main_app/views/common/ajax.py`

 * *Files 1% similar despite different names*

```diff
@@ -268,15 +268,15 @@
 
 
 @method_decorator(login_required, name="dispatch")
 class EditTemplateVersionManagerView(EditObjectModalView):
     form_class = EditTemplateForm
     model = TemplateVersionManager
     success_url = reverse_lazy("core-admin:core_main_app_templates")
-    success_message = "Name edited with success."
+    success_message = "Name edited."
 
     def _save(self, form):
         # Save treatment.
         try:
             template_version_manager_api.edit_title(
                 self.object,
                 form.cleaned_data.get("title"),
```

### Comparing `core_main_app-2.8.0/core_main_app/views/common/views.py` & `core_main_app-2.9.0/core_main_app/views/common/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -478,15 +478,14 @@
 
             # Get template by id
             template = template_api.get_by_id(
                 request.POST.get("template"), request=request
             )
 
             template_xsl_rendering_api.add_or_delete(
-                template_xsl_rendering_id=request.POST.get("id"),
                 template=template,
                 list_xslt=list_xslt,
                 default_detail_xslt=default_detail_xslt,
                 list_detail_xslt=list_detail_xslt,
             )
 
             return HttpResponseRedirect(
@@ -828,15 +827,15 @@
         # validate content
         error = main_xml_utils.validate_xml_data(
             xsd_tree, xml_tree, request=self.request
         )
         if error is not None:
             raise exceptions.XMLError(error)
         return HttpResponse(
-            json.dumps("Validated successfully"),
+            json.dumps("Document is valid"),
             "application/javascript",
         )
 
     def generate(self, *args, **kwargs):
         """Generate xml content
 
         Args:
@@ -1034,15 +1033,15 @@
                     ]
                 )
             )
         except Exception as exc:
             raise JSONError(str(exc))
 
         return HttpResponse(
-            json.dumps("Validated successfully"),
+            json.dumps("Document is valid"),
             "application/javascript",
         )
 
     def _get_assets(self):
         """get assets
 
         Return:
@@ -1165,18 +1164,23 @@
             data.content = content
             # save data
             data_api.upsert(data, request)
             lock_api.remove_lock_on_object(data, request.user)
             messages.add_message(
                 request,
                 messages.SUCCESS,
-                get_data_label().capitalize() + " saved with success.",
+                get_data_label().capitalize() + " saved.",
+            )
+            reverse_url = (
+                reverse("core_dashboard_records")
+                if "core_dashboard_common_app" in conf_settings.INSTALLED_APPS
+                else reverse("core_main_app_homepage")
             )
             return HttpResponse(
-                json.dumps({"url": reverse("core_main_app_homepage")}),
+                json.dumps({"url": reverse_url}),
                 "application/javascript",
             )
         except AccessControlError as ace:
             return HttpResponseForbidden(html_escape(str(ace)))
         except DoesNotExist as dne:
             return HttpResponseBadRequest(html_escape(str(dne)))
         except Exception as e:
@@ -1313,15 +1317,15 @@
         error = main_xml_utils.validate_xml_schema(
             xsd_tree, request=self.request
         )
         if error is not None:
             raise exceptions.XMLError(error)
 
         return HttpResponse(
-            json.dumps("Validated successfully"),
+            json.dumps("Document is valid"),
             "application/javascript",
         )
 
 
 class DataJSONEditor(DataMixin, JSONEditor):
     """JSON Editor View"""
 
@@ -1355,15 +1359,15 @@
         try:
             # validate content
             is_schema_valid(content)
         except Exception as e:
             raise JSONError(str(e))
 
         return HttpResponse(
-            json.dumps("Validated successfully"),
+            json.dumps("Document is valid"),
             "application/javascript",
         )
 
 
 class ViewBlob(CommonView):
     """
     View blob.
```

### Comparing `core_main_app-2.8.0/core_main_app/views/user/ajax.py` & `core_main_app-2.9.0/core_main_app/views/user/ajax.py`

 * *Files 0% similar despite different names*

```diff
@@ -670,15 +670,15 @@
             return HttpResponseBadRequest("Permission denied.")
         except Exception:
             return HttpResponseBadRequest("An unexpected error occurred.")
 
         messages.add_message(
             request,
             messages.INFO,
-            "Metadata successfully removed.",
+            "Metadata removed.",
         )
         return HttpResponse(json.dumps({}), "application/javascript")
 
 
 @method_decorator(login_required, name="dispatch")
 class UploadFile(View):
     """Upload file"""
@@ -700,15 +700,15 @@
                     blob=form.files["file"],
                     user_id=str(request.user.id),
                 )
                 blob_api.insert(blob, request.user)
                 messages.add_message(
                     request,
                     messages.SUCCESS,
-                    "File successfully uploaded.",
+                    "File uploaded.",
                 )
                 return HttpResponse(json.dumps({}))
             else:
                 return HttpResponseBadRequest(
                     json.dumps({"message": str(form.errors.as_text())})
                 )
         except Exception:
```

### Comparing `core_main_app-2.8.0/core_main_app/views/user/forms.py` & `core_main_app-2.9.0/core_main_app/views/user/forms.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app/views/user/views.py` & `core_main_app-2.9.0/core_main_app/views/user/views.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/core_main_app.egg-info/PKG-INFO` & `core_main_app-2.9.0/core_main_app.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: core-main-app
-Version: 2.8.0
+Version: 2.9.0
 Summary: Main functionalities for the curator core project
 Home-page: https://github.com/usnistgov/core_main_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: =============
         Core Main App
```

### Comparing `core_main_app-2.8.0/core_main_app.egg-info/SOURCES.txt` & `core_main_app-2.9.0/core_main_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/docs/conf.py` & `core_main_app-2.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/setup.py` & `core_main_app-2.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_main_app",
-    version="2.8.0",
+    version="2.9.0",
     description="Main functionalities for the curator core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_main_app",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `core_main_app-2.8.0/tests/access_control/api/tests_unit.py` & `core_main_app-2.9.0/tests/access_control/api/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/access_control/tests_access_control.py` & `core_main_app-2.9.0/tests/access_control/tests_access_control.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/access_control/utils/tests_unit.py` & `core_main_app-2.9.0/tests/access_control/utils/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/commons/exceptions/test_unit.py` & `core_main_app-2.9.0/tests/commons/exceptions/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/commons/validators/test_unit.py` & `core_main_app-2.9.0/tests/commons/validators/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/components/blob/fixtures/fixtures.py` & `core_main_app-2.9.0/tests/components/blob/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/components/blob/tests_int.py` & `core_main_app-2.9.0/tests/components/blob/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/components/blob/tests_int_access_control.py` & `core_main_app-2.9.0/tests/components/blob/tests_int_access_control.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/components/blob/tests_unit.py` & `core_main_app-2.9.0/tests/components/blob/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/components/data/access_control/tests_unit.py` & `core_main_app-2.9.0/tests/components/data/access_control/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/components/data/fixtures/fixtures.py` & `core_main_app-2.9.0/tests/components/data/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/components/data/tests_int.py` & `core_main_app-2.9.0/tests/components/data/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/components/data/tests_int_access_control.py` & `core_main_app-2.9.0/tests/components/data/tests_int_access_control.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/components/data/tests_int_ordering.py` & `core_main_app-2.9.0/tests/components/data/tests_int_ordering.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/components/data/tests_unit.py` & `core_main_app-2.9.0/tests/components/data/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/components/group/fixtures/fixtures.py` & `core_main_app-2.9.0/tests/components/group/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/components/group/fixtures/tests_int.py` & `core_main_app-2.9.0/tests/components/group/fixtures/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/components/group/tests_int.py` & `core_main_app-2.9.0/tests/components/group/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/components/lock/tests_int.py` & `core_main_app-2.9.0/tests/components/lock/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/components/lock/tests_unit.py` & `core_main_app-2.9.0/tests/components/lock/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/components/mongo_data/tests_int_access_control.py` & `core_main_app-2.9.0/tests/components/mongo_data/tests_int_access_control.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/components/mongo_data/tests_unit.py` & `core_main_app-2.9.0/tests/components/mongo_data/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/components/template/fixtures/fixtures.py` & `core_main_app-2.9.0/tests/components/template/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/components/template/tests_int_access_control.py` & `core_main_app-2.9.0/tests/components/template/tests_int_access_control.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/components/template/tests_unit.py` & `core_main_app-2.9.0/tests/components/template/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/components/template_version_manager/fixtures/fixtures.py` & `core_main_app-2.9.0/tests/components/template_version_manager/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/components/template_version_manager/tests_int_access_control.py` & `core_main_app-2.9.0/tests/components/template_version_manager/tests_int_access_control.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/components/template_version_manager/tests_unit.py` & `core_main_app-2.9.0/tests/components/template_version_manager/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/components/template_xsl_rendering/fixtures/fixtures.py` & `core_main_app-2.9.0/tests/components/template_xsl_rendering/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/components/template_xsl_rendering/tests_int.py` & `core_main_app-2.9.0/tests/components/template_xsl_rendering/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/components/template_xsl_rendering/tests_unit.py` & `core_main_app-2.9.0/tests/components/template_xsl_rendering/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/components/user/fixtures/fixtures.py` & `core_main_app-2.9.0/tests/components/user/fixtures/fixtures.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             is_staff=is_staff,
         )
         user.save()
         return user
 
     @staticmethod
     def create_super_user(username="username", password="pass", email="email"):
-        """create super user
+        """create superuser
 
         Args:
             username:
             password:
             email:
 
         Returns:
```

### Comparing `core_main_app-2.8.0/tests/components/user/fixtures/tests_int.py` & `core_main_app-2.9.0/tests/components/user/fixtures/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/components/user/tests_int.py` & `core_main_app-2.9.0/tests/components/user/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/components/user_preferences/fixtures/fixtures.py` & `core_main_app-2.9.0/tests/components/user_preferences/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/components/user_preferences/tests_int.py` & `core_main_app-2.9.0/tests/components/user_preferences/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/components/user_preferences/tests_int_access_control.py` & `core_main_app-2.9.0/tests/components/user_preferences/tests_int_access_control.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/components/user_preferences/tests_unit.py` & `core_main_app-2.9.0/tests/components/user_preferences/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/components/version_manager/tests_int_access_control.py` & `core_main_app-2.9.0/tests/components/version_manager/tests_int_access_control.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/components/version_manager/tests_unit.py` & `core_main_app-2.9.0/tests/components/version_manager/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/components/web_page/tests_unit.py` & `core_main_app-2.9.0/tests/components/web_page/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/components/web_page_login/tests_unit.py` & `core_main_app-2.9.0/tests/components/web_page_login/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/components/workspace/fixtures/fixtures.py` & `core_main_app-2.9.0/tests/components/workspace/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/components/workspace/fixtures/tests_int.py` & `core_main_app-2.9.0/tests/components/workspace/fixtures/tests_int.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,16 +18,18 @@
         """test create workspace
 
         Returns:
 
         """
         # Context
         workspace_count = len(workspace_api.get_all())
-        self.assertEqual(workspace_count, 0)
+        self.assertEqual(workspace_count, 1)
 
         # Act
         WorkspaceFixtures().create_workspace("1", TITLE)
 
         # Assert
         list_workspace = workspace_api.get_all()
-        self.assertEqual(list_workspace[0].title, TITLE)
+        self.assertTrue(
+            TITLE in [workspace.title for workspace in list_workspace]
+        )
         self.assertEqual(len(list_workspace), workspace_count + 1)
```

### Comparing `core_main_app-2.8.0/tests/components/workspace/tests_int.py` & `core_main_app-2.9.0/tests/components/workspace/tests_int.py`

 * *Files 3% similar despite different names*

```diff
@@ -121,45 +121,29 @@
 
     def test_get_global_workspace(self):
         """test get global workspace
 
         Returns:
 
         """
-        # Context
-        workspace = WorkspaceFixtures.create_global_workspace(TITLE_1)
         # Act
-        result = workspace_api.get_global_workspace()
+        workspace = workspace_api.get_global_workspace()
         # Assert
-        self.assertEqual(workspace, result)
+        self.assertTrue(workspace.title == "Global Public Workspace")
 
     def test_get_global_workspace_multiple_workspace(self):
         """test get global workspace multiple workspace
 
         Returns:
 
         """
         # Context
-        global_workspace = WorkspaceFixtures.create_global_workspace(TITLE_1)
-        WorkspaceFixtures.create_workspace("1", TITLE_1)
-        # Act
-        result = workspace_api.get_global_workspace()
-        # Assert
-        self.assertEqual(global_workspace, result)
-
-    def test_get_global_workspace_not_global(self):
-        """test get global workspace not global
-
-        Returns:
-
-        """
-        # Context
-        WorkspaceFixtures.create_workspace("1", TITLE_1)
-        # Act
-        with self.assertRaises(exceptions.DoesNotExist):
+        WorkspaceFixtures.create_global_workspace(TITLE_1)
+        # Act + Assert
+        with self.assertRaises(exceptions.ModelError):
             workspace_api.get_global_workspace()
 
 
 class TestCheckIfWorkspaceCanBeChanged(IntegrationTransactionTestCase):
     """Test Check If Workspace Can Be Changed"""
 
     def test_workspace_can_be_changed_return_true_if_workspace_is_none_and_allow_public_is_false(
```

### Comparing `core_main_app-2.8.0/tests/components/xsl_transformation/tests_unit.py` & `core_main_app-2.9.0/tests/components/xsl_transformation/tests_unit.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,20 +51,20 @@
         Args:
             mock_get_by_name:
 
         Returns:
 
         """
         # Arrange
-        mock_unexisting_name = "unexisting_xslt_name"
-        mock_get_by_name.side_effect = Exception()
+        mock_bad_name = "bad_xslt_name"
+        mock_get_by_name.side_effect = exceptions.DoesNotExist("error")
 
         # Act + Assert
-        with self.assertRaises(exceptions.ApiError):
-            xsl_transformation_api.get_by_name(mock_unexisting_name)
+        with self.assertRaises(exceptions.DoesNotExist):
+            xsl_transformation_api.get_by_name(mock_bad_name)
 
 
 class TestXslTransformationGetById(TestCase):
     """TestXslTransformationGetById"""
 
     @patch.object(XslTransformation, "get_by_id")
     def test_xsl_transformation_get_by_id_raises_api_error_if_does_not_exisst(
```

### Comparing `core_main_app-2.8.0/tests/middleware/tests_unit.py` & `core_main_app-2.9.0/tests/middleware/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/rest/blob/tests_int.py` & `core_main_app-2.9.0/tests/rest/blob/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/rest/blob/tests_permissions.py` & `core_main_app-2.9.0/tests/rest/blob/tests_permissions.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/rest/data/tests_int.py` & `core_main_app-2.9.0/tests/rest/data/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/rest/data/tests_permissions.py` & `core_main_app-2.9.0/tests/rest/data/tests_permissions.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/rest/data/tests_unit.py` & `core_main_app-2.9.0/tests/rest/data/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/rest/template/tests_int.py` & `core_main_app-2.9.0/tests/rest/template/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/rest/template/tests_permission.py` & `core_main_app-2.9.0/tests/rest/template/tests_permission.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/rest/template/tests_unit.py` & `core_main_app-2.9.0/tests/rest/template/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/rest/template_version_manager/tests_int.py` & `core_main_app-2.9.0/tests/rest/template_version_manager/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/rest/template_version_manager/tests_permission.py` & `core_main_app-2.9.0/tests/rest/template_version_manager/tests_permission.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/rest/template_version_manager/tests_unit.py` & `core_main_app-2.9.0/tests/rest/template_version_manager/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/rest/template_xsl_rendering/tests_int.py` & `core_main_app-2.9.0/tests/rest/template_xsl_rendering/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/rest/template_xsl_rendering/tests_permissions.py` & `core_main_app-2.9.0/tests/rest/template_xsl_rendering/tests_permissions.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/rest/tests_views.py` & `core_main_app-2.9.0/tests/rest/tests_views.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/rest/user/tests_int.py` & `core_main_app-2.9.0/tests/rest/user/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/rest/user/tests_permissions.py` & `core_main_app-2.9.0/tests/rest/user/tests_permissions.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/rest/user/tests_unit.py` & `core_main_app-2.9.0/tests/rest/user/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/rest/web_page/tests_permission.py` & `core_main_app-2.9.0/tests/rest/web_page/tests_permission.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/rest/workspace/tests_int.py` & `core_main_app-2.9.0/tests/rest/workspace/tests_int.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """ Integration Test for Workspace Rest API
 """
-
+from django.contrib.auth.models import Group
 from rest_framework import status
 from tests.components.group.fixtures.fixtures import GroupFixtures
 from tests.components.user.fixtures.fixtures import UserFixtures
 from tests.components.workspace.fixtures.fixtures import WorkspaceFixtures
 
 from core_main_app.components.workspace import api as workspace_api
+from core_main_app.permissions import rights
 from core_main_app.rest.workspace import views as workspace_rest_views
 from core_main_app.utils.integration_tests.integration_base_transaction_test_case import (
     IntegrationTransactionTestCase,
 )
 from core_main_app.utils.tests_tools.RequestMock import RequestMock
 
 TITLE_1 = "title 1"
@@ -221,25 +222,26 @@
         Returns:
 
         """
         # Context
         user = UserFixtures().create_super_user(username="user1")
         other_user = UserFixtures().create_user(username="user2")
 
+        workspace_count = len(workspace_api.get_all())
         WorkspaceFixtures().create_workspace(user.id, TITLE_1)
         WorkspaceFixtures().create_workspace(user.id, TITLE_2)
         WorkspaceFixtures().create_workspace(other_user.id, TITLE_3)
 
         # Act
         response = RequestMock.do_request_get(
             workspace_rest_views.WorkspaceList.as_view(), user
         )
 
         # Assert
-        self.assertEqual(len(response.data), 3)
+        self.assertEqual(len(response.data), workspace_count + 3)
 
     def test_post_returns_http_201(self):
         """test_post_returns_http_201
 
         Returns:
 
         """
@@ -350,15 +352,17 @@
 
         # Act
         response = RequestMock.do_request_get(
             workspace_rest_views.get_workspaces_with_read_access, user
         )
 
         # Assert
-        self.assertEqual(response.data[0]["title"], TITLE_1)
+        self.assertTrue(
+            TITLE_1 in [workspace["title"] for workspace in response.data]
+        )
 
     def test_get_workspace_with_read_access_admin(self):
         """test_get_workspace_with_read_access_admin
 
         Returns:
 
         """
@@ -369,15 +373,17 @@
 
         # Act
         response = RequestMock.do_request_get(
             workspace_rest_views.get_workspaces_with_read_access, user2
         )
 
         # Assert
-        self.assertEqual(response.data[0]["title"], TITLE_1)
+        self.assertTrue(
+            TITLE_1 in [workspace["title"] for workspace in response.data]
+        )
 
     def test_get_workspace_with_read_access_other_workspace(self):
         """test_get_workspace_with_read_access_other_workspace
 
         Returns:
 
         """
@@ -389,15 +395,17 @@
 
         # Act
         response = RequestMock.do_request_get(
             workspace_rest_views.get_workspaces_with_read_access, user2
         )
 
         # Assert
-        self.assertEqual(response.data[0]["title"], TITLE_1)
+        self.assertTrue(
+            TITLE_1 in [workspace["title"] for workspace in response.data]
+        )
 
     def test_get_workspace_with_read_access_public_workspace(self):
         """test_get_workspace_with_read_access_public_workspace
 
         Returns:
 
         """
@@ -410,15 +418,17 @@
 
         # Act
         response = RequestMock.do_request_get(
             workspace_rest_views.get_workspaces_with_read_access, user2
         )
 
         # Assert
-        self.assertEqual(response.data[0]["title"], TITLE_1)
+        self.assertTrue(
+            TITLE_1 in [workspace["title"] for workspace in response.data]
+        )
 
 
 class TestWorkspaceWriteAccess(IntegrationTransactionTestCase):
     """Test Workspace Write Access"""
 
     def test_get_workspace_with_write_access_return_http_200(self):
         """test_get_workspace_with_write_access_return_http_200
@@ -468,15 +478,17 @@
 
         # Act
         response = RequestMock.do_request_get(
             workspace_rest_views.get_workspaces_with_write_access, user2
         )
 
         # Assert
-        self.assertEqual(response.data[0]["title"], TITLE_1)
+        self.assertTrue(
+            TITLE_1 in [workspace["title"] for workspace in response.data]
+        )
 
     def test_get_workspace_with_write_access_other_workspace(self):
         """test_get_workspace_with_write_access_other_workspace
 
         Returns:
 
         """
@@ -632,14 +644,16 @@
 
         Returns:
 
         """
         # Context
         user = UserFixtures().create_user(username="user1")
         workspace = WorkspaceFixtures().create_workspace(user.id, TITLE_1)
+        default_group = Group.objects.get(name=rights.DEFAULT_GROUP)
+        default_group.user_set.remove(user)
 
         # Act
         response = RequestMock.do_request_patch(
             workspace_rest_views.set_workspace_public,
             user,
             param={"pk": workspace.id},
         )
```

### Comparing `core_main_app-2.8.0/tests/rest/workspace/tests_permissions.py` & `core_main_app-2.9.0/tests/rest/workspace/tests_permissions.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/rest/xsl_transformation/fixtures/fixtures.py` & `core_main_app-2.9.0/tests/rest/xsl_transformation/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/rest/xsl_transformation/tests_int.py` & `core_main_app-2.9.0/tests/rest/xsl_transformation/tests_int.py`

 * *Files 1% similar despite different names*

```diff
@@ -277,16 +277,16 @@
         )
 
         # Assert
         self.assertEqual(
             response.status_code, status.HTTP_500_INTERNAL_SERVER_ERROR
         )
 
-    def test_post_return_204_if_document_is_deleted_whit_success(self):
-        """test_post_return_204_if_document_is_deleted_whit_success
+    def test_post_return_204_if_document_is_deleted_with_success(self):
+        """test_post_return_204_if_document_is_deleted_with_success
 
         Returns:
 
         """
         # Arrange
         user = create_mock_user("0", True, True)
         self.param = {"pk": self.fixture.data_1.id}
```

### Comparing `core_main_app-2.8.0/tests/rest/xsl_transformation/tests_permission.py` & `core_main_app-2.9.0/tests/rest/xsl_transformation/tests_permission.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/rest/xsl_transformation/tests_unit.py` & `core_main_app-2.9.0/tests/rest/xsl_transformation/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/rest_urls.py` & `core_main_app-2.9.0/tests/rest_urls.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/system/blob/api/tests_unit.py` & `core_main_app-2.9.0/tests/system/blob/api/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/system/test_unit.py` & `core_main_app-2.9.0/tests/system/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/templatetags/auth_extras/tests_unit.py` & `core_main_app-2.9.0/tests/templatetags/auth_extras/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/templatetags/test_blob_tags.py` & `core_main_app-2.9.0/tests/templatetags/test_blob_tags.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/templatetags/test_format_json.py` & `core_main_app-2.9.0/tests/templatetags/test_format_json.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/templatetags/test_get_attribute.py` & `core_main_app-2.9.0/tests/templatetags/test_get_attribute.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/templatetags/test_parse_date.py` & `core_main_app-2.9.0/tests/templatetags/test_parse_date.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/test_settings.py` & `core_main_app-2.9.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/urls.py` & `core_main_app-2.9.0/tests/urls.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/utils/checksum/tests_checksum.py` & `core_main_app-2.9.0/tests/utils/checksum/tests_checksum.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/utils/dict/tests_unit.py` & `core_main_app-2.9.0/tests/utils/dict/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/utils/json_utils/tests_unit.py` & `core_main_app-2.9.0/tests/utils/json_utils/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/utils/migrations/tests_unit.py` & `core_main_app-2.9.0/tests/utils/migrations/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/utils/query/mongo/tests_unit.py` & `core_main_app-2.9.0/tests/utils/query/mongo/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/utils/requests_utls/tests_ssl.py` & `core_main_app-2.9.0/tests/utils/requests_utls/tests_ssl.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/utils/routers/tests_db_router.py` & `core_main_app-2.9.0/tests/utils/routers/tests_db_router.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/utils/settings/tests_unit.py` & `core_main_app-2.9.0/tests/utils/settings/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/utils/test_unit_apps.py` & `core_main_app-2.9.0/tests/utils/test_unit_apps.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/utils/test_unit_urls.py` & `core_main_app-2.9.0/tests/utils/test_unit_urls.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/utils/tests_int_blob_downloader.py` & `core_main_app-2.9.0/tests/utils/tests_int_blob_downloader.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/utils/tests_int_file.py` & `core_main_app-2.9.0/tests/utils/tests_int_file.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/utils/tests_unit_admin_site.py` & `core_main_app-2.9.0/tests/utils/tests_unit_admin_site.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/utils/tests_unit_boolean.py` & `core_main_app-2.9.0/tests/utils/tests_unit_boolean.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/utils/tests_unit_xml_operation.py` & `core_main_app-2.9.0/tests/utils/tests_unit_xml_operation.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/utils/tests_view_data.py` & `core_main_app-2.9.0/tests/utils/tests_view_data.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/utils/validation/tests_unit_validation.py` & `core_main_app-2.9.0/tests/utils/validation/tests_unit_validation.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/utils/xsd_flattener/tests_unit.py` & `core_main_app-2.9.0/tests/utils/xsd_flattener/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/views/admin/ajax/test_unit.py` & `core_main_app-2.9.0/tests/views/admin/ajax/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/views/admin/forms/test_unit.py` & `core_main_app-2.9.0/tests/views/admin/forms/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/views/admin/views/test_unit.py` & `core_main_app-2.9.0/tests/views/admin/views/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/views/common/ajax/tests_unit.py` & `core_main_app-2.9.0/tests/views/common/ajax/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/views/common/views/test_unit.py` & `core_main_app-2.9.0/tests/views/common/views/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/views/fixtures.py` & `core_main_app-2.9.0/tests/views/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/views/tests_int_access_control.py` & `core_main_app-2.9.0/tests/views/tests_int_access_control.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/views/tests_permissions.py` & `core_main_app-2.9.0/tests/views/tests_permissions.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/views/user/forms/test_unit.py` & `core_main_app-2.9.0/tests/views/user/forms/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.8.0/tests/views/user/views/test_unit.py` & `core_main_app-2.9.0/tests/views/user/views/test_unit.py`

 * *Files identical despite different names*

