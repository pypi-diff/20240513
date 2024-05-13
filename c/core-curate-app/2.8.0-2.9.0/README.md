# Comparing `tmp/core_curate_app-2.8.0.tar.gz` & `tmp/core_curate_app-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_curate_app-2.8.0.tar", last modified: Tue Mar 12 18:57:40 2024, max compression
+gzip compressed data, was "core_curate_app-2.9.0.tar", last modified: Mon May 13 16:03:05 2024, max compression
```

## Comparing `core_curate_app-2.8.0.tar` & `core_curate_app-2.9.0.tar`

### file list

```diff
@@ -1,180 +1,180 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:40.347357 core_curate_app-2.8.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2024-03-12 18:57:32.000000 core_curate_app-2.8.0/LICENSE.md
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      138 2024-03-12 18:57:32.000000 core_curate_app-2.8.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1016 2024-03-12 18:57:40.342172 core_curate_app-2.8.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      532 2024-03-12 18:57:32.000000 core_curate_app-2.8.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:37.753068 core_curate_app-2.8.0/core_curate_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       73 2024-03-12 18:57:32.000000 core_curate_app-2.8.0/core_curate_app/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:37.885940 core_curate_app-2.8.0/core_curate_app/access_control/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:32.000000 core_curate_app-2.8.0/core_curate_app/access_control/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3185 2024-03-12 18:57:32.000000 core_curate_app-2.8.0/core_curate_app/access_control/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1236 2024-03-12 18:57:32.000000 core_curate_app-2.8.0/core_curate_app/admin.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      478 2024-03-12 18:57:32.000000 core_curate_app-2.8.0/core_curate_app/apps.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:37.926928 core_curate_app-2.8.0/core_curate_app/common/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:32.000000 core_curate_app-2.8.0/core_curate_app/common/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      207 2024-03-12 18:57:32.000000 core_curate_app-2.8.0/core_curate_app/common/exceptions.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:37.958535 core_curate_app-2.8.0/core_curate_app/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:32.000000 core_curate_app-2.8.0/core_curate_app/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:38.048864 core_curate_app-2.8.0/core_curate_app/components/curate_data_structure/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:32.000000 core_curate_app-2.8.0/core_curate_app/components/curate_data_structure/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      464 2024-03-12 18:57:32.000000 core_curate_app-2.8.0/core_curate_app/components/curate_data_structure/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5762 2024-03-12 18:57:32.000000 core_curate_app-2.8.0/core_curate_app/components/curate_data_structure/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6244 2024-03-12 18:57:32.000000 core_curate_app-2.8.0/core_curate_app/components/curate_data_structure/models.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      233 2024-03-12 18:57:32.000000 core_curate_app-2.8.0/core_curate_app/menus.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:38.089228 core_curate_app-2.8.0/core_curate_app/migrations/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2186 2024-03-12 18:57:32.000000 core_curate_app-2.8.0/core_curate_app/migrations/0001_initial.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:32.000000 core_curate_app-2.8.0/core_curate_app/migrations/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      738 2024-03-12 18:57:32.000000 core_curate_app-2.8.0/core_curate_app/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:38.153828 core_curate_app-2.8.0/core_curate_app/permissions/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:32.000000 core_curate_app-2.8.0/core_curate_app/permissions/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1306 2024-03-12 18:57:32.000000 core_curate_app-2.8.0/core_curate_app/permissions/discover.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      221 2024-03-12 18:57:32.000000 core_curate_app-2.8.0/core_curate_app/permissions/rights.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:38.195824 core_curate_app-2.8.0/core_curate_app/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:32.000000 core_curate_app-2.8.0/core_curate_app/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:38.287316 core_curate_app-2.8.0/core_curate_app/rest/curate_data_structure/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:32.000000 core_curate_app-2.8.0/core_curate_app/rest/curate_data_structure/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1396 2024-03-12 18:57:32.000000 core_curate_app-2.8.0/core_curate_app/rest/curate_data_structure/admin_serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2131 2024-03-12 18:57:32.000000 core_curate_app-2.8.0/core_curate_app/rest/curate_data_structure/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11996 2024-03-12 18:57:32.000000 core_curate_app-2.8.0/core_curate_app/rest/curate_data_structure/views.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      668 2024-03-12 18:57:32.000000 core_curate_app-2.8.0/core_curate_app/rest/urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1243 2024-03-12 18:57:32.000000 core_curate_app-2.8.0/core_curate_app/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:37.283795 core_curate_app-2.8.0/core_curate_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:37.287867 core_curate_app-2.8.0/core_curate_app/static/core_curate_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:37.305920 core_curate_app-2.8.0/core_curate_app/static/core_curate_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:38.380089 core_curate_app-2.8.0/core_curate_app/static/core_curate_app/user/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      692 2024-03-12 18:57:32.000000 core_curate_app-2.8.0/core_curate_app/static/core_curate_app/user/css/common.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       67 2024-03-12 18:57:32.000000 core_curate_app-2.8.0/core_curate_app/static/core_curate_app/user/css/json_form.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2033 2024-03-12 18:57:32.000000 core_curate_app-2.8.0/core_curate_app/static/core_curate_app/user/css/style.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      668 2024-03-12 18:57:32.000000 core_curate_app-2.8.0/core_curate_app/static/core_curate_app/user/css/xsd_form.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:38.422204 core_curate_app-2.8.0/core_curate_app/static/core_curate_app/user/img/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      246 2024-03-12 18:57:32.000000 core_curate_app-2.8.0/core_curate_app/static/core_curate_app/user/img/collapse.png
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      253 2024-03-12 18:57:32.000000 core_curate_app-2.8.0/core_curate_app/static/core_curate_app/user/img/expand.png
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:38.647543 core_curate_app-2.8.0/core_curate_app/static/core_curate_app/user/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      157 2024-03-12 18:57:32.000000 core_curate_app-2.8.0/core_curate_app/static/core_curate_app/user/js/buttons.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       89 2024-03-12 18:57:32.000000 core_curate_app-2.8.0/core_curate_app/static/core_curate_app/user/js/choice.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    15791 2024-03-12 18:57:32.000000 core_curate_app-2.8.0/core_curate_app/static/core_curate_app/user/js/enter_data.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      866 2024-03-12 18:57:32.000000 core_curate_app-2.8.0/core_curate_app/static/core_curate_app/user/js/enter_data.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6638 2024-03-12 18:57:32.000000 core_curate_app-2.8.0/core_curate_app/static/core_curate_app/user/js/select_template.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      121 2024-03-12 18:57:32.000000 core_curate_app-2.8.0/core_curate_app/static/core_curate_app/user/js/select_template.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1088 2024-03-12 18:57:32.000000 core_curate_app-2.8.0/core_curate_app/static/core_curate_app/user/js/switch_editor.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      140 2024-03-12 18:57:32.000000 core_curate_app-2.8.0/core_curate_app/static/core_curate_app/user/js/switch_editor.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      163 2024-03-12 18:57:32.000000 core_curate_app-2.8.0/core_curate_app/static/core_curate_app/user/js/text_editor.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1609 2024-03-12 18:57:32.000000 core_curate_app-2.8.0/core_curate_app/static/core_curate_app/user/js/view_data.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      296 2024-03-12 18:57:32.000000 core_curate_app-2.8.0/core_curate_app/static/core_curate_app/user/js/view_data.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:38.688962 core_curate_app-2.8.0/core_curate_app/static/core_curate_app/user/js/xml_entities_tooltip/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      598 2024-03-12 18:57:32.000000 core_curate_app-2.8.0/core_curate_app/static/core_curate_app/user/js/xml_entities_tooltip/popover.bs4.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      922 2024-03-12 18:57:32.000000 core_curate_app-2.8.0/core_curate_app/static/core_curate_app/user/js/xml_entities_tooltip/popover.bs5.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3831 2024-03-12 18:57:32.000000 core_curate_app-2.8.0/core_curate_app/static/core_curate_app/user/js/xml_entities_tooltip.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:37.324595 core_curate_app-2.8.0/core_curate_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:37.340149 core_curate_app-2.8.0/core_curate_app/templates/core_curate_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:38.865059 core_curate_app-2.8.0/core_curate_app/templates/core_curate_app/admin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      366 2024-03-12 18:57:32.000000 core_curate_app-2.8.0/core_curate_app/templates/core_curate_app/admin/detail.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      348 2024-03-12 18:57:32.000000 core_curate_app-2.8.0/core_curate_app/templates/core_curate_app/admin/view_curate_data_structure.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:38.915149 core_curate_app-2.8.0/core_curate_app/templates/core_curate_app/common/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      167 2024-03-12 18:57:32.000000 core_curate_app-2.8.0/core_curate_app/templates/core_curate_app/common/detail_curate_data_structure.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      274 2024-03-12 18:57:32.000000 core_curate_app-2.8.0/core_curate_app/templates/core_curate_app/common/tools_curate_data_structure.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:39.018688 core_curate_app-2.8.0/core_curate_app/templates/core_curate_app/user/
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     1528 2024-03-12 18:57:32.000000 core_curate_app-2.8.0/core_curate_app/templates/core_curate_app/user/curate.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1601 2024-03-12 18:57:32.000000 core_curate_app-2.8.0/core_curate_app/templates/core_curate_app/user/curate_full_start.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      628 2024-03-12 18:57:32.000000 core_curate_app-2.8.0/core_curate_app/templates/core_curate_app/user/curate_start.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:39.039267 core_curate_app-2.8.0/core_curate_app/templates/core_curate_app/user/data-entry/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3080 2024-03-12 18:57:32.000000 core_curate_app-2.8.0/core_curate_app/templates/core_curate_app/user/data-entry/enter_data.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:39.266621 core_curate_app-2.8.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      682 2024-03-12 18:57:32.000000 core_curate_app-2.8.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/cancel-changes.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      778 2024-03-12 18:57:32.000000 core_curate_app-2.8.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/cancel-form.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      692 2024-03-12 18:57:32.000000 core_curate_app-2.8.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/clear-fields.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1245 2024-03-12 18:57:32.000000 core_curate_app-2.8.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/download-options.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      662 2024-03-12 18:57:32.000000 core_curate_app-2.8.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/save-form.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      789 2024-03-12 18:57:32.000000 core_curate_app-2.8.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/switch_to_form_editor.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      790 2024-03-12 18:57:33.000000 core_curate_app-2.8.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/switch_to_text_editor.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      964 2024-03-12 18:57:33.000000 core_curate_app-2.8.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/use-validation.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      499 2024-03-12 18:57:33.000000 core_curate_app-2.8.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/validation-error.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      361 2024-03-12 18:57:33.000000 core_curate_app-2.8.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/validation-warning.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      789 2024-03-12 18:57:33.000000 core_curate_app-2.8.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/xml-valid.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:39.291562 core_curate_app-2.8.0/core_curate_app/templates/core_curate_app/user/data-review/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:39.315202 core_curate_app-2.8.0/core_curate_app/templates/core_curate_app/user/data-review/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      483 2024-03-12 18:57:33.000000 core_curate_app-2.8.0/core_curate_app/templates/core_curate_app/user/data-review/modals/save-error.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1844 2024-03-12 18:57:33.000000 core_curate_app-2.8.0/core_curate_app/templates/core_curate_app/user/data-review/view_data.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      318 2024-03-12 18:57:33.000000 core_curate_app-2.8.0/core_curate_app/templates/core_curate_app/user/detail.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       32 2024-03-12 18:57:33.000000 core_curate_app-2.8.0/core_curate_app/templates/core_curate_app/user/errors.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:39.338389 core_curate_app-2.8.0/core_curate_app/templates/core_curate_app/user/list/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      207 2024-03-12 18:57:33.000000 core_curate_app-2.8.0/core_curate_app/templates/core_curate_app/user/list/list.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3598 2024-03-12 18:57:33.000000 core_curate_app-2.8.0/core_curate_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:39.383812 core_curate_app-2.8.0/core_curate_app/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:33.000000 core_curate_app-2.8.0/core_curate_app/utils/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      764 2024-03-12 18:57:33.000000 core_curate_app-2.8.0/core_curate_app/utils/parser.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:39.416000 core_curate_app-2.8.0/core_curate_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:33.000000 core_curate_app-2.8.0/core_curate_app/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:39.468687 core_curate_app-2.8.0/core_curate_app/views/admin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:33.000000 core_curate_app-2.8.0/core_curate_app/views/admin/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1844 2024-03-12 18:57:33.000000 core_curate_app-2.8.0/core_curate_app/views/admin/ajax.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:39.514963 core_curate_app-2.8.0/core_curate_app/views/common/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:33.000000 core_curate_app-2.8.0/core_curate_app/views/common/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8161 2024-03-12 18:57:33.000000 core_curate_app-2.8.0/core_curate_app/views/common/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:39.595546 core_curate_app-2.8.0/core_curate_app/views/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:33.000000 core_curate_app-2.8.0/core_curate_app/views/user/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    23611 2024-03-12 18:57:33.000000 core_curate_app-2.8.0/core_curate_app/views/user/ajax.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3713 2024-03-12 18:57:33.000000 core_curate_app-2.8.0/core_curate_app/views/user/forms.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    22010 2024-03-12 18:57:33.000000 core_curate_app-2.8.0/core_curate_app/views/user/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:37.840819 core_curate_app-2.8.0/core_curate_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1016 2024-03-12 18:57:36.000000 core_curate_app-2.8.0/core_curate_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6226 2024-03-12 18:57:37.000000 core_curate_app-2.8.0/core_curate_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2024-03-12 18:57:36.000000 core_curate_app-2.8.0/core_curate_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       70 2024-03-12 18:57:36.000000 core_curate_app-2.8.0/core_curate_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       27 2024-03-12 18:57:36.000000 core_curate_app-2.8.0/core_curate_app.egg-info/top_level.txt
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:39.658341 core_curate_app-2.8.0/docs/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:33.000000 core_curate_app-2.8.0/docs/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11286 2024-03-12 18:57:33.000000 core_curate_app-2.8.0/docs/conf.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      283 2024-03-12 18:57:33.000000 core_curate_app-2.8.0/docs/conf_urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2024-03-12 18:57:33.000000 core_curate_app-2.8.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       44 2024-03-12 18:57:33.000000 core_curate_app-2.8.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2024-03-12 18:57:40.349720 core_curate_app-2.8.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1508 2024-03-12 18:57:33.000000 core_curate_app-2.8.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:39.740327 core_curate_app-2.8.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:33.000000 core_curate_app-2.8.0/tests/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:39.784383 core_curate_app-2.8.0/tests/access_control/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:34.000000 core_curate_app-2.8.0/tests/access_control/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3307 2024-03-12 18:57:34.000000 core_curate_app-2.8.0/tests/access_control/tests_access_control.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:39.806260 core_curate_app-2.8.0/tests/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:34.000000 core_curate_app-2.8.0/tests/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:39.887811 core_curate_app-2.8.0/tests/components/curate_data_structure/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:34.000000 core_curate_app-2.8.0/tests/components/curate_data_structure/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:39.930285 core_curate_app-2.8.0/tests/components/curate_data_structure/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:34.000000 core_curate_app-2.8.0/tests/components/curate_data_structure/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7311 2024-03-12 18:57:34.000000 core_curate_app-2.8.0/tests/components/curate_data_structure/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4891 2024-03-12 18:57:34.000000 core_curate_app-2.8.0/tests/components/curate_data_structure/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    20058 2024-03-12 18:57:34.000000 core_curate_app-2.8.0/tests/components/curate_data_structure/tests_int_access_control.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14240 2024-03-12 18:57:34.000000 core_curate_app-2.8.0/tests/components/curate_data_structure/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:39.950682 core_curate_app-2.8.0/tests/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:34.000000 core_curate_app-2.8.0/tests/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:40.012962 core_curate_app-2.8.0/tests/rest/curate_data_structure/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:34.000000 core_curate_app-2.8.0/tests/rest/curate_data_structure/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11400 2024-03-12 18:57:34.000000 core_curate_app-2.8.0/tests/rest/curate_data_structure/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    13049 2024-03-12 18:57:34.000000 core_curate_app-2.8.0/tests/rest/curate_data_structure/tests_permissions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1735 2024-03-12 18:57:34.000000 core_curate_app-2.8.0/tests/test_settings.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      237 2024-03-12 18:57:34.000000 core_curate_app-2.8.0/tests/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:40.029318 core_curate_app-2.8.0/tests/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:34.000000 core_curate_app-2.8.0/tests/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:40.048933 core_curate_app-2.8.0/tests/views/admin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:34.000000 core_curate_app-2.8.0/tests/views/admin/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:40.088344 core_curate_app-2.8.0/tests/views/admin/ajax/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:34.000000 core_curate_app-2.8.0/tests/views/admin/ajax/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2685 2024-03-12 18:57:34.000000 core_curate_app-2.8.0/tests/views/admin/ajax/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:40.105296 core_curate_app-2.8.0/tests/views/common/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:34.000000 core_curate_app-2.8.0/tests/views/common/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:40.160686 core_curate_app-2.8.0/tests/views/common/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:34.000000 core_curate_app-2.8.0/tests/views/common/views/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1354 2024-03-12 18:57:34.000000 core_curate_app-2.8.0/tests/views/common/views/test_unit.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14958 2024-03-12 18:57:34.000000 core_curate_app-2.8.0/tests/views/common/views/tests_int_access_control.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:40.179261 core_curate_app-2.8.0/tests/views/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:34.000000 core_curate_app-2.8.0/tests/views/user/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:40.240935 core_curate_app-2.8.0/tests/views/user/ajax/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:34.000000 core_curate_app-2.8.0/tests/views/user/ajax/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    38080 2024-03-12 18:57:34.000000 core_curate_app-2.8.0/tests/views/user/ajax/test_unit.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    12628 2024-03-12 18:57:34.000000 core_curate_app-2.8.0/tests/views/user/ajax/tests_int_access_control.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:40.281359 core_curate_app-2.8.0/tests/views/user/forms/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:34.000000 core_curate_app-2.8.0/tests/views/user/forms/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2300 2024-03-12 18:57:34.000000 core_curate_app-2.8.0/tests/views/user/forms/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:40.322818 core_curate_app-2.8.0/tests/views/user/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:57:34.000000 core_curate_app-2.8.0/tests/views/user/views/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    30854 2024-03-12 18:57:34.000000 core_curate_app-2.8.0/tests/views/user/views/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:05.012950 core_curate_app-2.9.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2024-05-13 16:02:55.000000 core_curate_app-2.9.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      138 2024-05-13 16:02:55.000000 core_curate_app-2.9.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1016 2024-05-13 16:03:05.006885 core_curate_app-2.9.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      532 2024-05-13 16:02:55.000000 core_curate_app-2.9.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:02.212733 core_curate_app-2.9.0/core_curate_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       73 2024-05-13 16:02:55.000000 core_curate_app-2.9.0/core_curate_app/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:02.376863 core_curate_app-2.9.0/core_curate_app/access_control/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:55.000000 core_curate_app-2.9.0/core_curate_app/access_control/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3185 2024-05-13 16:02:55.000000 core_curate_app-2.9.0/core_curate_app/access_control/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1236 2024-05-13 16:02:55.000000 core_curate_app-2.9.0/core_curate_app/admin.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      478 2024-05-13 16:02:55.000000 core_curate_app-2.9.0/core_curate_app/apps.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:02.418481 core_curate_app-2.9.0/core_curate_app/common/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:55.000000 core_curate_app-2.9.0/core_curate_app/common/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      207 2024-05-13 16:02:55.000000 core_curate_app-2.9.0/core_curate_app/common/exceptions.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:02.439970 core_curate_app-2.9.0/core_curate_app/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:55.000000 core_curate_app-2.9.0/core_curate_app/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:02.539399 core_curate_app-2.9.0/core_curate_app/components/curate_data_structure/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:56.000000 core_curate_app-2.9.0/core_curate_app/components/curate_data_structure/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      464 2024-05-13 16:02:56.000000 core_curate_app-2.9.0/core_curate_app/components/curate_data_structure/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5762 2024-05-13 16:02:56.000000 core_curate_app-2.9.0/core_curate_app/components/curate_data_structure/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6244 2024-05-13 16:02:56.000000 core_curate_app-2.9.0/core_curate_app/components/curate_data_structure/models.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      233 2024-05-13 16:02:56.000000 core_curate_app-2.9.0/core_curate_app/menus.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:02.576077 core_curate_app-2.9.0/core_curate_app/migrations/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2186 2024-05-13 16:02:56.000000 core_curate_app-2.9.0/core_curate_app/migrations/0001_initial.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:56.000000 core_curate_app-2.9.0/core_curate_app/migrations/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      738 2024-05-13 16:02:56.000000 core_curate_app-2.9.0/core_curate_app/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:02.634153 core_curate_app-2.9.0/core_curate_app/permissions/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:56.000000 core_curate_app-2.9.0/core_curate_app/permissions/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1306 2024-05-13 16:02:56.000000 core_curate_app-2.9.0/core_curate_app/permissions/discover.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      221 2024-05-13 16:02:56.000000 core_curate_app-2.9.0/core_curate_app/permissions/rights.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:02.672235 core_curate_app-2.9.0/core_curate_app/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:56.000000 core_curate_app-2.9.0/core_curate_app/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:02.792872 core_curate_app-2.9.0/core_curate_app/rest/curate_data_structure/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:56.000000 core_curate_app-2.9.0/core_curate_app/rest/curate_data_structure/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1396 2024-05-13 16:02:56.000000 core_curate_app-2.9.0/core_curate_app/rest/curate_data_structure/admin_serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2131 2024-05-13 16:02:56.000000 core_curate_app-2.9.0/core_curate_app/rest/curate_data_structure/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11996 2024-05-13 16:02:56.000000 core_curate_app-2.9.0/core_curate_app/rest/curate_data_structure/views.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      668 2024-05-13 16:02:56.000000 core_curate_app-2.9.0/core_curate_app/rest/urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1243 2024-05-13 16:02:56.000000 core_curate_app-2.9.0/core_curate_app/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:01.514737 core_curate_app-2.9.0/core_curate_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:01.540830 core_curate_app-2.9.0/core_curate_app/static/core_curate_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:01.556427 core_curate_app-2.9.0/core_curate_app/static/core_curate_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:02.866007 core_curate_app-2.9.0/core_curate_app/static/core_curate_app/user/css/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      692 2024-05-13 16:02:56.000000 core_curate_app-2.9.0/core_curate_app/static/core_curate_app/user/css/common.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       67 2024-05-13 16:02:56.000000 core_curate_app-2.9.0/core_curate_app/static/core_curate_app/user/css/json_form.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2033 2024-05-13 16:02:56.000000 core_curate_app-2.9.0/core_curate_app/static/core_curate_app/user/css/style.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      668 2024-05-13 16:02:56.000000 core_curate_app-2.9.0/core_curate_app/static/core_curate_app/user/css/xsd_form.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:02.900163 core_curate_app-2.9.0/core_curate_app/static/core_curate_app/user/img/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      246 2024-05-13 16:02:56.000000 core_curate_app-2.9.0/core_curate_app/static/core_curate_app/user/img/collapse.png
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      253 2024-05-13 16:02:56.000000 core_curate_app-2.9.0/core_curate_app/static/core_curate_app/user/img/expand.png
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:03.172630 core_curate_app-2.9.0/core_curate_app/static/core_curate_app/user/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      157 2024-05-13 16:02:56.000000 core_curate_app-2.9.0/core_curate_app/static/core_curate_app/user/js/buttons.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       89 2024-05-13 16:02:56.000000 core_curate_app-2.9.0/core_curate_app/static/core_curate_app/user/js/choice.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    15752 2024-05-13 16:02:56.000000 core_curate_app-2.9.0/core_curate_app/static/core_curate_app/user/js/enter_data.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      866 2024-05-13 16:02:56.000000 core_curate_app-2.9.0/core_curate_app/static/core_curate_app/user/js/enter_data.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6638 2024-05-13 16:02:56.000000 core_curate_app-2.9.0/core_curate_app/static/core_curate_app/user/js/select_template.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      121 2024-05-13 16:02:56.000000 core_curate_app-2.9.0/core_curate_app/static/core_curate_app/user/js/select_template.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1100 2024-05-13 16:02:56.000000 core_curate_app-2.9.0/core_curate_app/static/core_curate_app/user/js/switch_editor.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      140 2024-05-13 16:02:56.000000 core_curate_app-2.9.0/core_curate_app/static/core_curate_app/user/js/switch_editor.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      163 2024-05-13 16:02:56.000000 core_curate_app-2.9.0/core_curate_app/static/core_curate_app/user/js/text_editor.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1609 2024-05-13 16:02:56.000000 core_curate_app-2.9.0/core_curate_app/static/core_curate_app/user/js/view_data.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      296 2024-05-13 16:02:56.000000 core_curate_app-2.9.0/core_curate_app/static/core_curate_app/user/js/view_data.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:03.237870 core_curate_app-2.9.0/core_curate_app/static/core_curate_app/user/js/xml_entities_tooltip/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      598 2024-05-13 16:02:56.000000 core_curate_app-2.9.0/core_curate_app/static/core_curate_app/user/js/xml_entities_tooltip/popover.bs4.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      922 2024-05-13 16:02:56.000000 core_curate_app-2.9.0/core_curate_app/static/core_curate_app/user/js/xml_entities_tooltip/popover.bs5.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3831 2024-05-13 16:02:56.000000 core_curate_app-2.9.0/core_curate_app/static/core_curate_app/user/js/xml_entities_tooltip.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:01.595043 core_curate_app-2.9.0/core_curate_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:01.610783 core_curate_app-2.9.0/core_curate_app/templates/core_curate_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:03.275146 core_curate_app-2.9.0/core_curate_app/templates/core_curate_app/admin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      366 2024-05-13 16:02:56.000000 core_curate_app-2.9.0/core_curate_app/templates/core_curate_app/admin/detail.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      348 2024-05-13 16:02:56.000000 core_curate_app-2.9.0/core_curate_app/templates/core_curate_app/admin/view_curate_data_structure.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:03.326398 core_curate_app-2.9.0/core_curate_app/templates/core_curate_app/common/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      167 2024-05-13 16:02:56.000000 core_curate_app-2.9.0/core_curate_app/templates/core_curate_app/common/detail_curate_data_structure.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      274 2024-05-13 16:02:56.000000 core_curate_app-2.9.0/core_curate_app/templates/core_curate_app/common/tools_curate_data_structure.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:03.407521 core_curate_app-2.9.0/core_curate_app/templates/core_curate_app/user/
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     1528 2024-05-13 16:02:56.000000 core_curate_app-2.9.0/core_curate_app/templates/core_curate_app/user/curate.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1601 2024-05-13 16:02:56.000000 core_curate_app-2.9.0/core_curate_app/templates/core_curate_app/user/curate_full_start.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      628 2024-05-13 16:02:56.000000 core_curate_app-2.9.0/core_curate_app/templates/core_curate_app/user/curate_start.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:03.425227 core_curate_app-2.9.0/core_curate_app/templates/core_curate_app/user/data-entry/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3080 2024-05-13 16:02:56.000000 core_curate_app-2.9.0/core_curate_app/templates/core_curate_app/user/data-entry/enter_data.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:03.683921 core_curate_app-2.9.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      682 2024-05-13 16:02:56.000000 core_curate_app-2.9.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/cancel-changes.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      778 2024-05-13 16:02:57.000000 core_curate_app-2.9.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/cancel-form.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      692 2024-05-13 16:02:57.000000 core_curate_app-2.9.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/clear-fields.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1245 2024-05-13 16:02:57.000000 core_curate_app-2.9.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/download-options.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      662 2024-05-13 16:02:57.000000 core_curate_app-2.9.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/save-form.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      789 2024-05-13 16:02:57.000000 core_curate_app-2.9.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/switch_to_form_editor.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      790 2024-05-13 16:02:57.000000 core_curate_app-2.9.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/switch_to_text_editor.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      964 2024-05-13 16:02:57.000000 core_curate_app-2.9.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/use-validation.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      499 2024-05-13 16:02:57.000000 core_curate_app-2.9.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/validation-error.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      361 2024-05-13 16:02:57.000000 core_curate_app-2.9.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/validation-warning.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      789 2024-05-13 16:02:57.000000 core_curate_app-2.9.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/xml-valid.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:03.731216 core_curate_app-2.9.0/core_curate_app/templates/core_curate_app/user/data-review/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:03.753373 core_curate_app-2.9.0/core_curate_app/templates/core_curate_app/user/data-review/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      483 2024-05-13 16:02:57.000000 core_curate_app-2.9.0/core_curate_app/templates/core_curate_app/user/data-review/modals/save-error.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1844 2024-05-13 16:02:57.000000 core_curate_app-2.9.0/core_curate_app/templates/core_curate_app/user/data-review/view_data.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      318 2024-05-13 16:02:57.000000 core_curate_app-2.9.0/core_curate_app/templates/core_curate_app/user/detail.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       32 2024-05-13 16:02:57.000000 core_curate_app-2.9.0/core_curate_app/templates/core_curate_app/user/errors.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:03.801024 core_curate_app-2.9.0/core_curate_app/templates/core_curate_app/user/list/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      207 2024-05-13 16:02:57.000000 core_curate_app-2.9.0/core_curate_app/templates/core_curate_app/user/list/list.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3598 2024-05-13 16:02:57.000000 core_curate_app-2.9.0/core_curate_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:03.845035 core_curate_app-2.9.0/core_curate_app/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:57.000000 core_curate_app-2.9.0/core_curate_app/utils/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      764 2024-05-13 16:02:57.000000 core_curate_app-2.9.0/core_curate_app/utils/parser.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:03.869826 core_curate_app-2.9.0/core_curate_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:57.000000 core_curate_app-2.9.0/core_curate_app/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:03.918924 core_curate_app-2.9.0/core_curate_app/views/admin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:57.000000 core_curate_app-2.9.0/core_curate_app/views/admin/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1861 2024-05-13 16:02:57.000000 core_curate_app-2.9.0/core_curate_app/views/admin/ajax.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:03.959140 core_curate_app-2.9.0/core_curate_app/views/common/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:57.000000 core_curate_app-2.9.0/core_curate_app/views/common/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8148 2024-05-13 16:02:57.000000 core_curate_app-2.9.0/core_curate_app/views/common/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:04.065044 core_curate_app-2.9.0/core_curate_app/views/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:57.000000 core_curate_app-2.9.0/core_curate_app/views/user/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    23491 2024-05-13 16:02:57.000000 core_curate_app-2.9.0/core_curate_app/views/user/ajax.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3713 2024-05-13 16:02:57.000000 core_curate_app-2.9.0/core_curate_app/views/user/forms.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    22010 2024-05-13 16:02:57.000000 core_curate_app-2.9.0/core_curate_app/views/user/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:02.336033 core_curate_app-2.9.0/core_curate_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1016 2024-05-13 16:03:00.000000 core_curate_app-2.9.0/core_curate_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6226 2024-05-13 16:03:01.000000 core_curate_app-2.9.0/core_curate_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2024-05-13 16:03:00.000000 core_curate_app-2.9.0/core_curate_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       70 2024-05-13 16:03:00.000000 core_curate_app-2.9.0/core_curate_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       27 2024-05-13 16:03:00.000000 core_curate_app-2.9.0/core_curate_app.egg-info/top_level.txt
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:04.129781 core_curate_app-2.9.0/docs/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:57.000000 core_curate_app-2.9.0/docs/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11286 2024-05-13 16:02:57.000000 core_curate_app-2.9.0/docs/conf.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      283 2024-05-13 16:02:57.000000 core_curate_app-2.9.0/docs/conf_urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2024-05-13 16:02:57.000000 core_curate_app-2.9.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       44 2024-05-13 16:02:57.000000 core_curate_app-2.9.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2024-05-13 16:03:05.015258 core_curate_app-2.9.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1508 2024-05-13 16:02:58.000000 core_curate_app-2.9.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:04.192834 core_curate_app-2.9.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:58.000000 core_curate_app-2.9.0/tests/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:04.236773 core_curate_app-2.9.0/tests/access_control/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:58.000000 core_curate_app-2.9.0/tests/access_control/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3307 2024-05-13 16:02:58.000000 core_curate_app-2.9.0/tests/access_control/tests_access_control.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:04.256879 core_curate_app-2.9.0/tests/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:58.000000 core_curate_app-2.9.0/tests/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:04.365834 core_curate_app-2.9.0/tests/components/curate_data_structure/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:58.000000 core_curate_app-2.9.0/tests/components/curate_data_structure/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:04.409449 core_curate_app-2.9.0/tests/components/curate_data_structure/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:58.000000 core_curate_app-2.9.0/tests/components/curate_data_structure/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7311 2024-05-13 16:02:58.000000 core_curate_app-2.9.0/tests/components/curate_data_structure/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4891 2024-05-13 16:02:58.000000 core_curate_app-2.9.0/tests/components/curate_data_structure/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    20058 2024-05-13 16:02:58.000000 core_curate_app-2.9.0/tests/components/curate_data_structure/tests_int_access_control.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14240 2024-05-13 16:02:58.000000 core_curate_app-2.9.0/tests/components/curate_data_structure/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:04.431753 core_curate_app-2.9.0/tests/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:58.000000 core_curate_app-2.9.0/tests/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:04.501521 core_curate_app-2.9.0/tests/rest/curate_data_structure/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:58.000000 core_curate_app-2.9.0/tests/rest/curate_data_structure/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11400 2024-05-13 16:02:58.000000 core_curate_app-2.9.0/tests/rest/curate_data_structure/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    13049 2024-05-13 16:02:58.000000 core_curate_app-2.9.0/tests/rest/curate_data_structure/tests_permissions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1735 2024-05-13 16:02:58.000000 core_curate_app-2.9.0/tests/test_settings.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      237 2024-05-13 16:02:58.000000 core_curate_app-2.9.0/tests/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:04.523228 core_curate_app-2.9.0/tests/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:58.000000 core_curate_app-2.9.0/tests/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:04.547702 core_curate_app-2.9.0/tests/views/admin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:58.000000 core_curate_app-2.9.0/tests/views/admin/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:04.589820 core_curate_app-2.9.0/tests/views/admin/ajax/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:58.000000 core_curate_app-2.9.0/tests/views/admin/ajax/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2685 2024-05-13 16:02:58.000000 core_curate_app-2.9.0/tests/views/admin/ajax/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:04.607890 core_curate_app-2.9.0/tests/views/common/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:58.000000 core_curate_app-2.9.0/tests/views/common/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:04.692477 core_curate_app-2.9.0/tests/views/common/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:58.000000 core_curate_app-2.9.0/tests/views/common/views/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1354 2024-05-13 16:02:58.000000 core_curate_app-2.9.0/tests/views/common/views/test_unit.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14958 2024-05-13 16:02:58.000000 core_curate_app-2.9.0/tests/views/common/views/tests_int_access_control.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:04.721063 core_curate_app-2.9.0/tests/views/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:58.000000 core_curate_app-2.9.0/tests/views/user/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:04.830817 core_curate_app-2.9.0/tests/views/user/ajax/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:58.000000 core_curate_app-2.9.0/tests/views/user/ajax/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    38045 2024-05-13 16:02:58.000000 core_curate_app-2.9.0/tests/views/user/ajax/test_unit.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    12628 2024-05-13 16:02:58.000000 core_curate_app-2.9.0/tests/views/user/ajax/tests_int_access_control.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:04.888177 core_curate_app-2.9.0/tests/views/user/forms/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:58.000000 core_curate_app-2.9.0/tests/views/user/forms/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2300 2024-05-13 16:02:58.000000 core_curate_app-2.9.0/tests/views/user/forms/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:04.961933 core_curate_app-2.9.0/tests/views/user/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:02:58.000000 core_curate_app-2.9.0/tests/views/user/views/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    30854 2024-05-13 16:02:58.000000 core_curate_app-2.9.0/tests/views/user/views/test_unit.py
```

### Comparing `core_curate_app-2.8.0/LICENSE.md` & `core_curate_app-2.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.8.0/PKG-INFO` & `core_curate_app-2.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_curate_app
-Version: 2.8.0
+Version: 2.9.0
 Summary: Curation functionalities for the curator core project
 Home-page: https://github.com/usnistgov/core_curate_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: ===============
         Core Curate App
```

### Comparing `core_curate_app-2.8.0/README.rst` & `core_curate_app-2.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.8.0/core_curate_app/access_control/api.py` & `core_curate_app-2.9.0/core_curate_app/access_control/api.py`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.8.0/core_curate_app/admin.py` & `core_curate_app-2.9.0/core_curate_app/admin.py`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.8.0/core_curate_app/components/curate_data_structure/api.py` & `core_curate_app-2.9.0/core_curate_app/components/curate_data_structure/api.py`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.8.0/core_curate_app/components/curate_data_structure/models.py` & `core_curate_app-2.9.0/core_curate_app/components/curate_data_structure/models.py`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.8.0/core_curate_app/migrations/0001_initial.py` & `core_curate_app-2.9.0/core_curate_app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.8.0/core_curate_app/models.py` & `core_curate_app-2.9.0/core_curate_app/models.py`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.8.0/core_curate_app/permissions/discover.py` & `core_curate_app-2.9.0/core_curate_app/permissions/discover.py`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.8.0/core_curate_app/rest/curate_data_structure/admin_serializers.py` & `core_curate_app-2.9.0/core_curate_app/rest/curate_data_structure/admin_serializers.py`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.8.0/core_curate_app/rest/curate_data_structure/serializers.py` & `core_curate_app-2.9.0/core_curate_app/rest/curate_data_structure/serializers.py`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.8.0/core_curate_app/rest/curate_data_structure/views.py` & `core_curate_app-2.9.0/core_curate_app/rest/curate_data_structure/views.py`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.8.0/core_curate_app/rest/urls.py` & `core_curate_app-2.9.0/core_curate_app/rest/urls.py`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.8.0/core_curate_app/settings.py` & `core_curate_app-2.9.0/core_curate_app/settings.py`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.8.0/core_curate_app/static/core_curate_app/user/css/common.css` & `core_curate_app-2.9.0/core_curate_app/static/core_curate_app/user/css/common.css`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.8.0/core_curate_app/static/core_curate_app/user/css/style.css` & `core_curate_app-2.9.0/core_curate_app/static/core_curate_app/user/css/style.css`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.8.0/core_curate_app/static/core_curate_app/user/css/xsd_form.css` & `core_curate_app-2.9.0/core_curate_app/static/core_curate_app/user/css/xsd_form.css`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.8.0/core_curate_app/static/core_curate_app/user/js/enter_data.js` & `core_curate_app-2.9.0/core_curate_app/static/core_curate_app/user/js/enter_data.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -46,29 +46,29 @@
                 });
 
                 $('script.module').each(function(index, item) {
                     item.remove();
                 });
 
                 initModules();
-                $.notify("Fields cleared with success.", "success");
+                $.notify("Fields cleared.", "success");
             },
             error: function() {
                 $.notify("An error occurred while clearing fields.", "danger");
             }
         }).always(function(data) {
             // get old button icon
             hideSpinner($("[id^='btn-clear-fields'] > i"), icon)
             $("#clear-fields-modal").modal("hide");
         });
     } else if (contentFormat == "JSON") {
         initJSONFormEditor();
         hideSpinner($("[id^='btn-clear-fields'] > i"), icon)
         $("#clear-fields-modal").modal("hide");
-        $.notify("Fields cleared with success.", "success");
+        $.notify("Fields cleared.", "success");
     } else $.notify("Template format not supported.", "danger");
 
 };
 
 
 /**
  * Cancel the changes of the current curated data
@@ -107,15 +107,15 @@
                 initModules();
             } else {
                 if (data.content == "")
                     editor.setValue({});
                 else
                     editor.setValue(JSON.parse(data.content));
             }
-            $.notify("Changes canceled  with success.", "success");
+            $.notify("Changes canceled .", "success");
         },
         error: function() {
             $.notify("An error occurred while canceling changes.", "danger");
         }
     }).always(function() {
         // get old button icon
         hideSpinner($("[id^='btn-cancel-changes'] > i"), icon)
```

### Comparing `core_curate_app-2.8.0/core_curate_app/static/core_curate_app/user/js/enter_data.raw.js` & `core_curate_app-2.9.0/core_curate_app/static/core_curate_app/user/js/enter_data.raw.js`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.8.0/core_curate_app/static/core_curate_app/user/js/select_template.js` & `core_curate_app-2.9.0/core_curate_app/static/core_curate_app/user/js/select_template.js`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.8.0/core_curate_app/static/core_curate_app/user/js/switch_editor.js` & `core_curate_app-2.9.0/core_curate_app/static/core_curate_app/user/js/switch_editor.js`

 * *Files 13% similar despite different names*

#### js-beautify {}

```diff
@@ -19,15 +19,15 @@
         dataType: 'json',
         success: function(data) {
             window.location = switchToFormUrl.replace("curate_data_structure_id", documentID);
         },
         error: function(dataXHR) {
             $.notify(dataXHR.responseJSON.error, "danger");
             if ("details" in dataXHR.responseJSON) {
-                jqError.html('<i class="fas fa-exclamation-triangle"></i> ' + dataXHR.responseJSON.details);
+                $("#error_message").html('<i class="fas fa-exclamation-triangle"></i> ' + dataXHR.responseJSON.details);
                 jqError.show();
             }
         }
     }).always(function(data) {
         $("#switch-to-form-editor").modal("hide");
     });
 }
```

### Comparing `core_curate_app-2.8.0/core_curate_app/static/core_curate_app/user/js/view_data.js` & `core_curate_app-2.9.0/core_curate_app/static/core_curate_app/user/js/view_data.js`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.8.0/core_curate_app/static/core_curate_app/user/js/xml_entities_tooltip/popover.bs4.js` & `core_curate_app-2.9.0/core_curate_app/static/core_curate_app/user/js/xml_entities_tooltip/popover.bs4.js`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.8.0/core_curate_app/static/core_curate_app/user/js/xml_entities_tooltip/popover.bs5.js` & `core_curate_app-2.9.0/core_curate_app/static/core_curate_app/user/js/xml_entities_tooltip/popover.bs5.js`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.8.0/core_curate_app/static/core_curate_app/user/js/xml_entities_tooltip.js` & `core_curate_app-2.9.0/core_curate_app/static/core_curate_app/user/js/xml_entities_tooltip.js`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.8.0/core_curate_app/templates/core_curate_app/user/curate.html` & `core_curate_app-2.9.0/core_curate_app/templates/core_curate_app/user/curate.html`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.8.0/core_curate_app/templates/core_curate_app/user/curate_full_start.html` & `core_curate_app-2.9.0/core_curate_app/templates/core_curate_app/user/curate_full_start.html`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.8.0/core_curate_app/templates/core_curate_app/user/curate_start.html` & `core_curate_app-2.9.0/core_curate_app/templates/core_curate_app/user/curate_start.html`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.8.0/core_curate_app/templates/core_curate_app/user/data-entry/enter_data.html` & `core_curate_app-2.9.0/core_curate_app/templates/core_curate_app/user/data-entry/enter_data.html`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.8.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/cancel-changes.html` & `core_curate_app-2.9.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/cancel-changes.html`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.8.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/cancel-form.html` & `core_curate_app-2.9.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/cancel-form.html`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.8.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/clear-fields.html` & `core_curate_app-2.9.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/clear-fields.html`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.8.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/download-options.html` & `core_curate_app-2.9.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/download-options.html`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.8.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/save-form.html` & `core_curate_app-2.9.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/save-form.html`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.8.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/switch_to_form_editor.html` & `core_curate_app-2.9.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/switch_to_form_editor.html`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.8.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/switch_to_text_editor.html` & `core_curate_app-2.9.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/switch_to_text_editor.html`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.8.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/use-validation.html` & `core_curate_app-2.9.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/use-validation.html`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.8.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/xml-valid.html` & `core_curate_app-2.9.0/core_curate_app/templates/core_curate_app/user/data-entry/modals/xml-valid.html`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.8.0/core_curate_app/templates/core_curate_app/user/data-review/view_data.html` & `core_curate_app-2.9.0/core_curate_app/templates/core_curate_app/user/data-review/view_data.html`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.8.0/core_curate_app/urls.py` & `core_curate_app-2.9.0/core_curate_app/urls.py`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.8.0/core_curate_app/utils/parser.py` & `core_curate_app-2.9.0/core_curate_app/utils/parser.py`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.8.0/core_curate_app/views/admin/ajax.py` & `core_curate_app-2.9.0/core_curate_app/views/admin/ajax.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     HttpResponseBadRequest,
 )
 
 import core_main_app.components.data.api as data_api
 
 from core_main_app.commons.exceptions import DoesNotExist
 
-from core_main_app.utils.labels import get_data_label
+from core_main_app.utils.labels import get_data_label, get_form_label
 
 import core_curate_app.components.curate_data_structure.api as curate_data_structure_api
 
 
 @staff_member_required
 def delete_record_drafts(request, pk):
     """Delete record drafts.
@@ -37,15 +37,15 @@
         # delete curate data structures
         curate_data_structure_api.delete_curate_data_structures_by_data(
             data, request.user
         )
 
         message = Message(
             messages.SUCCESS,
-            "Drafts deleted with success",
+            get_form_label() + " deleted.",
         )
     except DoesNotExist:
         message = Message(
             messages.ERROR,
             "It seems a "
             + get_data_label()
             + " is missing. Please refresh the page.",
```

### Comparing `core_curate_app-2.8.0/core_curate_app/views/common/views.py` & `core_curate_app-2.9.0/core_curate_app/views/common/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -223,15 +223,15 @@
             data.content = content
             # save data
             data_api.upsert(data, request)
             data_structure_api.delete(data_structure, request.user)
             messages.add_message(
                 request,
                 messages.SUCCESS,
-                get_data_label().capitalize() + " saved with success.",
+                get_data_label().capitalize() + " saved.",
             )
             return HttpResponse(
                 json.dumps({"url": reverse("core_curate_index")}),
                 "application/javascript",
             )
         except AccessControlError as ace:
             return HttpResponseForbidden(html_escape(str(ace)))
```

### Comparing `core_curate_app-2.8.0/core_curate_app/views/user/ajax.py` & `core_curate_app-2.9.0/core_curate_app/views/user/ajax.py`

 * *Files 1% similar despite different names*

```diff
@@ -321,15 +321,15 @@
             )
         curate_data_structure_api.delete(curate_data_structure, request.user)
 
         # add success message
         messages.add_message(
             request,
             messages.SUCCESS,
-            get_form_label().capitalize() + " deleted with success.",
+            get_form_label().capitalize() + " deleted.",
         )
 
         return HttpResponse(json.dumps({}), content_type="application/json")
     except Exception as exception:
         error_message = (
             "An unexpected error has occurred while cancelling "
             f"the {get_form_label()}"
@@ -384,19 +384,15 @@
         # update curate data structure data
         curate_data_structure.form_string = form_string
 
         # save data structure
         curate_data_structure_api.upsert(curate_data_structure, request.user)
 
         return HttpResponse(
-            json.dumps(
-                {
-                    "message": f"{get_form_label().capitalize()} saved with success."
-                }
-            ),
+            json.dumps({"message": f"{get_form_label().capitalize()} saved."}),
             content_type="application/json",
         )
     except Exception as exception:
         error_message = (
             f"An error occurred while saving the {get_form_label()}"
         )
         logger.error("%s: %s", error_message, str(exception))
@@ -535,15 +531,15 @@
         data = data_api.upsert(data, request)
 
         curate_data_structure_api.delete(curate_data_structure, request.user)
 
         messages.add_message(
             request,
             messages.SUCCESS,
-            get_data_label().capitalize() + " saved with success.",
+            get_data_label().capitalize() + " saved.",
         )
     except Exception as exception:
         return HttpResponseBadRequest(
             str(exception).replace('"', "'"),
             content_type="application/javascript",
         )
 
@@ -626,15 +622,15 @@
             # set content
             data.content = content
             # save data
             data_api.upsert(data, request)
             messages.add_message(
                 request,
                 messages.SUCCESS,
-                get_data_label().capitalize() + " saved with success.",
+                get_data_label().capitalize() + " saved.",
             )
             url = reverse("core_main_app_data_detail") + f"?id={str(data.id)}"
         else:
             curate_data_structure = CurateDataStructure(
                 user=user_id,
                 template=template_api.get_by_id(template_id, request=request),
                 name=name,
```

### Comparing `core_curate_app-2.8.0/core_curate_app/views/user/forms.py` & `core_curate_app-2.9.0/core_curate_app/views/user/forms.py`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.8.0/core_curate_app/views/user/views.py` & `core_curate_app-2.9.0/core_curate_app/views/user/views.py`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.8.0/core_curate_app.egg-info/PKG-INFO` & `core_curate_app-2.9.0/core_curate_app.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-curate-app
-Version: 2.8.0
+Version: 2.9.0
 Summary: Curation functionalities for the curator core project
 Home-page: https://github.com/usnistgov/core_curate_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: ===============
         Core Curate App
```

### Comparing `core_curate_app-2.8.0/core_curate_app.egg-info/SOURCES.txt` & `core_curate_app-2.9.0/core_curate_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.8.0/docs/conf.py` & `core_curate_app-2.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.8.0/setup.py` & `core_curate_app-2.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 chdir(normpath(join(abspath(__file__), pardir)))
 
 dep_links = [r for r in required if r.startswith("https://")]
 required = [req_link(r) if r.startswith("https://") else r for r in required]
 
 setup(
     name="core_curate_app",
-    version="2.8.0",
+    version="2.9.0",
     description="Curation functionalities for the curator core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_curate_app",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `core_curate_app-2.8.0/tests/access_control/tests_access_control.py` & `core_curate_app-2.9.0/tests/access_control/tests_access_control.py`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.8.0/tests/components/curate_data_structure/fixtures/fixtures.py` & `core_curate_app-2.9.0/tests/components/curate_data_structure/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.8.0/tests/components/curate_data_structure/tests_int.py` & `core_curate_app-2.9.0/tests/components/curate_data_structure/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.8.0/tests/components/curate_data_structure/tests_int_access_control.py` & `core_curate_app-2.9.0/tests/components/curate_data_structure/tests_int_access_control.py`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.8.0/tests/components/curate_data_structure/tests_unit.py` & `core_curate_app-2.9.0/tests/components/curate_data_structure/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.8.0/tests/rest/curate_data_structure/tests_int.py` & `core_curate_app-2.9.0/tests/rest/curate_data_structure/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.8.0/tests/rest/curate_data_structure/tests_permissions.py` & `core_curate_app-2.9.0/tests/rest/curate_data_structure/tests_permissions.py`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.8.0/tests/test_settings.py` & `core_curate_app-2.9.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.8.0/tests/views/admin/ajax/test_unit.py` & `core_curate_app-2.9.0/tests/views/admin/ajax/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.8.0/tests/views/common/views/test_unit.py` & `core_curate_app-2.9.0/tests/views/common/views/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.8.0/tests/views/common/views/tests_int_access_control.py` & `core_curate_app-2.9.0/tests/views/common/views/tests_int_access_control.py`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.8.0/tests/views/user/ajax/test_unit.py` & `core_curate_app-2.9.0/tests/views/user/ajax/test_unit.py`

 * *Files 0% similar despite different names*

```diff
@@ -382,17 +382,15 @@
         mock_curate_data_structure_api.get_by_id.return_value = MagicMock(
             template=mock_template, data=None, name="title"
         )
         mock_curate_data_structure_api.upsert.return_value = None
 
         response = curate_user_ajax.save_form(self.request)
         self.assertEqual(response.status_code, 200)
-        self.assertTrue(
-            "saved with success." in response.content.decode("utf-8")
-        )
+        self.assertTrue("saved." in response.content.decode("utf-8"))
 
     @patch.object(curate_user_ajax, "curate_data_structure_api")
     def test_save_form_with_well_formed_content_returns_http_200(
         self, mock_curate_data_structure_api
     ):
         """test_save_form_with_well_formed_content_returns_http_200"""
         mock_curate_data_structure = CurateDataStructure(
```

### Comparing `core_curate_app-2.8.0/tests/views/user/ajax/tests_int_access_control.py` & `core_curate_app-2.9.0/tests/views/user/ajax/tests_int_access_control.py`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.8.0/tests/views/user/forms/test_unit.py` & `core_curate_app-2.9.0/tests/views/user/forms/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_curate_app-2.8.0/tests/views/user/views/test_unit.py` & `core_curate_app-2.9.0/tests/views/user/views/test_unit.py`

 * *Files identical despite different names*

