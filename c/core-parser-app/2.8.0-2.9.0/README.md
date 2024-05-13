# Comparing `tmp/core_parser_app-2.8.0.tar.gz` & `tmp/core_parser_app-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_parser_app-2.8.0.tar", last modified: Tue Mar 12 19:06:57 2024, max compression
+gzip compressed data, was "core_parser_app-2.9.0.tar", last modified: Mon May 13 16:12:10 2024, max compression
```

## Comparing `core_parser_app-2.8.0.tar` & `core_parser_app-2.9.0.tar`

### file list

```diff
@@ -1,258 +1,269 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:57.713427 core_parser_app-2.8.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2024-03-12 19:06:41.000000 core_parser_app-2.8.0/LICENSE.md
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      395 2024-03-12 19:06:41.000000 core_parser_app-2.8.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2332 2024-03-12 19:06:57.706885 core_parser_app-2.8.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1696 2024-03-12 19:06:41.000000 core_parser_app-2.8.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:54.064608 core_parser_app-2.8.0/core_parser_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       64 2024-03-12 19:06:41.000000 core_parser_app-2.8.0/core_parser_app/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4397 2024-03-12 19:06:41.000000 core_parser_app-2.8.0/core_parser_app/access_control.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1411 2024-03-12 19:06:41.000000 core_parser_app-2.8.0/core_parser_app/admin.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      205 2024-03-12 19:06:41.000000 core_parser_app-2.8.0/core_parser_app/apps.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:54.177227 core_parser_app-2.8.0/core_parser_app/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:41.000000 core_parser_app-2.8.0/core_parser_app/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:54.273205 core_parser_app-2.8.0/core_parser_app/components/data_structure/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:41.000000 core_parser_app-2.8.0/core_parser_app/components/data_structure/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      376 2024-03-12 19:06:41.000000 core_parser_app-2.8.0/core_parser_app/components/data_structure/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      304 2024-03-12 19:06:41.000000 core_parser_app-2.8.0/core_parser_app/components/data_structure/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6887 2024-03-12 19:06:41.000000 core_parser_app-2.8.0/core_parser_app/components/data_structure/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:54.336017 core_parser_app-2.8.0/core_parser_app/components/data_structure_element/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:41.000000 core_parser_app-2.8.0/core_parser_app/components/data_structure_element/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      398 2024-03-12 19:06:41.000000 core_parser_app-2.8.0/core_parser_app/components/data_structure_element/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2871 2024-03-12 19:06:41.000000 core_parser_app-2.8.0/core_parser_app/components/data_structure_element/api.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:54.410045 core_parser_app-2.8.0/core_parser_app/components/module/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:41.000000 core_parser_app-2.8.0/core_parser_app/components/module/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      353 2024-03-12 19:06:41.000000 core_parser_app-2.8.0/core_parser_app/components/module/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2236 2024-03-12 19:06:41.000000 core_parser_app-2.8.0/core_parser_app/components/module/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1887 2024-03-12 19:06:41.000000 core_parser_app-2.8.0/core_parser_app/components/module/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:54.443230 core_parser_app-2.8.0/core_parser_app/migrations/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3972 2024-03-12 19:06:41.000000 core_parser_app-2.8.0/core_parser_app/migrations/0001_initial.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:41.000000 core_parser_app-2.8.0/core_parser_app/migrations/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      880 2024-03-12 19:06:41.000000 core_parser_app-2.8.0/core_parser_app/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:53.385719 core_parser_app-2.8.0/core_parser_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:53.390226 core_parser_app-2.8.0/core_parser_app/static/core_parser_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:53.409059 core_parser_app-2.8.0/core_parser_app/static/core_parser_app/common/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:54.474044 core_parser_app-2.8.0/core_parser_app/static/core_parser_app/common/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      161 2024-03-12 19:06:41.000000 core_parser_app-2.8.0/core_parser_app/static/core_parser_app/common/css/modules.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:54.511764 core_parser_app-2.8.0/core_parser_app/static/core_parser_app/common/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3620 2024-03-12 19:06:41.000000 core_parser_app-2.8.0/core_parser_app/static/core_parser_app/common/js/module_manager.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      169 2024-03-12 19:06:41.000000 core_parser_app-2.8.0/core_parser_app/static/core_parser_app/common/js/module_manager.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:54.568773 core_parser_app-2.8.0/core_parser_app/static/core_parser_app/common/xsd/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2682 2024-03-12 19:06:41.000000 core_parser_app-2.8.0/core_parser_app/static/core_parser_app/common/xsd/annotations.xsd
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      996 2024-03-12 19:06:41.000000 core_parser_app-2.8.0/core_parser_app/static/core_parser_app/common/xsd/boolean.xsd
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      996 2024-03-12 19:06:41.000000 core_parser_app-2.8.0/core_parser_app/static/core_parser_app/common/xsd/date.xsd
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:54.614950 core_parser_app-2.8.0/core_parser_app/system/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:41.000000 core_parser_app-2.8.0/core_parser_app/system/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      533 2024-03-12 19:06:41.000000 core_parser_app-2.8.0/core_parser_app/system/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      346 2024-03-12 19:06:41.000000 core_parser_app-2.8.0/core_parser_app/tasks.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:53.430174 core_parser_app-2.8.0/core_parser_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:53.434798 core_parser_app-2.8.0/core_parser_app/templates/core_parser_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:54.677896 core_parser_app-2.8.0/core_parser_app/templates/core_parser_app/common/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:54.698122 core_parser_app-2.8.0/core_parser_app/templates/core_parser_app/common/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1067 2024-03-12 19:06:41.000000 core_parser_app-2.8.0/core_parser_app/templates/core_parser_app/common/modals/add_module.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      268 2024-03-12 19:06:41.000000 core_parser_app-2.8.0/core_parser_app/templates/core_parser_app/common/module_manager.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      695 2024-03-12 19:06:41.000000 core_parser_app-2.8.0/core_parser_app/templates/core_parser_app/common/module_manager_box.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      473 2024-03-12 19:06:41.000000 core_parser_app-2.8.0/core_parser_app/templates/core_parser_app/common/modules.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:54.718239 core_parser_app-2.8.0/core_parser_app/tools/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:41.000000 core_parser_app-2.8.0/core_parser_app/tools/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:54.860852 core_parser_app-2.8.0/core_parser_app/tools/modules/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:41.000000 core_parser_app-2.8.0/core_parser_app/tools/modules/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2823 2024-03-12 19:06:41.000000 core_parser_app-2.8.0/core_parser_app/tools/modules/discover.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      182 2024-03-12 19:06:41.000000 core_parser_app-2.8.0/core_parser_app/tools/modules/exceptions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1825 2024-03-12 19:06:41.000000 core_parser_app-2.8.0/core_parser_app/tools/modules/sanitize.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:53.472224 core_parser_app-2.8.0/core_parser_app/tools/modules/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:53.514623 core_parser_app-2.8.0/core_parser_app/tools/modules/static/core_parser_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:53.488582 core_parser_app-2.8.0/core_parser_app/tools/modules/static/core_parser_app/css/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:54.914556 core_parser_app-2.8.0/core_parser_app/tools/modules/static/core_parser_app/css/builtin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       86 2024-03-12 19:06:41.000000 core_parser_app-2.8.0/core_parser_app/tools/modules/static/core_parser_app/css/builtin/checkboxes.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      128 2024-03-12 19:06:41.000000 core_parser_app-2.8.0/core_parser_app/tools/modules/static/core_parser_app/css/builtin/textarea.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:54.954450 core_parser_app-2.8.0/core_parser_app/tools/modules/static/core_parser_app/js/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:55.100083 core_parser_app-2.8.0/core_parser_app/tools/modules/static/core_parser_app/js/builtin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      128 2024-03-12 19:06:42.000000 core_parser_app-2.8.0/core_parser_app/tools/modules/static/core_parser_app/js/builtin/autocomplete.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      412 2024-03-12 19:06:42.000000 core_parser_app-2.8.0/core_parser_app/tools/modules/static/core_parser_app/js/builtin/checkboxes.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      265 2024-03-12 19:06:42.000000 core_parser_app-2.8.0/core_parser_app/tools/modules/static/core_parser_app/js/builtin/input.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      227 2024-03-12 19:06:42.000000 core_parser_app-2.8.0/core_parser_app/tools/modules/static/core_parser_app/js/builtin/options.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1379 2024-03-12 19:06:42.000000 core_parser_app-2.8.0/core_parser_app/tools/modules/static/core_parser_app/js/builtin/popup.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      240 2024-03-12 19:06:42.000000 core_parser_app-2.8.0/core_parser_app/tools/modules/static/core_parser_app/js/builtin/sync_input.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      229 2024-03-12 19:06:42.000000 core_parser_app-2.8.0/core_parser_app/tools/modules/static/core_parser_app/js/builtin/textarea.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:55.123232 core_parser_app-2.8.0/core_parser_app/tools/modules/static/core_parser_app/js/commons/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      512 2024-03-12 19:06:42.000000 core_parser_app-2.8.0/core_parser_app/tools/modules/static/core_parser_app/js/commons/file_uploader.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3135 2024-03-12 19:06:42.000000 core_parser_app-2.8.0/core_parser_app/tools/modules/static/core_parser_app/js/modules.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       75 2024-03-12 19:06:42.000000 core_parser_app-2.8.0/core_parser_app/tools/modules/static/core_parser_app/js/modules.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:55.146548 core_parser_app-2.8.0/core_parser_app/tools/modules/static/core_parser_app/xsl/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6048 2024-03-12 19:06:42.000000 core_parser_app-2.8.0/core_parser_app/tools/modules/static/core_parser_app/xsl/xsd2html4modules.xsl
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:53.527612 core_parser_app-2.8.0/core_parser_app/tools/modules/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:55.174225 core_parser_app-2.8.0/core_parser_app/tools/modules/templates/core_parser_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:55.354205 core_parser_app-2.8.0/core_parser_app/tools/modules/templates/core_parser_app/builtin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      142 2024-03-12 19:06:42.000000 core_parser_app-2.8.0/core_parser_app/tools/modules/templates/core_parser_app/builtin/autocomplete.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      303 2024-03-12 19:06:42.000000 core_parser_app-2.8.0/core_parser_app/tools/modules/templates/core_parser_app/builtin/checkboxes.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      255 2024-03-12 19:06:42.000000 core_parser_app-2.8.0/core_parser_app/tools/modules/templates/core_parser_app/builtin/input.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      149 2024-03-12 19:06:42.000000 core_parser_app-2.8.0/core_parser_app/tools/modules/templates/core_parser_app/builtin/input_button.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      577 2024-03-12 19:06:42.000000 core_parser_app-2.8.0/core_parser_app/tools/modules/templates/core_parser_app/builtin/modal_wrapper.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      237 2024-03-12 19:06:42.000000 core_parser_app-2.8.0/core_parser_app/tools/modules/templates/core_parser_app/builtin/options.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      267 2024-03-12 19:06:42.000000 core_parser_app-2.8.0/core_parser_app/tools/modules/templates/core_parser_app/builtin/popup.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      254 2024-03-12 19:06:42.000000 core_parser_app-2.8.0/core_parser_app/tools/modules/templates/core_parser_app/builtin/sync_input.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      126 2024-03-12 19:06:42.000000 core_parser_app-2.8.0/core_parser_app/tools/modules/templates/core_parser_app/builtin/textarea.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:55.376631 core_parser_app-2.8.0/core_parser_app/tools/modules/templates/core_parser_app/commons/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      477 2024-03-12 19:06:42.000000 core_parser_app-2.8.0/core_parser_app/tools/modules/templates/core_parser_app/commons/file_uploader.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      264 2024-03-12 19:06:42.000000 core_parser_app-2.8.0/core_parser_app/tools/modules/templates/core_parser_app/module.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      352 2024-03-12 19:06:42.000000 core_parser_app-2.8.0/core_parser_app/tools/modules/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:55.439606 core_parser_app-2.8.0/core_parser_app/tools/modules/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:42.000000 core_parser_app-2.8.0/core_parser_app/tools/modules/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:55.632665 core_parser_app-2.8.0/core_parser_app/tools/modules/views/builtin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:42.000000 core_parser_app-2.8.0/core_parser_app/tools/modules/views/builtin/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1022 2024-03-12 19:06:42.000000 core_parser_app-2.8.0/core_parser_app/tools/modules/views/builtin/autocomplete_module.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3012 2024-03-12 19:06:42.000000 core_parser_app-2.8.0/core_parser_app/tools/modules/views/builtin/checkboxes_module.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1253 2024-03-12 19:06:42.000000 core_parser_app-2.8.0/core_parser_app/tools/modules/views/builtin/input_button_module.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1533 2024-03-12 19:06:42.000000 core_parser_app-2.8.0/core_parser_app/tools/modules/views/builtin/input_module.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1882 2024-03-12 19:06:42.000000 core_parser_app-2.8.0/core_parser_app/tools/modules/views/builtin/options_module.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1300 2024-03-12 19:06:42.000000 core_parser_app-2.8.0/core_parser_app/tools/modules/views/builtin/popup_module.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1627 2024-03-12 19:06:42.000000 core_parser_app-2.8.0/core_parser_app/tools/modules/views/builtin/sync_input_module.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1011 2024-03-12 19:06:42.000000 core_parser_app-2.8.0/core_parser_app/tools/modules/views/builtin/textarea_module.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7787 2024-03-12 19:06:42.000000 core_parser_app-2.8.0/core_parser_app/tools/modules/views/module.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4172 2024-03-12 19:06:42.000000 core_parser_app-2.8.0/core_parser_app/tools/modules/views/views.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3201 2024-03-12 19:06:42.000000 core_parser_app-2.8.0/core_parser_app/tools/modules/xpathaccessor.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:55.693970 core_parser_app-2.8.0/core_parser_app/tools/parser/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:42.000000 core_parser_app-2.8.0/core_parser_app/tools/parser/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      326 2024-03-12 19:06:42.000000 core_parser_app-2.8.0/core_parser_app/tools/parser/exceptions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)   117543 2024-03-12 19:06:42.000000 core_parser_app-2.8.0/core_parser_app/tools/parser/parser.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:55.792156 core_parser_app-2.8.0/core_parser_app/tools/parser/renderer/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8352 2024-03-12 19:06:42.000000 core_parser_app-2.8.0/core_parser_app/tools/parser/renderer/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      901 2024-03-12 19:06:42.000000 core_parser_app-2.8.0/core_parser_app/tools/parser/renderer/checkbox.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    27114 2024-03-12 19:06:42.000000 core_parser_app-2.8.0/core_parser_app/tools/parser/renderer/list.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10019 2024-03-12 19:06:42.000000 core_parser_app-2.8.0/core_parser_app/tools/parser/renderer/table.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    24119 2024-03-12 19:06:42.000000 core_parser_app-2.8.0/core_parser_app/tools/parser/renderer/xml.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:53.587909 core_parser_app-2.8.0/core_parser_app/tools/parser/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:53.599010 core_parser_app-2.8.0/core_parser_app/tools/parser/static/core_parser_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:55.818365 core_parser_app-2.8.0/core_parser_app/tools/parser/static/core_parser_app/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      958 2024-03-12 19:06:42.000000 core_parser_app-2.8.0/core_parser_app/tools/parser/static/core_parser_app/css/use.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:55.913073 core_parser_app-2.8.0/core_parser_app/tools/parser/static/core_parser_app/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      934 2024-03-12 19:06:42.000000 core_parser_app-2.8.0/core_parser_app/tools/parser/static/core_parser_app/js/autosave.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       89 2024-03-12 19:06:42.000000 core_parser_app-2.8.0/core_parser_app/tools/parser/static/core_parser_app/js/autosave.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      882 2024-03-12 19:06:42.000000 core_parser_app-2.8.0/core_parser_app/tools/parser/static/core_parser_app/js/autosave_checkbox.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4673 2024-03-12 19:06:42.000000 core_parser_app-2.8.0/core_parser_app/tools/parser/static/core_parser_app/js/buttons.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5179 2024-03-12 19:06:42.000000 core_parser_app-2.8.0/core_parser_app/tools/parser/static/core_parser_app/js/choice.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:53.613991 core_parser_app-2.8.0/core_parser_app/tools/parser/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:53.654976 core_parser_app-2.8.0/core_parser_app/tools/parser/templates/renderer/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:55.989029 core_parser_app-2.8.0/core_parser_app/tools/parser/templates/renderer/default/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:56.050607 core_parser_app-2.8.0/core_parser_app/tools/parser/templates/renderer/default/buttons/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       98 2024-03-12 19:06:42.000000 core_parser_app-2.8.0/core_parser_app/tools/parser/templates/renderer/default/buttons/add.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       81 2024-03-12 19:06:42.000000 core_parser_app-2.8.0/core_parser_app/tools/parser/templates/renderer/default/buttons/collapse.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      104 2024-03-12 19:06:42.000000 core_parser_app-2.8.0/core_parser_app/tools/parser/templates/renderer/default/buttons/delete.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      110 2024-03-12 19:06:42.000000 core_parser_app-2.8.0/core_parser_app/tools/parser/templates/renderer/default/form-error.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:56.156125 core_parser_app-2.8.0/core_parser_app/tools/parser/templates/renderer/default/inputs/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      346 2024-03-12 19:06:42.000000 core_parser_app-2.8.0/core_parser_app/tools/parser/templates/renderer/default/inputs/boolean.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       76 2024-03-12 19:06:42.000000 core_parser_app-2.8.0/core_parser_app/tools/parser/templates/renderer/default/inputs/checkbox.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      502 2024-03-12 19:06:42.000000 core_parser_app-2.8.0/core_parser_app/tools/parser/templates/renderer/default/inputs/date.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      490 2024-03-12 19:06:42.000000 core_parser_app-2.8.0/core_parser_app/tools/parser/templates/renderer/default/inputs/input.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      446 2024-03-12 19:06:42.000000 core_parser_app-2.8.0/core_parser_app/tools/parser/templates/renderer/default/inputs/select.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:56.197409 core_parser_app-2.8.0/core_parser_app/tools/parser/templates/renderer/default/test/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       44 2024-03-12 19:06:42.000000 core_parser_app-2.8.0/core_parser_app/tools/parser/templates/renderer/default/test/sample_no_data.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       52 2024-03-12 19:06:42.000000 core_parser_app-2.8.0/core_parser_app/tools/parser/templates/renderer/default/test/sample_with_data.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       83 2024-03-12 19:06:42.000000 core_parser_app-2.8.0/core_parser_app/tools/parser/templates/renderer/default/ul.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       86 2024-03-12 19:06:42.000000 core_parser_app-2.8.0/core_parser_app/tools/parser/templates/renderer/default/warning.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:56.260017 core_parser_app-2.8.0/core_parser_app/tools/parser/templates/renderer/list/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      149 2024-03-12 19:06:42.000000 core_parser_app-2.8.0/core_parser_app/tools/parser/templates/renderer/list/attributes.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       75 2024-03-12 19:06:42.000000 core_parser_app-2.8.0/core_parser_app/tools/parser/templates/renderer/list/li.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      131 2024-03-12 19:06:42.000000 core_parser_app-2.8.0/core_parser_app/tools/parser/templates/renderer/list/ul.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:56.321959 core_parser_app-2.8.0/core_parser_app/tools/parser/templates/renderer/table/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       99 2024-03-12 19:06:42.000000 core_parser_app-2.8.0/core_parser_app/tools/parser/templates/renderer/table/table.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       75 2024-03-12 19:06:42.000000 core_parser_app-2.8.0/core_parser_app/tools/parser/templates/renderer/table/tr.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       41 2024-03-12 19:06:42.000000 core_parser_app-2.8.0/core_parser_app/tools/parser/templates/renderer/table/wrap.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:56.350888 core_parser_app-2.8.0/core_parser_app/tools/parser/templates/renderer/xml/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       99 2024-03-12 19:06:42.000000 core_parser_app-2.8.0/core_parser_app/tools/parser/templates/renderer/xml/element.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:56.414975 core_parser_app-2.8.0/core_parser_app/tools/parser/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:43.000000 core_parser_app-2.8.0/core_parser_app/tools/parser/utils/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      278 2024-03-12 19:06:43.000000 core_parser_app-2.8.0/core_parser_app/tools/parser/utils/rendering.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3519 2024-03-12 19:06:43.000000 core_parser_app-2.8.0/core_parser_app/tools/parser/utils/xml.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1075 2024-03-12 19:06:43.000000 core_parser_app-2.8.0/core_parser_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:56.468574 core_parser_app-2.8.0/core_parser_app/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:43.000000 core_parser_app-2.8.0/core_parser_app/utils/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2190 2024-03-12 19:06:43.000000 core_parser_app-2.8.0/core_parser_app/utils/xml.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:56.491811 core_parser_app-2.8.0/core_parser_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:43.000000 core_parser_app-2.8.0/core_parser_app/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:56.541184 core_parser_app-2.8.0/core_parser_app/views/admin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:43.000000 core_parser_app-2.8.0/core_parser_app/views/admin/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1592 2024-03-12 19:06:43.000000 core_parser_app-2.8.0/core_parser_app/views/admin/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:56.606688 core_parser_app-2.8.0/core_parser_app/views/common/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:43.000000 core_parser_app-2.8.0/core_parser_app/views/common/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1808 2024-03-12 19:06:43.000000 core_parser_app-2.8.0/core_parser_app/views/common/ajax.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3516 2024-03-12 19:06:43.000000 core_parser_app-2.8.0/core_parser_app/views/common/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:56.649899 core_parser_app-2.8.0/core_parser_app/views/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:43.000000 core_parser_app-2.8.0/core_parser_app/views/user/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2477 2024-03-12 19:06:43.000000 core_parser_app-2.8.0/core_parser_app/views/user/ajax.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:54.153970 core_parser_app-2.8.0/core_parser_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2332 2024-03-12 19:06:52.000000 core_parser_app-2.8.0/core_parser_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9281 2024-03-12 19:06:53.000000 core_parser_app-2.8.0/core_parser_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2024-03-12 19:06:52.000000 core_parser_app-2.8.0/core_parser_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       67 2024-03-12 19:06:52.000000 core_parser_app-2.8.0/core_parser_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       22 2024-03-12 19:06:52.000000 core_parser_app-2.8.0/core_parser_app.egg-info/top_level.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2024-03-12 19:06:44.000000 core_parser_app-2.8.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       21 2024-03-12 19:06:44.000000 core_parser_app-2.8.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       46 2024-03-12 19:06:44.000000 core_parser_app-2.8.0/requirements.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2024-03-12 19:06:57.716240 core_parser_app-2.8.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1441 2024-03-12 19:06:44.000000 core_parser_app-2.8.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:56.775785 core_parser_app-2.8.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:44.000000 core_parser_app-2.8.0/tests/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:56.819508 core_parser_app-2.8.0/tests/access_control/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:44.000000 core_parser_app-2.8.0/tests/access_control/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2180 2024-03-12 19:06:44.000000 core_parser_app-2.8.0/tests/access_control/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:56.840848 core_parser_app-2.8.0/tests/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:44.000000 core_parser_app-2.8.0/tests/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:56.910580 core_parser_app-2.8.0/tests/components/data_structure/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:44.000000 core_parser_app-2.8.0/tests/components/data_structure/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:44.000000 core_parser_app-2.8.0/tests/components/data_structure/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1619 2024-03-12 19:06:44.000000 core_parser_app-2.8.0/tests/components/data_structure/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:56.995168 core_parser_app-2.8.0/tests/components/data_structure_element/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:44.000000 core_parser_app-2.8.0/tests/components/data_structure_element/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:57.039871 core_parser_app-2.8.0/tests/components/data_structure_element/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:44.000000 core_parser_app-2.8.0/tests/components/data_structure_element/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6726 2024-03-12 19:06:44.000000 core_parser_app-2.8.0/tests/components/data_structure_element/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    20077 2024-03-12 19:06:44.000000 core_parser_app-2.8.0/tests/components/data_structure_element/test_int_access_control.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5869 2024-03-12 19:06:44.000000 core_parser_app-2.8.0/tests/components/data_structure_element/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4901 2024-03-12 19:06:44.000000 core_parser_app-2.8.0/tests/components/data_structure_element/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:57.089679 core_parser_app-2.8.0/tests/components/module/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:44.000000 core_parser_app-2.8.0/tests/components/module/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5876 2024-03-12 19:06:44.000000 core_parser_app-2.8.0/tests/components/module/tests_unit.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1093 2024-03-12 19:06:44.000000 core_parser_app-2.8.0/tests/fixtures_utils.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      646 2024-03-12 19:06:44.000000 core_parser_app-2.8.0/tests/models.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      185 2024-03-12 19:06:44.000000 core_parser_app-2.8.0/tests/rights.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1026 2024-03-12 19:06:44.000000 core_parser_app-2.8.0/tests/test_settings.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2718 2024-03-12 19:06:44.000000 core_parser_app-2.8.0/tests/test_utils.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:57.120283 core_parser_app-2.8.0/tests/tools/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:44.000000 core_parser_app-2.8.0/tests/tools/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:57.145320 core_parser_app-2.8.0/tests/tools/modules/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:44.000000 core_parser_app-2.8.0/tests/tools/modules/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:57.227622 core_parser_app-2.8.0/tests/tools/modules/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:44.000000 core_parser_app-2.8.0/tests/tools/modules/tests/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2950 2024-03-12 19:06:44.000000 core_parser_app-2.8.0/tests/tools/modules/tests/tests_unit_checkboxes_module.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9401 2024-03-12 19:06:44.000000 core_parser_app-2.8.0/tests/tools/modules/tests/tests_unit_module.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2292 2024-03-12 19:06:44.000000 core_parser_app-2.8.0/tests/tools/modules/tests/tests_unit_sanitize.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:57.252081 core_parser_app-2.8.0/tests/tools/parser/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:44.000000 core_parser_app-2.8.0/tests/tools/parser/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:57.446594 core_parser_app-2.8.0/tests/tools/parser/parser/
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:49.000000 core_parser_app-2.8.0/tests/tools/parser/parser/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7131 2024-03-12 19:06:49.000000 core_parser_app-2.8.0/tests/tools/parser/parser/test_choice.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5010 2024-03-12 19:06:49.000000 core_parser_app-2.8.0/tests/tools/parser/parser/test_complex_content.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10789 2024-03-12 19:06:49.000000 core_parser_app-2.8.0/tests/tools/parser/parser/test_complex_type.py
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)    11082 2024-03-12 19:06:49.000000 core_parser_app-2.8.0/tests/tools/parser/parser/test_element.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8882 2024-03-12 19:06:49.000000 core_parser_app-2.8.0/tests/tools/parser/parser/test_extension.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      876 2024-03-12 19:06:49.000000 core_parser_app-2.8.0/tests/tools/parser/parser/test_parser.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3811 2024-03-12 19:06:49.000000 core_parser_app-2.8.0/tests/tools/parser/parser/test_restriction.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7071 2024-03-12 19:06:49.000000 core_parser_app-2.8.0/tests/tools/parser/parser/test_sequence.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:57.495157 core_parser_app-2.8.0/tests/tools/parser/renderer/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:49.000000 core_parser_app-2.8.0/tests/tools/parser/renderer/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:57.541209 core_parser_app-2.8.0/tests/tools/parser/renderer/list/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:49.000000 core_parser_app-2.8.0/tests/tools/parser/renderer/list/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1546 2024-03-12 19:06:49.000000 core_parser_app-2.8.0/tests/tools/parser/renderer/list/tests_unit.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1959 2024-03-12 19:06:49.000000 core_parser_app-2.8.0/tests/tools/parser/renderer/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:57.562932 core_parser_app-2.8.0/tests/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:49.000000 core_parser_app-2.8.0/tests/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:57.604755 core_parser_app-2.8.0/tests/views/common/
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:49.000000 core_parser_app-2.8.0/tests/views/common/__init__.py
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     1288 2024-03-12 19:06:49.000000 core_parser_app-2.8.0/tests/views/common/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:57.624621 core_parser_app-2.8.0/tests/views/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:49.000000 core_parser_app-2.8.0/tests/views/user/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:57.685189 core_parser_app-2.8.0/tests/views/user/ajax/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 19:06:49.000000 core_parser_app-2.8.0/tests/views/user/ajax/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1980 2024-03-12 19:06:49.000000 core_parser_app-2.8.0/tests/views/user/ajax/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5125 2024-03-12 19:06:49.000000 core_parser_app-2.8.0/tests/views/user/ajax/test_int_access_control.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:10.615356 core_parser_app-2.9.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2024-05-13 16:11:50.000000 core_parser_app-2.9.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      395 2024-05-13 16:11:50.000000 core_parser_app-2.9.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2332 2024-05-13 16:12:10.609356 core_parser_app-2.9.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1696 2024-05-13 16:11:50.000000 core_parser_app-2.9.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:06.903877 core_parser_app-2.9.0/core_parser_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       64 2024-05-13 16:11:50.000000 core_parser_app-2.9.0/core_parser_app/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4397 2024-05-13 16:11:50.000000 core_parser_app-2.9.0/core_parser_app/access_control.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1411 2024-05-13 16:11:50.000000 core_parser_app-2.9.0/core_parser_app/admin.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      205 2024-05-13 16:11:50.000000 core_parser_app-2.9.0/core_parser_app/apps.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:07.022087 core_parser_app-2.9.0/core_parser_app/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:50.000000 core_parser_app-2.9.0/core_parser_app/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:07.105632 core_parser_app-2.9.0/core_parser_app/components/data_structure/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:50.000000 core_parser_app-2.9.0/core_parser_app/components/data_structure/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      376 2024-05-13 16:11:50.000000 core_parser_app-2.9.0/core_parser_app/components/data_structure/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      304 2024-05-13 16:11:50.000000 core_parser_app-2.9.0/core_parser_app/components/data_structure/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6887 2024-05-13 16:11:50.000000 core_parser_app-2.9.0/core_parser_app/components/data_structure/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:07.160783 core_parser_app-2.9.0/core_parser_app/components/data_structure_element/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:50.000000 core_parser_app-2.9.0/core_parser_app/components/data_structure_element/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      398 2024-05-13 16:11:50.000000 core_parser_app-2.9.0/core_parser_app/components/data_structure_element/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2871 2024-05-13 16:11:50.000000 core_parser_app-2.9.0/core_parser_app/components/data_structure_element/api.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:07.235416 core_parser_app-2.9.0/core_parser_app/components/module/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:50.000000 core_parser_app-2.9.0/core_parser_app/components/module/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      353 2024-05-13 16:11:50.000000 core_parser_app-2.9.0/core_parser_app/components/module/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2236 2024-05-13 16:11:50.000000 core_parser_app-2.9.0/core_parser_app/components/module/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1887 2024-05-13 16:11:50.000000 core_parser_app-2.9.0/core_parser_app/components/module/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:07.253048 core_parser_app-2.9.0/core_parser_app/management/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:50.000000 core_parser_app-2.9.0/core_parser_app/management/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:07.295491 core_parser_app-2.9.0/core_parser_app/management/commands/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:50.000000 core_parser_app-2.9.0/core_parser_app/management/commands/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      565 2024-05-13 16:11:50.000000 core_parser_app-2.9.0/core_parser_app/management/commands/loadmodules.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:07.340870 core_parser_app-2.9.0/core_parser_app/migrations/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3972 2024-05-13 16:11:50.000000 core_parser_app-2.9.0/core_parser_app/migrations/0001_initial.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:50.000000 core_parser_app-2.9.0/core_parser_app/migrations/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      880 2024-05-13 16:11:50.000000 core_parser_app-2.9.0/core_parser_app/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:06.146986 core_parser_app-2.9.0/core_parser_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:06.151115 core_parser_app-2.9.0/core_parser_app/static/core_parser_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:06.166397 core_parser_app-2.9.0/core_parser_app/static/core_parser_app/common/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:07.376388 core_parser_app-2.9.0/core_parser_app/static/core_parser_app/common/css/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      161 2024-05-13 16:11:50.000000 core_parser_app-2.9.0/core_parser_app/static/core_parser_app/common/css/modules.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:07.416250 core_parser_app-2.9.0/core_parser_app/static/core_parser_app/common/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3620 2024-05-13 16:11:50.000000 core_parser_app-2.9.0/core_parser_app/static/core_parser_app/common/js/module_manager.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      169 2024-05-13 16:11:50.000000 core_parser_app-2.9.0/core_parser_app/static/core_parser_app/common/js/module_manager.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:07.473271 core_parser_app-2.9.0/core_parser_app/static/core_parser_app/common/xsd/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2682 2024-05-13 16:11:50.000000 core_parser_app-2.9.0/core_parser_app/static/core_parser_app/common/xsd/annotations.xsd
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      996 2024-05-13 16:11:50.000000 core_parser_app-2.9.0/core_parser_app/static/core_parser_app/common/xsd/boolean.xsd
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      996 2024-05-13 16:11:50.000000 core_parser_app-2.9.0/core_parser_app/static/core_parser_app/common/xsd/date.xsd
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:07.512860 core_parser_app-2.9.0/core_parser_app/system/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:50.000000 core_parser_app-2.9.0/core_parser_app/system/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      533 2024-05-13 16:11:50.000000 core_parser_app-2.9.0/core_parser_app/system/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      346 2024-05-13 16:11:50.000000 core_parser_app-2.9.0/core_parser_app/tasks.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:06.192410 core_parser_app-2.9.0/core_parser_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:06.196523 core_parser_app-2.9.0/core_parser_app/templates/core_parser_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:07.568264 core_parser_app-2.9.0/core_parser_app/templates/core_parser_app/common/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:07.592813 core_parser_app-2.9.0/core_parser_app/templates/core_parser_app/common/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1067 2024-05-13 16:11:50.000000 core_parser_app-2.9.0/core_parser_app/templates/core_parser_app/common/modals/add_module.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      268 2024-05-13 16:11:50.000000 core_parser_app-2.9.0/core_parser_app/templates/core_parser_app/common/module_manager.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      695 2024-05-13 16:11:50.000000 core_parser_app-2.9.0/core_parser_app/templates/core_parser_app/common/module_manager_box.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      473 2024-05-13 16:11:50.000000 core_parser_app-2.9.0/core_parser_app/templates/core_parser_app/common/modules.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:07.615465 core_parser_app-2.9.0/core_parser_app/tools/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:50.000000 core_parser_app-2.9.0/core_parser_app/tools/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:07.724378 core_parser_app-2.9.0/core_parser_app/tools/modules/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:50.000000 core_parser_app-2.9.0/core_parser_app/tools/modules/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2961 2024-05-13 16:11:50.000000 core_parser_app-2.9.0/core_parser_app/tools/modules/discover.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      182 2024-05-13 16:11:50.000000 core_parser_app-2.9.0/core_parser_app/tools/modules/exceptions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1825 2024-05-13 16:11:50.000000 core_parser_app-2.9.0/core_parser_app/tools/modules/sanitize.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:06.228497 core_parser_app-2.9.0/core_parser_app/tools/modules/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:06.289757 core_parser_app-2.9.0/core_parser_app/tools/modules/static/core_parser_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:06.244475 core_parser_app-2.9.0/core_parser_app/tools/modules/static/core_parser_app/css/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:07.777199 core_parser_app-2.9.0/core_parser_app/tools/modules/static/core_parser_app/css/builtin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       86 2024-05-13 16:11:50.000000 core_parser_app-2.9.0/core_parser_app/tools/modules/static/core_parser_app/css/builtin/checkboxes.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      128 2024-05-13 16:11:50.000000 core_parser_app-2.9.0/core_parser_app/tools/modules/static/core_parser_app/css/builtin/textarea.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:07.811216 core_parser_app-2.9.0/core_parser_app/tools/modules/static/core_parser_app/js/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:07.921123 core_parser_app-2.9.0/core_parser_app/tools/modules/static/core_parser_app/js/builtin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      128 2024-05-13 16:11:50.000000 core_parser_app-2.9.0/core_parser_app/tools/modules/static/core_parser_app/js/builtin/autocomplete.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      412 2024-05-13 16:11:51.000000 core_parser_app-2.9.0/core_parser_app/tools/modules/static/core_parser_app/js/builtin/checkboxes.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      265 2024-05-13 16:11:51.000000 core_parser_app-2.9.0/core_parser_app/tools/modules/static/core_parser_app/js/builtin/input.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      227 2024-05-13 16:11:51.000000 core_parser_app-2.9.0/core_parser_app/tools/modules/static/core_parser_app/js/builtin/options.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1379 2024-05-13 16:11:51.000000 core_parser_app-2.9.0/core_parser_app/tools/modules/static/core_parser_app/js/builtin/popup.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      240 2024-05-13 16:11:51.000000 core_parser_app-2.9.0/core_parser_app/tools/modules/static/core_parser_app/js/builtin/sync_input.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      229 2024-05-13 16:11:51.000000 core_parser_app-2.9.0/core_parser_app/tools/modules/static/core_parser_app/js/builtin/textarea.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:07.939046 core_parser_app-2.9.0/core_parser_app/tools/modules/static/core_parser_app/js/commons/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      512 2024-05-13 16:11:51.000000 core_parser_app-2.9.0/core_parser_app/tools/modules/static/core_parser_app/js/commons/file_uploader.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3135 2024-05-13 16:11:51.000000 core_parser_app-2.9.0/core_parser_app/tools/modules/static/core_parser_app/js/modules.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       75 2024-05-13 16:11:51.000000 core_parser_app-2.9.0/core_parser_app/tools/modules/static/core_parser_app/js/modules.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:07.966744 core_parser_app-2.9.0/core_parser_app/tools/modules/static/core_parser_app/xsl/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6048 2024-05-13 16:11:51.000000 core_parser_app-2.9.0/core_parser_app/tools/modules/static/core_parser_app/xsl/xsd2html4modules.xsl
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:06.301935 core_parser_app-2.9.0/core_parser_app/tools/modules/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:07.988418 core_parser_app-2.9.0/core_parser_app/tools/modules/templates/core_parser_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:08.159842 core_parser_app-2.9.0/core_parser_app/tools/modules/templates/core_parser_app/builtin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      142 2024-05-13 16:11:51.000000 core_parser_app-2.9.0/core_parser_app/tools/modules/templates/core_parser_app/builtin/autocomplete.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      303 2024-05-13 16:11:51.000000 core_parser_app-2.9.0/core_parser_app/tools/modules/templates/core_parser_app/builtin/checkboxes.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      255 2024-05-13 16:11:51.000000 core_parser_app-2.9.0/core_parser_app/tools/modules/templates/core_parser_app/builtin/input.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      149 2024-05-13 16:11:51.000000 core_parser_app-2.9.0/core_parser_app/tools/modules/templates/core_parser_app/builtin/input_button.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      577 2024-05-13 16:11:51.000000 core_parser_app-2.9.0/core_parser_app/tools/modules/templates/core_parser_app/builtin/modal_wrapper.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      237 2024-05-13 16:11:51.000000 core_parser_app-2.9.0/core_parser_app/tools/modules/templates/core_parser_app/builtin/options.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      267 2024-05-13 16:11:51.000000 core_parser_app-2.9.0/core_parser_app/tools/modules/templates/core_parser_app/builtin/popup.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      254 2024-05-13 16:11:51.000000 core_parser_app-2.9.0/core_parser_app/tools/modules/templates/core_parser_app/builtin/sync_input.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      126 2024-05-13 16:11:51.000000 core_parser_app-2.9.0/core_parser_app/tools/modules/templates/core_parser_app/builtin/textarea.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:08.176511 core_parser_app-2.9.0/core_parser_app/tools/modules/templates/core_parser_app/commons/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      477 2024-05-13 16:11:51.000000 core_parser_app-2.9.0/core_parser_app/tools/modules/templates/core_parser_app/commons/file_uploader.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      264 2024-05-13 16:11:51.000000 core_parser_app-2.9.0/core_parser_app/tools/modules/templates/core_parser_app/module.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      352 2024-05-13 16:11:51.000000 core_parser_app-2.9.0/core_parser_app/tools/modules/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:08.260013 core_parser_app-2.9.0/core_parser_app/tools/modules/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:51.000000 core_parser_app-2.9.0/core_parser_app/tools/modules/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:08.434115 core_parser_app-2.9.0/core_parser_app/tools/modules/views/builtin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:51.000000 core_parser_app-2.9.0/core_parser_app/tools/modules/views/builtin/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1022 2024-05-13 16:11:51.000000 core_parser_app-2.9.0/core_parser_app/tools/modules/views/builtin/autocomplete_module.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3012 2024-05-13 16:11:51.000000 core_parser_app-2.9.0/core_parser_app/tools/modules/views/builtin/checkboxes_module.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1253 2024-05-13 16:11:51.000000 core_parser_app-2.9.0/core_parser_app/tools/modules/views/builtin/input_button_module.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1533 2024-05-13 16:11:51.000000 core_parser_app-2.9.0/core_parser_app/tools/modules/views/builtin/input_module.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1882 2024-05-13 16:11:51.000000 core_parser_app-2.9.0/core_parser_app/tools/modules/views/builtin/options_module.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1300 2024-05-13 16:11:51.000000 core_parser_app-2.9.0/core_parser_app/tools/modules/views/builtin/popup_module.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1627 2024-05-13 16:11:51.000000 core_parser_app-2.9.0/core_parser_app/tools/modules/views/builtin/sync_input_module.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1011 2024-05-13 16:11:51.000000 core_parser_app-2.9.0/core_parser_app/tools/modules/views/builtin/textarea_module.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7741 2024-05-13 16:11:51.000000 core_parser_app-2.9.0/core_parser_app/tools/modules/views/module.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4172 2024-05-13 16:11:51.000000 core_parser_app-2.9.0/core_parser_app/tools/modules/views/views.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3201 2024-05-13 16:11:51.000000 core_parser_app-2.9.0/core_parser_app/tools/modules/xpathaccessor.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:08.498864 core_parser_app-2.9.0/core_parser_app/tools/parser/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:51.000000 core_parser_app-2.9.0/core_parser_app/tools/parser/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      326 2024-05-13 16:11:51.000000 core_parser_app-2.9.0/core_parser_app/tools/parser/exceptions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)   117543 2024-05-13 16:11:51.000000 core_parser_app-2.9.0/core_parser_app/tools/parser/parser.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:08.612079 core_parser_app-2.9.0/core_parser_app/tools/parser/renderer/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8352 2024-05-13 16:11:51.000000 core_parser_app-2.9.0/core_parser_app/tools/parser/renderer/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      901 2024-05-13 16:11:51.000000 core_parser_app-2.9.0/core_parser_app/tools/parser/renderer/checkbox.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    27114 2024-05-13 16:11:51.000000 core_parser_app-2.9.0/core_parser_app/tools/parser/renderer/list.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10019 2024-05-13 16:11:51.000000 core_parser_app-2.9.0/core_parser_app/tools/parser/renderer/table.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    24119 2024-05-13 16:11:51.000000 core_parser_app-2.9.0/core_parser_app/tools/parser/renderer/xml.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:06.352391 core_parser_app-2.9.0/core_parser_app/tools/parser/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:06.371120 core_parser_app-2.9.0/core_parser_app/tools/parser/static/core_parser_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:08.641705 core_parser_app-2.9.0/core_parser_app/tools/parser/static/core_parser_app/css/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      958 2024-05-13 16:11:51.000000 core_parser_app-2.9.0/core_parser_app/tools/parser/static/core_parser_app/css/use.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:08.744142 core_parser_app-2.9.0/core_parser_app/tools/parser/static/core_parser_app/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      934 2024-05-13 16:11:51.000000 core_parser_app-2.9.0/core_parser_app/tools/parser/static/core_parser_app/js/autosave.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       89 2024-05-13 16:11:51.000000 core_parser_app-2.9.0/core_parser_app/tools/parser/static/core_parser_app/js/autosave.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      882 2024-05-13 16:11:51.000000 core_parser_app-2.9.0/core_parser_app/tools/parser/static/core_parser_app/js/autosave_checkbox.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4647 2024-05-13 16:11:51.000000 core_parser_app-2.9.0/core_parser_app/tools/parser/static/core_parser_app/js/buttons.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5179 2024-05-13 16:11:51.000000 core_parser_app-2.9.0/core_parser_app/tools/parser/static/core_parser_app/js/choice.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:06.384649 core_parser_app-2.9.0/core_parser_app/tools/parser/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:06.431132 core_parser_app-2.9.0/core_parser_app/tools/parser/templates/renderer/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:08.812225 core_parser_app-2.9.0/core_parser_app/tools/parser/templates/renderer/default/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:08.889022 core_parser_app-2.9.0/core_parser_app/tools/parser/templates/renderer/default/buttons/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       98 2024-05-13 16:11:51.000000 core_parser_app-2.9.0/core_parser_app/tools/parser/templates/renderer/default/buttons/add.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       81 2024-05-13 16:11:51.000000 core_parser_app-2.9.0/core_parser_app/tools/parser/templates/renderer/default/buttons/collapse.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      104 2024-05-13 16:11:51.000000 core_parser_app-2.9.0/core_parser_app/tools/parser/templates/renderer/default/buttons/delete.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      110 2024-05-13 16:11:51.000000 core_parser_app-2.9.0/core_parser_app/tools/parser/templates/renderer/default/form-error.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:08.987076 core_parser_app-2.9.0/core_parser_app/tools/parser/templates/renderer/default/inputs/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      346 2024-05-13 16:11:51.000000 core_parser_app-2.9.0/core_parser_app/tools/parser/templates/renderer/default/inputs/boolean.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       76 2024-05-13 16:11:51.000000 core_parser_app-2.9.0/core_parser_app/tools/parser/templates/renderer/default/inputs/checkbox.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      502 2024-05-13 16:11:51.000000 core_parser_app-2.9.0/core_parser_app/tools/parser/templates/renderer/default/inputs/date.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      490 2024-05-13 16:11:51.000000 core_parser_app-2.9.0/core_parser_app/tools/parser/templates/renderer/default/inputs/input.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      446 2024-05-13 16:11:51.000000 core_parser_app-2.9.0/core_parser_app/tools/parser/templates/renderer/default/inputs/select.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:09.033331 core_parser_app-2.9.0/core_parser_app/tools/parser/templates/renderer/default/test/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       44 2024-05-13 16:11:51.000000 core_parser_app-2.9.0/core_parser_app/tools/parser/templates/renderer/default/test/sample_no_data.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       52 2024-05-13 16:11:51.000000 core_parser_app-2.9.0/core_parser_app/tools/parser/templates/renderer/default/test/sample_with_data.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       83 2024-05-13 16:11:51.000000 core_parser_app-2.9.0/core_parser_app/tools/parser/templates/renderer/default/ul.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       86 2024-05-13 16:11:51.000000 core_parser_app-2.9.0/core_parser_app/tools/parser/templates/renderer/default/warning.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:09.099874 core_parser_app-2.9.0/core_parser_app/tools/parser/templates/renderer/list/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      149 2024-05-13 16:11:51.000000 core_parser_app-2.9.0/core_parser_app/tools/parser/templates/renderer/list/attributes.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       75 2024-05-13 16:11:51.000000 core_parser_app-2.9.0/core_parser_app/tools/parser/templates/renderer/list/li.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      131 2024-05-13 16:11:51.000000 core_parser_app-2.9.0/core_parser_app/tools/parser/templates/renderer/list/ul.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:09.157607 core_parser_app-2.9.0/core_parser_app/tools/parser/templates/renderer/table/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       99 2024-05-13 16:11:52.000000 core_parser_app-2.9.0/core_parser_app/tools/parser/templates/renderer/table/table.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       75 2024-05-13 16:11:52.000000 core_parser_app-2.9.0/core_parser_app/tools/parser/templates/renderer/table/tr.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       41 2024-05-13 16:11:52.000000 core_parser_app-2.9.0/core_parser_app/tools/parser/templates/renderer/table/wrap.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:09.177123 core_parser_app-2.9.0/core_parser_app/tools/parser/templates/renderer/xml/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       99 2024-05-13 16:11:52.000000 core_parser_app-2.9.0/core_parser_app/tools/parser/templates/renderer/xml/element.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:09.233440 core_parser_app-2.9.0/core_parser_app/tools/parser/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:52.000000 core_parser_app-2.9.0/core_parser_app/tools/parser/utils/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      278 2024-05-13 16:11:52.000000 core_parser_app-2.9.0/core_parser_app/tools/parser/utils/rendering.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3519 2024-05-13 16:11:52.000000 core_parser_app-2.9.0/core_parser_app/tools/parser/utils/xml.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1075 2024-05-13 16:11:52.000000 core_parser_app-2.9.0/core_parser_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:09.271034 core_parser_app-2.9.0/core_parser_app/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:52.000000 core_parser_app-2.9.0/core_parser_app/utils/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2190 2024-05-13 16:11:52.000000 core_parser_app-2.9.0/core_parser_app/utils/xml.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:09.290492 core_parser_app-2.9.0/core_parser_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:52.000000 core_parser_app-2.9.0/core_parser_app/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:09.334346 core_parser_app-2.9.0/core_parser_app/views/admin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:52.000000 core_parser_app-2.9.0/core_parser_app/views/admin/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1592 2024-05-13 16:11:52.000000 core_parser_app-2.9.0/core_parser_app/views/admin/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:09.400881 core_parser_app-2.9.0/core_parser_app/views/common/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:52.000000 core_parser_app-2.9.0/core_parser_app/views/common/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1808 2024-05-13 16:11:52.000000 core_parser_app-2.9.0/core_parser_app/views/common/ajax.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3516 2024-05-13 16:11:52.000000 core_parser_app-2.9.0/core_parser_app/views/common/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:09.442824 core_parser_app-2.9.0/core_parser_app/views/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:52.000000 core_parser_app-2.9.0/core_parser_app/views/user/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2477 2024-05-13 16:11:52.000000 core_parser_app-2.9.0/core_parser_app/views/user/ajax.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:07.000131 core_parser_app-2.9.0/core_parser_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2332 2024-05-13 16:12:04.000000 core_parser_app-2.9.0/core_parser_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9531 2024-05-13 16:12:05.000000 core_parser_app-2.9.0/core_parser_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2024-05-13 16:12:05.000000 core_parser_app-2.9.0/core_parser_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       67 2024-05-13 16:12:05.000000 core_parser_app-2.9.0/core_parser_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       22 2024-05-13 16:12:05.000000 core_parser_app-2.9.0/core_parser_app.egg-info/top_level.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2024-05-13 16:11:53.000000 core_parser_app-2.9.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       21 2024-05-13 16:11:53.000000 core_parser_app-2.9.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       46 2024-05-13 16:11:53.000000 core_parser_app-2.9.0/requirements.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2024-05-13 16:12:10.617522 core_parser_app-2.9.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1441 2024-05-13 16:11:53.000000 core_parser_app-2.9.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:09.582114 core_parser_app-2.9.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:53.000000 core_parser_app-2.9.0/tests/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:09.622393 core_parser_app-2.9.0/tests/access_control/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:53.000000 core_parser_app-2.9.0/tests/access_control/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2180 2024-05-13 16:11:53.000000 core_parser_app-2.9.0/tests/access_control/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:09.667917 core_parser_app-2.9.0/tests/commands/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:53.000000 core_parser_app-2.9.0/tests/commands/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      406 2024-05-13 16:11:53.000000 core_parser_app-2.9.0/tests/commands/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:09.690140 core_parser_app-2.9.0/tests/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:53.000000 core_parser_app-2.9.0/tests/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:09.759429 core_parser_app-2.9.0/tests/components/data_structure/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:53.000000 core_parser_app-2.9.0/tests/components/data_structure/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:53.000000 core_parser_app-2.9.0/tests/components/data_structure/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1619 2024-05-13 16:11:53.000000 core_parser_app-2.9.0/tests/components/data_structure/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:09.845874 core_parser_app-2.9.0/tests/components/data_structure_element/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:53.000000 core_parser_app-2.9.0/tests/components/data_structure_element/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:09.886394 core_parser_app-2.9.0/tests/components/data_structure_element/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:53.000000 core_parser_app-2.9.0/tests/components/data_structure_element/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6726 2024-05-13 16:11:53.000000 core_parser_app-2.9.0/tests/components/data_structure_element/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    20077 2024-05-13 16:11:53.000000 core_parser_app-2.9.0/tests/components/data_structure_element/test_int_access_control.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5869 2024-05-13 16:11:53.000000 core_parser_app-2.9.0/tests/components/data_structure_element/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4901 2024-05-13 16:11:53.000000 core_parser_app-2.9.0/tests/components/data_structure_element/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:09.962498 core_parser_app-2.9.0/tests/components/module/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:53.000000 core_parser_app-2.9.0/tests/components/module/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5876 2024-05-13 16:11:53.000000 core_parser_app-2.9.0/tests/components/module/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:10.003805 core_parser_app-2.9.0/tests/discover/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:53.000000 core_parser_app-2.9.0/tests/discover/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4223 2024-05-13 16:11:53.000000 core_parser_app-2.9.0/tests/discover/tests_unit.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1093 2024-05-13 16:11:53.000000 core_parser_app-2.9.0/tests/fixtures_utils.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      646 2024-05-13 16:11:53.000000 core_parser_app-2.9.0/tests/models.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      185 2024-05-13 16:11:53.000000 core_parser_app-2.9.0/tests/rights.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1026 2024-05-13 16:11:53.000000 core_parser_app-2.9.0/tests/test_settings.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2718 2024-05-13 16:11:53.000000 core_parser_app-2.9.0/tests/test_utils.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:10.026083 core_parser_app-2.9.0/tests/tools/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:53.000000 core_parser_app-2.9.0/tests/tools/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:10.051231 core_parser_app-2.9.0/tests/tools/modules/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:53.000000 core_parser_app-2.9.0/tests/tools/modules/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:10.150666 core_parser_app-2.9.0/tests/tools/modules/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:53.000000 core_parser_app-2.9.0/tests/tools/modules/tests/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2950 2024-05-13 16:11:53.000000 core_parser_app-2.9.0/tests/tools/modules/tests/tests_unit_checkboxes_module.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9401 2024-05-13 16:11:53.000000 core_parser_app-2.9.0/tests/tools/modules/tests/tests_unit_module.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2292 2024-05-13 16:11:53.000000 core_parser_app-2.9.0/tests/tools/modules/tests/tests_unit_sanitize.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:10.169946 core_parser_app-2.9.0/tests/tools/parser/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:53.000000 core_parser_app-2.9.0/tests/tools/parser/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:10.329648 core_parser_app-2.9.0/tests/tools/parser/parser/
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:56.000000 core_parser_app-2.9.0/tests/tools/parser/parser/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7131 2024-05-13 16:11:56.000000 core_parser_app-2.9.0/tests/tools/parser/parser/test_choice.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5010 2024-05-13 16:11:56.000000 core_parser_app-2.9.0/tests/tools/parser/parser/test_complex_content.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10789 2024-05-13 16:11:56.000000 core_parser_app-2.9.0/tests/tools/parser/parser/test_complex_type.py
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)    11082 2024-05-13 16:11:56.000000 core_parser_app-2.9.0/tests/tools/parser/parser/test_element.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8882 2024-05-13 16:11:56.000000 core_parser_app-2.9.0/tests/tools/parser/parser/test_extension.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      876 2024-05-13 16:11:56.000000 core_parser_app-2.9.0/tests/tools/parser/parser/test_parser.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3811 2024-05-13 16:11:56.000000 core_parser_app-2.9.0/tests/tools/parser/parser/test_restriction.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7071 2024-05-13 16:11:56.000000 core_parser_app-2.9.0/tests/tools/parser/parser/test_sequence.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:10.366642 core_parser_app-2.9.0/tests/tools/parser/renderer/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:56.000000 core_parser_app-2.9.0/tests/tools/parser/renderer/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:10.405910 core_parser_app-2.9.0/tests/tools/parser/renderer/list/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:56.000000 core_parser_app-2.9.0/tests/tools/parser/renderer/list/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1546 2024-05-13 16:11:56.000000 core_parser_app-2.9.0/tests/tools/parser/renderer/list/tests_unit.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1959 2024-05-13 16:11:56.000000 core_parser_app-2.9.0/tests/tools/parser/renderer/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:10.427723 core_parser_app-2.9.0/tests/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:56.000000 core_parser_app-2.9.0/tests/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:10.488396 core_parser_app-2.9.0/tests/views/common/
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:57.000000 core_parser_app-2.9.0/tests/views/common/__init__.py
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     1288 2024-05-13 16:11:57.000000 core_parser_app-2.9.0/tests/views/common/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:10.508118 core_parser_app-2.9.0/tests/views/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:57.000000 core_parser_app-2.9.0/tests/views/user/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:12:10.577049 core_parser_app-2.9.0/tests/views/user/ajax/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:11:57.000000 core_parser_app-2.9.0/tests/views/user/ajax/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1980 2024-05-13 16:11:57.000000 core_parser_app-2.9.0/tests/views/user/ajax/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5125 2024-05-13 16:11:57.000000 core_parser_app-2.9.0/tests/views/user/ajax/test_int_access_control.py
```

### Comparing `core_parser_app-2.8.0/LICENSE.md` & `core_parser_app-2.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.8.0/PKG-INFO` & `core_parser_app-2.9.0/core_parser_app.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
-Name: core_parser_app
-Version: 2.8.0
+Name: core-parser-app
+Version: 2.9.0
 Summary: XSD parser tools for the curator core project
 Home-page: https://github.com/usnistgov/core_parser_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: ===============
         Core Parser App
```

### Comparing `core_parser_app-2.8.0/README.rst` & `core_parser_app-2.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.8.0/core_parser_app/access_control.py` & `core_parser_app-2.9.0/core_parser_app/access_control.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.8.0/core_parser_app/admin.py` & `core_parser_app-2.9.0/core_parser_app/admin.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.8.0/core_parser_app/components/data_structure/models.py` & `core_parser_app-2.9.0/core_parser_app/components/data_structure/models.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.8.0/core_parser_app/components/data_structure_element/api.py` & `core_parser_app-2.9.0/core_parser_app/components/data_structure_element/api.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.8.0/core_parser_app/components/module/api.py` & `core_parser_app-2.9.0/core_parser_app/components/module/api.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.8.0/core_parser_app/components/module/models.py` & `core_parser_app-2.9.0/core_parser_app/components/module/models.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.8.0/core_parser_app/migrations/0001_initial.py` & `core_parser_app-2.9.0/core_parser_app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.8.0/core_parser_app/settings.py` & `core_parser_app-2.9.0/core_parser_app/settings.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.8.0/core_parser_app/static/core_parser_app/common/js/module_manager.js` & `core_parser_app-2.9.0/core_parser_app/static/core_parser_app/common/js/module_manager.js`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.8.0/core_parser_app/static/core_parser_app/common/xsd/annotations.xsd` & `core_parser_app-2.9.0/core_parser_app/static/core_parser_app/common/xsd/annotations.xsd`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.8.0/core_parser_app/static/core_parser_app/common/xsd/boolean.xsd` & `core_parser_app-2.9.0/core_parser_app/static/core_parser_app/common/xsd/boolean.xsd`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.8.0/core_parser_app/static/core_parser_app/common/xsd/date.xsd` & `core_parser_app-2.9.0/core_parser_app/static/core_parser_app/common/xsd/date.xsd`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.8.0/core_parser_app/system/api.py` & `core_parser_app-2.9.0/core_parser_app/system/api.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.8.0/core_parser_app/templates/core_parser_app/common/modals/add_module.html` & `core_parser_app-2.9.0/core_parser_app/templates/core_parser_app/common/modals/add_module.html`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.8.0/core_parser_app/templates/core_parser_app/common/module_manager_box.html` & `core_parser_app-2.9.0/core_parser_app/templates/core_parser_app/common/module_manager_box.html`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.8.0/core_parser_app/tools/modules/discover.py` & `core_parser_app-2.9.0/core_parser_app/tools/modules/discover.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,77 +1,101 @@
 """Auto discovery of modules
 """
 import logging
 
 from django.db import IntegrityError
+from django.urls import URLPattern, URLResolver
 
 from core_main_app.commons.exceptions import ModelError
 from core_parser_app.components.module import api as module_api
 from core_parser_app.components.module.models import Module
 from core_parser_app.tools.modules.exceptions import ModuleError
 from core_parser_app.tools.modules.views.module import AbstractModule
 
 logger = logging.getLogger(__name__)
 
 
-def discover_modules(urls):
-    """
+def reload_modules(urls):
+    """Reload modules in database
 
     :return:
     """
     logger.info("START discover modules.")
 
     try:
         # Remove all existing modules
         module_api.delete_all()
-    except Exception:
-        logger.warning("Module table is not ready yet")
+    except Exception as exc:
+        logger.warning(str(exc))
         return
 
     # Look for modules in project urls
     try:
         for url in urls:
-            if hasattr(url, "url_patterns"):
+            if isinstance(url, URLPattern):
+                _save_module(url)
+            elif isinstance(url, URLResolver):
                 for url_pattern in url.url_patterns:
-                    module_view_name = (
-                        url_pattern.lookup_str
-                        if hasattr(url_pattern, "lookup_str")
-                        else ""
-                    )
-                    if module_view_name.startswith("core_module_"):
-                        module_view = AbstractModule.get_view_from_view_path(
-                            module_view_name
-                        )
-                        if issubclass(module_view, AbstractModule):
-                            # FIXME: do not use private field
-                            module_object = Module(
-                                url=url_pattern.pattern._regex,
-                                name=url_pattern.name,
-                                view=module_view_name,
-                                multiple=module_view.is_managing_occurrences,
-                            )
-                            try:
-                                module_api.upsert(module_object)
-                            except IntegrityError:
-                                logger.info(
-                                    "The module %s is already present in the database.",
-                                    url_pattern.name,
-                                )
+                    _save_module(url_pattern)
     except ModelError:
         # something went wrong, delete already added modules
-        module_api.delete_all()
-
         error_msg = (
             "A validation error occurred during the module discovery. "
             "Please provide a name to all modules urls using the name argument."
         )
 
-        logger.error("Discover modules failed with %s.", error_msg)
-
+        logger.error(
+            "Discover modules failed with error %s. All modules will be deleted.",
+            error_msg,
+        )
+        module_api.delete_all()
         raise ModuleError(error_msg)
     except Exception as exception:
         # something went wrong, delete already added modules
+        logger.error(
+            "Discover modules failed with error %s. All modules will be deleted.",
+            str(exception),
+        )
         module_api.delete_all()
-        logger.error("Discover modules failed with %s.", str(exception))
         raise exception
 
     logger.info("FINISH discover modules.")
+
+
+def _save_module(url_pattern):
+    """Save module from a URL pattern
+
+    Args:
+        url_pattern:
+
+    Returns:
+
+    """
+    module_view_name = _get_module_view_name_from_url(url_pattern)
+    if module_view_name.startswith("core_module_"):
+        module_view = AbstractModule.get_view_from_view_path(module_view_name)
+        if issubclass(module_view, AbstractModule):
+            module_object = Module(
+                url=url_pattern.pattern.regex.pattern,
+                name=url_pattern.name,
+                view=module_view_name,
+                multiple=module_view.is_managing_occurrences,
+            )
+            try:
+                module_api.upsert(module_object)
+            except IntegrityError:
+                logger.info(
+                    "The module %s is already present in the database.",
+                    url_pattern.name,
+                )
+
+
+def _get_module_view_name_from_url(url_pattern):
+    """
+
+    Args:
+        url_pattern:
+
+    Returns:
+
+    """
+    return url_pattern.lookup_str if hasattr(url_pattern, "lookup_str") else ""
```

### Comparing `core_parser_app-2.8.0/core_parser_app/tools/modules/sanitize.py` & `core_parser_app-2.9.0/core_parser_app/tools/modules/sanitize.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.8.0/core_parser_app/tools/modules/static/core_parser_app/js/builtin/popup.js` & `core_parser_app-2.9.0/core_parser_app/tools/modules/static/core_parser_app/js/builtin/popup.js`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.8.0/core_parser_app/tools/modules/static/core_parser_app/js/commons/file_uploader.js` & `core_parser_app-2.9.0/core_parser_app/tools/modules/static/core_parser_app/js/commons/file_uploader.js`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.8.0/core_parser_app/tools/modules/static/core_parser_app/js/modules.js` & `core_parser_app-2.9.0/core_parser_app/tools/modules/static/core_parser_app/js/modules.js`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.8.0/core_parser_app/tools/modules/static/core_parser_app/xsl/xsd2html4modules.xsl` & `core_parser_app-2.9.0/core_parser_app/tools/modules/static/core_parser_app/xsl/xsd2html4modules.xsl`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.8.0/core_parser_app/tools/modules/templates/core_parser_app/builtin/modal_wrapper.html` & `core_parser_app-2.9.0/core_parser_app/tools/modules/templates/core_parser_app/builtin/modal_wrapper.html`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.8.0/core_parser_app/tools/modules/views/builtin/autocomplete_module.py` & `core_parser_app-2.9.0/core_parser_app/tools/modules/views/builtin/autocomplete_module.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.8.0/core_parser_app/tools/modules/views/builtin/checkboxes_module.py` & `core_parser_app-2.9.0/core_parser_app/tools/modules/views/builtin/checkboxes_module.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.8.0/core_parser_app/tools/modules/views/builtin/input_button_module.py` & `core_parser_app-2.9.0/core_parser_app/tools/modules/views/builtin/input_button_module.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.8.0/core_parser_app/tools/modules/views/builtin/input_module.py` & `core_parser_app-2.9.0/core_parser_app/tools/modules/views/builtin/input_module.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.8.0/core_parser_app/tools/modules/views/builtin/options_module.py` & `core_parser_app-2.9.0/core_parser_app/tools/modules/views/builtin/options_module.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.8.0/core_parser_app/tools/modules/views/builtin/popup_module.py` & `core_parser_app-2.9.0/core_parser_app/tools/modules/views/builtin/popup_module.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.8.0/core_parser_app/tools/modules/views/builtin/sync_input_module.py` & `core_parser_app-2.9.0/core_parser_app/tools/modules/views/builtin/sync_input_module.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.8.0/core_parser_app/tools/modules/views/builtin/textarea_module.py` & `core_parser_app-2.9.0/core_parser_app/tools/modules/views/builtin/textarea_module.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.8.0/core_parser_app/tools/modules/views/module.py` & `core_parser_app-2.9.0/core_parser_app/tools/modules/views/module.py`

 * *Files 1% similar despite different names*

```diff
@@ -243,15 +243,14 @@
     @staticmethod
     def get_view_from_view_path(view):
         """Returns module view from its view string
 
         :param view:
         :return:
         """
-        # module = module_api.get_by_url(url)
         pkglist = view.split(".")
 
         pkgs = ".".join(pkglist[:-1])
         func = pkglist[-1:][0]
 
         imported_pkgs = importlib.import_module(pkgs)
         return getattr(imported_pkgs, func)
```

### Comparing `core_parser_app-2.8.0/core_parser_app/tools/modules/views/views.py` & `core_parser_app-2.9.0/core_parser_app/tools/modules/views/views.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.8.0/core_parser_app/tools/modules/xpathaccessor.py` & `core_parser_app-2.9.0/core_parser_app/tools/modules/xpathaccessor.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.8.0/core_parser_app/tools/parser/parser.py` & `core_parser_app-2.9.0/core_parser_app/tools/parser/parser.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.8.0/core_parser_app/tools/parser/renderer/__init__.py` & `core_parser_app-2.9.0/core_parser_app/tools/parser/renderer/__init__.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.8.0/core_parser_app/tools/parser/renderer/checkbox.py` & `core_parser_app-2.9.0/core_parser_app/tools/parser/renderer/checkbox.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.8.0/core_parser_app/tools/parser/renderer/list.py` & `core_parser_app-2.9.0/core_parser_app/tools/parser/renderer/list.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.8.0/core_parser_app/tools/parser/renderer/table.py` & `core_parser_app-2.9.0/core_parser_app/tools/parser/renderer/table.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.8.0/core_parser_app/tools/parser/renderer/xml.py` & `core_parser_app-2.9.0/core_parser_app/tools/parser/renderer/xml.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.8.0/core_parser_app/tools/parser/static/core_parser_app/css/use.css` & `core_parser_app-2.9.0/core_parser_app/tools/parser/static/core_parser_app/css/use.css`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.8.0/core_parser_app/tools/parser/static/core_parser_app/js/autosave.js` & `core_parser_app-2.9.0/core_parser_app/tools/parser/static/core_parser_app/js/autosave.js`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.8.0/core_parser_app/tools/parser/static/core_parser_app/js/autosave_checkbox.js` & `core_parser_app-2.9.0/core_parser_app/tools/parser/static/core_parser_app/js/autosave_checkbox.js`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.8.0/core_parser_app/tools/parser/static/core_parser_app/js/buttons.js` & `core_parser_app-2.9.0/core_parser_app/tools/parser/static/core_parser_app/js/buttons.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -56,15 +56,15 @@
                     $data.removeClass();
                     $data.addClass(elementClass);
                 }
 
                 // If new modules are included, we need to load the resources
                 initModules();
 
-                console.log("Element " + elementId + " successfully created");
+                console.log("Element " + elementId + " created");
             },
             error: function() {
                 console.error("An error occurred while generating a new element.");
             },
             complete: function() {
                 unblock_buttons();
             }
@@ -105,15 +105,15 @@
                     });
                 } else if (data.code === 2) { // Elements need to be rewritten
                     console.log('Element ' + elementId + ' need to be rewritten');
                     $element.after(data.html);
                 }
 
                 $element.remove();
-                console.log("Element " + elementId + " successfully removed");
+                console.log("Element " + elementId + " removed");
             },
             error: function() {
                 console.error("An error occurred while generating a new element.");
             },
             complete: function() {
                 unblock_buttons();
             }
```

### Comparing `core_parser_app-2.8.0/core_parser_app/tools/parser/static/core_parser_app/js/choice.js` & `core_parser_app-2.9.0/core_parser_app/tools/parser/static/core_parser_app/js/choice.js`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.8.0/core_parser_app/tools/parser/utils/xml.py` & `core_parser_app-2.9.0/core_parser_app/tools/parser/utils/xml.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.8.0/core_parser_app/urls.py` & `core_parser_app-2.9.0/core_parser_app/urls.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.8.0/core_parser_app/utils/xml.py` & `core_parser_app-2.9.0/core_parser_app/utils/xml.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.8.0/core_parser_app/views/admin/views.py` & `core_parser_app-2.9.0/core_parser_app/views/admin/views.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.8.0/core_parser_app/views/common/ajax.py` & `core_parser_app-2.9.0/core_parser_app/views/common/ajax.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.8.0/core_parser_app/views/common/views.py` & `core_parser_app-2.9.0/core_parser_app/views/common/views.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.8.0/core_parser_app/views/user/ajax.py` & `core_parser_app-2.9.0/core_parser_app/views/user/ajax.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.8.0/core_parser_app.egg-info/PKG-INFO` & `core_parser_app-2.9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
-Name: core-parser-app
-Version: 2.8.0
+Name: core_parser_app
+Version: 2.9.0
 Summary: XSD parser tools for the curator core project
 Home-page: https://github.com/usnistgov/core_parser_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: ===============
         Core Parser App
```

### Comparing `core_parser_app-2.8.0/core_parser_app.egg-info/SOURCES.txt` & `core_parser_app-2.9.0/core_parser_app.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,17 @@
 core_parser_app/components/data_structure_element/__init__.py
 core_parser_app/components/data_structure_element/admin_site.py
 core_parser_app/components/data_structure_element/api.py
 core_parser_app/components/module/__init__.py
 core_parser_app/components/module/admin_site.py
 core_parser_app/components/module/api.py
 core_parser_app/components/module/models.py
+core_parser_app/management/__init__.py
+core_parser_app/management/commands/__init__.py
+core_parser_app/management/commands/loadmodules.py
 core_parser_app/migrations/0001_initial.py
 core_parser_app/migrations/__init__.py
 core_parser_app/static/core_parser_app/common/css/modules.css
 core_parser_app/static/core_parser_app/common/js/module_manager.js
 core_parser_app/static/core_parser_app/common/js/module_manager.raw.js
 core_parser_app/static/core_parser_app/common/xsd/annotations.xsd
 core_parser_app/static/core_parser_app/common/xsd/boolean.xsd
@@ -137,26 +140,30 @@
 tests/fixtures_utils.py
 tests/models.py
 tests/rights.py
 tests/test_settings.py
 tests/test_utils.py
 tests/access_control/__init__.py
 tests/access_control/test_unit.py
+tests/commands/__init__.py
+tests/commands/tests_unit.py
 tests/components/__init__.py
 tests/components/data_structure/__init__.py
 tests/components/data_structure/tests_int.py
 tests/components/data_structure/tests_unit.py
 tests/components/data_structure_element/__init__.py
 tests/components/data_structure_element/test_int_access_control.py
 tests/components/data_structure_element/tests_int.py
 tests/components/data_structure_element/tests_unit.py
 tests/components/data_structure_element/fixtures/__init__.py
 tests/components/data_structure_element/fixtures/fixtures.py
 tests/components/module/__init__.py
 tests/components/module/tests_unit.py
+tests/discover/__init__.py
+tests/discover/tests_unit.py
 tests/tools/__init__.py
 tests/tools/modules/__init__.py
 tests/tools/modules/tests/__init__.py
 tests/tools/modules/tests/tests_unit_checkboxes_module.py
 tests/tools/modules/tests/tests_unit_module.py
 tests/tools/modules/tests/tests_unit_sanitize.py
 tests/tools/parser/__init__.py
```

### Comparing `core_parser_app-2.8.0/setup.py` & `core_parser_app-2.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 chdir(normpath(join(abspath(__file__), pardir)))
 
 dep_links = [r for r in required if r.startswith("https://")]
 required = [req_link(r) if r.startswith("https://") else r for r in required]
 
 setup(
     name="core_parser_app",
-    version="2.8.0",
+    version="2.9.0",
     description="XSD parser tools for the curator core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_parser_app",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `core_parser_app-2.8.0/tests/access_control/test_unit.py` & `core_parser_app-2.9.0/tests/access_control/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.8.0/tests/components/data_structure/tests_unit.py` & `core_parser_app-2.9.0/tests/components/data_structure/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.8.0/tests/components/data_structure_element/fixtures/fixtures.py` & `core_parser_app-2.9.0/tests/components/data_structure_element/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.8.0/tests/components/data_structure_element/test_int_access_control.py` & `core_parser_app-2.9.0/tests/components/data_structure_element/test_int_access_control.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.8.0/tests/components/data_structure_element/tests_int.py` & `core_parser_app-2.9.0/tests/components/data_structure_element/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.8.0/tests/components/data_structure_element/tests_unit.py` & `core_parser_app-2.9.0/tests/components/data_structure_element/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.8.0/tests/components/module/tests_unit.py` & `core_parser_app-2.9.0/tests/components/module/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.8.0/tests/fixtures_utils.py` & `core_parser_app-2.9.0/tests/fixtures_utils.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.8.0/tests/models.py` & `core_parser_app-2.9.0/tests/models.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.8.0/tests/test_settings.py` & `core_parser_app-2.9.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.8.0/tests/test_utils.py` & `core_parser_app-2.9.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.8.0/tests/tools/modules/tests/tests_unit_checkboxes_module.py` & `core_parser_app-2.9.0/tests/tools/modules/tests/tests_unit_checkboxes_module.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.8.0/tests/tools/modules/tests/tests_unit_module.py` & `core_parser_app-2.9.0/tests/tools/modules/tests/tests_unit_module.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.8.0/tests/tools/modules/tests/tests_unit_sanitize.py` & `core_parser_app-2.9.0/tests/tools/modules/tests/tests_unit_sanitize.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.8.0/tests/tools/parser/parser/test_choice.py` & `core_parser_app-2.9.0/tests/tools/parser/parser/test_choice.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.8.0/tests/tools/parser/parser/test_complex_content.py` & `core_parser_app-2.9.0/tests/tools/parser/parser/test_complex_content.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.8.0/tests/tools/parser/parser/test_complex_type.py` & `core_parser_app-2.9.0/tests/tools/parser/parser/test_complex_type.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.8.0/tests/tools/parser/parser/test_element.py` & `core_parser_app-2.9.0/tests/tools/parser/parser/test_element.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.8.0/tests/tools/parser/parser/test_extension.py` & `core_parser_app-2.9.0/tests/tools/parser/parser/test_extension.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.8.0/tests/tools/parser/parser/test_parser.py` & `core_parser_app-2.9.0/tests/tools/parser/parser/test_parser.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.8.0/tests/tools/parser/parser/test_restriction.py` & `core_parser_app-2.9.0/tests/tools/parser/parser/test_restriction.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.8.0/tests/tools/parser/parser/test_sequence.py` & `core_parser_app-2.9.0/tests/tools/parser/parser/test_sequence.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.8.0/tests/tools/parser/renderer/list/tests_unit.py` & `core_parser_app-2.9.0/tests/tools/parser/renderer/list/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.8.0/tests/tools/parser/renderer/tests_unit.py` & `core_parser_app-2.9.0/tests/tools/parser/renderer/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.8.0/tests/views/common/test_unit.py` & `core_parser_app-2.9.0/tests/views/common/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.8.0/tests/views/user/ajax/fixtures.py` & `core_parser_app-2.9.0/tests/views/user/ajax/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_parser_app-2.8.0/tests/views/user/ajax/test_int_access_control.py` & `core_parser_app-2.9.0/tests/views/user/ajax/test_int_access_control.py`

 * *Files identical despite different names*

