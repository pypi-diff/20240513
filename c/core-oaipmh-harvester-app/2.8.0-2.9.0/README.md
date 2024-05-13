# Comparing `tmp/core_oaipmh_harvester_app-2.8.0.tar.gz` & `tmp/core_oaipmh_harvester_app-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_oaipmh_harvester_app-2.8.0.tar", last modified: Tue Mar 12 19:06:04 2024, max compression
+gzip compressed data, was "core_oaipmh_harvester_app-2.9.0.tar", last modified: Mon May 13 16:11:09 2024, max compression
```

## Comparing `core_oaipmh_harvester_app-2.8.0.tar` & `core_oaipmh_harvester_app-2.9.0.tar`

### file list

```diff
@@ -1,236 +1,236 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:04.224227 core_oaipmh_harvester_app-2.8.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2024-03-12 19:05:53.000000 core_oaipmh_harvester_app-2.8.0/LICENSE.md
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      183 2024-03-12 19:05:53.000000 core_oaipmh_harvester_app-2.8.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1133 2024-03-12 19:06:04.216451 core_oaipmh_harvester_app-2.8.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      622 2024-03-12 19:05:53.000000 core_oaipmh_harvester_app-2.8.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:00.860810 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       99 2024-03-12 19:05:53.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4375 2024-03-12 19:05:53.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/admin.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      785 2024-03-12 19:05:53.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/apps.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:01.006452 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/commons/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:53.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/commons/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      324 2024-03-12 19:05:53.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/commons/rights.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:01.032553 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:53.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:01.100373 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/components/mongo/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:53.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/components/mongo/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1106 2024-03-12 19:05:53.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/components/mongo/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7801 2024-03-12 19:05:53.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/components/mongo/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:01.177247 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/components/oai_harvester_metadata_format/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:53.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/components/oai_harvester_metadata_format/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6394 2024-03-12 19:05:53.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/components/oai_harvester_metadata_format/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5715 2024-03-12 19:05:53.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/components/oai_harvester_metadata_format/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:01.243671 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/components/oai_harvester_metadata_format_set/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:53.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/components/oai_harvester_metadata_format_set/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2120 2024-03-12 19:05:53.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/components/oai_harvester_metadata_format_set/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2554 2024-03-12 19:05:53.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/components/oai_harvester_metadata_format_set/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:01.312294 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/components/oai_harvester_set/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:53.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/components/oai_harvester_set/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3537 2024-03-12 19:05:53.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/components/oai_harvester_set/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3667 2024-03-12 19:05:53.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/components/oai_harvester_set/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:01.377418 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/components/oai_identify/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:53.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/components/oai_identify/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1060 2024-03-12 19:05:53.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/components/oai_identify/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2243 2024-03-12 19:05:53.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/components/oai_identify/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:01.462087 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/components/oai_record/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:53.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/components/oai_record/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3076 2024-03-12 19:05:53.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/components/oai_record/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5872 2024-03-12 19:05:53.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/components/oai_record/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:01.527372 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/components/oai_registry/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:54.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/components/oai_registry/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    22180 2024-03-12 19:05:54.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/components/oai_registry/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3224 2024-03-12 19:05:54.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/components/oai_registry/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:01.575288 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/components/oai_verbs/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:54.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/components/oai_verbs/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8565 2024-03-12 19:05:54.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/components/oai_verbs/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      480 2024-03-12 19:05:54.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/menus.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:01.657112 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/migrations/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11396 2024-03-12 19:05:54.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/migrations/0001_initial.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1636 2024-03-12 19:05:54.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/migrations/0002_psql_full_text.py
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      421 2024-03-12 19:05:54.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/migrations/0003_remove_oairecord_xml_file_oairecord_file.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:54.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/migrations/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:01.728028 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:54.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:01.774429 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/rest/mongo/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:54.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/rest/mongo/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1492 2024-03-12 19:05:54.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/rest/mongo/serializers.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:01.838001 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/rest/oai_record/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:54.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/rest/oai_record/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5698 2024-03-12 19:05:54.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/rest/oai_record/abstract_views.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2145 2024-03-12 19:05:54.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/rest/oai_record/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:01.905123 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/rest/oai_registry/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:54.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/rest/oai_registry/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    17640 2024-03-12 19:05:54.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/rest/oai_registry/views.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2384 2024-03-12 19:05:54.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/rest/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1685 2024-03-12 19:05:54.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/rest/urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      943 2024-03-12 19:05:54.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:00.264975 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:00.336677 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:00.305228 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:00.278154 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/css/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:00.293154 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/css/registries/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:00.287195 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/css/registries/list/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:01.973374 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/css/registries/list/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      805 2024-03-12 19:05:54.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/css/registries/list/modals/edit_harvest_registry.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      487 2024-03-12 19:05:54.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/css/registries/list/modals/view_registry.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:01.996628 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/css/registries/request_builder/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      345 2024-03-12 19:05:54.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/css/registries/request_builder/main.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:00.309420 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:00.324869 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:00.318196 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:02.348013 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      477 2024-03-12 19:05:54.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/activate_registry.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       98 2024-03-12 19:05:54.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/activate_registry.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1632 2024-03-12 19:05:54.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/add_registry.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      175 2024-03-12 19:05:54.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/add_registry.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1287 2024-03-12 19:05:54.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/check_registry.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       92 2024-03-12 19:05:54.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/check_registry.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      970 2024-03-12 19:05:54.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/deactivate_registry.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      102 2024-03-12 19:05:54.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/deactivate_registry.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      926 2024-03-12 19:05:54.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/delete_registry.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       94 2024-03-12 19:05:54.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/delete_registry.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1605 2024-03-12 19:05:54.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/harvest_registry.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      204 2024-03-12 19:05:54.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/harvest_registry.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      618 2024-03-12 19:05:54.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/refresh.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1713 2024-03-12 19:05:54.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/update_registry.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      200 2024-03-12 19:05:54.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/update_registry.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      868 2024-03-12 19:05:54.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/view_registry.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       90 2024-03-12 19:05:54.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/view_registry.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:02.429955 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/request_builder/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3062 2024-03-12 19:05:54.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/request_builder/init.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      204 2024-03-12 19:05:54.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/request_builder/init.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3993 2024-03-12 19:05:54.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/request_builder/submit.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2024-03-12 19:05:54.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/request_builder/submit.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:00.340802 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/libs/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:00.345372 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/libs/bootstrap-datetimepicker/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:00.356052 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/libs/bootstrap-datetimepicker/1.0/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:02.469436 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/libs/bootstrap-datetimepicker/1.0/css/
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)    12339 2024-03-12 19:05:54.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/libs/bootstrap-datetimepicker/1.0/css/bootstrap-datetimepicker.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:02.491867 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/libs/bootstrap-datetimepicker/1.0/js/
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)    67527 2024-03-12 19:05:54.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/libs/bootstrap-datetimepicker/1.0/js/bootstrap-datetimepicker.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:02.539062 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/system/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:54.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/system/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      901 2024-03-12 19:05:54.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/system/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9073 2024-03-12 19:05:54.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/tasks.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:00.378418 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:00.382988 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:00.387547 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:02.589223 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:02.609116 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:02.801997 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1213 2024-03-12 19:05:54.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/add_registry.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      854 2024-03-12 19:05:54.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/deactivate_registry.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      784 2024-03-12 19:05:54.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/delete_registry.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1130 2024-03-12 19:05:54.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/edit_harvest_registry.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1957 2024-03-12 19:05:54.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/edit_harvest_registry_form.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      901 2024-03-12 19:05:54.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/view_registry.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      484 2024-03-12 19:05:54.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/view_registry_table.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1015 2024-03-12 19:05:54.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/view_registry_table_general.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3410 2024-03-12 19:05:54.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/view_registry_table_identity.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2023 2024-03-12 19:05:54.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/view_registry_table_metadata_formats.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1947 2024-03-12 19:05:54.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/view_registry_table_sets.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4588 2024-03-12 19:05:54.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/table.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      332 2024-03-12 19:05:54.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:02.822733 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/request_builder/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4343 2024-03-12 19:05:54.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/request_builder/main.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      343 2024-03-12 19:05:54.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/request_builder.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      204 2024-03-12 19:05:54.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:02.900753 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:54.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/utils/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:02.922704 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/utils/query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:54.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/utils/query/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:02.978542 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/utils/query/mongo/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:54.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/utils/query/mongo/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2002 2024-03-12 19:05:54.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/utils/query/mongo/query_builder.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4012 2024-03-12 19:05:54.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/utils/sickle_operations.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1392 2024-03-12 19:05:54.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/utils/sickle_serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2303 2024-03-12 19:05:54.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/utils/transform_operations.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:03.013425 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:54.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:03.099060 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/views/admin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:54.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/views/admin/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    16030 2024-03-12 19:05:54.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/views/admin/ajax.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6535 2024-03-12 19:05:55.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/views/admin/forms.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4419 2024-03-12 19:05:55.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/views/admin/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:00.960782 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1133 2024-03-12 19:05:59.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10047 2024-03-12 19:06:00.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2024-03-12 19:05:59.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      127 2024-03-12 19:05:59.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       37 2024-03-12 19:05:59.000000 core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app.egg-info/top_level.txt
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:03.166139 core_oaipmh_harvester_app-2.8.0/docs/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:55.000000 core_oaipmh_harvester_app-2.8.0/docs/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11074 2024-03-12 19:05:55.000000 core_oaipmh_harvester_app-2.8.0/docs/conf.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      313 2024-03-12 19:05:55.000000 core_oaipmh_harvester_app-2.8.0/docs/conf_urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2024-03-12 19:05:56.000000 core_oaipmh_harvester_app-2.8.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       51 2024-03-12 19:05:56.000000 core_oaipmh_harvester_app-2.8.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       76 2024-03-12 19:05:56.000000 core_oaipmh_harvester_app-2.8.0/requirements.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2024-03-12 19:06:04.226732 core_oaipmh_harvester_app-2.8.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1485 2024-03-12 19:05:56.000000 core_oaipmh_harvester_app-2.8.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:03.236920 core_oaipmh_harvester_app-2.8.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:56.000000 core_oaipmh_harvester_app-2.8.0/tests/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:03.260000 core_oaipmh_harvester_app-2.8.0/tests/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:56.000000 core_oaipmh_harvester_app-2.8.0/tests/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:03.287141 core_oaipmh_harvester_app-2.8.0/tests/components/mongo/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:56.000000 core_oaipmh_harvester_app-2.8.0/tests/components/mongo/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:03.336699 core_oaipmh_harvester_app-2.8.0/tests/components/mongo/models/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:56.000000 core_oaipmh_harvester_app-2.8.0/tests/components/mongo/models/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5392 2024-03-12 19:05:56.000000 core_oaipmh_harvester_app-2.8.0/tests/components/mongo/models/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:03.378854 core_oaipmh_harvester_app-2.8.0/tests/components/oai_harvester_metadata_format/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:56.000000 core_oaipmh_harvester_app-2.8.0/tests/components/oai_harvester_metadata_format/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    18812 2024-03-12 19:05:56.000000 core_oaipmh_harvester_app-2.8.0/tests/components/oai_harvester_metadata_format/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:03.420974 core_oaipmh_harvester_app-2.8.0/tests/components/oai_harvester_metadata_format_set/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:56.000000 core_oaipmh_harvester_app-2.8.0/tests/components/oai_harvester_metadata_format_set/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8124 2024-03-12 19:05:56.000000 core_oaipmh_harvester_app-2.8.0/tests/components/oai_harvester_metadata_format_set/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:03.468494 core_oaipmh_harvester_app-2.8.0/tests/components/oai_harvester_set/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:56.000000 core_oaipmh_harvester_app-2.8.0/tests/components/oai_harvester_set/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11182 2024-03-12 19:05:56.000000 core_oaipmh_harvester_app-2.8.0/tests/components/oai_harvester_set/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:03.513795 core_oaipmh_harvester_app-2.8.0/tests/components/oai_identify/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:56.000000 core_oaipmh_harvester_app-2.8.0/tests/components/oai_identify/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5739 2024-03-12 19:05:56.000000 core_oaipmh_harvester_app-2.8.0/tests/components/oai_identify/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:03.558906 core_oaipmh_harvester_app-2.8.0/tests/components/oai_record/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:56.000000 core_oaipmh_harvester_app-2.8.0/tests/components/oai_record/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8799 2024-03-12 19:05:56.000000 core_oaipmh_harvester_app-2.8.0/tests/components/oai_record/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:03.617836 core_oaipmh_harvester_app-2.8.0/tests/components/oai_registry/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:56.000000 core_oaipmh_harvester_app-2.8.0/tests/components/oai_registry/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:03.660279 core_oaipmh_harvester_app-2.8.0/tests/components/oai_registry/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:56.000000 core_oaipmh_harvester_app-2.8.0/tests/components/oai_registry/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8366 2024-03-12 19:05:56.000000 core_oaipmh_harvester_app-2.8.0/tests/components/oai_registry/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    33272 2024-03-12 19:05:56.000000 core_oaipmh_harvester_app-2.8.0/tests/components/oai_registry/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    36268 2024-03-12 19:05:56.000000 core_oaipmh_harvester_app-2.8.0/tests/components/oai_registry/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:03.703118 core_oaipmh_harvester_app-2.8.0/tests/components/oai_verbs/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:56.000000 core_oaipmh_harvester_app-2.8.0/tests/components/oai_verbs/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7759 2024-03-12 19:05:56.000000 core_oaipmh_harvester_app-2.8.0/tests/components/oai_verbs/tests_unit.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      268 2024-03-12 19:05:56.000000 core_oaipmh_harvester_app-2.8.0/tests/mocks.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:03.723785 core_oaipmh_harvester_app-2.8.0/tests/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:56.000000 core_oaipmh_harvester_app-2.8.0/tests/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:03.808345 core_oaipmh_harvester_app-2.8.0/tests/rest/oai_record/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:56.000000 core_oaipmh_harvester_app-2.8.0/tests/rest/oai_record/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2948 2024-03-12 19:05:56.000000 core_oaipmh_harvester_app-2.8.0/tests/rest/oai_record/tests_int_mongo.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2683 2024-03-12 19:05:56.000000 core_oaipmh_harvester_app-2.8.0/tests/rest/oai_record/tests_int_psql.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4883 2024-03-12 19:05:56.000000 core_oaipmh_harvester_app-2.8.0/tests/rest/oai_record/tests_permissions.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:03.891451 core_oaipmh_harvester_app-2.8.0/tests/rest/oai_registry/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:56.000000 core_oaipmh_harvester_app-2.8.0/tests/rest/oai_registry/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6446 2024-03-12 19:05:56.000000 core_oaipmh_harvester_app-2.8.0/tests/rest/oai_registry/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    21070 2024-03-12 19:05:56.000000 core_oaipmh_harvester_app-2.8.0/tests/rest/oai_registry/tests_permissions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14434 2024-03-12 19:05:56.000000 core_oaipmh_harvester_app-2.8.0/tests/rest/oai_registry/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:03.910948 core_oaipmh_harvester_app-2.8.0/tests/system/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:56.000000 core_oaipmh_harvester_app-2.8.0/tests/system/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:03.978824 core_oaipmh_harvester_app-2.8.0/tests/system/api/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:56.000000 core_oaipmh_harvester_app-2.8.0/tests/system/api/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1858 2024-03-12 19:05:56.000000 core_oaipmh_harvester_app-2.8.0/tests/system/api/tests_unit.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1705 2024-03-12 19:05:56.000000 core_oaipmh_harvester_app-2.8.0/tests/test_settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:04.044700 core_oaipmh_harvester_app-2.8.0/tests/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:56.000000 core_oaipmh_harvester_app-2.8.0/tests/utils/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2697 2024-03-12 19:05:56.000000 core_oaipmh_harvester_app-2.8.0/tests/utils/tests_unit_query_builder.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3838 2024-03-12 19:05:56.000000 core_oaipmh_harvester_app-2.8.0/tests/utils/tests_unit_transform_operations.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:04.064725 core_oaipmh_harvester_app-2.8.0/tests/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:56.000000 core_oaipmh_harvester_app-2.8.0/tests/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:04.090890 core_oaipmh_harvester_app-2.8.0/tests/views/admin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:56.000000 core_oaipmh_harvester_app-2.8.0/tests/views/admin/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:04.140967 core_oaipmh_harvester_app-2.8.0/tests/views/admin/ajax/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:56.000000 core_oaipmh_harvester_app-2.8.0/tests/views/admin/ajax/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1358 2024-03-12 19:05:56.000000 core_oaipmh_harvester_app-2.8.0/tests/views/admin/ajax/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:04.193858 core_oaipmh_harvester_app-2.8.0/tests/views/admin/forms/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:05:56.000000 core_oaipmh_harvester_app-2.8.0/tests/views/admin/forms/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1639 2024-03-12 19:05:56.000000 core_oaipmh_harvester_app-2.8.0/tests/views/admin/forms/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:09.803234 core_oaipmh_harvester_app-2.9.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2024-05-13 16:10:57.000000 core_oaipmh_harvester_app-2.9.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      183 2024-05-13 16:10:57.000000 core_oaipmh_harvester_app-2.9.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1133 2024-05-13 16:11:09.797427 core_oaipmh_harvester_app-2.9.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      622 2024-05-13 16:10:57.000000 core_oaipmh_harvester_app-2.9.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:06.377190 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       99 2024-05-13 16:10:57.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4375 2024-05-13 16:10:57.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/admin.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      785 2024-05-13 16:10:57.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/apps.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:06.525304 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/commons/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:57.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/commons/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      324 2024-05-13 16:10:57.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/commons/rights.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:06.547948 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:57.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:06.617816 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/components/mongo/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:57.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/components/mongo/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1106 2024-05-13 16:10:57.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/components/mongo/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7801 2024-05-13 16:10:57.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/components/mongo/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:06.698139 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/components/oai_harvester_metadata_format/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:57.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/components/oai_harvester_metadata_format/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6394 2024-05-13 16:10:57.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/components/oai_harvester_metadata_format/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5715 2024-05-13 16:10:57.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/components/oai_harvester_metadata_format/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:06.759340 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/components/oai_harvester_metadata_format_set/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:57.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/components/oai_harvester_metadata_format_set/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2120 2024-05-13 16:10:57.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/components/oai_harvester_metadata_format_set/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2554 2024-05-13 16:10:57.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/components/oai_harvester_metadata_format_set/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:06.839008 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/components/oai_harvester_set/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:57.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/components/oai_harvester_set/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3537 2024-05-13 16:10:57.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/components/oai_harvester_set/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3667 2024-05-13 16:10:57.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/components/oai_harvester_set/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:06.902814 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/components/oai_identify/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:57.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/components/oai_identify/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1060 2024-05-13 16:10:57.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/components/oai_identify/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2243 2024-05-13 16:10:57.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/components/oai_identify/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:06.964768 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/components/oai_record/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:57.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/components/oai_record/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3076 2024-05-13 16:10:57.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/components/oai_record/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5872 2024-05-13 16:10:57.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/components/oai_record/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:07.038424 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/components/oai_registry/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:57.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/components/oai_registry/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    22180 2024-05-13 16:10:57.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/components/oai_registry/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3224 2024-05-13 16:10:58.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/components/oai_registry/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:07.082895 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/components/oai_verbs/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:58.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/components/oai_verbs/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8565 2024-05-13 16:10:58.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/components/oai_verbs/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      480 2024-05-13 16:10:58.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/menus.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:07.151836 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/migrations/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11396 2024-05-13 16:10:58.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/migrations/0001_initial.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1636 2024-05-13 16:10:58.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/migrations/0002_psql_full_text.py
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      421 2024-05-13 16:10:58.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/migrations/0003_remove_oairecord_xml_file_oairecord_file.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:58.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/migrations/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:07.214069 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:58.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:07.255357 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/rest/mongo/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:58.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/rest/mongo/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1492 2024-05-13 16:10:58.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/rest/mongo/serializers.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:07.360444 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/rest/oai_record/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:58.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/rest/oai_record/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5698 2024-05-13 16:10:58.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/rest/oai_record/abstract_views.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2145 2024-05-13 16:10:58.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/rest/oai_record/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:07.401551 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/rest/oai_registry/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:58.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/rest/oai_registry/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    17511 2024-05-13 16:10:58.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/rest/oai_registry/views.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2384 2024-05-13 16:10:58.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/rest/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1685 2024-05-13 16:10:58.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/rest/urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      943 2024-05-13 16:10:58.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:05.665039 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:05.738161 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:05.706262 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:05.679538 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/css/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:05.694399 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/css/registries/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:05.688305 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/css/registries/list/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:07.460012 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/css/registries/list/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      805 2024-05-13 16:10:58.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/css/registries/list/modals/edit_harvest_registry.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      487 2024-05-13 16:10:58.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/css/registries/list/modals/view_registry.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:07.481084 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/css/registries/request_builder/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      345 2024-05-13 16:10:58.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/css/registries/request_builder/main.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:05.710821 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:05.726119 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:05.719652 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:07.836916 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      477 2024-05-13 16:10:58.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/activate_registry.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       98 2024-05-13 16:10:58.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/activate_registry.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1632 2024-05-13 16:10:58.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/add_registry.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      175 2024-05-13 16:10:58.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/add_registry.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1287 2024-05-13 16:10:58.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/check_registry.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       92 2024-05-13 16:10:58.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/check_registry.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      970 2024-05-13 16:10:58.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/deactivate_registry.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      102 2024-05-13 16:10:58.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/deactivate_registry.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      926 2024-05-13 16:10:58.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/delete_registry.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       94 2024-05-13 16:10:58.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/delete_registry.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1605 2024-05-13 16:10:58.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/harvest_registry.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      204 2024-05-13 16:10:58.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/harvest_registry.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      618 2024-05-13 16:10:58.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/refresh.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1713 2024-05-13 16:10:58.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/update_registry.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      200 2024-05-13 16:10:58.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/update_registry.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      868 2024-05-13 16:10:58.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/view_registry.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       90 2024-05-13 16:10:58.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/view_registry.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:07.962681 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/request_builder/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3062 2024-05-13 16:10:58.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/request_builder/init.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      204 2024-05-13 16:10:58.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/request_builder/init.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3993 2024-05-13 16:10:58.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/request_builder/submit.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2024-05-13 16:10:58.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/request_builder/submit.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:05.742236 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/libs/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:05.746638 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/libs/bootstrap-datetimepicker/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:05.756936 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/libs/bootstrap-datetimepicker/1.0/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:08.006735 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/libs/bootstrap-datetimepicker/1.0/css/
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)    12339 2024-05-13 16:10:58.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/libs/bootstrap-datetimepicker/1.0/css/bootstrap-datetimepicker.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:08.030957 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/libs/bootstrap-datetimepicker/1.0/js/
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)    67527 2024-05-13 16:10:58.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/libs/bootstrap-datetimepicker/1.0/js/bootstrap-datetimepicker.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:08.075107 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/system/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:58.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/system/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      901 2024-05-13 16:10:58.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/system/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9073 2024-05-13 16:10:58.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/tasks.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:05.805775 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:05.809765 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:05.813997 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:08.122684 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:08.146967 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:08.368137 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1213 2024-05-13 16:10:58.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/add_registry.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      854 2024-05-13 16:10:58.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/deactivate_registry.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      784 2024-05-13 16:10:58.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/delete_registry.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1130 2024-05-13 16:10:58.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/edit_harvest_registry.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1957 2024-05-13 16:10:58.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/edit_harvest_registry_form.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      901 2024-05-13 16:10:58.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/view_registry.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      484 2024-05-13 16:10:59.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/view_registry_table.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1015 2024-05-13 16:10:59.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/view_registry_table_general.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3410 2024-05-13 16:10:59.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/view_registry_table_identity.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2023 2024-05-13 16:10:59.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/view_registry_table_metadata_formats.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1947 2024-05-13 16:10:59.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/view_registry_table_sets.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4588 2024-05-13 16:10:59.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/table.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      332 2024-05-13 16:10:58.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:08.399218 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/request_builder/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4343 2024-05-13 16:10:59.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/request_builder/main.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      343 2024-05-13 16:10:59.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/request_builder.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      204 2024-05-13 16:10:59.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:08.482814 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:59.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/utils/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:08.503768 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/utils/query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:59.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/utils/query/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:08.568913 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/utils/query/mongo/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:59.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/utils/query/mongo/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2002 2024-05-13 16:10:59.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/utils/query/mongo/query_builder.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4012 2024-05-13 16:10:59.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/utils/sickle_operations.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1392 2024-05-13 16:10:59.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/utils/sickle_serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2303 2024-05-13 16:10:59.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/utils/transform_operations.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:08.588771 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:59.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:08.666729 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/views/admin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:59.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/views/admin/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    15991 2024-05-13 16:10:59.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/views/admin/ajax.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6535 2024-05-13 16:10:59.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/views/admin/forms.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4419 2024-05-13 16:10:59.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/views/admin/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:06.467719 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1133 2024-05-13 16:11:04.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10047 2024-05-13 16:11:05.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2024-05-13 16:11:04.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      127 2024-05-13 16:11:04.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       37 2024-05-13 16:11:04.000000 core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app.egg-info/top_level.txt
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:08.732921 core_oaipmh_harvester_app-2.9.0/docs/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:10:59.000000 core_oaipmh_harvester_app-2.9.0/docs/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11074 2024-05-13 16:11:00.000000 core_oaipmh_harvester_app-2.9.0/docs/conf.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      313 2024-05-13 16:11:00.000000 core_oaipmh_harvester_app-2.9.0/docs/conf_urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2024-05-13 16:11:00.000000 core_oaipmh_harvester_app-2.9.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       51 2024-05-13 16:11:00.000000 core_oaipmh_harvester_app-2.9.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       76 2024-05-13 16:11:00.000000 core_oaipmh_harvester_app-2.9.0/requirements.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2024-05-13 16:11:09.826027 core_oaipmh_harvester_app-2.9.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1485 2024-05-13 16:11:01.000000 core_oaipmh_harvester_app-2.9.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:08.794584 core_oaipmh_harvester_app-2.9.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:01.000000 core_oaipmh_harvester_app-2.9.0/tests/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:08.812205 core_oaipmh_harvester_app-2.9.0/tests/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:01.000000 core_oaipmh_harvester_app-2.9.0/tests/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:08.834664 core_oaipmh_harvester_app-2.9.0/tests/components/mongo/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:01.000000 core_oaipmh_harvester_app-2.9.0/tests/components/mongo/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:08.889403 core_oaipmh_harvester_app-2.9.0/tests/components/mongo/models/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:01.000000 core_oaipmh_harvester_app-2.9.0/tests/components/mongo/models/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5392 2024-05-13 16:11:01.000000 core_oaipmh_harvester_app-2.9.0/tests/components/mongo/models/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:08.930942 core_oaipmh_harvester_app-2.9.0/tests/components/oai_harvester_metadata_format/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:01.000000 core_oaipmh_harvester_app-2.9.0/tests/components/oai_harvester_metadata_format/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    18812 2024-05-13 16:11:01.000000 core_oaipmh_harvester_app-2.9.0/tests/components/oai_harvester_metadata_format/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:08.972751 core_oaipmh_harvester_app-2.9.0/tests/components/oai_harvester_metadata_format_set/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:01.000000 core_oaipmh_harvester_app-2.9.0/tests/components/oai_harvester_metadata_format_set/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8124 2024-05-13 16:11:01.000000 core_oaipmh_harvester_app-2.9.0/tests/components/oai_harvester_metadata_format_set/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:09.026811 core_oaipmh_harvester_app-2.9.0/tests/components/oai_harvester_set/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:01.000000 core_oaipmh_harvester_app-2.9.0/tests/components/oai_harvester_set/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11182 2024-05-13 16:11:01.000000 core_oaipmh_harvester_app-2.9.0/tests/components/oai_harvester_set/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:09.067862 core_oaipmh_harvester_app-2.9.0/tests/components/oai_identify/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:01.000000 core_oaipmh_harvester_app-2.9.0/tests/components/oai_identify/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5727 2024-05-13 16:11:01.000000 core_oaipmh_harvester_app-2.9.0/tests/components/oai_identify/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:09.110204 core_oaipmh_harvester_app-2.9.0/tests/components/oai_record/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:01.000000 core_oaipmh_harvester_app-2.9.0/tests/components/oai_record/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8799 2024-05-13 16:11:01.000000 core_oaipmh_harvester_app-2.9.0/tests/components/oai_record/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:09.173882 core_oaipmh_harvester_app-2.9.0/tests/components/oai_registry/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:01.000000 core_oaipmh_harvester_app-2.9.0/tests/components/oai_registry/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:09.214977 core_oaipmh_harvester_app-2.9.0/tests/components/oai_registry/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:01.000000 core_oaipmh_harvester_app-2.9.0/tests/components/oai_registry/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8366 2024-05-13 16:11:01.000000 core_oaipmh_harvester_app-2.9.0/tests/components/oai_registry/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    33272 2024-05-13 16:11:01.000000 core_oaipmh_harvester_app-2.9.0/tests/components/oai_registry/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    36268 2024-05-13 16:11:01.000000 core_oaipmh_harvester_app-2.9.0/tests/components/oai_registry/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:09.276561 core_oaipmh_harvester_app-2.9.0/tests/components/oai_verbs/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:01.000000 core_oaipmh_harvester_app-2.9.0/tests/components/oai_verbs/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7759 2024-05-13 16:11:01.000000 core_oaipmh_harvester_app-2.9.0/tests/components/oai_verbs/tests_unit.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      268 2024-05-13 16:11:01.000000 core_oaipmh_harvester_app-2.9.0/tests/mocks.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:09.301378 core_oaipmh_harvester_app-2.9.0/tests/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:01.000000 core_oaipmh_harvester_app-2.9.0/tests/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:09.386888 core_oaipmh_harvester_app-2.9.0/tests/rest/oai_record/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:01.000000 core_oaipmh_harvester_app-2.9.0/tests/rest/oai_record/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2948 2024-05-13 16:11:01.000000 core_oaipmh_harvester_app-2.9.0/tests/rest/oai_record/tests_int_mongo.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2683 2024-05-13 16:11:01.000000 core_oaipmh_harvester_app-2.9.0/tests/rest/oai_record/tests_int_psql.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4883 2024-05-13 16:11:01.000000 core_oaipmh_harvester_app-2.9.0/tests/rest/oai_record/tests_permissions.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:09.467759 core_oaipmh_harvester_app-2.9.0/tests/rest/oai_registry/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:01.000000 core_oaipmh_harvester_app-2.9.0/tests/rest/oai_registry/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6446 2024-05-13 16:11:01.000000 core_oaipmh_harvester_app-2.9.0/tests/rest/oai_registry/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    21070 2024-05-13 16:11:01.000000 core_oaipmh_harvester_app-2.9.0/tests/rest/oai_registry/tests_permissions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14434 2024-05-13 16:11:01.000000 core_oaipmh_harvester_app-2.9.0/tests/rest/oai_registry/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:09.488184 core_oaipmh_harvester_app-2.9.0/tests/system/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:01.000000 core_oaipmh_harvester_app-2.9.0/tests/system/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:09.546577 core_oaipmh_harvester_app-2.9.0/tests/system/api/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:01.000000 core_oaipmh_harvester_app-2.9.0/tests/system/api/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1858 2024-05-13 16:11:01.000000 core_oaipmh_harvester_app-2.9.0/tests/system/api/tests_unit.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1705 2024-05-13 16:11:01.000000 core_oaipmh_harvester_app-2.9.0/tests/test_settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:09.624371 core_oaipmh_harvester_app-2.9.0/tests/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:01.000000 core_oaipmh_harvester_app-2.9.0/tests/utils/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2697 2024-05-13 16:11:01.000000 core_oaipmh_harvester_app-2.9.0/tests/utils/tests_unit_query_builder.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3838 2024-05-13 16:11:01.000000 core_oaipmh_harvester_app-2.9.0/tests/utils/tests_unit_transform_operations.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:09.644950 core_oaipmh_harvester_app-2.9.0/tests/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:01.000000 core_oaipmh_harvester_app-2.9.0/tests/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:09.669447 core_oaipmh_harvester_app-2.9.0/tests/views/admin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:02.000000 core_oaipmh_harvester_app-2.9.0/tests/views/admin/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:09.736417 core_oaipmh_harvester_app-2.9.0/tests/views/admin/ajax/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:02.000000 core_oaipmh_harvester_app-2.9.0/tests/views/admin/ajax/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1358 2024-05-13 16:11:02.000000 core_oaipmh_harvester_app-2.9.0/tests/views/admin/ajax/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:09.778186 core_oaipmh_harvester_app-2.9.0/tests/views/admin/forms/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:02.000000 core_oaipmh_harvester_app-2.9.0/tests/views/admin/forms/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1639 2024-05-13 16:11:02.000000 core_oaipmh_harvester_app-2.9.0/tests/views/admin/forms/test_unit.py
```

### Comparing `core_oaipmh_harvester_app-2.8.0/LICENSE.md` & `core_oaipmh_harvester_app-2.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/PKG-INFO` & `core_oaipmh_harvester_app-2.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_oaipmh_harvester_app
-Version: 2.8.0
+Version: 2.9.0
 Summary: OAI-PMH harvesting capabilities for the curator core project
 Home-page: https://github.com/usnistgov/core_oaipmh_harvester_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: =========================
         Core Oaipmh Harvester App
```

### Comparing `core_oaipmh_harvester_app-2.8.0/README.rst` & `core_oaipmh_harvester_app-2.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/admin.py` & `core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/admin.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/apps.py` & `core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/apps.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/components/mongo/api.py` & `core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/components/mongo/api.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/components/mongo/models.py` & `core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/components/mongo/models.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/components/oai_harvester_metadata_format/api.py` & `core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/components/oai_harvester_metadata_format/api.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/components/oai_harvester_metadata_format/models.py` & `core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/components/oai_harvester_metadata_format/models.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/components/oai_harvester_metadata_format_set/api.py` & `core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/components/oai_harvester_metadata_format_set/api.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/components/oai_harvester_metadata_format_set/models.py` & `core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/components/oai_harvester_metadata_format_set/models.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/components/oai_harvester_set/api.py` & `core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/components/oai_harvester_set/api.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/components/oai_harvester_set/models.py` & `core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/components/oai_harvester_set/models.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/components/oai_identify/api.py` & `core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/components/oai_identify/api.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/components/oai_identify/models.py` & `core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/components/oai_identify/models.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/components/oai_record/api.py` & `core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/components/oai_record/api.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/components/oai_record/models.py` & `core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/components/oai_record/models.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/components/oai_registry/api.py` & `core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/components/oai_registry/api.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/components/oai_registry/models.py` & `core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/components/oai_registry/models.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/components/oai_verbs/api.py` & `core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/components/oai_verbs/api.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/migrations/0001_initial.py` & `core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/migrations/0002_psql_full_text.py` & `core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/migrations/0002_psql_full_text.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/rest/mongo/serializers.py` & `core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/rest/mongo/serializers.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/rest/oai_record/abstract_views.py` & `core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/rest/oai_record/abstract_views.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/rest/oai_record/views.py` & `core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/rest/oai_record/views.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/rest/oai_registry/views.py` & `core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/rest/oai_registry/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,15 @@
                 data=request.data, context={"request": request}
             )
             # Validate data
             serializer.is_valid(raise_exception=True)
             # Save data
             registry = serializer.save()
             content = OaiPmhMessage.get_message_labelled(
-                "Registry {0} added with success.".format(registry.name)
+                "Registry {0} added.".format(registry.name)
             )
 
             return Response(content, status=status.HTTP_201_CREATED)
         except ValidationError as validation_exception:
             content = OaiPmhMessage.get_message_labelled(
                 validation_exception.detail
             )
@@ -231,15 +231,15 @@
                 instance=registry, data=request.data
             )
             # Validate data
             serializer.is_valid(raise_exception=True)
             # Save data
             serializer.save()
             content = OaiPmhMessage.get_message_labelled(
-                "Registry {0} updated with success.".format(registry.name)
+                "Registry {0} updated.".format(registry.name)
             )
 
             return Response(content, status=status.HTTP_200_OK)
         except ValidationError as validation_exception:
             content = OaiPmhMessage.get_message_labelled(
                 validation_exception.detail
             )
@@ -280,15 +280,15 @@
               content: Internal server error
         """
         try:
             registry = oai_registry_api.get_by_id(registry_id)
             registry.is_activated = True
             oai_registry_api.upsert(registry)
             content = OaiPmhMessage.get_message_labelled(
-                "Registry {0} activated with success.".format(registry.name)
+                "Registry {0} activated.".format(registry.name)
             )
 
             return Response(content, status=status.HTTP_200_OK)
         except exceptions.DoesNotExist:
             content = OaiPmhMessage.get_message_labelled(
                 "No registry found with the given id."
             )
@@ -324,15 +324,15 @@
               content: Internal server error
         """
         try:
             registry = oai_registry_api.get_by_id(registry_id)
             registry.is_activated = False
             oai_registry_api.upsert(registry)
             content = OaiPmhMessage.get_message_labelled(
-                "Registry {0} deactivated with success.".format(registry.name)
+                "Registry {0} deactivated.".format(registry.name)
             )
 
             return Response(content, status=status.HTTP_200_OK)
         except exceptions.DoesNotExist:
             content = OaiPmhMessage.get_message_labelled(
                 "No registry found with the given id."
             )
@@ -369,17 +369,15 @@
         """
         try:
             registry = oai_registry_api.get_by_id(registry_id)
             registry = oai_registry_api.update_registry_info(
                 registry, request=request
             )
             content = OaiPmhMessage.get_message_labelled(
-                "Registry {0} information updated with success.".format(
-                    registry.name
-                )
+                "Registry {0} information updated.".format(registry.name)
             )
 
             return Response(content, status=status.HTTP_200_OK)
         except exceptions.DoesNotExist as exception:
             content = OaiPmhMessage.get_message_labelled(str(exception))
             return Response(content, status=status.HTTP_404_NOT_FOUND)
         except exceptions_oai.OAIAPIException as exception:
@@ -416,15 +414,15 @@
             registry = oai_registry_api.get_by_id(registry_id)
             all_errors = oai_registry_api.harvest_registry(registry)
             if len(all_errors) > 0:
                 raise exceptions_oai.OAIAPISerializeLabelledException(
                     errors=all_errors, status_code=status.HTTP_400_BAD_REQUEST
                 )
             content = OaiPmhMessage.get_message_labelled(
-                "Registry {0} harvested with success.".format(registry.name)
+                "Registry {0} harvested.".format(registry.name)
             )
             return Response(content, status=status.HTTP_200_OK)
         except exceptions.DoesNotExist as exception:
             content = OaiPmhMessage.get_message_labelled(str(exception))
             return Response(content, status=status.HTTP_404_NOT_FOUND)
         except exceptions_oai.OAIAPIException as exception:
             return exception.response()
@@ -490,15 +488,15 @@
             # Set all sets to false (Do not harvest)
             oai_set_api.update_for_all_harvest_by_list_ids(
                 registry_sets, False
             )
             # Set given sets to True (Harvest)
             oai_set_api.update_for_all_harvest_by_list_ids(sets, True)
             content = OaiPmhMessage.get_message_labelled(
-                "Registry harvesting configuration updated with success."
+                "Registry harvesting configuration updated."
             )
 
             return Response(content, status=status.HTTP_200_OK)
         except ValidationError as validation_exception:
             content = OaiPmhMessage.get_message_labelled(
                 validation_exception.detail
             )
```

### Comparing `core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/rest/serializers.py` & `core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/rest/serializers.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/rest/urls.py` & `core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/rest/urls.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/settings.py` & `core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/settings.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/css/registries/list/modals/edit_harvest_registry.css` & `core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/css/registries/list/modals/edit_harvest_registry.css`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/add_registry.js` & `core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/add_registry.js`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/check_registry.js` & `core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/check_registry.js`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/deactivate_registry.js` & `core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/deactivate_registry.js`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/delete_registry.js` & `core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/delete_registry.js`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/harvest_registry.js` & `core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/harvest_registry.js`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/refresh.js` & `core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/refresh.js`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/update_registry.js` & `core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/update_registry.js`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/view_registry.js` & `core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/list/modals/view_registry.js`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/request_builder/init.js` & `core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/request_builder/init.js`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/request_builder/submit.js` & `core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/admin/js/registries/request_builder/submit.js`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/libs/bootstrap-datetimepicker/1.0/css/bootstrap-datetimepicker.css` & `core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/libs/bootstrap-datetimepicker/1.0/css/bootstrap-datetimepicker.css`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/libs/bootstrap-datetimepicker/1.0/js/bootstrap-datetimepicker.js` & `core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/static/core_oaipmh_harvester_app/libs/bootstrap-datetimepicker/1.0/js/bootstrap-datetimepicker.js`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/system/api.py` & `core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/system/api.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/tasks.py` & `core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/tasks.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/add_registry.html` & `core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/add_registry.html`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/deactivate_registry.html` & `core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/deactivate_registry.html`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/delete_registry.html` & `core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/delete_registry.html`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/edit_harvest_registry.html` & `core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/edit_harvest_registry.html`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/edit_harvest_registry_form.html` & `core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/edit_harvest_registry_form.html`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/view_registry.html` & `core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/view_registry.html`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/view_registry_table_general.html` & `core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/view_registry_table_general.html`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/view_registry_table_identity.html` & `core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/view_registry_table_identity.html`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/view_registry_table_metadata_formats.html` & `core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/view_registry_table_metadata_formats.html`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/view_registry_table_sets.html` & `core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/modals/view_registry_table_sets.html`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/table.html` & `core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/list/table.html`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/request_builder/main.html` & `core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/templates/core_oaipmh_harvester_app/admin/registries/request_builder/main.html`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/utils/query/mongo/query_builder.py` & `core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/utils/query/mongo/query_builder.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/utils/sickle_operations.py` & `core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/utils/sickle_operations.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/utils/sickle_serializers.py` & `core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/utils/sickle_serializers.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/utils/transform_operations.py` & `core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/utils/transform_operations.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/views/admin/ajax.py` & `core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/views/admin/ajax.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
                 harvest = form.cleaned_data.get("harvest")
                 oai_registry_api.add_registry_by_url(
                     url, harvest_rate, harvest, request=request
                 )
                 messages.add_message(
                     request,
                     messages.SUCCESS,
-                    "Data provider added with success.",
+                    "Data provider added.",
                 )
             else:
                 return HttpResponseBadRequest("Please enter a valid URL.")
     except Exception as exception:
         return HttpResponseBadRequest(
             escape(str(exception)), content_type="application/javascript"
         )
@@ -164,15 +164,15 @@
     """Edit Registry View"""
 
     form_class = EditRegistryForm
     model = OaiRegistry
     success_url = reverse_lazy(
         "core-admin:core_oaipmh_harvester_app_registries"
     )
-    success_message = "Data provider edited with success."
+    success_message = "Data provider edited."
 
     def _save(self, form):
         # Save treatment.
         try:
             oai_registry_api.upsert(self.object)
         except Exception as exception:
             form.add_error(None, str(exception))
@@ -218,15 +218,15 @@
 
     template_name = "core_oaipmh_harvester_app/admin/registries/list/modals/edit_harvest_registry_form.html"
     form_class = EditHarvestRegistryForm
     model = OaiRegistry
     success_url = reverse_lazy(
         "core-admin:core_oaipmh_harvester_app_registries"
     )
-    success_message = "Data provider edited with success."
+    success_message = "Data provider edited."
     metadata_formats = None
     sets = None
 
     def _save(self, form):
         # Save treatment.
         try:
             registry_id = self.object.id
```

### Comparing `core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/views/admin/forms.py` & `core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/views/admin/forms.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app/views/admin/views.py` & `core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app/views/admin/views.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app.egg-info/PKG-INFO` & `core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-oaipmh-harvester-app
-Version: 2.8.0
+Version: 2.9.0
 Summary: OAI-PMH harvesting capabilities for the curator core project
 Home-page: https://github.com/usnistgov/core_oaipmh_harvester_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: =========================
         Core Oaipmh Harvester App
```

### Comparing `core_oaipmh_harvester_app-2.8.0/core_oaipmh_harvester_app.egg-info/SOURCES.txt` & `core_oaipmh_harvester_app-2.9.0/core_oaipmh_harvester_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/docs/conf.py` & `core_oaipmh_harvester_app-2.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/setup.py` & `core_oaipmh_harvester_app-2.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_oaipmh_harvester_app",
-    version="2.8.0",
+    version="2.9.0",
     description="OAI-PMH harvesting capabilities for the curator core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_oaipmh_harvester_app",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `core_oaipmh_harvester_app-2.8.0/tests/components/mongo/models/test_unit.py` & `core_oaipmh_harvester_app-2.9.0/tests/components/mongo/models/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/tests/components/oai_harvester_metadata_format/tests_unit.py` & `core_oaipmh_harvester_app-2.9.0/tests/components/oai_harvester_metadata_format/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/tests/components/oai_harvester_metadata_format_set/tests_unit.py` & `core_oaipmh_harvester_app-2.9.0/tests/components/oai_harvester_metadata_format_set/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/tests/components/oai_harvester_set/tests_unit.py` & `core_oaipmh_harvester_app-2.9.0/tests/components/oai_harvester_set/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/tests/components/oai_identify/tests_unit.py` & `core_oaipmh_harvester_app-2.9.0/tests/components/oai_identify/tests_unit.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """
 
 from unittest.case import TestCase
 from unittest.mock import Mock, patch
 
 import core_oaipmh_harvester_app.components.oai_identify.api as oai_identify_api
 from core_main_app.commons import exceptions
-from core_main_app.utils.xml import OrderedDict
+from collections import OrderedDict
 from core_oaipmh_harvester_app.components.oai_identify.models import (
     OaiIdentify,
 )
 from core_oaipmh_harvester_app.components.oai_registry.models import (
     OaiRegistry,
 )
```

### Comparing `core_oaipmh_harvester_app-2.8.0/tests/components/oai_record/tests_unit.py` & `core_oaipmh_harvester_app-2.9.0/tests/components/oai_record/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/tests/components/oai_registry/fixtures/fixtures.py` & `core_oaipmh_harvester_app-2.9.0/tests/components/oai_registry/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/tests/components/oai_registry/tests_int.py` & `core_oaipmh_harvester_app-2.9.0/tests/components/oai_registry/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/tests/components/oai_registry/tests_unit.py` & `core_oaipmh_harvester_app-2.9.0/tests/components/oai_registry/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/tests/components/oai_verbs/tests_unit.py` & `core_oaipmh_harvester_app-2.9.0/tests/components/oai_verbs/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/tests/rest/oai_record/tests_int_mongo.py` & `core_oaipmh_harvester_app-2.9.0/tests/rest/oai_record/tests_int_mongo.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/tests/rest/oai_record/tests_int_psql.py` & `core_oaipmh_harvester_app-2.9.0/tests/rest/oai_record/tests_int_psql.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/tests/rest/oai_record/tests_permissions.py` & `core_oaipmh_harvester_app-2.9.0/tests/rest/oai_record/tests_permissions.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/tests/rest/oai_registry/tests_int.py` & `core_oaipmh_harvester_app-2.9.0/tests/rest/oai_registry/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/tests/rest/oai_registry/tests_permissions.py` & `core_oaipmh_harvester_app-2.9.0/tests/rest/oai_registry/tests_permissions.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/tests/rest/oai_registry/tests_unit.py` & `core_oaipmh_harvester_app-2.9.0/tests/rest/oai_registry/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/tests/system/api/tests_unit.py` & `core_oaipmh_harvester_app-2.9.0/tests/system/api/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/tests/test_settings.py` & `core_oaipmh_harvester_app-2.9.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/tests/utils/tests_unit_query_builder.py` & `core_oaipmh_harvester_app-2.9.0/tests/utils/tests_unit_query_builder.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/tests/utils/tests_unit_transform_operations.py` & `core_oaipmh_harvester_app-2.9.0/tests/utils/tests_unit_transform_operations.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/tests/views/admin/ajax/tests_unit.py` & `core_oaipmh_harvester_app-2.9.0/tests/views/admin/ajax/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_harvester_app-2.8.0/tests/views/admin/forms/test_unit.py` & `core_oaipmh_harvester_app-2.9.0/tests/views/admin/forms/test_unit.py`

 * *Files identical despite different names*

