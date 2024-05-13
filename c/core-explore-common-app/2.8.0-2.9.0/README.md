# Comparing `tmp/core_explore_common_app-2.8.0.tar.gz` & `tmp/core_explore_common_app-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_explore_common_app-2.8.0.tar", last modified: Tue Mar 12 18:58:59 2024, max compression
+gzip compressed data, was "core_explore_common_app-2.9.0.tar", last modified: Mon May 13 16:04:33 2024, max compression
```

## Comparing `core_explore_common_app-2.8.0.tar` & `core_explore_common_app-2.9.0.tar`

### file list

```diff
@@ -1,170 +1,170 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:59.127664 core_explore_common_app-2.8.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2024-03-12 18:58:51.000000 core_explore_common_app-2.8.0/LICENSE.md
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      154 2024-03-12 18:58:51.000000 core_explore_common_app-2.8.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1108 2024-03-12 18:58:59.121486 core_explore_common_app-2.8.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      607 2024-03-12 18:58:51.000000 core_explore_common_app-2.8.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:56.754899 core_explore_common_app-2.8.0/core_explore_common_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       79 2024-03-12 18:58:51.000000 core_explore_common_app-2.8.0/core_explore_common_app/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:56.924972 core_explore_common_app-2.8.0/core_explore_common_app/access_control/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:51.000000 core_explore_common_app-2.8.0/core_explore_common_app/access_control/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4732 2024-03-12 18:58:51.000000 core_explore_common_app-2.8.0/core_explore_common_app/access_control/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      282 2024-03-12 18:58:51.000000 core_explore_common_app-2.8.0/core_explore_common_app/admin.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      450 2024-03-12 18:58:51.000000 core_explore_common_app-2.8.0/core_explore_common_app/apps.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:56.976967 core_explore_common_app-2.8.0/core_explore_common_app/commons/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:51.000000 core_explore_common_app-2.8.0/core_explore_common_app/commons/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      409 2024-03-12 18:58:51.000000 core_explore_common_app-2.8.0/core_explore_common_app/commons/exceptions.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:57.000324 core_explore_common_app-2.8.0/core_explore_common_app/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:51.000000 core_explore_common_app-2.8.0/core_explore_common_app/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:57.062794 core_explore_common_app-2.8.0/core_explore_common_app/components/abstract_persistent_query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:51.000000 core_explore_common_app-2.8.0/core_explore_common_app/components/abstract_persistent_query/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2123 2024-03-12 18:58:51.000000 core_explore_common_app-2.8.0/core_explore_common_app/components/abstract_persistent_query/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      552 2024-03-12 18:58:51.000000 core_explore_common_app-2.8.0/core_explore_common_app/components/abstract_persistent_query/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:57.102820 core_explore_common_app-2.8.0/core_explore_common_app/components/abstract_query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:51.000000 core_explore_common_app-2.8.0/core_explore_common_app/components/abstract_query/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1616 2024-03-12 18:58:51.000000 core_explore_common_app-2.8.0/core_explore_common_app/components/abstract_query/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:57.183240 core_explore_common_app-2.8.0/core_explore_common_app/components/query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:51.000000 core_explore_common_app-2.8.0/core_explore_common_app/components/query/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      372 2024-03-12 18:58:51.000000 core_explore_common_app-2.8.0/core_explore_common_app/components/query/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3755 2024-03-12 18:58:51.000000 core_explore_common_app-2.8.0/core_explore_common_app/components/query/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1335 2024-03-12 18:58:51.000000 core_explore_common_app-2.8.0/core_explore_common_app/components/query/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:57.221826 core_explore_common_app-2.8.0/core_explore_common_app/components/result/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:51.000000 core_explore_common_app-2.8.0/core_explore_common_app/components/result/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      632 2024-03-12 18:58:51.000000 core_explore_common_app-2.8.0/core_explore_common_app/components/result/models.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      172 2024-03-12 18:58:51.000000 core_explore_common_app-2.8.0/core_explore_common_app/constants.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      876 2024-03-12 18:58:51.000000 core_explore_common_app-2.8.0/core_explore_common_app/discover.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:57.322901 core_explore_common_app-2.8.0/core_explore_common_app/migrations/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2499 2024-03-12 18:58:51.000000 core_explore_common_app-2.8.0/core_explore_common_app/migrations/0001_initial.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      416 2024-03-12 18:58:51.000000 core_explore_common_app-2.8.0/core_explore_common_app/migrations/0002_result_blob_url.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      383 2024-03-12 18:58:51.000000 core_explore_common_app-2.8.0/core_explore_common_app/migrations/0003_rename_xml_content_result_content.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:51.000000 core_explore_common_app-2.8.0/core_explore_common_app/migrations/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:57.369724 core_explore_common_app-2.8.0/core_explore_common_app/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:51.000000 core_explore_common_app-2.8.0/core_explore_common_app/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:57.410818 core_explore_common_app-2.8.0/core_explore_common_app/rest/query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:51.000000 core_explore_common_app-2.8.0/core_explore_common_app/rest/query/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5910 2024-03-12 18:58:51.000000 core_explore_common_app-2.8.0/core_explore_common_app/rest/query/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:57.472312 core_explore_common_app-2.8.0/core_explore_common_app/rest/result/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:51.000000 core_explore_common_app-2.8.0/core_explore_common_app/rest/result/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      481 2024-03-12 18:58:51.000000 core_explore_common_app-2.8.0/core_explore_common_app/rest/result/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1760 2024-03-12 18:58:51.000000 core_explore_common_app-2.8.0/core_explore_common_app/rest/result/views.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      308 2024-03-12 18:58:51.000000 core_explore_common_app-2.8.0/core_explore_common_app/rest/urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2200 2024-03-12 18:58:51.000000 core_explore_common_app-2.8.0/core_explore_common_app/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:56.253608 core_explore_common_app-2.8.0/core_explore_common_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:56.268584 core_explore_common_app-2.8.0/core_explore_common_app/static/core_explore_common_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:56.261573 core_explore_common_app-2.8.0/core_explore_common_app/static/core_explore_common_app/common/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:57.504805 core_explore_common_app-2.8.0/core_explore_common_app/static/core_explore_common_app/common/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      734 2024-03-12 18:58:51.000000 core_explore_common_app-2.8.0/core_explore_common_app/static/core_explore_common_app/common/js/tools.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:56.278383 core_explore_common_app-2.8.0/core_explore_common_app/static/core_explore_common_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:57.563475 core_explore_common_app-2.8.0/core_explore_common_app/static/core_explore_common_app/user/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      126 2024-03-12 18:58:51.000000 core_explore_common_app-2.8.0/core_explore_common_app/static/core_explore_common_app/user/css/query_result.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2311 2024-03-12 18:58:51.000000 core_explore_common_app-2.8.0/core_explore_common_app/static/core_explore_common_app/user/css/results.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3484 2024-03-12 18:58:51.000000 core_explore_common_app-2.8.0/core_explore_common_app/static/core_explore_common_app/user/css/toggle.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:57.678288 core_explore_common_app-2.8.0/core_explore_common_app/static/core_explore_common_app/user/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1629 2024-03-12 18:58:51.000000 core_explore_common_app-2.8.0/core_explore_common_app/static/core_explore_common_app/user/js/local_selector.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2616 2024-03-12 18:58:51.000000 core_explore_common_app-2.8.0/core_explore_common_app/static/core_explore_common_app/user/js/persistent_query_config.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9831 2024-03-12 18:58:51.000000 core_explore_common_app-2.8.0/core_explore_common_app/static/core_explore_common_app/user/js/results.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      557 2024-03-12 18:58:51.000000 core_explore_common_app-2.8.0/core_explore_common_app/static/core_explore_common_app/user/js/results.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7244 2024-03-12 18:58:51.000000 core_explore_common_app-2.8.0/core_explore_common_app/static/core_explore_common_app/user/js/sorting_multi_criteria.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5507 2024-03-12 18:58:51.000000 core_explore_common_app-2.8.0/core_explore_common_app/static/core_explore_common_app/user/js/sorting_single_criteria.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:57.718698 core_explore_common_app-2.8.0/core_explore_common_app/system/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:51.000000 core_explore_common_app-2.8.0/core_explore_common_app/system/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      190 2024-03-12 18:58:51.000000 core_explore_common_app-2.8.0/core_explore_common_app/system/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1049 2024-03-12 18:58:51.000000 core_explore_common_app-2.8.0/core_explore_common_app/tasks.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:56.298170 core_explore_common_app-2.8.0/core_explore_common_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:56.318318 core_explore_common_app-2.8.0/core_explore_common_app/templates/core_explore_common_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:56.305699 core_explore_common_app-2.8.0/core_explore_common_app/templates/core_explore_common_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:57.767797 core_explore_common_app-2.8.0/core_explore_common_app/templates/core_explore_common_app/admin/persistent_query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      300 2024-03-12 18:58:51.000000 core_explore_common_app-2.8.0/core_explore_common_app/templates/core_explore_common_app/admin/persistent_query/content_query_box.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      342 2024-03-12 18:58:51.000000 core_explore_common_app-2.8.0/core_explore_common_app/templates/core_explore_common_app/admin/persistent_query/view_query_content.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:57.788725 core_explore_common_app-2.8.0/core_explore_common_app/templates/core_explore_common_app/commons/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      463 2024-03-12 18:58:51.000000 core_explore_common_app-2.8.0/core_explore_common_app/templates/core_explore_common_app/commons/query_content.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:56.378959 core_explore_common_app-2.8.0/core_explore_common_app/templates/core_explore_common_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:57.828987 core_explore_common_app-2.8.0/core_explore_common_app/templates/core_explore_common_app/user/ordering_menu/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      697 2024-03-12 18:58:51.000000 core_explore_common_app-2.8.0/core_explore_common_app/templates/core_explore_common_app/user/ordering_menu/multi_criteria_sorting_menu.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      821 2024-03-12 18:58:52.000000 core_explore_common_app-2.8.0/core_explore_common_app/templates/core_explore_common_app/user/ordering_menu/single_criteria_sorting_menu.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:57.903914 core_explore_common_app-2.8.0/core_explore_common_app/templates/core_explore_common_app/user/persistent_query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      429 2024-03-12 18:58:52.000000 core_explore_common_app-2.8.0/core_explore_common_app/templates/core_explore_common_app/user/persistent_query/button.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      914 2024-03-12 18:58:52.000000 core_explore_common_app-2.8.0/core_explore_common_app/templates/core_explore_common_app/user/persistent_query/modal.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      317 2024-03-12 18:58:52.000000 core_explore_common_app-2.8.0/core_explore_common_app/templates/core_explore_common_app/user/persistent_query/persistent_query_content.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3163 2024-03-12 18:58:52.000000 core_explore_common_app-2.8.0/core_explore_common_app/templates/core_explore_common_app/user/persistent_query/persistent_query_pagination.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:58.014048 core_explore_common_app-2.8.0/core_explore_common_app/templates/core_explore_common_app/user/results/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2505 2024-03-12 18:58:52.000000 core_explore_common_app-2.8.0/core_explore_common_app/templates/core_explore_common_app/user/results/data_source_info.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1266 2024-03-12 18:58:52.000000 core_explore_common_app-2.8.0/core_explore_common_app/templates/core_explore_common_app/user/results/data_source_pagination.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      884 2024-03-12 18:58:52.000000 core_explore_common_app-2.8.0/core_explore_common_app/templates/core_explore_common_app/user/results/data_source_results.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3115 2024-03-12 18:58:52.000000 core_explore_common_app-2.8.0/core_explore_common_app/templates/core_explore_common_app/user/results/data_sources_results.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       92 2024-03-12 18:58:52.000000 core_explore_common_app-2.8.0/core_explore_common_app/templates/core_explore_common_app/user/results/results.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:58.085676 core_explore_common_app-2.8.0/core_explore_common_app/templates/core_explore_common_app/user/selector/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      784 2024-03-12 18:58:52.000000 core_explore_common_app-2.8.0/core_explore_common_app/templates/core_explore_common_app/user/selector/data_sources_selector.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      324 2024-03-12 18:58:52.000000 core_explore_common_app-2.8.0/core_explore_common_app/templates/core_explore_common_app/user/selector/list_selector_base.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      311 2024-03-12 18:58:52.000000 core_explore_common_app-2.8.0/core_explore_common_app/templates/core_explore_common_app/user/selector/local_content.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      723 2024-03-12 18:58:52.000000 core_explore_common_app-2.8.0/core_explore_common_app/templates/core_explore_common_app/user/selector/local_selector.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1361 2024-03-12 18:58:52.000000 core_explore_common_app-2.8.0/core_explore_common_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:58.105153 core_explore_common_app-2.8.0/core_explore_common_app/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:52.000000 core_explore_common_app-2.8.0/core_explore_common_app/utils/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:58.278893 core_explore_common_app-2.8.0/core_explore_common_app/utils/linked_records/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:52.000000 core_explore_common_app-2.8.0/core_explore_common_app/utils/linked_records/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1386 2024-03-12 18:58:52.000000 core_explore_common_app-2.8.0/core_explore_common_app/utils/linked_records/pid.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:58.320261 core_explore_common_app-2.8.0/core_explore_common_app/utils/oaipmh/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:52.000000 core_explore_common_app-2.8.0/core_explore_common_app/utils/oaipmh/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      597 2024-03-12 18:58:52.000000 core_explore_common_app-2.8.0/core_explore_common_app/utils/oaipmh/oaipmh.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:58.380557 core_explore_common_app-2.8.0/core_explore_common_app/utils/protocols/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:52.000000 core_explore_common_app-2.8.0/core_explore_common_app/utils/protocols/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      263 2024-03-12 18:58:52.000000 core_explore_common_app-2.8.0/core_explore_common_app/utils/protocols/commons.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3055 2024-03-12 18:58:52.000000 core_explore_common_app-2.8.0/core_explore_common_app/utils/protocols/oauth2.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:58.424682 core_explore_common_app-2.8.0/core_explore_common_app/utils/query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:52.000000 core_explore_common_app-2.8.0/core_explore_common_app/utils/query/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3361 2024-03-12 18:58:52.000000 core_explore_common_app-2.8.0/core_explore_common_app/utils/query/query.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:58.481177 core_explore_common_app-2.8.0/core_explore_common_app/utils/result/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:52.000000 core_explore_common_app-2.8.0/core_explore_common_app/utils/result/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1404 2024-03-12 18:58:52.000000 core_explore_common_app-2.8.0/core_explore_common_app/utils/result/result.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:58.505343 core_explore_common_app-2.8.0/core_explore_common_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:52.000000 core_explore_common_app-2.8.0/core_explore_common_app/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:58.578781 core_explore_common_app-2.8.0/core_explore_common_app/views/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:52.000000 core_explore_common_app-2.8.0/core_explore_common_app/views/user/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14618 2024-03-12 18:58:52.000000 core_explore_common_app-2.8.0/core_explore_common_app/views/user/ajax.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8610 2024-03-12 18:58:52.000000 core_explore_common_app-2.8.0/core_explore_common_app/views/user/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:56.856969 core_explore_common_app-2.8.0/core_explore_common_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1108 2024-03-12 18:58:55.000000 core_explore_common_app-2.8.0/core_explore_common_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6155 2024-03-12 18:58:56.000000 core_explore_common_app-2.8.0/core_explore_common_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2024-03-12 18:58:55.000000 core_explore_common_app-2.8.0/core_explore_common_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       69 2024-03-12 18:58:55.000000 core_explore_common_app-2.8.0/core_explore_common_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       30 2024-03-12 18:58:55.000000 core_explore_common_app-2.8.0/core_explore_common_app.egg-info/top_level.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2024-03-12 18:58:53.000000 core_explore_common_app-2.8.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       21 2024-03-12 18:58:53.000000 core_explore_common_app-2.8.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2024-03-12 18:58:59.130130 core_explore_common_app-2.8.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1479 2024-03-12 18:58:53.000000 core_explore_common_app-2.8.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:58.641390 core_explore_common_app-2.8.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:53.000000 core_explore_common_app-2.8.0/tests/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:58.662957 core_explore_common_app-2.8.0/tests/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:53.000000 core_explore_common_app-2.8.0/tests/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:58.687289 core_explore_common_app-2.8.0/tests/components/abstract_persistent_query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:53.000000 core_explore_common_app-2.8.0/tests/components/abstract_persistent_query/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:58.732544 core_explore_common_app-2.8.0/tests/components/query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:53.000000 core_explore_common_app-2.8.0/tests/components/query/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7526 2024-03-12 18:58:53.000000 core_explore_common_app-2.8.0/tests/components/query/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:58.752922 core_explore_common_app-2.8.0/tests/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:53.000000 core_explore_common_app-2.8.0/tests/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:58.776937 core_explore_common_app-2.8.0/tests/rest/query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:53.000000 core_explore_common_app-2.8.0/tests/rest/query/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:58.831845 core_explore_common_app-2.8.0/tests/rest/query/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:53.000000 core_explore_common_app-2.8.0/tests/rest/query/views/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6758 2024-03-12 18:58:53.000000 core_explore_common_app-2.8.0/tests/rest/query/views/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:58.897948 core_explore_common_app-2.8.0/tests/rest/result/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:53.000000 core_explore_common_app-2.8.0/tests/rest/result/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2544 2024-03-12 18:58:53.000000 core_explore_common_app-2.8.0/tests/rest/result/tests_permissions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       47 2024-03-12 18:58:53.000000 core_explore_common_app-2.8.0/tests/rest/result/tests_unit.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1808 2024-03-12 18:58:53.000000 core_explore_common_app-2.8.0/tests/test_settings.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      854 2024-03-12 18:58:53.000000 core_explore_common_app-2.8.0/tests/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:58.919756 core_explore_common_app-2.8.0/tests/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:53.000000 core_explore_common_app-2.8.0/tests/utils/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:58.968275 core_explore_common_app-2.8.0/tests/utils/linked_records/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:53.000000 core_explore_common_app-2.8.0/tests/utils/linked_records/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4666 2024-03-12 18:58:53.000000 core_explore_common_app-2.8.0/tests/utils/linked_records/tests_pid.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:59.012324 core_explore_common_app-2.8.0/tests/utils/oaipmh/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:53.000000 core_explore_common_app-2.8.0/tests/utils/oaipmh/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1860 2024-03-12 18:58:53.000000 core_explore_common_app-2.8.0/tests/utils/oaipmh/tests_oaipmh.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:59.056136 core_explore_common_app-2.8.0/tests/utils/query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:53.000000 core_explore_common_app-2.8.0/tests/utils/query/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2990 2024-03-12 18:58:53.000000 core_explore_common_app-2.8.0/tests/utils/query/tests_query.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:59.101459 core_explore_common_app-2.8.0/tests/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:58:53.000000 core_explore_common_app-2.8.0/tests/views/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    20193 2024-03-12 18:58:53.000000 core_explore_common_app-2.8.0/tests/views/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:33.043530 core_explore_common_app-2.9.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2024-05-13 16:04:22.000000 core_explore_common_app-2.9.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      154 2024-05-13 16:04:22.000000 core_explore_common_app-2.9.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1108 2024-05-13 16:04:33.037224 core_explore_common_app-2.9.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      607 2024-05-13 16:04:22.000000 core_explore_common_app-2.9.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:30.017447 core_explore_common_app-2.9.0/core_explore_common_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       79 2024-05-13 16:04:23.000000 core_explore_common_app-2.9.0/core_explore_common_app/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:30.230519 core_explore_common_app-2.9.0/core_explore_common_app/access_control/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:23.000000 core_explore_common_app-2.9.0/core_explore_common_app/access_control/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4732 2024-05-13 16:04:23.000000 core_explore_common_app-2.9.0/core_explore_common_app/access_control/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      282 2024-05-13 16:04:23.000000 core_explore_common_app-2.9.0/core_explore_common_app/admin.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      450 2024-05-13 16:04:23.000000 core_explore_common_app-2.9.0/core_explore_common_app/apps.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:30.273645 core_explore_common_app-2.9.0/core_explore_common_app/commons/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:23.000000 core_explore_common_app-2.9.0/core_explore_common_app/commons/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      409 2024-05-13 16:04:23.000000 core_explore_common_app-2.9.0/core_explore_common_app/commons/exceptions.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:30.294641 core_explore_common_app-2.9.0/core_explore_common_app/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:23.000000 core_explore_common_app-2.9.0/core_explore_common_app/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:30.356322 core_explore_common_app-2.9.0/core_explore_common_app/components/abstract_persistent_query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:23.000000 core_explore_common_app-2.9.0/core_explore_common_app/components/abstract_persistent_query/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2123 2024-05-13 16:04:23.000000 core_explore_common_app-2.9.0/core_explore_common_app/components/abstract_persistent_query/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      552 2024-05-13 16:04:23.000000 core_explore_common_app-2.9.0/core_explore_common_app/components/abstract_persistent_query/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:30.398635 core_explore_common_app-2.9.0/core_explore_common_app/components/abstract_query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:23.000000 core_explore_common_app-2.9.0/core_explore_common_app/components/abstract_query/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1616 2024-05-13 16:04:23.000000 core_explore_common_app-2.9.0/core_explore_common_app/components/abstract_query/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:30.475912 core_explore_common_app-2.9.0/core_explore_common_app/components/query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:23.000000 core_explore_common_app-2.9.0/core_explore_common_app/components/query/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      372 2024-05-13 16:04:23.000000 core_explore_common_app-2.9.0/core_explore_common_app/components/query/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3755 2024-05-13 16:04:23.000000 core_explore_common_app-2.9.0/core_explore_common_app/components/query/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1335 2024-05-13 16:04:23.000000 core_explore_common_app-2.9.0/core_explore_common_app/components/query/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:30.518265 core_explore_common_app-2.9.0/core_explore_common_app/components/result/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:23.000000 core_explore_common_app-2.9.0/core_explore_common_app/components/result/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      632 2024-05-13 16:04:23.000000 core_explore_common_app-2.9.0/core_explore_common_app/components/result/models.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      172 2024-05-13 16:04:23.000000 core_explore_common_app-2.9.0/core_explore_common_app/constants.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      876 2024-05-13 16:04:23.000000 core_explore_common_app-2.9.0/core_explore_common_app/discover.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:30.618177 core_explore_common_app-2.9.0/core_explore_common_app/migrations/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2499 2024-05-13 16:04:23.000000 core_explore_common_app-2.9.0/core_explore_common_app/migrations/0001_initial.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      416 2024-05-13 16:04:23.000000 core_explore_common_app-2.9.0/core_explore_common_app/migrations/0002_result_blob_url.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      383 2024-05-13 16:04:23.000000 core_explore_common_app-2.9.0/core_explore_common_app/migrations/0003_rename_xml_content_result_content.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:23.000000 core_explore_common_app-2.9.0/core_explore_common_app/migrations/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:30.664548 core_explore_common_app-2.9.0/core_explore_common_app/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:23.000000 core_explore_common_app-2.9.0/core_explore_common_app/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:30.724300 core_explore_common_app-2.9.0/core_explore_common_app/rest/query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:23.000000 core_explore_common_app-2.9.0/core_explore_common_app/rest/query/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5910 2024-05-13 16:04:23.000000 core_explore_common_app-2.9.0/core_explore_common_app/rest/query/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:30.781176 core_explore_common_app-2.9.0/core_explore_common_app/rest/result/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:23.000000 core_explore_common_app-2.9.0/core_explore_common_app/rest/result/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      481 2024-05-13 16:04:23.000000 core_explore_common_app-2.9.0/core_explore_common_app/rest/result/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1760 2024-05-13 16:04:23.000000 core_explore_common_app-2.9.0/core_explore_common_app/rest/result/views.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      308 2024-05-13 16:04:23.000000 core_explore_common_app-2.9.0/core_explore_common_app/rest/urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2200 2024-05-13 16:04:23.000000 core_explore_common_app-2.9.0/core_explore_common_app/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:29.332451 core_explore_common_app-2.9.0/core_explore_common_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:29.370306 core_explore_common_app-2.9.0/core_explore_common_app/static/core_explore_common_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:29.362528 core_explore_common_app-2.9.0/core_explore_common_app/static/core_explore_common_app/common/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:30.842648 core_explore_common_app-2.9.0/core_explore_common_app/static/core_explore_common_app/common/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      734 2024-05-13 16:04:23.000000 core_explore_common_app-2.9.0/core_explore_common_app/static/core_explore_common_app/common/js/tools.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:29.380616 core_explore_common_app-2.9.0/core_explore_common_app/static/core_explore_common_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:30.896963 core_explore_common_app-2.9.0/core_explore_common_app/static/core_explore_common_app/user/css/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      126 2024-05-13 16:04:23.000000 core_explore_common_app-2.9.0/core_explore_common_app/static/core_explore_common_app/user/css/query_result.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2311 2024-05-13 16:04:23.000000 core_explore_common_app-2.9.0/core_explore_common_app/static/core_explore_common_app/user/css/results.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3484 2024-05-13 16:04:23.000000 core_explore_common_app-2.9.0/core_explore_common_app/static/core_explore_common_app/user/css/toggle.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:31.050792 core_explore_common_app-2.9.0/core_explore_common_app/static/core_explore_common_app/user/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1629 2024-05-13 16:04:23.000000 core_explore_common_app-2.9.0/core_explore_common_app/static/core_explore_common_app/user/js/local_selector.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2616 2024-05-13 16:04:23.000000 core_explore_common_app-2.9.0/core_explore_common_app/static/core_explore_common_app/user/js/persistent_query_config.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9831 2024-05-13 16:04:24.000000 core_explore_common_app-2.9.0/core_explore_common_app/static/core_explore_common_app/user/js/results.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      557 2024-05-13 16:04:24.000000 core_explore_common_app-2.9.0/core_explore_common_app/static/core_explore_common_app/user/js/results.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7244 2024-05-13 16:04:24.000000 core_explore_common_app-2.9.0/core_explore_common_app/static/core_explore_common_app/user/js/sorting_multi_criteria.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5507 2024-05-13 16:04:24.000000 core_explore_common_app-2.9.0/core_explore_common_app/static/core_explore_common_app/user/js/sorting_single_criteria.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:31.077080 core_explore_common_app-2.9.0/core_explore_common_app/system/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:24.000000 core_explore_common_app-2.9.0/core_explore_common_app/system/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      190 2024-05-13 16:04:24.000000 core_explore_common_app-2.9.0/core_explore_common_app/system/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1049 2024-05-13 16:04:24.000000 core_explore_common_app-2.9.0/core_explore_common_app/tasks.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:29.402713 core_explore_common_app-2.9.0/core_explore_common_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:29.444839 core_explore_common_app-2.9.0/core_explore_common_app/templates/core_explore_common_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:29.410769 core_explore_common_app-2.9.0/core_explore_common_app/templates/core_explore_common_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:31.123914 core_explore_common_app-2.9.0/core_explore_common_app/templates/core_explore_common_app/admin/persistent_query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      300 2024-05-13 16:04:24.000000 core_explore_common_app-2.9.0/core_explore_common_app/templates/core_explore_common_app/admin/persistent_query/content_query_box.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      342 2024-05-13 16:04:24.000000 core_explore_common_app-2.9.0/core_explore_common_app/templates/core_explore_common_app/admin/persistent_query/view_query_content.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:31.169288 core_explore_common_app-2.9.0/core_explore_common_app/templates/core_explore_common_app/commons/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      463 2024-05-13 16:04:24.000000 core_explore_common_app-2.9.0/core_explore_common_app/templates/core_explore_common_app/commons/query_content.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:29.493840 core_explore_common_app-2.9.0/core_explore_common_app/templates/core_explore_common_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:31.194991 core_explore_common_app-2.9.0/core_explore_common_app/templates/core_explore_common_app/user/ordering_menu/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      697 2024-05-13 16:04:24.000000 core_explore_common_app-2.9.0/core_explore_common_app/templates/core_explore_common_app/user/ordering_menu/multi_criteria_sorting_menu.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      821 2024-05-13 16:04:24.000000 core_explore_common_app-2.9.0/core_explore_common_app/templates/core_explore_common_app/user/ordering_menu/single_criteria_sorting_menu.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:31.270048 core_explore_common_app-2.9.0/core_explore_common_app/templates/core_explore_common_app/user/persistent_query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      429 2024-05-13 16:04:24.000000 core_explore_common_app-2.9.0/core_explore_common_app/templates/core_explore_common_app/user/persistent_query/button.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      914 2024-05-13 16:04:24.000000 core_explore_common_app-2.9.0/core_explore_common_app/templates/core_explore_common_app/user/persistent_query/modal.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      317 2024-05-13 16:04:24.000000 core_explore_common_app-2.9.0/core_explore_common_app/templates/core_explore_common_app/user/persistent_query/persistent_query_content.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3163 2024-05-13 16:04:24.000000 core_explore_common_app-2.9.0/core_explore_common_app/templates/core_explore_common_app/user/persistent_query/persistent_query_pagination.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:31.364274 core_explore_common_app-2.9.0/core_explore_common_app/templates/core_explore_common_app/user/results/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2505 2024-05-13 16:04:24.000000 core_explore_common_app-2.9.0/core_explore_common_app/templates/core_explore_common_app/user/results/data_source_info.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1266 2024-05-13 16:04:24.000000 core_explore_common_app-2.9.0/core_explore_common_app/templates/core_explore_common_app/user/results/data_source_pagination.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      884 2024-05-13 16:04:24.000000 core_explore_common_app-2.9.0/core_explore_common_app/templates/core_explore_common_app/user/results/data_source_results.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3115 2024-05-13 16:04:24.000000 core_explore_common_app-2.9.0/core_explore_common_app/templates/core_explore_common_app/user/results/data_sources_results.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       92 2024-05-13 16:04:24.000000 core_explore_common_app-2.9.0/core_explore_common_app/templates/core_explore_common_app/user/results/results.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:31.460142 core_explore_common_app-2.9.0/core_explore_common_app/templates/core_explore_common_app/user/selector/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      784 2024-05-13 16:04:24.000000 core_explore_common_app-2.9.0/core_explore_common_app/templates/core_explore_common_app/user/selector/data_sources_selector.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      324 2024-05-13 16:04:24.000000 core_explore_common_app-2.9.0/core_explore_common_app/templates/core_explore_common_app/user/selector/list_selector_base.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      311 2024-05-13 16:04:24.000000 core_explore_common_app-2.9.0/core_explore_common_app/templates/core_explore_common_app/user/selector/local_content.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      723 2024-05-13 16:04:24.000000 core_explore_common_app-2.9.0/core_explore_common_app/templates/core_explore_common_app/user/selector/local_selector.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1361 2024-05-13 16:04:24.000000 core_explore_common_app-2.9.0/core_explore_common_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:31.481284 core_explore_common_app-2.9.0/core_explore_common_app/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:24.000000 core_explore_common_app-2.9.0/core_explore_common_app/utils/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:31.561227 core_explore_common_app-2.9.0/core_explore_common_app/utils/linked_records/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:24.000000 core_explore_common_app-2.9.0/core_explore_common_app/utils/linked_records/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1386 2024-05-13 16:04:24.000000 core_explore_common_app-2.9.0/core_explore_common_app/utils/linked_records/pid.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:31.634679 core_explore_common_app-2.9.0/core_explore_common_app/utils/oaipmh/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:24.000000 core_explore_common_app-2.9.0/core_explore_common_app/utils/oaipmh/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      597 2024-05-13 16:04:24.000000 core_explore_common_app-2.9.0/core_explore_common_app/utils/oaipmh/oaipmh.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:31.702689 core_explore_common_app-2.9.0/core_explore_common_app/utils/protocols/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:24.000000 core_explore_common_app-2.9.0/core_explore_common_app/utils/protocols/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      263 2024-05-13 16:04:24.000000 core_explore_common_app-2.9.0/core_explore_common_app/utils/protocols/commons.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3055 2024-05-13 16:04:24.000000 core_explore_common_app-2.9.0/core_explore_common_app/utils/protocols/oauth2.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:31.742718 core_explore_common_app-2.9.0/core_explore_common_app/utils/query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:24.000000 core_explore_common_app-2.9.0/core_explore_common_app/utils/query/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3361 2024-05-13 16:04:24.000000 core_explore_common_app-2.9.0/core_explore_common_app/utils/query/query.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:31.783079 core_explore_common_app-2.9.0/core_explore_common_app/utils/result/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:24.000000 core_explore_common_app-2.9.0/core_explore_common_app/utils/result/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1404 2024-05-13 16:04:24.000000 core_explore_common_app-2.9.0/core_explore_common_app/utils/result/result.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:31.802742 core_explore_common_app-2.9.0/core_explore_common_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:24.000000 core_explore_common_app-2.9.0/core_explore_common_app/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:32.321019 core_explore_common_app-2.9.0/core_explore_common_app/views/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:24.000000 core_explore_common_app-2.9.0/core_explore_common_app/views/user/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14927 2024-05-13 16:04:24.000000 core_explore_common_app-2.9.0/core_explore_common_app/views/user/ajax.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8610 2024-05-13 16:04:24.000000 core_explore_common_app-2.9.0/core_explore_common_app/views/user/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:30.188514 core_explore_common_app-2.9.0/core_explore_common_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1108 2024-05-13 16:04:28.000000 core_explore_common_app-2.9.0/core_explore_common_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6155 2024-05-13 16:04:29.000000 core_explore_common_app-2.9.0/core_explore_common_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2024-05-13 16:04:28.000000 core_explore_common_app-2.9.0/core_explore_common_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       69 2024-05-13 16:04:28.000000 core_explore_common_app-2.9.0/core_explore_common_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       30 2024-05-13 16:04:28.000000 core_explore_common_app-2.9.0/core_explore_common_app.egg-info/top_level.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2024-05-13 16:04:25.000000 core_explore_common_app-2.9.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       21 2024-05-13 16:04:25.000000 core_explore_common_app-2.9.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2024-05-13 16:04:33.071707 core_explore_common_app-2.9.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1479 2024-05-13 16:04:25.000000 core_explore_common_app-2.9.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:32.449926 core_explore_common_app-2.9.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:25.000000 core_explore_common_app-2.9.0/tests/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:32.471974 core_explore_common_app-2.9.0/tests/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:25.000000 core_explore_common_app-2.9.0/tests/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:32.498363 core_explore_common_app-2.9.0/tests/components/abstract_persistent_query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:25.000000 core_explore_common_app-2.9.0/tests/components/abstract_persistent_query/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:32.564708 core_explore_common_app-2.9.0/tests/components/query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:25.000000 core_explore_common_app-2.9.0/tests/components/query/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7526 2024-05-13 16:04:26.000000 core_explore_common_app-2.9.0/tests/components/query/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:32.583974 core_explore_common_app-2.9.0/tests/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:26.000000 core_explore_common_app-2.9.0/tests/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:32.607014 core_explore_common_app-2.9.0/tests/rest/query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:26.000000 core_explore_common_app-2.9.0/tests/rest/query/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:32.652326 core_explore_common_app-2.9.0/tests/rest/query/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:26.000000 core_explore_common_app-2.9.0/tests/rest/query/views/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6758 2024-05-13 16:04:26.000000 core_explore_common_app-2.9.0/tests/rest/query/views/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:32.711356 core_explore_common_app-2.9.0/tests/rest/result/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:26.000000 core_explore_common_app-2.9.0/tests/rest/result/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2544 2024-05-13 16:04:26.000000 core_explore_common_app-2.9.0/tests/rest/result/tests_permissions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       47 2024-05-13 16:04:26.000000 core_explore_common_app-2.9.0/tests/rest/result/tests_unit.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1808 2024-05-13 16:04:26.000000 core_explore_common_app-2.9.0/tests/test_settings.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      854 2024-05-13 16:04:26.000000 core_explore_common_app-2.9.0/tests/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:32.766113 core_explore_common_app-2.9.0/tests/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:26.000000 core_explore_common_app-2.9.0/tests/utils/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:32.839949 core_explore_common_app-2.9.0/tests/utils/linked_records/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:26.000000 core_explore_common_app-2.9.0/tests/utils/linked_records/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4666 2024-05-13 16:04:26.000000 core_explore_common_app-2.9.0/tests/utils/linked_records/tests_pid.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:32.882689 core_explore_common_app-2.9.0/tests/utils/oaipmh/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:26.000000 core_explore_common_app-2.9.0/tests/utils/oaipmh/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1860 2024-05-13 16:04:26.000000 core_explore_common_app-2.9.0/tests/utils/oaipmh/tests_oaipmh.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:32.951214 core_explore_common_app-2.9.0/tests/utils/query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:26.000000 core_explore_common_app-2.9.0/tests/utils/query/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2990 2024-05-13 16:04:26.000000 core_explore_common_app-2.9.0/tests/utils/query/tests_query.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:33.016008 core_explore_common_app-2.9.0/tests/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:04:26.000000 core_explore_common_app-2.9.0/tests/views/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    25171 2024-05-13 16:04:26.000000 core_explore_common_app-2.9.0/tests/views/test_unit.py
```

### Comparing `core_explore_common_app-2.8.0/LICENSE.md` & `core_explore_common_app-2.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.8.0/PKG-INFO` & `core_explore_common_app-2.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_explore_common_app
-Version: 2.8.0
+Version: 2.9.0
 Summary: Base exploration function for the curator core project
 Home-page: https://github.com/usnistgov/core_explore_common_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: =======================
         Core Explore Common App
```

### Comparing `core_explore_common_app-2.8.0/README.rst` & `core_explore_common_app-2.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.8.0/core_explore_common_app/access_control/api.py` & `core_explore_common_app-2.9.0/core_explore_common_app/access_control/api.py`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.8.0/core_explore_common_app/components/abstract_persistent_query/api.py` & `core_explore_common_app-2.9.0/core_explore_common_app/components/abstract_persistent_query/api.py`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.8.0/core_explore_common_app/components/abstract_persistent_query/models.py` & `core_explore_common_app-2.9.0/core_explore_common_app/components/abstract_persistent_query/models.py`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.8.0/core_explore_common_app/components/abstract_query/models.py` & `core_explore_common_app-2.9.0/core_explore_common_app/components/abstract_query/models.py`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.8.0/core_explore_common_app/components/query/api.py` & `core_explore_common_app-2.9.0/core_explore_common_app/components/query/api.py`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.8.0/core_explore_common_app/components/query/models.py` & `core_explore_common_app-2.9.0/core_explore_common_app/components/query/models.py`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.8.0/core_explore_common_app/components/result/models.py` & `core_explore_common_app-2.9.0/core_explore_common_app/components/result/models.py`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.8.0/core_explore_common_app/discover.py` & `core_explore_common_app-2.9.0/core_explore_common_app/discover.py`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.8.0/core_explore_common_app/migrations/0001_initial.py` & `core_explore_common_app-2.9.0/core_explore_common_app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.8.0/core_explore_common_app/rest/query/views.py` & `core_explore_common_app-2.9.0/core_explore_common_app/rest/query/views.py`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.8.0/core_explore_common_app/rest/result/views.py` & `core_explore_common_app-2.9.0/core_explore_common_app/rest/result/views.py`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.8.0/core_explore_common_app/settings.py` & `core_explore_common_app-2.9.0/core_explore_common_app/settings.py`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.8.0/core_explore_common_app/static/core_explore_common_app/common/js/tools.js` & `core_explore_common_app-2.9.0/core_explore_common_app/static/core_explore_common_app/common/js/tools.js`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.8.0/core_explore_common_app/static/core_explore_common_app/user/css/results.css` & `core_explore_common_app-2.9.0/core_explore_common_app/static/core_explore_common_app/user/css/results.css`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.8.0/core_explore_common_app/static/core_explore_common_app/user/css/toggle.css` & `core_explore_common_app-2.9.0/core_explore_common_app/static/core_explore_common_app/user/css/toggle.css`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.8.0/core_explore_common_app/static/core_explore_common_app/user/js/local_selector.js` & `core_explore_common_app-2.9.0/core_explore_common_app/static/core_explore_common_app/user/js/local_selector.js`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.8.0/core_explore_common_app/static/core_explore_common_app/user/js/persistent_query_config.js` & `core_explore_common_app-2.9.0/core_explore_common_app/static/core_explore_common_app/user/js/persistent_query_config.js`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.8.0/core_explore_common_app/static/core_explore_common_app/user/js/results.js` & `core_explore_common_app-2.9.0/core_explore_common_app/static/core_explore_common_app/user/js/results.js`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.8.0/core_explore_common_app/static/core_explore_common_app/user/js/results.raw.js` & `core_explore_common_app-2.9.0/core_explore_common_app/static/core_explore_common_app/user/js/results.raw.js`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.8.0/core_explore_common_app/static/core_explore_common_app/user/js/sorting_multi_criteria.js` & `core_explore_common_app-2.9.0/core_explore_common_app/static/core_explore_common_app/user/js/sorting_multi_criteria.js`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.8.0/core_explore_common_app/static/core_explore_common_app/user/js/sorting_single_criteria.js` & `core_explore_common_app-2.9.0/core_explore_common_app/static/core_explore_common_app/user/js/sorting_single_criteria.js`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.8.0/core_explore_common_app/tasks.py` & `core_explore_common_app-2.9.0/core_explore_common_app/tasks.py`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.8.0/core_explore_common_app/templates/core_explore_common_app/user/ordering_menu/multi_criteria_sorting_menu.html` & `core_explore_common_app-2.9.0/core_explore_common_app/templates/core_explore_common_app/user/ordering_menu/multi_criteria_sorting_menu.html`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.8.0/core_explore_common_app/templates/core_explore_common_app/user/ordering_menu/single_criteria_sorting_menu.html` & `core_explore_common_app-2.9.0/core_explore_common_app/templates/core_explore_common_app/user/ordering_menu/single_criteria_sorting_menu.html`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.8.0/core_explore_common_app/templates/core_explore_common_app/user/persistent_query/modal.html` & `core_explore_common_app-2.9.0/core_explore_common_app/templates/core_explore_common_app/user/persistent_query/modal.html`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.8.0/core_explore_common_app/templates/core_explore_common_app/user/persistent_query/persistent_query_pagination.html` & `core_explore_common_app-2.9.0/core_explore_common_app/templates/core_explore_common_app/user/persistent_query/persistent_query_pagination.html`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.8.0/core_explore_common_app/templates/core_explore_common_app/user/results/data_source_info.html` & `core_explore_common_app-2.9.0/core_explore_common_app/templates/core_explore_common_app/user/results/data_source_info.html`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.8.0/core_explore_common_app/templates/core_explore_common_app/user/results/data_source_pagination.html` & `core_explore_common_app-2.9.0/core_explore_common_app/templates/core_explore_common_app/user/results/data_source_pagination.html`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.8.0/core_explore_common_app/templates/core_explore_common_app/user/results/data_source_results.html` & `core_explore_common_app-2.9.0/core_explore_common_app/templates/core_explore_common_app/user/results/data_source_results.html`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.8.0/core_explore_common_app/templates/core_explore_common_app/user/results/data_sources_results.html` & `core_explore_common_app-2.9.0/core_explore_common_app/templates/core_explore_common_app/user/results/data_sources_results.html`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.8.0/core_explore_common_app/templates/core_explore_common_app/user/selector/data_sources_selector.html` & `core_explore_common_app-2.9.0/core_explore_common_app/templates/core_explore_common_app/user/selector/data_sources_selector.html`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.8.0/core_explore_common_app/templates/core_explore_common_app/user/selector/local_selector.html` & `core_explore_common_app-2.9.0/core_explore_common_app/templates/core_explore_common_app/user/selector/local_selector.html`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.8.0/core_explore_common_app/urls.py` & `core_explore_common_app-2.9.0/core_explore_common_app/urls.py`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.8.0/core_explore_common_app/utils/linked_records/pid.py` & `core_explore_common_app-2.9.0/core_explore_common_app/utils/linked_records/pid.py`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.8.0/core_explore_common_app/utils/oaipmh/oaipmh.py` & `core_explore_common_app-2.9.0/core_explore_common_app/utils/oaipmh/oaipmh.py`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.8.0/core_explore_common_app/utils/protocols/oauth2.py` & `core_explore_common_app-2.9.0/core_explore_common_app/utils/protocols/oauth2.py`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.8.0/core_explore_common_app/utils/query/query.py` & `core_explore_common_app-2.9.0/core_explore_common_app/utils/query/query.py`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.8.0/core_explore_common_app/utils/result/result.py` & `core_explore_common_app-2.9.0/core_explore_common_app/utils/result/result.py`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.8.0/core_explore_common_app/views/user/ajax.py` & `core_explore_common_app-2.9.0/core_explore_common_app/views/user/ajax.py`

 * *Files 1% similar despite different names*

```diff
@@ -234,14 +234,22 @@
             except EmptyPage:
                 next_page_number = None
 
             has_other_pages = results.has_other_pages()
             has_previous = results.has_previous()
             has_next = results.has_next()
         else:
+            # Check template hash
+            if any(
+                not template["hash"]
+                for template in json.loads(json_query["templates"])
+            ):
+                raise ExploreRequestError(
+                    "Some selected templates are missing the hash value."
+                )
             # send query, and get results from data source
             results = query_utils.send(request, json_query, data_source, page)
             data_list = results["results"]
 
             # get pagination information
             previous_page_number = get_page_number(results["previous"])
             next_page_number = get_page_number(results["next"])
```

### Comparing `core_explore_common_app-2.8.0/core_explore_common_app/views/user/views.py` & `core_explore_common_app-2.9.0/core_explore_common_app/views/user/views.py`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.8.0/core_explore_common_app.egg-info/PKG-INFO` & `core_explore_common_app-2.9.0/core_explore_common_app.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-explore-common-app
-Version: 2.8.0
+Version: 2.9.0
 Summary: Base exploration function for the curator core project
 Home-page: https://github.com/usnistgov/core_explore_common_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: =======================
         Core Explore Common App
```

### Comparing `core_explore_common_app-2.8.0/core_explore_common_app.egg-info/SOURCES.txt` & `core_explore_common_app-2.9.0/core_explore_common_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.8.0/setup.py` & `core_explore_common_app-2.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 chdir(normpath(join(abspath(__file__), pardir)))
 
 dep_links = [r for r in required if r.startswith("https://")]
 required = [req_link(r) if r.startswith("https://") else r for r in required]
 
 setup(
     name="core_explore_common_app",
-    version="2.8.0",
+    version="2.9.0",
     description="Base exploration function for the curator core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_explore_common_app",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `core_explore_common_app-2.8.0/tests/components/query/tests_unit.py` & `core_explore_common_app-2.9.0/tests/components/query/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.8.0/tests/rest/query/views/tests_unit.py` & `core_explore_common_app-2.9.0/tests/rest/query/views/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.8.0/tests/rest/result/tests_permissions.py` & `core_explore_common_app-2.9.0/tests/rest/result/tests_permissions.py`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.8.0/tests/test_settings.py` & `core_explore_common_app-2.9.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.8.0/tests/urls.py` & `core_explore_common_app-2.9.0/tests/urls.py`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.8.0/tests/utils/linked_records/tests_pid.py` & `core_explore_common_app-2.9.0/tests/utils/linked_records/tests_pid.py`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.8.0/tests/utils/oaipmh/tests_oaipmh.py` & `core_explore_common_app-2.9.0/tests/utils/oaipmh/tests_oaipmh.py`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.8.0/tests/utils/query/tests_query.py` & `core_explore_common_app-2.9.0/tests/utils/query/tests_query.py`

 * *Files identical despite different names*

### Comparing `core_explore_common_app-2.8.0/tests/views/test_unit.py` & `core_explore_common_app-2.9.0/tests/views/test_unit.py`

 * *Files 10% similar despite different names*

```diff
@@ -369,14 +369,158 @@
         response = get_data_source_results(
             request, query_id=1, data_source_index=0
         )
         self.assertTrue(response.status_code == 200)
         self.assertTrue(mock_get_by_id.called)
         self.assertTrue(mock_send_query.called)
 
+    @patch("core_explore_common_app.components.query.api.get_by_id")
+    @patch("core_explore_common_app.utils.query.query.serialize_query")
+    @patch("core_explore_common_app.utils.query.query.send")
+    def test_get_oauth2_data_source_results_filtered_by_template_with_hash(
+        self,
+        mock_send_query,
+        mock_serialize_query,
+        mock_get_by_id,
+    ):
+        """test_get_oauth2_data_source_results_filtered_by_template_with_hash
+
+        Returns:
+
+        """
+        request = self.factory.get("core_explore_common_get_local_data_source")
+        request.user = self.user1
+
+        mock_query = MagicMock()
+        mock_query.content = {}
+
+        mock_data_source = {
+            "name": LOCAL_QUERY_NAME,
+            "url_query": SERVER_URI,
+            "query_options": {},
+            "order_by_field": [],
+            "authentication": {"auth_type": "oauth2"},
+        }
+        mock_serialize_query.return_value = {
+            "query": "{}",
+            "templates": '[{"id": 3, "hash": "a12946eda99c065243a9c02632682928e12a32bd"}]',
+            "options": "{}",
+            "order_by_field": [],
+        }
+
+        mock_query.data_sources = [mock_data_source]
+        mock_get_by_id.return_value = mock_query
+
+        mock_send_query.return_value = {
+            "results": [],
+            "previous": None,
+            "next": None,
+            "count": 1,
+        }
+
+        response = get_data_source_results(
+            request, query_id=1, data_source_index=0
+        )
+        self.assertTrue(response.status_code == 200)
+        self.assertTrue(mock_get_by_id.called)
+        self.assertTrue(mock_serialize_query.called)
+        self.assertTrue(mock_send_query.called)
+
+    @patch("core_explore_common_app.components.query.api.get_by_id")
+    @patch("core_explore_common_app.utils.query.query.serialize_query")
+    def test_get_oauth2_data_source_results_filtered_by_template_without_hash_returns_error(
+        self,
+        mock_serialize_query,
+        mock_get_by_id,
+    ):
+        """test_get_oauth2_data_source_results_filtered_by_template_without_hash_returns_error
+
+        Returns:
+
+        """
+        request = self.factory.get("core_explore_common_get_local_data_source")
+        request.user = self.user1
+
+        mock_query = MagicMock()
+        mock_query.content = {}
+
+        mock_data_source = {
+            "name": LOCAL_QUERY_NAME,
+            "url_query": SERVER_URI,
+            "query_options": {},
+            "order_by_field": [],
+            "authentication": {"auth_type": "oauth2"},
+        }
+        mock_serialize_query.return_value = {
+            "query": "{}",
+            "templates": '[{"id": 3, "hash": null}]',
+            "options": "{}",
+            "order_by_field": [],
+        }
+
+        mock_query.data_sources = [mock_data_source]
+        mock_get_by_id.return_value = mock_query
+
+        response = get_data_source_results(
+            request, query_id=1, data_source_index=0
+        )
+        self.assertTrue(response.status_code == 400)
+        self.assertTrue(mock_get_by_id.called)
+        self.assertTrue(mock_serialize_query.called)
+        self.assertEquals(
+            b"An error occurred while sending the query: Some selected templates are missing the hash value.",
+            response.content,
+        )
+
+    @patch("core_explore_common_app.components.query.api.get_by_id")
+    @patch("core_explore_common_app.utils.query.query.serialize_query")
+    def test_get_oauth2_data_source_results_filtered_by_templates_returns_error_when_hash_missing(
+        self,
+        mock_serialize_query,
+        mock_get_by_id,
+    ):
+        """test_get_oauth2_data_source_results_filtered_by_templates_returns_error_when_hash_missing
+
+        Returns:
+
+        """
+        request = self.factory.get("core_explore_common_get_local_data_source")
+        request.user = self.user1
+
+        mock_query = MagicMock()
+        mock_query.content = {}
+
+        mock_data_source = {
+            "name": LOCAL_QUERY_NAME,
+            "url_query": SERVER_URI,
+            "query_options": {},
+            "order_by_field": [],
+            "authentication": {"auth_type": "oauth2"},
+        }
+        mock_serialize_query.return_value = {
+            "query": "{}",
+            "templates": '[{"id": 3, "hash": null},{"id": 2, "hash": "a12946eda99c065243a9c02632682928e12a32bd"}]',
+            "options": "{}",
+            "order_by_field": [],
+        }
+
+        mock_query.data_sources = [mock_data_source]
+        mock_get_by_id.return_value = mock_query
+
+        response = get_data_source_results(
+            request, query_id=1, data_source_index=0
+        )
+        self.assertTrue(response.status_code == 400)
+        self.assertTrue(mock_get_by_id.called)
+        self.assertTrue(mock_serialize_query.called)
+        self.assertEquals(
+            b"An error occurred while sending the query: Some selected templates are missing the hash value.",
+            response.content,
+        )
+
 
 class TestGetDataSourceHTML(SimpleTestCase):
     """TestGetDataSourceHTML"""
 
     def setUp(self):
         """setUp
```

