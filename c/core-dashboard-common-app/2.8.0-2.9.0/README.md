# Comparing `tmp/core_dashboard_common_app-2.8.0.tar.gz` & `tmp/core_dashboard_common_app-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_dashboard_common_app-2.8.0.tar", last modified: Tue Mar 12 18:58:25 2024, max compression
+gzip compressed data, was "core_dashboard_common_app-2.9.0.tar", last modified: Mon May 13 16:03:56 2024, max compression
```

## Comparing `core_dashboard_common_app-2.8.0.tar` & `core_dashboard_common_app-2.9.0.tar`

### file list

```diff
@@ -1,129 +1,129 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:25.538231 core_dashboard_common_app-2.8.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2024-03-12 18:58:19.000000 core_dashboard_common_app-2.8.0/LICENSE.md
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      158 2024-03-12 18:58:19.000000 core_dashboard_common_app-2.8.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      865 2024-03-12 18:58:25.532047 core_dashboard_common_app-2.8.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      406 2024-03-12 18:58:19.000000 core_dashboard_common_app-2.8.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:23.702989 core_dashboard_common_app-2.8.0/core_dashboard_common_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:19.000000 core_dashboard_common_app-2.8.0/core_dashboard_common_app/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3778 2024-03-12 18:58:19.000000 core_dashboard_common_app-2.8.0/core_dashboard_common_app/constants.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1250 2024-03-12 18:58:19.000000 core_dashboard_common_app-2.8.0/core_dashboard_common_app/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:23.358352 core_dashboard_common_app-2.8.0/core_dashboard_common_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:23.410349 core_dashboard_common_app-2.8.0/core_dashboard_common_app/static/core_dashboard_common_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:23.367640 core_dashboard_common_app-2.8.0/core_dashboard_common_app/static/core_dashboard_common_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:23.954264 core_dashboard_common_app-2.8.0/core_dashboard_common_app/static/core_dashboard_common_app/admin/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      302 2024-03-12 18:58:19.000000 core_dashboard_common_app-2.8.0/core_dashboard_common_app/static/core_dashboard_common_app/admin/js/action_dashboard.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      441 2024-03-12 18:58:19.000000 core_dashboard_common_app-2.8.0/core_dashboard_common_app/static/core_dashboard_common_app/admin/js/count_checked.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      393 2024-03-12 18:58:19.000000 core_dashboard_common_app-2.8.0/core_dashboard_common_app/static/core_dashboard_common_app/admin/js/get_selected_document_admin.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      237 2024-03-12 18:58:19.000000 core_dashboard_common_app-2.8.0/core_dashboard_common_app/static/core_dashboard_common_app/admin/js/init_admin_menu.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:23.971869 core_dashboard_common_app-2.8.0/core_dashboard_common_app/static/core_dashboard_common_app/admin/js/list/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       71 2024-03-12 18:58:19.000000 core_dashboard_common_app-2.8.0/core_dashboard_common_app/static/core_dashboard_common_app/admin/js/list/view_record.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       68 2024-03-12 18:58:19.000000 core_dashboard_common_app-2.8.0/core_dashboard_common_app/static/core_dashboard_common_app/admin/js/my_dashboard_tabs.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      697 2024-03-12 18:58:19.000000 core_dashboard_common_app-2.8.0/core_dashboard_common_app/static/core_dashboard_common_app/admin/js/reset_checkbox.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      241 2024-03-12 18:58:19.000000 core_dashboard_common_app-2.8.0/core_dashboard_common_app/static/core_dashboard_common_app/admin/js/select_all.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:23.395000 core_dashboard_common_app-2.8.0/core_dashboard_common_app/static/core_dashboard_common_app/common/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:24.030074 core_dashboard_common_app-2.8.0/core_dashboard_common_app/static/core_dashboard_common_app/common/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      117 2024-03-12 18:58:19.000000 core_dashboard_common_app-2.8.0/core_dashboard_common_app/static/core_dashboard_common_app/common/css/content_query.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       35 2024-03-12 18:58:19.000000 core_dashboard_common_app-2.8.0/core_dashboard_common_app/static/core_dashboard_common_app/common/css/list.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       65 2024-03-12 18:58:19.000000 core_dashboard_common_app-2.8.0/core_dashboard_common_app/static/core_dashboard_common_app/common/css/password_form.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:24.100142 core_dashboard_common_app-2.8.0/core_dashboard_common_app/static/core_dashboard_common_app/common/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       84 2024-03-12 18:58:19.000000 core_dashboard_common_app-2.8.0/core_dashboard_common_app/static/core_dashboard_common_app/common/js/init_pagination.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:24.257918 core_dashboard_common_app-2.8.0/core_dashboard_common_app/static/core_dashboard_common_app/common/js/list/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      669 2024-03-12 18:58:19.000000 core_dashboard_common_app-2.8.0/core_dashboard_common_app/static/core_dashboard_common_app/common/js/list/delete_data_draft.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      177 2024-03-12 18:58:19.000000 core_dashboard_common_app-2.8.0/core_dashboard_common_app/static/core_dashboard_common_app/common/js/list/delete_data_draft.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      792 2024-03-12 18:58:19.000000 core_dashboard_common_app-2.8.0/core_dashboard_common_app/static/core_dashboard_common_app/common/js/list/open_document.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      147 2024-03-12 18:58:19.000000 core_dashboard_common_app-2.8.0/core_dashboard_common_app/static/core_dashboard_common_app/common/js/list/open_form.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      147 2024-03-12 18:58:19.000000 core_dashboard_common_app-2.8.0/core_dashboard_common_app/static/core_dashboard_common_app/common/js/list/open_record.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:19.000000 core_dashboard_common_app-2.8.0/core_dashboard_common_app/static/core_dashboard_common_app/common/js/list/open_template.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      427 2024-03-12 18:58:19.000000 core_dashboard_common_app-2.8.0/core_dashboard_common_app/static/core_dashboard_common_app/common/js/list/view_record.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1277 2024-03-12 18:58:19.000000 core_dashboard_common_app-2.8.0/core_dashboard_common_app/static/core_dashboard_common_app/common/js/persistent_query_config.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:23.421395 core_dashboard_common_app-2.8.0/core_dashboard_common_app/static/core_dashboard_common_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:24.277783 core_dashboard_common_app-2.8.0/core_dashboard_common_app/static/core_dashboard_common_app/user/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      831 2024-03-12 18:58:19.000000 core_dashboard_common_app-2.8.0/core_dashboard_common_app/static/core_dashboard_common_app/user/css/exploreTabs.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:24.377397 core_dashboard_common_app-2.8.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      150 2024-03-12 18:58:19.000000 core_dashboard_common_app-2.8.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/get_selected_document.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      577 2024-03-12 18:58:19.000000 core_dashboard_common_app-2.8.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/init.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       83 2024-03-12 18:58:19.000000 core_dashboard_common_app-2.8.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/init.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       68 2024-03-12 18:58:19.000000 core_dashboard_common_app-2.8.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/init_user.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:24.445529 core_dashboard_common_app-2.8.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      856 2024-03-12 18:58:19.000000 core_dashboard_common_app-2.8.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/edit_record.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       61 2024-03-12 18:58:19.000000 core_dashboard_common_app-2.8.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/edit_record.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:24.604301 core_dashboard_common_app-2.8.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1714 2024-03-12 18:58:19.000000 core_dashboard_common_app-2.8.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/change_owner.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       81 2024-03-12 18:58:19.000000 core_dashboard_common_app-2.8.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/change_owner.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1392 2024-03-12 18:58:19.000000 core_dashboard_common_app-2.8.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/delete_document.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       78 2024-03-12 18:58:20.000000 core_dashboard_common_app-2.8.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/delete_document.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1613 2024-03-12 18:58:20.000000 core_dashboard_common_app-2.8.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/edit_persistent_query.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2024-03-12 18:58:20.000000 core_dashboard_common_app-2.8.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/edit_query.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      933 2024-03-12 18:58:20.000000 core_dashboard_common_app-2.8.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/upload_file.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       56 2024-03-12 18:58:20.000000 core_dashboard_common_app-2.8.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/upload_file.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       60 2024-03-12 18:58:20.000000 core_dashboard_common_app-2.8.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/view_record.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       56 2024-03-12 18:58:20.000000 core_dashboard_common_app-2.8.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/my_dashboard_tabs.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:23.458740 core_dashboard_common_app-2.8.0/core_dashboard_common_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:24.727813 core_dashboard_common_app-2.8.0/core_dashboard_common_app/templates/core_dashboard_common_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:24.750648 core_dashboard_common_app-2.8.0/core_dashboard_common_app/templates/core_dashboard_common_app/admin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      380 2024-03-12 18:58:20.000000 core_dashboard_common_app-2.8.0/core_dashboard_common_app/templates/core_dashboard_common_app/admin/dashboard.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:23.477082 core_dashboard_common_app-2.8.0/core_dashboard_common_app/templates/core_dashboard_common_app/common/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:24.776213 core_dashboard_common_app-2.8.0/core_dashboard_common_app/templates/core_dashboard_common_app/common/pagination/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2701 2024-03-12 18:58:20.000000 core_dashboard_common_app-2.8.0/core_dashboard_common_app/templates/core_dashboard_common_app/common/pagination/data_source_pagination.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      123 2024-03-12 18:58:20.000000 core_dashboard_common_app-2.8.0/core_dashboard_common_app/templates/core_dashboard_common_app/home.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:24.978047 core_dashboard_common_app-2.8.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:25.032707 core_dashboard_common_app-2.8.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      954 2024-03-12 18:58:20.000000 core_dashboard_common_app-2.8.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/modals/change_owner.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1352 2024-03-12 18:58:20.000000 core_dashboard_common_app-2.8.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/modals/delete_document.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1167 2024-03-12 18:58:20.000000 core_dashboard_common_app-2.8.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/modals/edit_persistent_query.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4334 2024-03-12 18:58:20.000000 core_dashboard_common_app-2.8.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_files_table.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4055 2024-03-12 18:58:20.000000 core_dashboard_common_app-2.8.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_forms_table.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4828 2024-03-12 18:58:20.000000 core_dashboard_common_app-2.8.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_queries_table.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      211 2024-03-12 18:58:20.000000 core_dashboard_common_app-2.8.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_queries_table_pagination.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6801 2024-03-12 18:58:20.000000 core_dashboard_common_app-2.8.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_records_table.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      222 2024-03-12 18:58:20.000000 core_dashboard_common_app-2.8.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_records_table_datatable.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      258 2024-03-12 18:58:20.000000 core_dashboard_common_app-2.8.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_records_table_pagination.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3324 2024-03-12 18:58:20.000000 core_dashboard_common_app-2.8.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_templates_table.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2675 2024-03-12 18:58:20.000000 core_dashboard_common_app-2.8.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_types_table.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3432 2024-03-12 18:58:20.000000 core_dashboard_common_app-2.8.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_workspaces_table.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1767 2024-03-12 18:58:20.000000 core_dashboard_common_app-2.8.0/core_dashboard_common_app/templates/core_dashboard_common_app/my_dashboard.html
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     1697 2024-03-12 18:58:20.000000 core_dashboard_common_app-2.8.0/core_dashboard_common_app/templates/core_dashboard_common_app/my_profile.html
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      187 2024-03-12 18:58:20.000000 core_dashboard_common_app-2.8.0/core_dashboard_common_app/templates/core_dashboard_common_app/my_profile_change_password.html
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      854 2024-03-12 18:58:20.000000 core_dashboard_common_app-2.8.0/core_dashboard_common_app/templates/core_dashboard_common_app/my_profile_edit.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1007 2024-03-12 18:58:20.000000 core_dashboard_common_app-2.8.0/core_dashboard_common_app/templates/core_dashboard_common_app/password_change.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:25.084015 core_dashboard_common_app-2.8.0/core_dashboard_common_app/templatetags/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:20.000000 core_dashboard_common_app-2.8.0/core_dashboard_common_app/templatetags/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      453 2024-03-12 18:58:20.000000 core_dashboard_common_app-2.8.0/core_dashboard_common_app/templatetags/special_plural.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:25.113250 core_dashboard_common_app-2.8.0/core_dashboard_common_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:20.000000 core_dashboard_common_app-2.8.0/core_dashboard_common_app/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:25.190005 core_dashboard_common_app-2.8.0/core_dashboard_common_app/views/common/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:20.000000 core_dashboard_common_app-2.8.0/core_dashboard_common_app/views/common/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    19698 2024-03-12 18:58:20.000000 core_dashboard_common_app-2.8.0/core_dashboard_common_app/views/common/ajax.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1196 2024-03-12 18:58:20.000000 core_dashboard_common_app-2.8.0/core_dashboard_common_app/views/common/forms.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    56728 2024-03-12 18:58:20.000000 core_dashboard_common_app-2.8.0/core_dashboard_common_app/views/common/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:23.807187 core_dashboard_common_app-2.8.0/core_dashboard_common_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      865 2024-03-12 18:58:22.000000 core_dashboard_common_app-2.8.0/core_dashboard_common_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6570 2024-03-12 18:58:23.000000 core_dashboard_common_app-2.8.0/core_dashboard_common_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2024-03-12 18:58:22.000000 core_dashboard_common_app-2.8.0/core_dashboard_common_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       47 2024-03-12 18:58:22.000000 core_dashboard_common_app-2.8.0/core_dashboard_common_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       37 2024-03-12 18:58:22.000000 core_dashboard_common_app-2.8.0/core_dashboard_common_app.egg-info/top_level.txt
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:25.233303 core_dashboard_common_app-2.8.0/docs/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:20.000000 core_dashboard_common_app-2.8.0/docs/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11337 2024-03-12 18:58:20.000000 core_dashboard_common_app-2.8.0/docs/conf.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2024-03-12 18:58:20.000000 core_dashboard_common_app-2.8.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       21 2024-03-12 18:58:20.000000 core_dashboard_common_app-2.8.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2024-03-12 18:58:25.540583 core_dashboard_common_app-2.8.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1093 2024-03-12 18:58:20.000000 core_dashboard_common_app-2.8.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:25.311826 core_dashboard_common_app-2.8.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:20.000000 core_dashboard_common_app-2.8.0/tests/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      259 2024-03-12 18:58:20.000000 core_dashboard_common_app-2.8.0/tests/mocks.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1831 2024-03-12 18:58:20.000000 core_dashboard_common_app-2.8.0/tests/test_settings.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1027 2024-03-12 18:58:20.000000 core_dashboard_common_app-2.8.0/tests/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:25.352403 core_dashboard_common_app-2.8.0/tests/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:20.000000 core_dashboard_common_app-2.8.0/tests/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:25.371635 core_dashboard_common_app-2.8.0/tests/views/common/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:20.000000 core_dashboard_common_app-2.8.0/tests/views/common/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:25.434502 core_dashboard_common_app-2.8.0/tests/views/common/ajax/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:20.000000 core_dashboard_common_app-2.8.0/tests/views/common/ajax/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3703 2024-03-12 18:58:20.000000 core_dashboard_common_app-2.8.0/tests/views/common/ajax/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    28548 2024-03-12 18:58:20.000000 core_dashboard_common_app-2.8.0/tests/views/common/ajax/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:25.513952 core_dashboard_common_app-2.8.0/tests/views/common/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:21.000000 core_dashboard_common_app-2.8.0/tests/views/common/views/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2093 2024-03-12 18:58:21.000000 core_dashboard_common_app-2.8.0/tests/views/common/views/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6085 2024-03-12 18:58:21.000000 core_dashboard_common_app-2.8.0/tests/views/common/views/tests_unit.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4081 2024-03-12 18:58:21.000000 core_dashboard_common_app-2.8.0/tests/views/fixtures.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:56.194383 core_dashboard_common_app-2.9.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2024-05-13 16:03:45.000000 core_dashboard_common_app-2.9.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      158 2024-05-13 16:03:45.000000 core_dashboard_common_app-2.9.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      865 2024-05-13 16:03:56.187804 core_dashboard_common_app-2.9.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      406 2024-05-13 16:03:46.000000 core_dashboard_common_app-2.9.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:52.933777 core_dashboard_common_app-2.9.0/core_dashboard_common_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:46.000000 core_dashboard_common_app-2.9.0/core_dashboard_common_app/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3778 2024-05-13 16:03:46.000000 core_dashboard_common_app-2.9.0/core_dashboard_common_app/constants.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1250 2024-05-13 16:03:46.000000 core_dashboard_common_app-2.9.0/core_dashboard_common_app/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:52.378648 core_dashboard_common_app-2.9.0/core_dashboard_common_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:52.517985 core_dashboard_common_app-2.9.0/core_dashboard_common_app/static/core_dashboard_common_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:52.387612 core_dashboard_common_app-2.9.0/core_dashboard_common_app/static/core_dashboard_common_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:53.805468 core_dashboard_common_app-2.9.0/core_dashboard_common_app/static/core_dashboard_common_app/admin/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      302 2024-05-13 16:03:46.000000 core_dashboard_common_app-2.9.0/core_dashboard_common_app/static/core_dashboard_common_app/admin/js/action_dashboard.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      441 2024-05-13 16:03:46.000000 core_dashboard_common_app-2.9.0/core_dashboard_common_app/static/core_dashboard_common_app/admin/js/count_checked.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      393 2024-05-13 16:03:46.000000 core_dashboard_common_app-2.9.0/core_dashboard_common_app/static/core_dashboard_common_app/admin/js/get_selected_document_admin.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      237 2024-05-13 16:03:46.000000 core_dashboard_common_app-2.9.0/core_dashboard_common_app/static/core_dashboard_common_app/admin/js/init_admin_menu.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:53.827264 core_dashboard_common_app-2.9.0/core_dashboard_common_app/static/core_dashboard_common_app/admin/js/list/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       71 2024-05-13 16:03:46.000000 core_dashboard_common_app-2.9.0/core_dashboard_common_app/static/core_dashboard_common_app/admin/js/list/view_record.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       68 2024-05-13 16:03:46.000000 core_dashboard_common_app-2.9.0/core_dashboard_common_app/static/core_dashboard_common_app/admin/js/my_dashboard_tabs.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      697 2024-05-13 16:03:46.000000 core_dashboard_common_app-2.9.0/core_dashboard_common_app/static/core_dashboard_common_app/admin/js/reset_checkbox.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      241 2024-05-13 16:03:46.000000 core_dashboard_common_app-2.9.0/core_dashboard_common_app/static/core_dashboard_common_app/admin/js/select_all.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:52.503486 core_dashboard_common_app-2.9.0/core_dashboard_common_app/static/core_dashboard_common_app/common/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:53.889362 core_dashboard_common_app-2.9.0/core_dashboard_common_app/static/core_dashboard_common_app/common/css/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      117 2024-05-13 16:03:46.000000 core_dashboard_common_app-2.9.0/core_dashboard_common_app/static/core_dashboard_common_app/common/css/content_query.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       35 2024-05-13 16:03:46.000000 core_dashboard_common_app-2.9.0/core_dashboard_common_app/static/core_dashboard_common_app/common/css/list.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       65 2024-05-13 16:03:46.000000 core_dashboard_common_app-2.9.0/core_dashboard_common_app/static/core_dashboard_common_app/common/css/password_form.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:53.928379 core_dashboard_common_app-2.9.0/core_dashboard_common_app/static/core_dashboard_common_app/common/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       84 2024-05-13 16:03:46.000000 core_dashboard_common_app-2.9.0/core_dashboard_common_app/static/core_dashboard_common_app/common/js/init_pagination.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:54.187128 core_dashboard_common_app-2.9.0/core_dashboard_common_app/static/core_dashboard_common_app/common/js/list/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      669 2024-05-13 16:03:46.000000 core_dashboard_common_app-2.9.0/core_dashboard_common_app/static/core_dashboard_common_app/common/js/list/delete_data_draft.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      177 2024-05-13 16:03:46.000000 core_dashboard_common_app-2.9.0/core_dashboard_common_app/static/core_dashboard_common_app/common/js/list/delete_data_draft.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      792 2024-05-13 16:03:46.000000 core_dashboard_common_app-2.9.0/core_dashboard_common_app/static/core_dashboard_common_app/common/js/list/open_document.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      147 2024-05-13 16:03:46.000000 core_dashboard_common_app-2.9.0/core_dashboard_common_app/static/core_dashboard_common_app/common/js/list/open_form.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      147 2024-05-13 16:03:46.000000 core_dashboard_common_app-2.9.0/core_dashboard_common_app/static/core_dashboard_common_app/common/js/list/open_record.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:46.000000 core_dashboard_common_app-2.9.0/core_dashboard_common_app/static/core_dashboard_common_app/common/js/list/open_template.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      427 2024-05-13 16:03:46.000000 core_dashboard_common_app-2.9.0/core_dashboard_common_app/static/core_dashboard_common_app/common/js/list/view_record.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1277 2024-05-13 16:03:46.000000 core_dashboard_common_app-2.9.0/core_dashboard_common_app/static/core_dashboard_common_app/common/js/persistent_query_config.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:52.550236 core_dashboard_common_app-2.9.0/core_dashboard_common_app/static/core_dashboard_common_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:54.212915 core_dashboard_common_app-2.9.0/core_dashboard_common_app/static/core_dashboard_common_app/user/css/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      831 2024-05-13 16:03:46.000000 core_dashboard_common_app-2.9.0/core_dashboard_common_app/static/core_dashboard_common_app/user/css/exploreTabs.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:54.877908 core_dashboard_common_app-2.9.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      150 2024-05-13 16:03:46.000000 core_dashboard_common_app-2.9.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/get_selected_document.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      577 2024-05-13 16:03:46.000000 core_dashboard_common_app-2.9.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/init.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       83 2024-05-13 16:03:46.000000 core_dashboard_common_app-2.9.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/init.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       68 2024-05-13 16:03:46.000000 core_dashboard_common_app-2.9.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/init_user.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:54.932597 core_dashboard_common_app-2.9.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      856 2024-05-13 16:03:46.000000 core_dashboard_common_app-2.9.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/edit_record.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       61 2024-05-13 16:03:46.000000 core_dashboard_common_app-2.9.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/edit_record.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:55.132853 core_dashboard_common_app-2.9.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1714 2024-05-13 16:03:46.000000 core_dashboard_common_app-2.9.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/change_owner.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       81 2024-05-13 16:03:46.000000 core_dashboard_common_app-2.9.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/change_owner.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1392 2024-05-13 16:03:46.000000 core_dashboard_common_app-2.9.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/delete_document.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       78 2024-05-13 16:03:46.000000 core_dashboard_common_app-2.9.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/delete_document.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1613 2024-05-13 16:03:46.000000 core_dashboard_common_app-2.9.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/edit_persistent_query.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2024-05-13 16:03:46.000000 core_dashboard_common_app-2.9.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/edit_query.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      933 2024-05-13 16:03:46.000000 core_dashboard_common_app-2.9.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/upload_file.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       56 2024-05-13 16:03:46.000000 core_dashboard_common_app-2.9.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/upload_file.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       60 2024-05-13 16:03:46.000000 core_dashboard_common_app-2.9.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/view_record.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       56 2024-05-13 16:03:46.000000 core_dashboard_common_app-2.9.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/my_dashboard_tabs.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:52.614747 core_dashboard_common_app-2.9.0/core_dashboard_common_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:55.244537 core_dashboard_common_app-2.9.0/core_dashboard_common_app/templates/core_dashboard_common_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:55.301222 core_dashboard_common_app-2.9.0/core_dashboard_common_app/templates/core_dashboard_common_app/admin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      380 2024-05-13 16:03:46.000000 core_dashboard_common_app-2.9.0/core_dashboard_common_app/templates/core_dashboard_common_app/admin/dashboard.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:52.634660 core_dashboard_common_app-2.9.0/core_dashboard_common_app/templates/core_dashboard_common_app/common/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:55.324507 core_dashboard_common_app-2.9.0/core_dashboard_common_app/templates/core_dashboard_common_app/common/pagination/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2701 2024-05-13 16:03:46.000000 core_dashboard_common_app-2.9.0/core_dashboard_common_app/templates/core_dashboard_common_app/common/pagination/data_source_pagination.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      123 2024-05-13 16:03:46.000000 core_dashboard_common_app-2.9.0/core_dashboard_common_app/templates/core_dashboard_common_app/home.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:55.557816 core_dashboard_common_app-2.9.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:55.634447 core_dashboard_common_app-2.9.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      954 2024-05-13 16:03:46.000000 core_dashboard_common_app-2.9.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/modals/change_owner.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1352 2024-05-13 16:03:46.000000 core_dashboard_common_app-2.9.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/modals/delete_document.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1167 2024-05-13 16:03:46.000000 core_dashboard_common_app-2.9.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/modals/edit_persistent_query.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4334 2024-05-13 16:03:46.000000 core_dashboard_common_app-2.9.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_files_table.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4055 2024-05-13 16:03:46.000000 core_dashboard_common_app-2.9.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_forms_table.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4828 2024-05-13 16:03:46.000000 core_dashboard_common_app-2.9.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_queries_table.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      211 2024-05-13 16:03:47.000000 core_dashboard_common_app-2.9.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_queries_table_pagination.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6801 2024-05-13 16:03:47.000000 core_dashboard_common_app-2.9.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_records_table.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      222 2024-05-13 16:03:47.000000 core_dashboard_common_app-2.9.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_records_table_datatable.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      258 2024-05-13 16:03:47.000000 core_dashboard_common_app-2.9.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_records_table_pagination.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3324 2024-05-13 16:03:47.000000 core_dashboard_common_app-2.9.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_templates_table.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2675 2024-05-13 16:03:47.000000 core_dashboard_common_app-2.9.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_types_table.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3432 2024-05-13 16:03:47.000000 core_dashboard_common_app-2.9.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_workspaces_table.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1767 2024-05-13 16:03:47.000000 core_dashboard_common_app-2.9.0/core_dashboard_common_app/templates/core_dashboard_common_app/my_dashboard.html
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     1697 2024-05-13 16:03:47.000000 core_dashboard_common_app-2.9.0/core_dashboard_common_app/templates/core_dashboard_common_app/my_profile.html
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      187 2024-05-13 16:03:47.000000 core_dashboard_common_app-2.9.0/core_dashboard_common_app/templates/core_dashboard_common_app/my_profile_change_password.html
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      854 2024-05-13 16:03:47.000000 core_dashboard_common_app-2.9.0/core_dashboard_common_app/templates/core_dashboard_common_app/my_profile_edit.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1007 2024-05-13 16:03:47.000000 core_dashboard_common_app-2.9.0/core_dashboard_common_app/templates/core_dashboard_common_app/password_change.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:55.674100 core_dashboard_common_app-2.9.0/core_dashboard_common_app/templatetags/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:47.000000 core_dashboard_common_app-2.9.0/core_dashboard_common_app/templatetags/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      453 2024-05-13 16:03:47.000000 core_dashboard_common_app-2.9.0/core_dashboard_common_app/templatetags/special_plural.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:55.694234 core_dashboard_common_app-2.9.0/core_dashboard_common_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:47.000000 core_dashboard_common_app-2.9.0/core_dashboard_common_app/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:55.818260 core_dashboard_common_app-2.9.0/core_dashboard_common_app/views/common/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:47.000000 core_dashboard_common_app-2.9.0/core_dashboard_common_app/views/common/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    19624 2024-05-13 16:03:47.000000 core_dashboard_common_app-2.9.0/core_dashboard_common_app/views/common/ajax.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1196 2024-05-13 16:03:47.000000 core_dashboard_common_app-2.9.0/core_dashboard_common_app/views/common/forms.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    56715 2024-05-13 16:03:47.000000 core_dashboard_common_app-2.9.0/core_dashboard_common_app/views/common/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:53.033231 core_dashboard_common_app-2.9.0/core_dashboard_common_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      865 2024-05-13 16:03:50.000000 core_dashboard_common_app-2.9.0/core_dashboard_common_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6570 2024-05-13 16:03:51.000000 core_dashboard_common_app-2.9.0/core_dashboard_common_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2024-05-13 16:03:50.000000 core_dashboard_common_app-2.9.0/core_dashboard_common_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       47 2024-05-13 16:03:50.000000 core_dashboard_common_app-2.9.0/core_dashboard_common_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       37 2024-05-13 16:03:50.000000 core_dashboard_common_app-2.9.0/core_dashboard_common_app.egg-info/top_level.txt
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:55.863443 core_dashboard_common_app-2.9.0/docs/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:47.000000 core_dashboard_common_app-2.9.0/docs/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11337 2024-05-13 16:03:47.000000 core_dashboard_common_app-2.9.0/docs/conf.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2024-05-13 16:03:47.000000 core_dashboard_common_app-2.9.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       21 2024-05-13 16:03:47.000000 core_dashboard_common_app-2.9.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2024-05-13 16:03:56.196825 core_dashboard_common_app-2.9.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1093 2024-05-13 16:03:47.000000 core_dashboard_common_app-2.9.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:55.939030 core_dashboard_common_app-2.9.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:47.000000 core_dashboard_common_app-2.9.0/tests/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      259 2024-05-13 16:03:47.000000 core_dashboard_common_app-2.9.0/tests/mocks.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1831 2024-05-13 16:03:47.000000 core_dashboard_common_app-2.9.0/tests/test_settings.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1027 2024-05-13 16:03:47.000000 core_dashboard_common_app-2.9.0/tests/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:55.984147 core_dashboard_common_app-2.9.0/tests/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:47.000000 core_dashboard_common_app-2.9.0/tests/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:56.006898 core_dashboard_common_app-2.9.0/tests/views/common/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:47.000000 core_dashboard_common_app-2.9.0/tests/views/common/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:56.103567 core_dashboard_common_app-2.9.0/tests/views/common/ajax/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:47.000000 core_dashboard_common_app-2.9.0/tests/views/common/ajax/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3703 2024-05-13 16:03:47.000000 core_dashboard_common_app-2.9.0/tests/views/common/ajax/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    28548 2024-05-13 16:03:47.000000 core_dashboard_common_app-2.9.0/tests/views/common/ajax/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:56.168412 core_dashboard_common_app-2.9.0/tests/views/common/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:03:47.000000 core_dashboard_common_app-2.9.0/tests/views/common/views/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2093 2024-05-13 16:03:47.000000 core_dashboard_common_app-2.9.0/tests/views/common/views/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6085 2024-05-13 16:03:47.000000 core_dashboard_common_app-2.9.0/tests/views/common/views/tests_unit.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4081 2024-05-13 16:03:47.000000 core_dashboard_common_app-2.9.0/tests/views/fixtures.py
```

### Comparing `core_dashboard_common_app-2.8.0/LICENSE.md` & `core_dashboard_common_app-2.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `core_dashboard_common_app-2.8.0/PKG-INFO` & `core_dashboard_common_app-2.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_dashboard_common_app
-Version: 2.8.0
+Version: 2.9.0
 Summary: Resource management via a dashboard for the curator core project
 Home-page: https://github.com/usnistgov/core_dashboard_common_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: =========================
         Core Dashboard Common App
```

### Comparing `core_dashboard_common_app-2.8.0/core_dashboard_common_app/constants.py` & `core_dashboard_common_app-2.9.0/core_dashboard_common_app/constants.py`

 * *Files identical despite different names*

### Comparing `core_dashboard_common_app-2.8.0/core_dashboard_common_app/settings.py` & `core_dashboard_common_app-2.9.0/core_dashboard_common_app/settings.py`

 * *Files identical despite different names*

### Comparing `core_dashboard_common_app-2.8.0/core_dashboard_common_app/static/core_dashboard_common_app/admin/js/reset_checkbox.js` & `core_dashboard_common_app-2.9.0/core_dashboard_common_app/static/core_dashboard_common_app/admin/js/reset_checkbox.js`

 * *Files identical despite different names*

### Comparing `core_dashboard_common_app-2.8.0/core_dashboard_common_app/static/core_dashboard_common_app/common/js/list/delete_data_draft.js` & `core_dashboard_common_app-2.9.0/core_dashboard_common_app/static/core_dashboard_common_app/common/js/list/delete_data_draft.js`

 * *Files identical despite different names*

### Comparing `core_dashboard_common_app-2.8.0/core_dashboard_common_app/static/core_dashboard_common_app/common/js/list/open_document.js` & `core_dashboard_common_app-2.9.0/core_dashboard_common_app/static/core_dashboard_common_app/common/js/list/open_document.js`

 * *Files identical despite different names*

### Comparing `core_dashboard_common_app-2.8.0/core_dashboard_common_app/static/core_dashboard_common_app/common/js/persistent_query_config.js` & `core_dashboard_common_app-2.9.0/core_dashboard_common_app/static/core_dashboard_common_app/common/js/persistent_query_config.js`

 * *Files identical despite different names*

### Comparing `core_dashboard_common_app-2.8.0/core_dashboard_common_app/static/core_dashboard_common_app/user/css/exploreTabs.css` & `core_dashboard_common_app-2.9.0/core_dashboard_common_app/static/core_dashboard_common_app/user/css/exploreTabs.css`

 * *Files identical despite different names*

### Comparing `core_dashboard_common_app-2.8.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/init.js` & `core_dashboard_common_app-2.9.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/init.js`

 * *Files identical despite different names*

### Comparing `core_dashboard_common_app-2.8.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/edit_record.js` & `core_dashboard_common_app-2.9.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/edit_record.js`

 * *Files identical despite different names*

### Comparing `core_dashboard_common_app-2.8.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/change_owner.js` & `core_dashboard_common_app-2.9.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/change_owner.js`

 * *Files identical despite different names*

### Comparing `core_dashboard_common_app-2.8.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/delete_document.js` & `core_dashboard_common_app-2.9.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/delete_document.js`

 * *Files identical despite different names*

### Comparing `core_dashboard_common_app-2.8.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/edit_persistent_query.js` & `core_dashboard_common_app-2.9.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/edit_persistent_query.js`

 * *Files identical despite different names*

### Comparing `core_dashboard_common_app-2.8.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/upload_file.js` & `core_dashboard_common_app-2.9.0/core_dashboard_common_app/static/core_dashboard_common_app/user/js/list/modals/upload_file.js`

 * *Files identical despite different names*

### Comparing `core_dashboard_common_app-2.8.0/core_dashboard_common_app/templates/core_dashboard_common_app/common/pagination/data_source_pagination.html` & `core_dashboard_common_app-2.9.0/core_dashboard_common_app/templates/core_dashboard_common_app/common/pagination/data_source_pagination.html`

 * *Files identical despite different names*

### Comparing `core_dashboard_common_app-2.8.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/modals/change_owner.html` & `core_dashboard_common_app-2.9.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/modals/change_owner.html`

 * *Files identical despite different names*

### Comparing `core_dashboard_common_app-2.8.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/modals/delete_document.html` & `core_dashboard_common_app-2.9.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/modals/delete_document.html`

 * *Files identical despite different names*

### Comparing `core_dashboard_common_app-2.8.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/modals/edit_persistent_query.html` & `core_dashboard_common_app-2.9.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/modals/edit_persistent_query.html`

 * *Files identical despite different names*

### Comparing `core_dashboard_common_app-2.8.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_files_table.html` & `core_dashboard_common_app-2.9.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_files_table.html`

 * *Files identical despite different names*

### Comparing `core_dashboard_common_app-2.8.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_forms_table.html` & `core_dashboard_common_app-2.9.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_forms_table.html`

 * *Files identical despite different names*

### Comparing `core_dashboard_common_app-2.8.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_queries_table.html` & `core_dashboard_common_app-2.9.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_queries_table.html`

 * *Files identical despite different names*

### Comparing `core_dashboard_common_app-2.8.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_records_table.html` & `core_dashboard_common_app-2.9.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_records_table.html`

 * *Files identical despite different names*

### Comparing `core_dashboard_common_app-2.8.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_templates_table.html` & `core_dashboard_common_app-2.9.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_templates_table.html`

 * *Files identical despite different names*

### Comparing `core_dashboard_common_app-2.8.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_types_table.html` & `core_dashboard_common_app-2.9.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_types_table.html`

 * *Files identical despite different names*

### Comparing `core_dashboard_common_app-2.8.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_workspaces_table.html` & `core_dashboard_common_app-2.9.0/core_dashboard_common_app/templates/core_dashboard_common_app/list/my_dashboard_my_workspaces_table.html`

 * *Files identical despite different names*

### Comparing `core_dashboard_common_app-2.8.0/core_dashboard_common_app/templates/core_dashboard_common_app/my_dashboard.html` & `core_dashboard_common_app-2.9.0/core_dashboard_common_app/templates/core_dashboard_common_app/my_dashboard.html`

 * *Files identical despite different names*

### Comparing `core_dashboard_common_app-2.8.0/core_dashboard_common_app/templates/core_dashboard_common_app/my_profile.html` & `core_dashboard_common_app-2.9.0/core_dashboard_common_app/templates/core_dashboard_common_app/my_profile.html`

 * *Files identical despite different names*

### Comparing `core_dashboard_common_app-2.8.0/core_dashboard_common_app/templates/core_dashboard_common_app/my_profile_edit.html` & `core_dashboard_common_app-2.9.0/core_dashboard_common_app/templates/core_dashboard_common_app/my_profile_edit.html`

 * *Files identical despite different names*

### Comparing `core_dashboard_common_app-2.8.0/core_dashboard_common_app/templates/core_dashboard_common_app/password_change.html` & `core_dashboard_common_app-2.9.0/core_dashboard_common_app/templates/core_dashboard_common_app/password_change.html`

 * *Files identical despite different names*

### Comparing `core_dashboard_common_app-2.8.0/core_dashboard_common_app/views/common/ajax.py` & `core_dashboard_common_app-2.9.0/core_dashboard_common_app/views/common/ajax.py`

 * *Files 1% similar despite different names*

```diff
@@ -296,17 +296,15 @@
         return HttpResponse(
             json.dumps({}), content_type="application/javascript"
         )
 
     try:
         for blob in list_blob:
             blob_api.delete(blob, request.user)
-        messages.add_message(
-            request, messages.SUCCESS, "File deleted with success."
-        )
+        messages.add_message(request, messages.SUCCESS, "File deleted.")
     except Exception:
         messages.add_message(
             request, messages.ERROR, "A problem occurred while deleting."
         )
 
     return HttpResponse(json.dumps({}), content_type="application/javascript")
 
@@ -330,15 +328,15 @@
 
     try:
         for form in list_form:
             curate_data_structure_api.delete(form, request.user)
         messages.add_message(
             request,
             messages.SUCCESS,
-            get_form_label().capitalize() + " deleted with success.",
+            get_form_label().capitalize() + " deleted.",
         )
     except Exception:
         messages.add_message(
             request, messages.ERROR, "A problem occurred while deleting."
         )
 
     return HttpResponse(json.dumps({}), content_type="application/javascript")
@@ -377,15 +375,15 @@
                     content_type="application/javascript",
                 )
 
             data_api.delete(data, request.user)
         messages.add_message(
             request,
             messages.SUCCESS,
-            get_data_label().capitalize() + " deleted with success.",
+            get_data_label().capitalize() + " deleted.",
         )
     except Exception:
         messages.add_message(
             request, messages.ERROR, "A problem occurred while deleting."
         )
 
     return HttpResponse(json.dumps({}), content_type="application/javascript")
@@ -429,15 +427,15 @@
     try:
         for query in list_query:
             persistent_query_api.delete(query, request.user)
 
         messages.add_message(
             request,
             messages.SUCCESS,
-            " Query deleted with success.",
+            " Query deleted.",
         )
     except Exception:
         messages.add_message(
             request, messages.ERROR, "A problem occurred while deleting."
         )
 
     return HttpResponse(json.dumps({}), content_type="application/javascript")
```

### Comparing `core_dashboard_common_app-2.8.0/core_dashboard_common_app/views/common/forms.py` & `core_dashboard_common_app-2.9.0/core_dashboard_common_app/views/common/forms.py`

 * *Files identical despite different names*

### Comparing `core_dashboard_common_app-2.8.0/core_dashboard_common_app/views/common/views.py` & `core_dashboard_common_app-2.9.0/core_dashboard_common_app/views/common/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,15 +129,15 @@
                     _error_while_saving(request, form)
             except Exception:
                 _error_while_saving(request, form)
 
             messages.add_message(
                 request,
                 messages.SUCCESS,
-                "Profile information edited with success.",
+                "Profile information edited.",
             )
             return HttpResponseRedirect(reverse("core_dashboard_profile"))
     user = request.user
     data = {
         "firstname": user.first_name,
         "lastname": user.last_name,
         "username": user.username,
```

### Comparing `core_dashboard_common_app-2.8.0/core_dashboard_common_app.egg-info/PKG-INFO` & `core_dashboard_common_app-2.9.0/core_dashboard_common_app.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-dashboard-common-app
-Version: 2.8.0
+Version: 2.9.0
 Summary: Resource management via a dashboard for the curator core project
 Home-page: https://github.com/usnistgov/core_dashboard_common_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: =========================
         Core Dashboard Common App
```

### Comparing `core_dashboard_common_app-2.8.0/core_dashboard_common_app.egg-info/SOURCES.txt` & `core_dashboard_common_app-2.9.0/core_dashboard_common_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `core_dashboard_common_app-2.8.0/docs/conf.py` & `core_dashboard_common_app-2.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `core_dashboard_common_app-2.8.0/setup.py` & `core_dashboard_common_app-2.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_dashboard_common_app",
-    version="2.8.0",
+    version="2.9.0",
     description="Resource management via a dashboard for the curator core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_dashboard_common_app",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `core_dashboard_common_app-2.8.0/tests/test_settings.py` & `core_dashboard_common_app-2.9.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `core_dashboard_common_app-2.8.0/tests/urls.py` & `core_dashboard_common_app-2.9.0/tests/urls.py`

 * *Files identical despite different names*

### Comparing `core_dashboard_common_app-2.8.0/tests/views/common/ajax/tests_int.py` & `core_dashboard_common_app-2.9.0/tests/views/common/ajax/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_dashboard_common_app-2.8.0/tests/views/common/ajax/tests_unit.py` & `core_dashboard_common_app-2.9.0/tests/views/common/ajax/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_dashboard_common_app-2.8.0/tests/views/common/views/tests_int.py` & `core_dashboard_common_app-2.9.0/tests/views/common/views/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_dashboard_common_app-2.8.0/tests/views/common/views/tests_unit.py` & `core_dashboard_common_app-2.9.0/tests/views/common/views/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_dashboard_common_app-2.8.0/tests/views/fixtures.py` & `core_dashboard_common_app-2.9.0/tests/views/fixtures.py`

 * *Files identical despite different names*

