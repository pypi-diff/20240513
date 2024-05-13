# Comparing `tmp/core_oaipmh_provider_app-2.8.0.tar.gz` & `tmp/core_oaipmh_provider_app-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_oaipmh_provider_app-2.8.0.tar", last modified: Tue Mar 12 19:06:27 2024, max compression
+gzip compressed data, was "core_oaipmh_provider_app-2.9.0.tar", last modified: Mon May 13 16:11:36 2024, max compression
```

## Comparing `core_oaipmh_provider_app-2.8.0.tar` & `core_oaipmh_provider_app-2.9.0.tar`

### file list

```diff
@@ -1,228 +1,228 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:27.311612 core_oaipmh_provider_app-2.8.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2024-03-12 19:06:17.000000 core_oaipmh_provider_app-2.8.0/LICENSE.md
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      156 2024-03-12 19:06:17.000000 core_oaipmh_provider_app-2.8.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1118 2024-03-12 19:06:27.305615 core_oaipmh_provider_app-2.8.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      611 2024-03-12 19:06:17.000000 core_oaipmh_provider_app-2.8.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:24.205864 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       97 2024-03-12 19:06:17.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4465 2024-03-12 19:06:17.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/admin.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2593 2024-03-12 19:06:17.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/apps.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:24.377175 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/commons/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:17.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/commons/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      150 2024-03-12 19:06:17.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/commons/constants.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3064 2024-03-12 19:06:17.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/commons/exceptions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       54 2024-03-12 19:06:17.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/commons/status.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:24.397979 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:17.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:24.478616 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/components/oai_data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:17.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/components/oai_data/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3930 2024-03-12 19:06:17.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/components/oai_data/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5466 2024-03-12 19:06:17.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/components/oai_data/models.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1535 2024-03-12 19:06:17.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/components/oai_data/watch.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:24.557082 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/components/oai_provider_metadata_format/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:17.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/components/oai_provider_metadata_format/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11015 2024-03-12 19:06:17.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/components/oai_provider_metadata_format/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2310 2024-03-12 19:06:17.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/components/oai_provider_metadata_format/discover.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4113 2024-03-12 19:06:17.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/components/oai_provider_metadata_format/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:24.613588 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/components/oai_provider_set/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:17.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/components/oai_provider_set/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2308 2024-03-12 19:06:17.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/components/oai_provider_set/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2579 2024-03-12 19:06:17.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/components/oai_provider_set/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:24.671569 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/components/oai_request_page/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:17.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/components/oai_request_page/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1637 2024-03-12 19:06:17.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/components/oai_request_page/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1408 2024-03-12 19:06:17.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/components/oai_request_page/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:24.745779 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/components/oai_settings/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:17.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/components/oai_settings/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      465 2024-03-12 19:06:17.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/components/oai_settings/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1651 2024-03-12 19:06:17.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/components/oai_settings/discover.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1017 2024-03-12 19:06:17.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/components/oai_settings/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:24.801322 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/components/oai_xsl_template/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:17.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/components/oai_xsl_template/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2595 2024-03-12 19:06:17.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/components/oai_xsl_template/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3598 2024-03-12 19:06:17.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/components/oai_xsl_template/models.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      584 2024-03-12 19:06:17.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/menus.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:24.878502 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/migrations/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7245 2024-03-12 19:06:17.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/migrations/0001_initial.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      900 2024-03-12 19:06:17.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/migrations/0002_oai_data_on_delete.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      527 2024-03-12 19:06:17.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/migrations/0003_oai_data_bulk_delete.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:17.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/migrations/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:24.947433 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:17.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:24.991946 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/rest/oai_provider_metadata_format/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:17.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/rest/oai_provider_metadata_format/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14117 2024-03-12 19:06:17.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/rest/oai_provider_metadata_format/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:25.036857 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/rest/oai_provider_set/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:17.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/rest/oai_provider_set/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7804 2024-03-12 19:06:17.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/rest/oai_provider_set/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:25.098197 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/rest/oai_settings/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:17.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/rest/oai_settings/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4347 2024-03-12 19:06:17.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/rest/oai_settings/views.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8789 2024-03-12 19:06:17.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/rest/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1759 2024-03-12 19:06:17.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/rest/urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1568 2024-03-12 19:06:17.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:23.659211 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:23.713108 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:23.698908 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:23.672259 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/css/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:23.689190 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/css/registry/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:25.139918 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/css/registry/identity/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      619 2024-03-12 19:06:17.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/css/registry/identity/table_info.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:25.162200 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/css/registry/metadata_formats/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      183 2024-03-12 19:06:17.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/css/registry/metadata_formats/page.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:25.183736 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/css/registry/sets/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       63 2024-03-12 19:06:17.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/css/registry/sets/add_set.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:23.703152 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/js/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:23.707304 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/js/registry/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:25.230088 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/js/registry/identity/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1712 2024-03-12 19:06:17.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/js/registry/identity/check_registry.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       91 2024-03-12 19:06:17.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/js/registry/identity/check_registry.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:25.269393 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/xsd/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1444 2024-03-12 19:06:17.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/xsd/oai_dc.xsd
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3029 2024-03-12 19:06:17.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/xsd/simpledc20021212.xsd
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:25.309959 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/system/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:17.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/system/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      490 2024-03-12 19:06:17.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/system/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1976 2024-03-12 19:06:17.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/tasks.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:23.735728 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:23.784793 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:23.744764 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:25.387145 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:25.408761 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/forms/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      829 2024-03-12 19:06:17.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/forms/add_form.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:25.429892 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/identity/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2457 2024-03-12 19:06:17.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/identity/table.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      259 2024-03-12 19:06:17.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/identity.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:25.488932 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/metadata_formats/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1408 2024-03-12 19:06:17.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/metadata_formats/table_default.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2333 2024-03-12 19:06:17.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/metadata_formats/table_metadata_formats.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2114 2024-03-12 19:06:17.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/metadata_formats/table_template_metadata_formats.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      502 2024-03-12 19:06:17.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/metadata_formats.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:25.509903 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/sets/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1900 2024-03-12 19:06:17.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/sets/table.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      251 2024-03-12 19:06:17.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/sets.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:25.530104 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/xsl_template/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1978 2024-03-12 19:06:17.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/xsl_template/table.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      382 2024-03-12 19:06:17.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/xsl_template.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:23.789004 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:25.712922 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      717 2024-03-12 19:06:17.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/base.html
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      201 2024-03-12 19:06:17.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/error.html
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      635 2024-03-12 19:06:18.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/get_record.html
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      254 2024-03-12 19:06:18.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/header.html
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     1118 2024-03-12 19:06:18.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/identify.html
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      374 2024-03-12 19:06:18.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/list_identifiers.html
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      407 2024-03-12 19:06:18.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/list_metadata_formats.html
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      577 2024-03-12 19:06:18.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/list_records.html
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     1030 2024-03-12 19:06:18.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/list_sets.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      298 2024-03-12 19:06:18.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/resumption_token.xml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      566 2024-03-12 19:06:18.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:25.777064 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:18.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/utils/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5850 2024-03-12 19:06:18.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/utils/request_checker.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      903 2024-03-12 19:06:18.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/utils/template.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:25.811144 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:18.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:25.895297 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/views/admin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:18.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/views/admin/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    12125 2024-03-12 19:06:18.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/views/admin/ajax.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9014 2024-03-12 19:06:18.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/views/admin/forms.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7382 2024-03-12 19:06:18.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/views/admin/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:25.930655 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/views/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:18.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/views/user/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    24356 2024-03-12 19:06:18.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/views/user/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:24.300890 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1118 2024-03-12 19:06:22.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8176 2024-03-12 19:06:23.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2024-03-12 19:06:22.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      113 2024-03-12 19:06:22.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       36 2024-03-12 19:06:22.000000 core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app.egg-info/top_level.txt
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:25.987871 core_oaipmh_provider_app-2.8.0/docs/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:18.000000 core_oaipmh_provider_app-2.8.0/docs/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11332 2024-03-12 19:06:18.000000 core_oaipmh_provider_app-2.8.0/docs/conf.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      311 2024-03-12 19:06:18.000000 core_oaipmh_provider_app-2.8.0/docs/conf_urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2024-03-12 19:06:19.000000 core_oaipmh_provider_app-2.8.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       51 2024-03-12 19:06:19.000000 core_oaipmh_provider_app-2.8.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2024-03-12 19:06:27.313747 core_oaipmh_provider_app-2.8.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1481 2024-03-12 19:06:19.000000 core_oaipmh_provider_app-2.8.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:26.029651 core_oaipmh_provider_app-2.8.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:19.000000 core_oaipmh_provider_app-2.8.0/tests/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:26.074274 core_oaipmh_provider_app-2.8.0/tests/apps/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:19.000000 core_oaipmh_provider_app-2.8.0/tests/apps/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1799 2024-03-12 19:06:19.000000 core_oaipmh_provider_app-2.8.0/tests/apps/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:26.097020 core_oaipmh_provider_app-2.8.0/tests/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:19.000000 core_oaipmh_provider_app-2.8.0/tests/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:26.122510 core_oaipmh_provider_app-2.8.0/tests/components/oai_data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1527 2024-03-12 19:06:19.000000 core_oaipmh_provider_app-2.8.0/tests/components/oai_data/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:26.191716 core_oaipmh_provider_app-2.8.0/tests/components/oai_data/api/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:19.000000 core_oaipmh_provider_app-2.8.0/tests/components/oai_data/api/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2277 2024-03-12 19:06:19.000000 core_oaipmh_provider_app-2.8.0/tests/components/oai_data/api/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10294 2024-03-12 19:06:19.000000 core_oaipmh_provider_app-2.8.0/tests/components/oai_data/api/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:26.255006 core_oaipmh_provider_app-2.8.0/tests/components/oai_data/models/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:19.000000 core_oaipmh_provider_app-2.8.0/tests/components/oai_data/models/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1315 2024-03-12 19:06:19.000000 core_oaipmh_provider_app-2.8.0/tests/components/oai_data/models/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7942 2024-03-12 19:06:19.000000 core_oaipmh_provider_app-2.8.0/tests/components/oai_data/models/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:26.302800 core_oaipmh_provider_app-2.8.0/tests/components/oai_data/watch/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:19.000000 core_oaipmh_provider_app-2.8.0/tests/components/oai_data/watch/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1098 2024-03-12 19:06:19.000000 core_oaipmh_provider_app-2.8.0/tests/components/oai_data/watch/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:26.324386 core_oaipmh_provider_app-2.8.0/tests/components/oai_provider_metadata_format/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:19.000000 core_oaipmh_provider_app-2.8.0/tests/components/oai_provider_metadata_format/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:26.374610 core_oaipmh_provider_app-2.8.0/tests/components/oai_provider_metadata_format/api/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:19.000000 core_oaipmh_provider_app-2.8.0/tests/components/oai_provider_metadata_format/api/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    28019 2024-03-12 19:06:19.000000 core_oaipmh_provider_app-2.8.0/tests/components/oai_provider_metadata_format/api/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:26.423914 core_oaipmh_provider_app-2.8.0/tests/components/oai_provider_set/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:19.000000 core_oaipmh_provider_app-2.8.0/tests/components/oai_provider_set/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9462 2024-03-12 19:06:19.000000 core_oaipmh_provider_app-2.8.0/tests/components/oai_provider_set/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:26.470775 core_oaipmh_provider_app-2.8.0/tests/components/oai_settings/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:19.000000 core_oaipmh_provider_app-2.8.0/tests/components/oai_settings/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2770 2024-03-12 19:06:19.000000 core_oaipmh_provider_app-2.8.0/tests/components/oai_settings/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:26.570056 core_oaipmh_provider_app-2.8.0/tests/components/oai_xsl_template/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:19.000000 core_oaipmh_provider_app-2.8.0/tests/components/oai_xsl_template/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9663 2024-03-12 19:06:19.000000 core_oaipmh_provider_app-2.8.0/tests/components/oai_xsl_template/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:26.590868 core_oaipmh_provider_app-2.8.0/tests/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:19.000000 core_oaipmh_provider_app-2.8.0/tests/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:26.687129 core_oaipmh_provider_app-2.8.0/tests/rest/oai_provider_metadata_format/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:19.000000 core_oaipmh_provider_app-2.8.0/tests/rest/oai_provider_metadata_format/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6987 2024-03-12 19:06:19.000000 core_oaipmh_provider_app-2.8.0/tests/rest/oai_provider_metadata_format/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    16462 2024-03-12 19:06:19.000000 core_oaipmh_provider_app-2.8.0/tests/rest/oai_provider_metadata_format/tests_permissions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    17947 2024-03-12 19:06:19.000000 core_oaipmh_provider_app-2.8.0/tests/rest/oai_provider_metadata_format/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:26.771675 core_oaipmh_provider_app-2.8.0/tests/rest/oai_provider_set/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:19.000000 core_oaipmh_provider_app-2.8.0/tests/rest/oai_provider_set/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5329 2024-03-12 19:06:19.000000 core_oaipmh_provider_app-2.8.0/tests/rest/oai_provider_set/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8865 2024-03-12 19:06:19.000000 core_oaipmh_provider_app-2.8.0/tests/rest/oai_provider_set/tests_permissions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5925 2024-03-12 19:06:19.000000 core_oaipmh_provider_app-2.8.0/tests/rest/oai_provider_set/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:26.847442 core_oaipmh_provider_app-2.8.0/tests/rest/oai_settings/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:19.000000 core_oaipmh_provider_app-2.8.0/tests/rest/oai_settings/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2618 2024-03-12 19:06:19.000000 core_oaipmh_provider_app-2.8.0/tests/rest/oai_settings/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4840 2024-03-12 19:06:19.000000 core_oaipmh_provider_app-2.8.0/tests/rest/oai_settings/tests_permissions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3149 2024-03-12 19:06:19.000000 core_oaipmh_provider_app-2.8.0/tests/rest/oai_settings/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:26.890362 core_oaipmh_provider_app-2.8.0/tests/rest/serializers/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:19.000000 core_oaipmh_provider_app-2.8.0/tests/rest/serializers/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3984 2024-03-12 19:06:19.000000 core_oaipmh_provider_app-2.8.0/tests/rest/serializers/tests_unit.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1953 2024-03-12 19:06:19.000000 core_oaipmh_provider_app-2.8.0/tests/test_settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:26.954081 core_oaipmh_provider_app-2.8.0/tests/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:20.000000 core_oaipmh_provider_app-2.8.0/tests/utils/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:26.999544 core_oaipmh_provider_app-2.8.0/tests/utils/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:20.000000 core_oaipmh_provider_app-2.8.0/tests/utils/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    12394 2024-03-12 19:06:20.000000 core_oaipmh_provider_app-2.8.0/tests/utils/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      539 2024-03-12 19:06:20.000000 core_oaipmh_provider_app-2.8.0/tests/utils/mocks.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:27.050178 core_oaipmh_provider_app-2.8.0/tests/utils/template/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:20.000000 core_oaipmh_provider_app-2.8.0/tests/utils/template/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2699 2024-03-12 19:06:20.000000 core_oaipmh_provider_app-2.8.0/tests/utils/template/tests_unit.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1299 2024-03-12 19:06:20.000000 core_oaipmh_provider_app-2.8.0/tests/utils/test_oai_pmh_suite.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:27.072954 core_oaipmh_provider_app-2.8.0/tests/utils/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:20.000000 core_oaipmh_provider_app-2.8.0/tests/utils/tests/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:27.100145 core_oaipmh_provider_app-2.8.0/tests/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:20.000000 core_oaipmh_provider_app-2.8.0/tests/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:27.127008 core_oaipmh_provider_app-2.8.0/tests/views/admin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:20.000000 core_oaipmh_provider_app-2.8.0/tests/views/admin/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:27.178365 core_oaipmh_provider_app-2.8.0/tests/views/admin/ajax/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:20.000000 core_oaipmh_provider_app-2.8.0/tests/views/admin/ajax/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8671 2024-03-12 19:06:20.000000 core_oaipmh_provider_app-2.8.0/tests/views/admin/ajax/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:27.223478 core_oaipmh_provider_app-2.8.0/tests/views/admin/forms/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:20.000000 core_oaipmh_provider_app-2.8.0/tests/views/admin/forms/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11691 2024-03-12 19:06:20.000000 core_oaipmh_provider_app-2.8.0/tests/views/admin/forms/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:27.285259 core_oaipmh_provider_app-2.8.0/tests/views/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:20.000000 core_oaipmh_provider_app-2.8.0/tests/views/user/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5607 2024-03-12 19:06:20.000000 core_oaipmh_provider_app-2.8.0/tests/views/user/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    45422 2024-03-12 19:06:20.000000 core_oaipmh_provider_app-2.8.0/tests/views/user/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:36.824302 core_oaipmh_provider_app-2.9.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2024-05-13 16:11:22.000000 core_oaipmh_provider_app-2.9.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      156 2024-05-13 16:11:22.000000 core_oaipmh_provider_app-2.9.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1118 2024-05-13 16:11:36.817817 core_oaipmh_provider_app-2.9.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      611 2024-05-13 16:11:22.000000 core_oaipmh_provider_app-2.9.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:33.473225 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       97 2024-05-13 16:11:22.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4465 2024-05-13 16:11:22.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/admin.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2593 2024-05-13 16:11:22.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/apps.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:33.643717 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/commons/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:22.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/commons/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      150 2024-05-13 16:11:22.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/commons/constants.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3064 2024-05-13 16:11:22.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/commons/exceptions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       54 2024-05-13 16:11:22.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/commons/status.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:33.664287 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:22.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:33.738101 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/components/oai_data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:22.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/components/oai_data/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3930 2024-05-13 16:11:22.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/components/oai_data/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5466 2024-05-13 16:11:22.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/components/oai_data/models.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1535 2024-05-13 16:11:23.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/components/oai_data/watch.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:33.810168 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/components/oai_provider_metadata_format/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:23.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/components/oai_provider_metadata_format/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10945 2024-05-13 16:11:23.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/components/oai_provider_metadata_format/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2310 2024-05-13 16:11:23.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/components/oai_provider_metadata_format/discover.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4113 2024-05-13 16:11:23.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/components/oai_provider_metadata_format/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:33.870020 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/components/oai_provider_set/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:23.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/components/oai_provider_set/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2308 2024-05-13 16:11:23.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/components/oai_provider_set/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2579 2024-05-13 16:11:23.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/components/oai_provider_set/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:33.937520 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/components/oai_request_page/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:23.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/components/oai_request_page/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1637 2024-05-13 16:11:23.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/components/oai_request_page/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1408 2024-05-13 16:11:23.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/components/oai_request_page/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:34.026774 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/components/oai_settings/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:23.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/components/oai_settings/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      465 2024-05-13 16:11:23.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/components/oai_settings/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1651 2024-05-13 16:11:23.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/components/oai_settings/discover.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1017 2024-05-13 16:11:23.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/components/oai_settings/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:34.104880 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/components/oai_xsl_template/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:23.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/components/oai_xsl_template/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2595 2024-05-13 16:11:23.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/components/oai_xsl_template/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3598 2024-05-13 16:11:23.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/components/oai_xsl_template/models.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      584 2024-05-13 16:11:23.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/menus.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:34.187858 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/migrations/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7245 2024-05-13 16:11:23.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/migrations/0001_initial.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      900 2024-05-13 16:11:23.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/migrations/0002_oai_data_on_delete.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      527 2024-05-13 16:11:23.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/migrations/0003_oai_data_bulk_delete.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:23.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/migrations/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:34.256178 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:23.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:34.303709 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/rest/oai_provider_metadata_format/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:23.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/rest/oai_provider_metadata_format/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14061 2024-05-13 16:11:23.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/rest/oai_provider_metadata_format/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:34.347013 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/rest/oai_provider_set/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:23.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/rest/oai_provider_set/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7718 2024-05-13 16:11:23.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/rest/oai_provider_set/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:34.399622 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/rest/oai_settings/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:23.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/rest/oai_settings/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4334 2024-05-13 16:11:23.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/rest/oai_settings/views.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8789 2024-05-13 16:11:23.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/rest/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1759 2024-05-13 16:11:23.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/rest/urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1568 2024-05-13 16:11:23.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:32.845915 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:32.917015 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:32.902970 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:32.858775 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/css/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:32.882228 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/css/registry/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:34.438952 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/css/registry/identity/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      619 2024-05-13 16:11:23.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/css/registry/identity/table_info.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:34.460898 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/css/registry/metadata_formats/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      183 2024-05-13 16:11:23.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/css/registry/metadata_formats/page.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:34.482156 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/css/registry/sets/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       63 2024-05-13 16:11:23.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/css/registry/sets/add_set.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:32.907139 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/js/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:32.911236 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/js/registry/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:34.529249 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/js/registry/identity/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1699 2024-05-13 16:11:23.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/js/registry/identity/check_registry.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       91 2024-05-13 16:11:23.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/js/registry/identity/check_registry.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:34.567637 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/xsd/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1444 2024-05-13 16:11:23.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/xsd/oai_dc.xsd
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3029 2024-05-13 16:11:23.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/xsd/simpledc20021212.xsd
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:34.609947 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/system/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:23.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/system/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      490 2024-05-13 16:11:23.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/system/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1976 2024-05-13 16:11:23.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/tasks.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:32.938343 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:33.007134 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:32.946598 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:34.698722 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:34.719233 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/forms/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      829 2024-05-13 16:11:23.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/forms/add_form.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:34.739868 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/identity/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2457 2024-05-13 16:11:23.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/identity/table.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      259 2024-05-13 16:11:23.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/identity.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:34.819593 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/metadata_formats/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1408 2024-05-13 16:11:23.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/metadata_formats/table_default.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2333 2024-05-13 16:11:23.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/metadata_formats/table_metadata_formats.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2114 2024-05-13 16:11:23.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/metadata_formats/table_template_metadata_formats.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      502 2024-05-13 16:11:23.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/metadata_formats.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:34.839702 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/sets/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1900 2024-05-13 16:11:23.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/sets/table.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      251 2024-05-13 16:11:23.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/sets.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:34.864028 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/xsl_template/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1978 2024-05-13 16:11:23.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/xsl_template/table.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      382 2024-05-13 16:11:23.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/xsl_template.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:33.011041 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:35.073618 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      717 2024-05-13 16:11:23.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/base.html
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      201 2024-05-13 16:11:23.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/error.html
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      635 2024-05-13 16:11:23.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/get_record.html
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      254 2024-05-13 16:11:24.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/header.html
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     1118 2024-05-13 16:11:24.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/identify.html
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      374 2024-05-13 16:11:24.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/list_identifiers.html
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      407 2024-05-13 16:11:24.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/list_metadata_formats.html
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      577 2024-05-13 16:11:24.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/list_records.html
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     1030 2024-05-13 16:11:24.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/list_sets.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      298 2024-05-13 16:11:24.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/resumption_token.xml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      566 2024-05-13 16:11:24.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:35.134498 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:24.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/utils/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5850 2024-05-13 16:11:24.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/utils/request_checker.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      903 2024-05-13 16:11:24.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/utils/template.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:35.154647 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:24.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:35.237251 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/views/admin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:24.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/views/admin/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11982 2024-05-13 16:11:24.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/views/admin/ajax.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9014 2024-05-13 16:11:24.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/views/admin/forms.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7382 2024-05-13 16:11:24.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/views/admin/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:35.279808 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/views/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:24.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/views/user/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    24356 2024-05-13 16:11:24.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/views/user/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:33.568733 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1118 2024-05-13 16:11:31.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8176 2024-05-13 16:11:32.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2024-05-13 16:11:31.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      113 2024-05-13 16:11:31.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       36 2024-05-13 16:11:31.000000 core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app.egg-info/top_level.txt
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:35.339591 core_oaipmh_provider_app-2.9.0/docs/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:24.000000 core_oaipmh_provider_app-2.9.0/docs/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11332 2024-05-13 16:11:24.000000 core_oaipmh_provider_app-2.9.0/docs/conf.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      311 2024-05-13 16:11:24.000000 core_oaipmh_provider_app-2.9.0/docs/conf_urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2024-05-13 16:11:28.000000 core_oaipmh_provider_app-2.9.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       51 2024-05-13 16:11:28.000000 core_oaipmh_provider_app-2.9.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2024-05-13 16:11:36.834573 core_oaipmh_provider_app-2.9.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1481 2024-05-13 16:11:28.000000 core_oaipmh_provider_app-2.9.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:35.378896 core_oaipmh_provider_app-2.9.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:28.000000 core_oaipmh_provider_app-2.9.0/tests/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:35.433072 core_oaipmh_provider_app-2.9.0/tests/apps/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:28.000000 core_oaipmh_provider_app-2.9.0/tests/apps/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1799 2024-05-13 16:11:28.000000 core_oaipmh_provider_app-2.9.0/tests/apps/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:35.455915 core_oaipmh_provider_app-2.9.0/tests/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:28.000000 core_oaipmh_provider_app-2.9.0/tests/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:35.481582 core_oaipmh_provider_app-2.9.0/tests/components/oai_data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1527 2024-05-13 16:11:28.000000 core_oaipmh_provider_app-2.9.0/tests/components/oai_data/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:35.713614 core_oaipmh_provider_app-2.9.0/tests/components/oai_data/api/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:28.000000 core_oaipmh_provider_app-2.9.0/tests/components/oai_data/api/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2277 2024-05-13 16:11:28.000000 core_oaipmh_provider_app-2.9.0/tests/components/oai_data/api/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10294 2024-05-13 16:11:28.000000 core_oaipmh_provider_app-2.9.0/tests/components/oai_data/api/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:35.774659 core_oaipmh_provider_app-2.9.0/tests/components/oai_data/models/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:28.000000 core_oaipmh_provider_app-2.9.0/tests/components/oai_data/models/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1315 2024-05-13 16:11:28.000000 core_oaipmh_provider_app-2.9.0/tests/components/oai_data/models/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7942 2024-05-13 16:11:28.000000 core_oaipmh_provider_app-2.9.0/tests/components/oai_data/models/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:35.820058 core_oaipmh_provider_app-2.9.0/tests/components/oai_data/watch/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:28.000000 core_oaipmh_provider_app-2.9.0/tests/components/oai_data/watch/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1098 2024-05-13 16:11:28.000000 core_oaipmh_provider_app-2.9.0/tests/components/oai_data/watch/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:35.842319 core_oaipmh_provider_app-2.9.0/tests/components/oai_provider_metadata_format/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:28.000000 core_oaipmh_provider_app-2.9.0/tests/components/oai_provider_metadata_format/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:35.902029 core_oaipmh_provider_app-2.9.0/tests/components/oai_provider_metadata_format/api/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:28.000000 core_oaipmh_provider_app-2.9.0/tests/components/oai_provider_metadata_format/api/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    28019 2024-05-13 16:11:28.000000 core_oaipmh_provider_app-2.9.0/tests/components/oai_provider_metadata_format/api/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:35.948456 core_oaipmh_provider_app-2.9.0/tests/components/oai_provider_set/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:28.000000 core_oaipmh_provider_app-2.9.0/tests/components/oai_provider_set/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9462 2024-05-13 16:11:28.000000 core_oaipmh_provider_app-2.9.0/tests/components/oai_provider_set/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:35.991474 core_oaipmh_provider_app-2.9.0/tests/components/oai_settings/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:28.000000 core_oaipmh_provider_app-2.9.0/tests/components/oai_settings/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2770 2024-05-13 16:11:28.000000 core_oaipmh_provider_app-2.9.0/tests/components/oai_settings/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:36.037339 core_oaipmh_provider_app-2.9.0/tests/components/oai_xsl_template/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:28.000000 core_oaipmh_provider_app-2.9.0/tests/components/oai_xsl_template/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9663 2024-05-13 16:11:28.000000 core_oaipmh_provider_app-2.9.0/tests/components/oai_xsl_template/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:36.059726 core_oaipmh_provider_app-2.9.0/tests/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:28.000000 core_oaipmh_provider_app-2.9.0/tests/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:36.166278 core_oaipmh_provider_app-2.9.0/tests/rest/oai_provider_metadata_format/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:28.000000 core_oaipmh_provider_app-2.9.0/tests/rest/oai_provider_metadata_format/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6987 2024-05-13 16:11:28.000000 core_oaipmh_provider_app-2.9.0/tests/rest/oai_provider_metadata_format/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    16462 2024-05-13 16:11:28.000000 core_oaipmh_provider_app-2.9.0/tests/rest/oai_provider_metadata_format/tests_permissions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    17947 2024-05-13 16:11:28.000000 core_oaipmh_provider_app-2.9.0/tests/rest/oai_provider_metadata_format/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:36.275483 core_oaipmh_provider_app-2.9.0/tests/rest/oai_provider_set/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:28.000000 core_oaipmh_provider_app-2.9.0/tests/rest/oai_provider_set/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5329 2024-05-13 16:11:28.000000 core_oaipmh_provider_app-2.9.0/tests/rest/oai_provider_set/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8865 2024-05-13 16:11:28.000000 core_oaipmh_provider_app-2.9.0/tests/rest/oai_provider_set/tests_permissions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5925 2024-05-13 16:11:28.000000 core_oaipmh_provider_app-2.9.0/tests/rest/oai_provider_set/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:36.354496 core_oaipmh_provider_app-2.9.0/tests/rest/oai_settings/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:28.000000 core_oaipmh_provider_app-2.9.0/tests/rest/oai_settings/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2618 2024-05-13 16:11:28.000000 core_oaipmh_provider_app-2.9.0/tests/rest/oai_settings/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4840 2024-05-13 16:11:29.000000 core_oaipmh_provider_app-2.9.0/tests/rest/oai_settings/tests_permissions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3149 2024-05-13 16:11:29.000000 core_oaipmh_provider_app-2.9.0/tests/rest/oai_settings/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:36.401834 core_oaipmh_provider_app-2.9.0/tests/rest/serializers/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:29.000000 core_oaipmh_provider_app-2.9.0/tests/rest/serializers/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3984 2024-05-13 16:11:29.000000 core_oaipmh_provider_app-2.9.0/tests/rest/serializers/tests_unit.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1953 2024-05-13 16:11:29.000000 core_oaipmh_provider_app-2.9.0/tests/test_settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:36.473330 core_oaipmh_provider_app-2.9.0/tests/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:29.000000 core_oaipmh_provider_app-2.9.0/tests/utils/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:36.515901 core_oaipmh_provider_app-2.9.0/tests/utils/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:29.000000 core_oaipmh_provider_app-2.9.0/tests/utils/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    12394 2024-05-13 16:11:29.000000 core_oaipmh_provider_app-2.9.0/tests/utils/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      539 2024-05-13 16:11:29.000000 core_oaipmh_provider_app-2.9.0/tests/utils/mocks.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:36.558485 core_oaipmh_provider_app-2.9.0/tests/utils/template/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:29.000000 core_oaipmh_provider_app-2.9.0/tests/utils/template/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2699 2024-05-13 16:11:29.000000 core_oaipmh_provider_app-2.9.0/tests/utils/template/tests_unit.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1299 2024-05-13 16:11:29.000000 core_oaipmh_provider_app-2.9.0/tests/utils/test_oai_pmh_suite.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:36.579058 core_oaipmh_provider_app-2.9.0/tests/utils/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:29.000000 core_oaipmh_provider_app-2.9.0/tests/utils/tests/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:36.611179 core_oaipmh_provider_app-2.9.0/tests/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:29.000000 core_oaipmh_provider_app-2.9.0/tests/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:36.637358 core_oaipmh_provider_app-2.9.0/tests/views/admin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:29.000000 core_oaipmh_provider_app-2.9.0/tests/views/admin/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:36.697774 core_oaipmh_provider_app-2.9.0/tests/views/admin/ajax/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:29.000000 core_oaipmh_provider_app-2.9.0/tests/views/admin/ajax/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8671 2024-05-13 16:11:29.000000 core_oaipmh_provider_app-2.9.0/tests/views/admin/ajax/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:36.739999 core_oaipmh_provider_app-2.9.0/tests/views/admin/forms/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:29.000000 core_oaipmh_provider_app-2.9.0/tests/views/admin/forms/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11691 2024-05-13 16:11:29.000000 core_oaipmh_provider_app-2.9.0/tests/views/admin/forms/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:36.797381 core_oaipmh_provider_app-2.9.0/tests/views/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:29.000000 core_oaipmh_provider_app-2.9.0/tests/views/user/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5607 2024-05-13 16:11:29.000000 core_oaipmh_provider_app-2.9.0/tests/views/user/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    45422 2024-05-13 16:11:29.000000 core_oaipmh_provider_app-2.9.0/tests/views/user/tests_unit.py
```

### Comparing `core_oaipmh_provider_app-2.8.0/LICENSE.md` & `core_oaipmh_provider_app-2.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.8.0/PKG-INFO` & `core_oaipmh_provider_app-2.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_oaipmh_provider_app
-Version: 2.8.0
+Version: 2.9.0
 Summary: OAI-PMH provider capabilities for the curator core project
 Home-page: https://github.com/usnistgov/core_oaipmh_provider_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: ========================
         Core Oaipmh Provider App
```

### Comparing `core_oaipmh_provider_app-2.8.0/README.rst` & `core_oaipmh_provider_app-2.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/admin.py` & `core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/admin.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/apps.py` & `core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/apps.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/commons/exceptions.py` & `core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/commons/exceptions.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/components/oai_data/api.py` & `core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/components/oai_data/api.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/components/oai_data/models.py` & `core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/components/oai_data/models.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/components/oai_data/watch.py` & `core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/components/oai_data/watch.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/components/oai_provider_metadata_format/api.py` & `core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/components/oai_provider_metadata_format/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,17 +187,15 @@
             schema=schema_url,
             xml_schema=xml_schema,
             is_default=False,
             metadata_namespace=target_namespace,
             is_template=False,
         )
         upsert(obj, request=request)
-        content = OaiPmhMessage.get_message_labelled(
-            "Metadata format added with success."
-        )
+        content = OaiPmhMessage.get_message_labelled("Metadata format added.")
 
         return Response(content, status=status.HTTP_201_CREATED)
 
     except oai_pmh_exceptions.OAIAPILabelledException as exception:
         raise exception
     except (exceptions.XMLError, XSDError) as exception:
         raise oai_pmh_exceptions.OAIAPILabelledException(
@@ -247,17 +245,15 @@
             xml_schema=xml_schema,
             is_default=False,
             is_template=True,
             metadata_namespace=_get_target_namespace(xml_schema),
             template=template,
         )
         upsert(oai_provider_metadata_format, request=request)
-        content = OaiPmhMessage.get_message_labelled(
-            "Metadata format added with success."
-        )
+        content = OaiPmhMessage.get_message_labelled("Metadata format added.")
 
         return Response(content, status=status.HTTP_201_CREATED)
     except oai_pmh_exceptions.OAIAPILabelledException as exception:
         raise exception
     except DoesNotExist:
         raise oai_pmh_exceptions.OAIAPILabelledException(
             message="Unable to add the new metadata format. "
```

### Comparing `core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/components/oai_provider_metadata_format/discover.py` & `core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/components/oai_provider_metadata_format/discover.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/components/oai_provider_metadata_format/models.py` & `core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/components/oai_provider_metadata_format/models.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/components/oai_provider_set/api.py` & `core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/components/oai_provider_set/api.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/components/oai_provider_set/models.py` & `core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/components/oai_provider_set/models.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/components/oai_request_page/api.py` & `core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/components/oai_request_page/api.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/components/oai_request_page/models.py` & `core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/components/oai_request_page/models.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/components/oai_settings/discover.py` & `core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/components/oai_settings/discover.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/components/oai_settings/models.py` & `core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/components/oai_settings/models.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/components/oai_xsl_template/api.py` & `core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/components/oai_xsl_template/api.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/components/oai_xsl_template/models.py` & `core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/components/oai_xsl_template/models.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/menus.py` & `core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/menus.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/migrations/0001_initial.py` & `core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/migrations/0002_oai_data_on_delete.py` & `core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/migrations/0002_oai_data_on_delete.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/migrations/0003_oai_data_bulk_delete.py` & `core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/migrations/0003_oai_data_bulk_delete.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/rest/oai_provider_metadata_format/views.py` & `core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/rest/oai_provider_metadata_format/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -222,15 +222,15 @@
                 context={"request": request},
             )
             # Validate data
             serializer.is_valid(raise_exception=True)
             # Save data
             serializer.save()
             content = OaiPmhMessage.get_message_labelled(
-                "Metadata Format updated with success."
+                "Metadata Format updated."
             )
 
             return Response(content, status=status.HTTP_200_OK)
         except ValidationError as validation_exception:
             content = OaiPmhMessage.get_message_labelled(
                 validation_exception.detail
             )
@@ -335,17 +335,15 @@
             )
             # Validate data
             serializer.is_valid(raise_exception=True)
             # Try to set the instance
             serializer.init_instance()
             # Save data
             serializer.save()
-            content = OaiPmhMessage.get_message_labelled(
-                "Mapping configured with success."
-            )
+            content = OaiPmhMessage.get_message_labelled("Mapping configured.")
 
             return Response(content, status=status.HTTP_200_OK)
         except ValidationError as validation_exception:
             content = OaiPmhMessage.get_message_labelled(
                 validation_exception.detail
             )
             return Response(content, status=status.HTTP_400_BAD_REQUEST)
```

### Comparing `core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/rest/oai_provider_set/views.py` & `core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/rest/oai_provider_set/views.py`

 * *Files 5% similar despite different names*

```diff
@@ -76,17 +76,15 @@
             serializer = serializers.OaiProviderSetCreateUpdateSerializer(
                 data=request.data, context={"request": request}
             )
             # Validate data
             serializer.is_valid(raise_exception=True)
             # Save data
             serializer.save()
-            content = OaiPmhMessage.get_message_labelled(
-                "Set added with success."
-            )
+            content = OaiPmhMessage.get_message_labelled("Set added.")
 
             return Response(content, status=status.HTTP_201_CREATED)
         except ValidationError as validation_exception:
             content = OaiPmhMessage.get_message_labelled(
                 validation_exception.detail
             )
             return Response(content, status=status.HTTP_400_BAD_REQUEST)
@@ -209,17 +207,15 @@
             serializer = serializers.OaiProviderSetCreateUpdateSerializer(
                 instance=set_, data=request.data, context={"request": request}
             )
             # Validate data
             serializer.is_valid(raise_exception=True)
             # Save data
             serializer.save()
-            content = OaiPmhMessage.get_message_labelled(
-                "Set updated with success."
-            )
+            content = OaiPmhMessage.get_message_labelled("Set updated.")
 
             return Response(content, status=status.HTTP_200_OK)
         except ValidationError as validation_exception:
             content = OaiPmhMessage.get_message_labelled(
                 validation_exception.detail
             )
             return Response(content, status=status.HTTP_400_BAD_REQUEST)
```

### Comparing `core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/rest/oai_settings/views.py` & `core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/rest/oai_settings/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
                 instance=settings_, data=request.data
             )
             # Validate data
             serializer.is_valid(raise_exception=True)
             # Save data
             serializer.save()
             content = OaiPmhMessage.get_message_labelled(
-                "OAI-PMH Settings updated with success."
+                "OAI-PMH Settings updated."
             )
 
             return Response(content, status=status.HTTP_200_OK)
         except ValidationError as validation_exception:
             content = OaiPmhMessage.get_message_labelled(
                 validation_exception.detail
             )
```

### Comparing `core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/rest/serializers.py` & `core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/rest/serializers.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/rest/urls.py` & `core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/rest/urls.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/settings.py` & `core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/settings.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/css/registry/identity/table_info.css` & `core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/css/registry/identity/table_info.css`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/js/registry/identity/check_registry.js` & `core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/admin/js/registry/identity/check_registry.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -39,15 +39,15 @@
     // Create a temporary text field
     let $temp = $("<input>");
     $("body").append($temp);
     // Select the text field
     $temp.val($.trim($(".base-url").text())).select();
     // Copy the text inside the text field
     navigator.clipboard.writeText($temp.val()).then(function() {
-        $.notify("Base URL copied to clipboard successfully!", "success");
+        $.notify("Base URL copied to clipboard!", "success");
     }, function() {
         $.notify("An error has occurred while copying the base URL!", "danger");
     });
 
     // Remove a temporary text field
     $temp.remove();
 }
```

### Comparing `core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/xsd/oai_dc.xsd` & `core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/xsd/oai_dc.xsd`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/xsd/simpledc20021212.xsd` & `core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/static/core_oaipmh_provider_app/xsd/simpledc20021212.xsd`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/tasks.py` & `core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/tasks.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/forms/add_form.html` & `core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/forms/add_form.html`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/identity/table.html` & `core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/identity/table.html`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/metadata_formats/table_default.html` & `core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/metadata_formats/table_default.html`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/metadata_formats/table_metadata_formats.html` & `core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/metadata_formats/table_metadata_formats.html`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/metadata_formats/table_template_metadata_formats.html` & `core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/metadata_formats/table_template_metadata_formats.html`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/sets/table.html` & `core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/sets/table.html`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/xsl_template/table.html` & `core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/admin/registry/xsl_template/table.html`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/base.html` & `core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/base.html`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/get_record.html` & `core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/get_record.html`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/identify.html` & `core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/identify.html`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/list_records.html` & `core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/list_records.html`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/list_sets.html` & `core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/templates/core_oaipmh_provider_app/user/xml/list_sets.html`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/urls.py` & `core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/urls.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/utils/request_checker.py` & `core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/utils/request_checker.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/utils/template.py` & `core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/utils/template.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/views/admin/ajax.py` & `core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/views/admin/ajax.py`

 * *Files 4% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 
 class EditIdentityView(EditObjectModalView):
     """Edit Identity View"""
 
     form_class = EditIdentityForm
     model = OaiSettings
     success_url = reverse_lazy("core-admin:core_oaipmh_provider_app_identity")
-    success_message = "Data provider edited with success."
+    success_message = "Data provider edited."
 
     def _save(self, form):
         # Save treatment.
         try:
             oai_settings_api.upsert(self.object)
         except Exception as exception:
             form.add_error(None, str(exception))
@@ -102,15 +102,15 @@
         "core_oaipmh_provider_app/admin/registry/forms/add_form.html"
     )
     form_class = MetadataFormatForm
     model = OaiProviderMetadataFormat
     success_url = reverse_lazy(
         "core-admin:core_oaipmh_provider_app_metadata_formats"
     )
-    success_message = "Metadata Format created with success."
+    success_message = "Metadata format created."
 
     def _save(self, form):
         # Save treatment.
         try:
             oai_provider_metadata_format_api.add_metadata_format(
                 self.object.metadata_prefix,
                 self.object.schema,
@@ -123,15 +123,15 @@
 class DeleteMetadataFormatView(DeleteObjectModalView):
     """Delete Metadata Format View"""
 
     model = OaiProviderMetadataFormat
     success_url = reverse_lazy(
         "core-admin:core_oaipmh_provider_app_metadata_formats"
     )
-    success_message = "Metadata Format deleted with success."
+    success_message = "Metadata format deleted."
     field_for_name = "metadata_prefix"
 
     def _delete(self, form):
         # Delete treatment.
         oai_provider_metadata_format_api.delete(self.object)
 
 
@@ -139,26 +139,26 @@
     """Edit Metadata Format View"""
 
     form_class = EditMetadataFormatForm
     model = OaiProviderMetadataFormat
     success_url = reverse_lazy(
         "core-admin:core_oaipmh_provider_app_metadata_formats"
     )
-    success_message = "Metadata Format edited with success."
+    success_message = "Metadata format edited."
 
     def _save(self, form):
         # Save treatment.
         try:
             oai_provider_metadata_format_api.upsert(
                 self.object, request=self.request
             )
         except NotUniqueError:
             form.add_error(
                 None,
-                "A Metadata Format with the same prefix already exists. Please "
+                "A Metadata format with the same prefix already exists. Please "
                 "choose another prefix.",
             )
         except Exception as exception:
             form.add_error(None, str(exception))
 
 
 class AddTemplateMetadataFormatView(AddObjectModalView):
@@ -168,15 +168,15 @@
         "core_oaipmh_provider_app/admin/registry/forms/add_form.html"
     )
     form_class = TemplateMetadataFormatForm
     model = OaiProviderMetadataFormat
     success_url = reverse_lazy(
         "core-admin:core_oaipmh_provider_app_metadata_formats"
     )
-    success_message = "Template Metadata Format created with success."
+    success_message = "Template Metadata format created."
 
     def _save(self, form):
         # Save treatment.
         try:
             oai_provider_metadata_format_api.add_template_metadata_format(
                 self.object.metadata_prefix,
                 self.object.template.id,
@@ -200,15 +200,15 @@
 
     template_name = (
         "core_oaipmh_provider_app/admin/registry/forms/add_form.html"
     )
     form_class = SetForm
     model = OaiProviderSet
     success_url = reverse_lazy("core-admin:core_oaipmh_provider_app_sets")
-    success_message = "Set created with success."
+    success_message = "Set created."
 
     def _save(self, form):
         try:
             template_version_manager_id_list = form.cleaned_data[
                 "templates_manager"
             ]
             check_template_manager_in_xsd_format(
@@ -234,29 +234,29 @@
 
 
 class DeleteSetView(DeleteObjectModalView):
     """Delete Set View"""
 
     model = OaiProviderSet
     success_url = reverse_lazy("core-admin:core_oaipmh_provider_app_sets")
-    success_message = "Set deleted with success."
+    success_message = "Set deleted."
     field_for_name = "set_spec"
 
     def _delete(self, form):
         # Delete treatment.
         oai_provider_metadata_format_api.delete(self.object)
 
 
 class EditSetView(EditObjectModalView):
     """Edit Set View"""
 
     form_class = SetForm
     model = OaiProviderSet
     success_url = reverse_lazy("core-admin:core_oaipmh_provider_app_sets")
-    success_message = "Set edited with success."
+    success_message = "Set edited."
 
     def _save(self, form):
         try:
             template_version_manager_id_list = form.cleaned_data[
                 "templates_manager"
             ]
             check_template_manager_in_xsd_format(
@@ -294,15 +294,15 @@
 
 
 class AddTemplateMappingView(AddObjectModalView):
     """Add Template Mapping View"""
 
     form_class = MappingXSLTForm
     model = OaiXslTemplate
-    success_message = "Mapping created with success."
+    success_message = "Mapping created."
 
     def _save(self, form):
         # Save treatment.
         try:
             oai_xsl_template_api.upsert(self.object)
         except Exception as exception:
             form.add_error(None, str(exception))
@@ -338,15 +338,15 @@
 
 
 class DeleteTemplateMappingView(DeleteObjectModalView):
     """Delete Template Mapping View"""
 
     model = OaiXslTemplate
     success_url = reverse_lazy("core-admin:core_oaipmh_provider_app_sets")
-    success_message = "Mapping deleted with success."
+    success_message = "Mapping deleted."
 
     def _delete(self, form):
         # Delete treatment.
         oai_xsl_template_api.delete(self.object)
 
     def get_success_url(self):
         """get_success_url
@@ -365,15 +365,15 @@
 
 
 class EditTemplateMappingView(EditObjectModalView):
     """Edit Template Mapping View"""
 
     form_class = MappingXSLTForm
     model = OaiXslTemplate
-    success_message = "Mapping edited with success."
+    success_message = "Mapping edited."
 
     def _save(self, form):
         # Save treatment.
         try:
             oai_xsl_template_api.upsert(self.object)
         except Exception as exception:
             form.add_error(None, str(exception))
```

### Comparing `core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/views/admin/forms.py` & `core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/views/admin/forms.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/views/admin/views.py` & `core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/views/admin/views.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app/views/user/views.py` & `core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app/views/user/views.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app.egg-info/PKG-INFO` & `core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-oaipmh-provider-app
-Version: 2.8.0
+Version: 2.9.0
 Summary: OAI-PMH provider capabilities for the curator core project
 Home-page: https://github.com/usnistgov/core_oaipmh_provider_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: ========================
         Core Oaipmh Provider App
```

### Comparing `core_oaipmh_provider_app-2.8.0/core_oaipmh_provider_app.egg-info/SOURCES.txt` & `core_oaipmh_provider_app-2.9.0/core_oaipmh_provider_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.8.0/docs/conf.py` & `core_oaipmh_provider_app-2.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.8.0/setup.py` & `core_oaipmh_provider_app-2.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_oaipmh_provider_app",
-    version="2.8.0",
+    version="2.9.0",
     description="OAI-PMH provider capabilities for the curator core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_oaipmh_provider_app",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `core_oaipmh_provider_app-2.8.0/tests/apps/tests_unit.py` & `core_oaipmh_provider_app-2.9.0/tests/apps/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.8.0/tests/components/oai_data/__init__.py` & `core_oaipmh_provider_app-2.9.0/tests/components/oai_data/__init__.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.8.0/tests/components/oai_data/api/tests_int.py` & `core_oaipmh_provider_app-2.9.0/tests/components/oai_data/api/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.8.0/tests/components/oai_data/api/tests_unit.py` & `core_oaipmh_provider_app-2.9.0/tests/components/oai_data/api/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.8.0/tests/components/oai_data/models/tests_int.py` & `core_oaipmh_provider_app-2.9.0/tests/components/oai_data/models/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.8.0/tests/components/oai_data/models/tests_unit.py` & `core_oaipmh_provider_app-2.9.0/tests/components/oai_data/models/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.8.0/tests/components/oai_data/watch/tests_unit.py` & `core_oaipmh_provider_app-2.9.0/tests/components/oai_data/watch/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.8.0/tests/components/oai_provider_metadata_format/api/tests_unit.py` & `core_oaipmh_provider_app-2.9.0/tests/components/oai_provider_metadata_format/api/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.8.0/tests/components/oai_provider_set/tests_unit.py` & `core_oaipmh_provider_app-2.9.0/tests/components/oai_provider_set/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.8.0/tests/components/oai_settings/tests_unit.py` & `core_oaipmh_provider_app-2.9.0/tests/components/oai_settings/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.8.0/tests/components/oai_xsl_template/tests_unit.py` & `core_oaipmh_provider_app-2.9.0/tests/components/oai_xsl_template/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.8.0/tests/rest/oai_provider_metadata_format/tests_int.py` & `core_oaipmh_provider_app-2.9.0/tests/rest/oai_provider_metadata_format/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.8.0/tests/rest/oai_provider_metadata_format/tests_permissions.py` & `core_oaipmh_provider_app-2.9.0/tests/rest/oai_provider_metadata_format/tests_permissions.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.8.0/tests/rest/oai_provider_metadata_format/tests_unit.py` & `core_oaipmh_provider_app-2.9.0/tests/rest/oai_provider_metadata_format/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.8.0/tests/rest/oai_provider_set/tests_int.py` & `core_oaipmh_provider_app-2.9.0/tests/rest/oai_provider_set/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.8.0/tests/rest/oai_provider_set/tests_permissions.py` & `core_oaipmh_provider_app-2.9.0/tests/rest/oai_provider_set/tests_permissions.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.8.0/tests/rest/oai_provider_set/tests_unit.py` & `core_oaipmh_provider_app-2.9.0/tests/rest/oai_provider_set/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.8.0/tests/rest/oai_settings/tests_int.py` & `core_oaipmh_provider_app-2.9.0/tests/rest/oai_settings/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.8.0/tests/rest/oai_settings/tests_permissions.py` & `core_oaipmh_provider_app-2.9.0/tests/rest/oai_settings/tests_permissions.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.8.0/tests/rest/oai_settings/tests_unit.py` & `core_oaipmh_provider_app-2.9.0/tests/rest/oai_settings/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.8.0/tests/rest/serializers/tests_unit.py` & `core_oaipmh_provider_app-2.9.0/tests/rest/serializers/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.8.0/tests/test_settings.py` & `core_oaipmh_provider_app-2.9.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.8.0/tests/utils/fixtures/fixtures.py` & `core_oaipmh_provider_app-2.9.0/tests/utils/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.8.0/tests/utils/mocks.py` & `core_oaipmh_provider_app-2.9.0/tests/utils/mocks.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.8.0/tests/utils/template/tests_unit.py` & `core_oaipmh_provider_app-2.9.0/tests/utils/template/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.8.0/tests/utils/test_oai_pmh_suite.py` & `core_oaipmh_provider_app-2.9.0/tests/utils/test_oai_pmh_suite.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.8.0/tests/views/admin/ajax/tests_unit.py` & `core_oaipmh_provider_app-2.9.0/tests/views/admin/ajax/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.8.0/tests/views/admin/forms/tests_unit.py` & `core_oaipmh_provider_app-2.9.0/tests/views/admin/forms/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.8.0/tests/views/user/tests_int.py` & `core_oaipmh_provider_app-2.9.0/tests/views/user/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_oaipmh_provider_app-2.8.0/tests/views/user/tests_unit.py` & `core_oaipmh_provider_app-2.9.0/tests/views/user/tests_unit.py`

 * *Files identical despite different names*

