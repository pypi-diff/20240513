# Comparing `tmp/core_explore_keyword_app-2.8.0.tar.gz` & `tmp/core_explore_keyword_app-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_explore_keyword_app-2.8.0.tar", last modified: Tue Mar 12 18:59:54 2024, max compression
+gzip compressed data, was "core_explore_keyword_app-2.9.0.tar", last modified: Mon May 13 16:05:35 2024, max compression
```

## Comparing `core_explore_keyword_app-2.8.0.tar` & `core_explore_keyword_app-2.9.0.tar`

### file list

```diff
@@ -1,166 +1,166 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:54.289170 core_explore_keyword_app-2.8.0/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2024-03-12 18:59:46.000000 core_explore_keyword_app-2.8.0/LICENSE.md
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      156 2024-03-12 18:59:46.000000 core_explore_keyword_app-2.8.0/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3190 2024-03-12 18:59:54.283208 core_explore_keyword_app-2.8.0/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2305 2024-03-12 18:59:46.000000 core_explore_keyword_app-2.8.0/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:52.125957 core_explore_keyword_app-2.8.0/core_explore_keyword_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       95 2024-03-12 18:59:46.000000 core_explore_keyword_app-2.8.0/core_explore_keyword_app/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1696 2024-03-12 18:59:47.000000 core_explore_keyword_app-2.8.0/core_explore_keyword_app/admin.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      512 2024-03-12 18:59:47.000000 core_explore_keyword_app-2.8.0/core_explore_keyword_app/apps.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:52.243620 core_explore_keyword_app-2.8.0/core_explore_keyword_app/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:47.000000 core_explore_keyword_app-2.8.0/core_explore_keyword_app/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:52.323493 core_explore_keyword_app-2.8.0/core_explore_keyword_app/components/persistent_query_keyword/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:47.000000 core_explore_keyword_app-2.8.0/core_explore_keyword_app/components/persistent_query_keyword/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      372 2024-03-12 18:59:47.000000 core_explore_keyword_app-2.8.0/core_explore_keyword_app/components/persistent_query_keyword/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2256 2024-03-12 18:59:47.000000 core_explore_keyword_app-2.8.0/core_explore_keyword_app/components/persistent_query_keyword/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1972 2024-03-12 18:59:47.000000 core_explore_keyword_app-2.8.0/core_explore_keyword_app/components/persistent_query_keyword/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:52.398307 core_explore_keyword_app-2.8.0/core_explore_keyword_app/components/search_operator/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       34 2024-03-12 18:59:47.000000 core_explore_keyword_app-2.8.0/core_explore_keyword_app/components/search_operator/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      372 2024-03-12 18:59:47.000000 core_explore_keyword_app-2.8.0/core_explore_keyword_app/components/search_operator/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2367 2024-03-12 18:59:47.000000 core_explore_keyword_app-2.8.0/core_explore_keyword_app/components/search_operator/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3134 2024-03-12 18:59:47.000000 core_explore_keyword_app-2.8.0/core_explore_keyword_app/components/search_operator/models.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1988 2024-03-12 18:59:47.000000 core_explore_keyword_app-2.8.0/core_explore_keyword_app/forms.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      818 2024-03-12 18:59:47.000000 core_explore_keyword_app-2.8.0/core_explore_keyword_app/menus.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:52.432999 core_explore_keyword_app-2.8.0/core_explore_keyword_app/migrations/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3571 2024-03-12 18:59:47.000000 core_explore_keyword_app-2.8.0/core_explore_keyword_app/migrations/0001_initial.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:47.000000 core_explore_keyword_app-2.8.0/core_explore_keyword_app/migrations/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      541 2024-03-12 18:59:47.000000 core_explore_keyword_app-2.8.0/core_explore_keyword_app/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:52.495826 core_explore_keyword_app-2.8.0/core_explore_keyword_app/permissions/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:47.000000 core_explore_keyword_app-2.8.0/core_explore_keyword_app/permissions/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1117 2024-03-12 18:59:47.000000 core_explore_keyword_app-2.8.0/core_explore_keyword_app/permissions/discover.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      152 2024-03-12 18:59:47.000000 core_explore_keyword_app-2.8.0/core_explore_keyword_app/permissions/rights.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:52.536981 core_explore_keyword_app-2.8.0/core_explore_keyword_app/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:47.000000 core_explore_keyword_app-2.8.0/core_explore_keyword_app/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:52.599537 core_explore_keyword_app-2.8.0/core_explore_keyword_app/rest/persistent_query_keyword/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:47.000000 core_explore_keyword_app-2.8.0/core_explore_keyword_app/rest/persistent_query_keyword/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3197 2024-03-12 18:59:47.000000 core_explore_keyword_app-2.8.0/core_explore_keyword_app/rest/persistent_query_keyword/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    12256 2024-03-12 18:59:47.000000 core_explore_keyword_app-2.8.0/core_explore_keyword_app/rest/persistent_query_keyword/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:52.659819 core_explore_keyword_app-2.8.0/core_explore_keyword_app/rest/search_operators/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:47.000000 core_explore_keyword_app-2.8.0/core_explore_keyword_app/rest/search_operators/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1343 2024-03-12 18:59:47.000000 core_explore_keyword_app-2.8.0/core_explore_keyword_app/rest/search_operators/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7434 2024-03-12 18:59:47.000000 core_explore_keyword_app-2.8.0/core_explore_keyword_app/rest/search_operators/views.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1688 2024-03-12 18:59:47.000000 core_explore_keyword_app-2.8.0/core_explore_keyword_app/rest/urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      510 2024-03-12 18:59:47.000000 core_explore_keyword_app-2.8.0/core_explore_keyword_app/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:51.562902 core_explore_keyword_app-2.8.0/core_explore_keyword_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:51.625660 core_explore_keyword_app-2.8.0/core_explore_keyword_app/static/core_explore_keyword_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:51.577870 core_explore_keyword_app-2.8.0/core_explore_keyword_app/static/core_explore_keyword_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:52.691702 core_explore_keyword_app-2.8.0/core_explore_keyword_app/static/core_explore_keyword_app/admin/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      129 2024-03-12 18:59:47.000000 core_explore_keyword_app-2.8.0/core_explore_keyword_app/static/core_explore_keyword_app/admin/css/search_ops_manager.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:52.747230 core_explore_keyword_app-2.8.0/core_explore_keyword_app/static/core_explore_keyword_app/admin/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      183 2024-03-12 18:59:47.000000 core_explore_keyword_app-2.8.0/core_explore_keyword_app/static/core_explore_keyword_app/admin/js/search_operators.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3599 2024-03-12 18:59:47.000000 core_explore_keyword_app-2.8.0/core_explore_keyword_app/static/core_explore_keyword_app/admin/js/search_ops_manager.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      951 2024-03-12 18:59:47.000000 core_explore_keyword_app-2.8.0/core_explore_keyword_app/static/core_explore_keyword_app/admin/js/search_ops_manager_delete.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:51.600123 core_explore_keyword_app-2.8.0/core_explore_keyword_app/static/core_explore_keyword_app/libs/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:52.771175 core_explore_keyword_app-2.8.0/core_explore_keyword_app/static/core_explore_keyword_app/libs/stretchy/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2930 2024-03-12 18:59:47.000000 core_explore_keyword_app-2.8.0/core_explore_keyword_app/static/core_explore_keyword_app/libs/stretchy/stretchy.min.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:51.604508 core_explore_keyword_app-2.8.0/core_explore_keyword_app/static/core_explore_keyword_app/libs/tag-it/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:51.615360 core_explore_keyword_app-2.8.0/core_explore_keyword_app/static/core_explore_keyword_app/libs/tag-it/2.0/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:52.798502 core_explore_keyword_app-2.8.0/core_explore_keyword_app/static/core_explore_keyword_app/libs/tag-it/2.0/css/
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     1398 2024-03-12 18:59:47.000000 core_explore_keyword_app-2.8.0/core_explore_keyword_app/static/core_explore_keyword_app/libs/tag-it/2.0/css/jquery.tagit.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:52.819280 core_explore_keyword_app-2.8.0/core_explore_keyword_app/static/core_explore_keyword_app/libs/tag-it/2.0/js/
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)    23552 2024-03-12 18:59:47.000000 core_explore_keyword_app-2.8.0/core_explore_keyword_app/static/core_explore_keyword_app/libs/tag-it/2.0/js/tag-it.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:51.640570 core_explore_keyword_app-2.8.0/core_explore_keyword_app/static/core_explore_keyword_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:51.634716 core_explore_keyword_app-2.8.0/core_explore_keyword_app/static/core_explore_keyword_app/user/css/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:52.851766 core_explore_keyword_app-2.8.0/core_explore_keyword_app/static/core_explore_keyword_app/user/css/search/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3506 2024-03-12 18:59:47.000000 core_explore_keyword_app-2.8.0/core_explore_keyword_app/static/core_explore_keyword_app/user/css/search/search.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:52.873736 core_explore_keyword_app-2.8.0/core_explore_keyword_app/static/core_explore_keyword_app/user/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      320 2024-03-12 18:59:47.000000 core_explore_keyword_app-2.8.0/core_explore_keyword_app/static/core_explore_keyword_app/user/js/persistent_query.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:52.966326 core_explore_keyword_app-2.8.0/core_explore_keyword_app/static/core_explore_keyword_app/user/js/search/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      554 2024-03-12 18:59:47.000000 core_explore_keyword_app-2.8.0/core_explore_keyword_app/static/core_explore_keyword_app/user/js/search/autocomplete_source.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      283 2024-03-12 18:59:47.000000 core_explore_keyword_app-2.8.0/core_explore_keyword_app/static/core_explore_keyword_app/user/js/search/embedded_search.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10050 2024-03-12 18:59:47.000000 core_explore_keyword_app-2.8.0/core_explore_keyword_app/static/core_explore_keyword_app/user/js/search/search.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      156 2024-03-12 18:59:47.000000 core_explore_keyword_app-2.8.0/core_explore_keyword_app/static/core_explore_keyword_app/user/js/search/search.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:51.660536 core_explore_keyword_app-2.8.0/core_explore_keyword_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:51.720245 core_explore_keyword_app-2.8.0/core_explore_keyword_app/templates/core_explore_keyword_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:52.994280 core_explore_keyword_app-2.8.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:53.016750 core_explore_keyword_app-2.8.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/search_ops_manager/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1687 2024-03-12 18:59:47.000000 core_explore_keyword_app-2.8.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/search_ops_manager/box.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:51.714391 core_explore_keyword_app-2.8.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/search_ops_manager/modal/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:53.063851 core_explore_keyword_app-2.8.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/search_ops_manager/modal/config/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      957 2024-03-12 18:59:47.000000 core_explore_keyword_app-2.8.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/search_ops_manager/modal/config/form.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      812 2024-03-12 18:59:47.000000 core_explore_keyword_app-2.8.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/search_ops_manager/modal/config/modal.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:53.088069 core_explore_keyword_app-2.8.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/search_ops_manager/modal/delete/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      885 2024-03-12 18:59:47.000000 core_explore_keyword_app-2.8.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/search_ops_manager/modal/delete/modal.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      282 2024-03-12 18:59:47.000000 core_explore_keyword_app-2.8.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/search_ops_manager.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:53.225586 core_explore_keyword_app-2.8.0/core_explore_keyword_app/templates/core_explore_keyword_app/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1081 2024-03-12 18:59:47.000000 core_explore_keyword_app-2.8.0/core_explore_keyword_app/templates/core_explore_keyword_app/user/embedded_search_bar.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      350 2024-03-12 18:59:47.000000 core_explore_keyword_app-2.8.0/core_explore_keyword_app/templates/core_explore_keyword_app/user/extras.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1020 2024-03-12 18:59:47.000000 core_explore_keyword_app-2.8.0/core_explore_keyword_app/templates/core_explore_keyword_app/user/index.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      673 2024-03-12 18:59:47.000000 core_explore_keyword_app-2.8.0/core_explore_keyword_app/templates/core_explore_keyword_app/user/search_bar.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1819 2024-03-12 18:59:47.000000 core_explore_keyword_app-2.8.0/core_explore_keyword_app/templates/core_explore_keyword_app/user/template_filter.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:53.271796 core_explore_keyword_app-2.8.0/core_explore_keyword_app/templatetags/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:47.000000 core_explore_keyword_app-2.8.0/core_explore_keyword_app/templatetags/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1725 2024-03-12 18:59:47.000000 core_explore_keyword_app-2.8.0/core_explore_keyword_app/templatetags/core_explore_keyword_app_search_bar.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1484 2024-03-12 18:59:47.000000 core_explore_keyword_app-2.8.0/core_explore_keyword_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:53.336754 core_explore_keyword_app-2.8.0/core_explore_keyword_app/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:47.000000 core_explore_keyword_app-2.8.0/core_explore_keyword_app/utils/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      689 2024-03-12 18:59:47.000000 core_explore_keyword_app-2.8.0/core_explore_keyword_app/utils/abstract_keyword_search_extras.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2059 2024-03-12 18:59:47.000000 core_explore_keyword_app-2.8.0/core_explore_keyword_app/utils/search_operators.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:53.359541 core_explore_keyword_app-2.8.0/core_explore_keyword_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:47.000000 core_explore_keyword_app-2.8.0/core_explore_keyword_app/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:53.442917 core_explore_keyword_app-2.8.0/core_explore_keyword_app/views/admin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       43 2024-03-12 18:59:47.000000 core_explore_keyword_app-2.8.0/core_explore_keyword_app/views/admin/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3894 2024-03-12 18:59:47.000000 core_explore_keyword_app-2.8.0/core_explore_keyword_app/views/admin/ajax.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2421 2024-03-12 18:59:47.000000 core_explore_keyword_app-2.8.0/core_explore_keyword_app/views/admin/forms.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2389 2024-03-12 18:59:47.000000 core_explore_keyword_app-2.8.0/core_explore_keyword_app/views/admin/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:53.526735 core_explore_keyword_app-2.8.0/core_explore_keyword_app/views/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:47.000000 core_explore_keyword_app-2.8.0/core_explore_keyword_app/views/user/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6855 2024-03-12 18:59:47.000000 core_explore_keyword_app-2.8.0/core_explore_keyword_app/views/user/ajax.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    16154 2024-03-12 18:59:47.000000 core_explore_keyword_app-2.8.0/core_explore_keyword_app/views/user/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:52.223606 core_explore_keyword_app-2.8.0/core_explore_keyword_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3190 2024-03-12 18:59:50.000000 core_explore_keyword_app-2.8.0/core_explore_keyword_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5781 2024-03-12 18:59:51.000000 core_explore_keyword_app-2.8.0/core_explore_keyword_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2024-03-12 18:59:50.000000 core_explore_keyword_app-2.8.0/core_explore_keyword_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       98 2024-03-12 18:59:50.000000 core_explore_keyword_app-2.8.0/core_explore_keyword_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       36 2024-03-12 18:59:50.000000 core_explore_keyword_app-2.8.0/core_explore_keyword_app.egg-info/top_level.txt
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:53.594993 core_explore_keyword_app-2.8.0/docs/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:47.000000 core_explore_keyword_app-2.8.0/docs/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11113 2024-03-12 18:59:47.000000 core_explore_keyword_app-2.8.0/docs/conf.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      311 2024-03-12 18:59:48.000000 core_explore_keyword_app-2.8.0/docs/conf_urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2024-03-12 18:59:48.000000 core_explore_keyword_app-2.8.0/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       52 2024-03-12 18:59:48.000000 core_explore_keyword_app-2.8.0/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2024-03-12 18:59:54.291419 core_explore_keyword_app-2.8.0/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1078 2024-03-12 18:59:48.000000 core_explore_keyword_app-2.8.0/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:53.640942 core_explore_keyword_app-2.8.0/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:48.000000 core_explore_keyword_app-2.8.0/tests/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:53.665133 core_explore_keyword_app-2.8.0/tests/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:48.000000 core_explore_keyword_app-2.8.0/tests/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:53.739849 core_explore_keyword_app-2.8.0/tests/components/persistent_query_keyword/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:48.000000 core_explore_keyword_app-2.8.0/tests/components/persistent_query_keyword/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:53.789136 core_explore_keyword_app-2.8.0/tests/components/persistent_query_keyword/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:48.000000 core_explore_keyword_app-2.8.0/tests/components/persistent_query_keyword/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1545 2024-03-12 18:59:48.000000 core_explore_keyword_app-2.8.0/tests/components/persistent_query_keyword/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    15787 2024-03-12 18:59:48.000000 core_explore_keyword_app-2.8.0/tests/components/persistent_query_keyword/tests_int_access_control.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    12126 2024-03-12 18:59:48.000000 core_explore_keyword_app-2.8.0/tests/components/persistent_query_keyword/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:53.834940 core_explore_keyword_app-2.8.0/tests/components/search_operator/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:48.000000 core_explore_keyword_app-2.8.0/tests/components/search_operator/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5362 2024-03-12 18:59:48.000000 core_explore_keyword_app-2.8.0/tests/components/search_operator/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:53.883995 core_explore_keyword_app-2.8.0/tests/forms/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:48.000000 core_explore_keyword_app-2.8.0/tests/forms/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1772 2024-03-12 18:59:48.000000 core_explore_keyword_app-2.8.0/tests/forms/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:53.907017 core_explore_keyword_app-2.8.0/tests/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:48.000000 core_explore_keyword_app-2.8.0/tests/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:53.975851 core_explore_keyword_app-2.8.0/tests/rest/persistent_query_keyword/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:48.000000 core_explore_keyword_app-2.8.0/tests/rest/persistent_query_keyword/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11606 2024-03-12 18:59:48.000000 core_explore_keyword_app-2.8.0/tests/rest/persistent_query_keyword/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    17581 2024-03-12 18:59:48.000000 core_explore_keyword_app-2.8.0/tests/rest/persistent_query_keyword/tests_permissions.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:54.043899 core_explore_keyword_app-2.8.0/tests/rest/search_operators/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:48.000000 core_explore_keyword_app-2.8.0/tests/rest/search_operators/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9668 2024-03-12 18:59:48.000000 core_explore_keyword_app-2.8.0/tests/rest/search_operators/tests_permissions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14457 2024-03-12 18:59:48.000000 core_explore_keyword_app-2.8.0/tests/rest/search_operators/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:54.094473 core_explore_keyword_app-2.8.0/tests/templatetags/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:48.000000 core_explore_keyword_app-2.8.0/tests/templatetags/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1381 2024-03-12 18:59:48.000000 core_explore_keyword_app-2.8.0/tests/templatetags/test_unit.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1882 2024-03-12 18:59:48.000000 core_explore_keyword_app-2.8.0/tests/test_settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:54.117671 core_explore_keyword_app-2.8.0/tests/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:48.000000 core_explore_keyword_app-2.8.0/tests/utils/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:54.166635 core_explore_keyword_app-2.8.0/tests/utils/search_operators/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:48.000000 core_explore_keyword_app-2.8.0/tests/utils/search_operators/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4248 2024-03-12 18:59:48.000000 core_explore_keyword_app-2.8.0/tests/utils/search_operators/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:54.188953 core_explore_keyword_app-2.8.0/tests/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:48.000000 core_explore_keyword_app-2.8.0/tests/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:54.217144 core_explore_keyword_app-2.8.0/tests/views/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:48.000000 core_explore_keyword_app-2.8.0/tests/views/user/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:54.264297 core_explore_keyword_app-2.8.0/tests/views/user/ajax/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-03-12 18:59:48.000000 core_explore_keyword_app-2.8.0/tests/views/user/ajax/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    12542 2024-03-12 18:59:48.000000 core_explore_keyword_app-2.8.0/tests/views/user/ajax/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:35.301402 core_explore_keyword_app-2.9.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2024-05-13 16:05:22.000000 core_explore_keyword_app-2.9.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      156 2024-05-13 16:05:22.000000 core_explore_keyword_app-2.9.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3190 2024-05-13 16:05:35.294762 core_explore_keyword_app-2.9.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2305 2024-05-13 16:05:22.000000 core_explore_keyword_app-2.9.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:33.043033 core_explore_keyword_app-2.9.0/core_explore_keyword_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       95 2024-05-13 16:05:22.000000 core_explore_keyword_app-2.9.0/core_explore_keyword_app/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1696 2024-05-13 16:05:22.000000 core_explore_keyword_app-2.9.0/core_explore_keyword_app/admin.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      512 2024-05-13 16:05:22.000000 core_explore_keyword_app-2.9.0/core_explore_keyword_app/apps.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:33.163299 core_explore_keyword_app-2.9.0/core_explore_keyword_app/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:22.000000 core_explore_keyword_app-2.9.0/core_explore_keyword_app/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:33.240660 core_explore_keyword_app-2.9.0/core_explore_keyword_app/components/persistent_query_keyword/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:22.000000 core_explore_keyword_app-2.9.0/core_explore_keyword_app/components/persistent_query_keyword/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      372 2024-05-13 16:05:22.000000 core_explore_keyword_app-2.9.0/core_explore_keyword_app/components/persistent_query_keyword/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2256 2024-05-13 16:05:22.000000 core_explore_keyword_app-2.9.0/core_explore_keyword_app/components/persistent_query_keyword/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1972 2024-05-13 16:05:22.000000 core_explore_keyword_app-2.9.0/core_explore_keyword_app/components/persistent_query_keyword/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:33.310582 core_explore_keyword_app-2.9.0/core_explore_keyword_app/components/search_operator/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       34 2024-05-13 16:05:22.000000 core_explore_keyword_app-2.9.0/core_explore_keyword_app/components/search_operator/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      372 2024-05-13 16:05:22.000000 core_explore_keyword_app-2.9.0/core_explore_keyword_app/components/search_operator/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2367 2024-05-13 16:05:22.000000 core_explore_keyword_app-2.9.0/core_explore_keyword_app/components/search_operator/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3134 2024-05-13 16:05:22.000000 core_explore_keyword_app-2.9.0/core_explore_keyword_app/components/search_operator/models.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1988 2024-05-13 16:05:22.000000 core_explore_keyword_app-2.9.0/core_explore_keyword_app/forms.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      818 2024-05-13 16:05:22.000000 core_explore_keyword_app-2.9.0/core_explore_keyword_app/menus.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:33.344704 core_explore_keyword_app-2.9.0/core_explore_keyword_app/migrations/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3571 2024-05-13 16:05:22.000000 core_explore_keyword_app-2.9.0/core_explore_keyword_app/migrations/0001_initial.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:22.000000 core_explore_keyword_app-2.9.0/core_explore_keyword_app/migrations/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      541 2024-05-13 16:05:22.000000 core_explore_keyword_app-2.9.0/core_explore_keyword_app/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:33.413287 core_explore_keyword_app-2.9.0/core_explore_keyword_app/permissions/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:22.000000 core_explore_keyword_app-2.9.0/core_explore_keyword_app/permissions/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1117 2024-05-13 16:05:22.000000 core_explore_keyword_app-2.9.0/core_explore_keyword_app/permissions/discover.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      152 2024-05-13 16:05:22.000000 core_explore_keyword_app-2.9.0/core_explore_keyword_app/permissions/rights.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:33.451561 core_explore_keyword_app-2.9.0/core_explore_keyword_app/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:22.000000 core_explore_keyword_app-2.9.0/core_explore_keyword_app/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:33.518818 core_explore_keyword_app-2.9.0/core_explore_keyword_app/rest/persistent_query_keyword/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:22.000000 core_explore_keyword_app-2.9.0/core_explore_keyword_app/rest/persistent_query_keyword/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3197 2024-05-13 16:05:22.000000 core_explore_keyword_app-2.9.0/core_explore_keyword_app/rest/persistent_query_keyword/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    12256 2024-05-13 16:05:22.000000 core_explore_keyword_app-2.9.0/core_explore_keyword_app/rest/persistent_query_keyword/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:33.590368 core_explore_keyword_app-2.9.0/core_explore_keyword_app/rest/search_operators/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:22.000000 core_explore_keyword_app-2.9.0/core_explore_keyword_app/rest/search_operators/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1343 2024-05-13 16:05:22.000000 core_explore_keyword_app-2.9.0/core_explore_keyword_app/rest/search_operators/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7434 2024-05-13 16:05:22.000000 core_explore_keyword_app-2.9.0/core_explore_keyword_app/rest/search_operators/views.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1688 2024-05-13 16:05:22.000000 core_explore_keyword_app-2.9.0/core_explore_keyword_app/rest/urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      510 2024-05-13 16:05:22.000000 core_explore_keyword_app-2.9.0/core_explore_keyword_app/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:32.398632 core_explore_keyword_app-2.9.0/core_explore_keyword_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:32.476865 core_explore_keyword_app-2.9.0/core_explore_keyword_app/static/core_explore_keyword_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:32.421011 core_explore_keyword_app-2.9.0/core_explore_keyword_app/static/core_explore_keyword_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:33.622416 core_explore_keyword_app-2.9.0/core_explore_keyword_app/static/core_explore_keyword_app/admin/css/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      129 2024-05-13 16:05:23.000000 core_explore_keyword_app-2.9.0/core_explore_keyword_app/static/core_explore_keyword_app/admin/css/search_ops_manager.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:33.686205 core_explore_keyword_app-2.9.0/core_explore_keyword_app/static/core_explore_keyword_app/admin/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      183 2024-05-13 16:05:23.000000 core_explore_keyword_app-2.9.0/core_explore_keyword_app/static/core_explore_keyword_app/admin/js/search_operators.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3599 2024-05-13 16:05:23.000000 core_explore_keyword_app-2.9.0/core_explore_keyword_app/static/core_explore_keyword_app/admin/js/search_ops_manager.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      951 2024-05-13 16:05:23.000000 core_explore_keyword_app-2.9.0/core_explore_keyword_app/static/core_explore_keyword_app/admin/js/search_ops_manager_delete.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:32.442752 core_explore_keyword_app-2.9.0/core_explore_keyword_app/static/core_explore_keyword_app/libs/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:33.720897 core_explore_keyword_app-2.9.0/core_explore_keyword_app/static/core_explore_keyword_app/libs/stretchy/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2930 2024-05-13 16:05:23.000000 core_explore_keyword_app-2.9.0/core_explore_keyword_app/static/core_explore_keyword_app/libs/stretchy/stretchy.min.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:32.446944 core_explore_keyword_app-2.9.0/core_explore_keyword_app/static/core_explore_keyword_app/libs/tag-it/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:32.465420 core_explore_keyword_app-2.9.0/core_explore_keyword_app/static/core_explore_keyword_app/libs/tag-it/2.0/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:33.747516 core_explore_keyword_app-2.9.0/core_explore_keyword_app/static/core_explore_keyword_app/libs/tag-it/2.0/css/
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     1398 2024-05-13 16:05:23.000000 core_explore_keyword_app-2.9.0/core_explore_keyword_app/static/core_explore_keyword_app/libs/tag-it/2.0/css/jquery.tagit.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:33.768831 core_explore_keyword_app-2.9.0/core_explore_keyword_app/static/core_explore_keyword_app/libs/tag-it/2.0/js/
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)    23552 2024-05-13 16:05:23.000000 core_explore_keyword_app-2.9.0/core_explore_keyword_app/static/core_explore_keyword_app/libs/tag-it/2.0/js/tag-it.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:32.490528 core_explore_keyword_app-2.9.0/core_explore_keyword_app/static/core_explore_keyword_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:32.485065 core_explore_keyword_app-2.9.0/core_explore_keyword_app/static/core_explore_keyword_app/user/css/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:33.797816 core_explore_keyword_app-2.9.0/core_explore_keyword_app/static/core_explore_keyword_app/user/css/search/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3506 2024-05-13 16:05:23.000000 core_explore_keyword_app-2.9.0/core_explore_keyword_app/static/core_explore_keyword_app/user/css/search/search.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:33.830500 core_explore_keyword_app-2.9.0/core_explore_keyword_app/static/core_explore_keyword_app/user/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      320 2024-05-13 16:05:23.000000 core_explore_keyword_app-2.9.0/core_explore_keyword_app/static/core_explore_keyword_app/user/js/persistent_query.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:33.911745 core_explore_keyword_app-2.9.0/core_explore_keyword_app/static/core_explore_keyword_app/user/js/search/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      554 2024-05-13 16:05:23.000000 core_explore_keyword_app-2.9.0/core_explore_keyword_app/static/core_explore_keyword_app/user/js/search/autocomplete_source.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      283 2024-05-13 16:05:23.000000 core_explore_keyword_app-2.9.0/core_explore_keyword_app/static/core_explore_keyword_app/user/js/search/embedded_search.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10050 2024-05-13 16:05:23.000000 core_explore_keyword_app-2.9.0/core_explore_keyword_app/static/core_explore_keyword_app/user/js/search/search.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      156 2024-05-13 16:05:23.000000 core_explore_keyword_app-2.9.0/core_explore_keyword_app/static/core_explore_keyword_app/user/js/search/search.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:32.547261 core_explore_keyword_app-2.9.0/core_explore_keyword_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:32.583358 core_explore_keyword_app-2.9.0/core_explore_keyword_app/templates/core_explore_keyword_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:33.939952 core_explore_keyword_app-2.9.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:33.962518 core_explore_keyword_app-2.9.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/search_ops_manager/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1687 2024-05-13 16:05:23.000000 core_explore_keyword_app-2.9.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/search_ops_manager/box.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:32.577373 core_explore_keyword_app-2.9.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/search_ops_manager/modal/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:34.005831 core_explore_keyword_app-2.9.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/search_ops_manager/modal/config/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      957 2024-05-13 16:05:23.000000 core_explore_keyword_app-2.9.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/search_ops_manager/modal/config/form.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      812 2024-05-13 16:05:23.000000 core_explore_keyword_app-2.9.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/search_ops_manager/modal/config/modal.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:34.030837 core_explore_keyword_app-2.9.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/search_ops_manager/modal/delete/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      885 2024-05-13 16:05:23.000000 core_explore_keyword_app-2.9.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/search_ops_manager/modal/delete/modal.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      282 2024-05-13 16:05:23.000000 core_explore_keyword_app-2.9.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/search_ops_manager.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:34.167880 core_explore_keyword_app-2.9.0/core_explore_keyword_app/templates/core_explore_keyword_app/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1081 2024-05-13 16:05:23.000000 core_explore_keyword_app-2.9.0/core_explore_keyword_app/templates/core_explore_keyword_app/user/embedded_search_bar.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      350 2024-05-13 16:05:23.000000 core_explore_keyword_app-2.9.0/core_explore_keyword_app/templates/core_explore_keyword_app/user/extras.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1020 2024-05-13 16:05:23.000000 core_explore_keyword_app-2.9.0/core_explore_keyword_app/templates/core_explore_keyword_app/user/index.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      673 2024-05-13 16:05:23.000000 core_explore_keyword_app-2.9.0/core_explore_keyword_app/templates/core_explore_keyword_app/user/search_bar.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1819 2024-05-13 16:05:23.000000 core_explore_keyword_app-2.9.0/core_explore_keyword_app/templates/core_explore_keyword_app/user/template_filter.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:34.206439 core_explore_keyword_app-2.9.0/core_explore_keyword_app/templatetags/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:23.000000 core_explore_keyword_app-2.9.0/core_explore_keyword_app/templatetags/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1725 2024-05-13 16:05:23.000000 core_explore_keyword_app-2.9.0/core_explore_keyword_app/templatetags/core_explore_keyword_app_search_bar.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1484 2024-05-13 16:05:23.000000 core_explore_keyword_app-2.9.0/core_explore_keyword_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:34.262123 core_explore_keyword_app-2.9.0/core_explore_keyword_app/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:23.000000 core_explore_keyword_app-2.9.0/core_explore_keyword_app/utils/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      689 2024-05-13 16:05:23.000000 core_explore_keyword_app-2.9.0/core_explore_keyword_app/utils/abstract_keyword_search_extras.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2059 2024-05-13 16:05:23.000000 core_explore_keyword_app-2.9.0/core_explore_keyword_app/utils/search_operators.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:34.283227 core_explore_keyword_app-2.9.0/core_explore_keyword_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:23.000000 core_explore_keyword_app-2.9.0/core_explore_keyword_app/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:34.366394 core_explore_keyword_app-2.9.0/core_explore_keyword_app/views/admin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       43 2024-05-13 16:05:24.000000 core_explore_keyword_app-2.9.0/core_explore_keyword_app/views/admin/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3882 2024-05-13 16:05:24.000000 core_explore_keyword_app-2.9.0/core_explore_keyword_app/views/admin/ajax.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2421 2024-05-13 16:05:24.000000 core_explore_keyword_app-2.9.0/core_explore_keyword_app/views/admin/forms.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2389 2024-05-13 16:05:24.000000 core_explore_keyword_app-2.9.0/core_explore_keyword_app/views/admin/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:34.445301 core_explore_keyword_app-2.9.0/core_explore_keyword_app/views/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:24.000000 core_explore_keyword_app-2.9.0/core_explore_keyword_app/views/user/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6855 2024-05-13 16:05:24.000000 core_explore_keyword_app-2.9.0/core_explore_keyword_app/views/user/ajax.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    16154 2024-05-13 16:05:24.000000 core_explore_keyword_app-2.9.0/core_explore_keyword_app/views/user/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:33.141865 core_explore_keyword_app-2.9.0/core_explore_keyword_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3190 2024-05-13 16:05:26.000000 core_explore_keyword_app-2.9.0/core_explore_keyword_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5781 2024-05-13 16:05:32.000000 core_explore_keyword_app-2.9.0/core_explore_keyword_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2024-05-13 16:05:26.000000 core_explore_keyword_app-2.9.0/core_explore_keyword_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       98 2024-05-13 16:05:26.000000 core_explore_keyword_app-2.9.0/core_explore_keyword_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       36 2024-05-13 16:05:26.000000 core_explore_keyword_app-2.9.0/core_explore_keyword_app.egg-info/top_level.txt
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:34.526689 core_explore_keyword_app-2.9.0/docs/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:24.000000 core_explore_keyword_app-2.9.0/docs/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11113 2024-05-13 16:05:24.000000 core_explore_keyword_app-2.9.0/docs/conf.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      311 2024-05-13 16:05:24.000000 core_explore_keyword_app-2.9.0/docs/conf_urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2024-05-13 16:05:24.000000 core_explore_keyword_app-2.9.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       52 2024-05-13 16:05:24.000000 core_explore_keyword_app-2.9.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2024-05-13 16:05:35.303851 core_explore_keyword_app-2.9.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1078 2024-05-13 16:05:24.000000 core_explore_keyword_app-2.9.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:34.576230 core_explore_keyword_app-2.9.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:24.000000 core_explore_keyword_app-2.9.0/tests/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:34.617635 core_explore_keyword_app-2.9.0/tests/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:24.000000 core_explore_keyword_app-2.9.0/tests/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:34.687068 core_explore_keyword_app-2.9.0/tests/components/persistent_query_keyword/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:24.000000 core_explore_keyword_app-2.9.0/tests/components/persistent_query_keyword/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:34.741137 core_explore_keyword_app-2.9.0/tests/components/persistent_query_keyword/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:24.000000 core_explore_keyword_app-2.9.0/tests/components/persistent_query_keyword/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1545 2024-05-13 16:05:24.000000 core_explore_keyword_app-2.9.0/tests/components/persistent_query_keyword/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    15787 2024-05-13 16:05:24.000000 core_explore_keyword_app-2.9.0/tests/components/persistent_query_keyword/tests_int_access_control.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    12126 2024-05-13 16:05:24.000000 core_explore_keyword_app-2.9.0/tests/components/persistent_query_keyword/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:34.789253 core_explore_keyword_app-2.9.0/tests/components/search_operator/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:24.000000 core_explore_keyword_app-2.9.0/tests/components/search_operator/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5362 2024-05-13 16:05:24.000000 core_explore_keyword_app-2.9.0/tests/components/search_operator/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:34.836248 core_explore_keyword_app-2.9.0/tests/forms/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:24.000000 core_explore_keyword_app-2.9.0/tests/forms/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1772 2024-05-13 16:05:24.000000 core_explore_keyword_app-2.9.0/tests/forms/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:34.863954 core_explore_keyword_app-2.9.0/tests/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:24.000000 core_explore_keyword_app-2.9.0/tests/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:34.949973 core_explore_keyword_app-2.9.0/tests/rest/persistent_query_keyword/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:24.000000 core_explore_keyword_app-2.9.0/tests/rest/persistent_query_keyword/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11606 2024-05-13 16:05:24.000000 core_explore_keyword_app-2.9.0/tests/rest/persistent_query_keyword/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    17581 2024-05-13 16:05:24.000000 core_explore_keyword_app-2.9.0/tests/rest/persistent_query_keyword/tests_permissions.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:35.011242 core_explore_keyword_app-2.9.0/tests/rest/search_operators/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:24.000000 core_explore_keyword_app-2.9.0/tests/rest/search_operators/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9668 2024-05-13 16:05:24.000000 core_explore_keyword_app-2.9.0/tests/rest/search_operators/tests_permissions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14457 2024-05-13 16:05:24.000000 core_explore_keyword_app-2.9.0/tests/rest/search_operators/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:35.067929 core_explore_keyword_app-2.9.0/tests/templatetags/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:24.000000 core_explore_keyword_app-2.9.0/tests/templatetags/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1381 2024-05-13 16:05:24.000000 core_explore_keyword_app-2.9.0/tests/templatetags/test_unit.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1882 2024-05-13 16:05:24.000000 core_explore_keyword_app-2.9.0/tests/test_settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:35.088227 core_explore_keyword_app-2.9.0/tests/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:24.000000 core_explore_keyword_app-2.9.0/tests/utils/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:35.134818 core_explore_keyword_app-2.9.0/tests/utils/search_operators/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:24.000000 core_explore_keyword_app-2.9.0/tests/utils/search_operators/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4248 2024-05-13 16:05:24.000000 core_explore_keyword_app-2.9.0/tests/utils/search_operators/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:35.156274 core_explore_keyword_app-2.9.0/tests/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:24.000000 core_explore_keyword_app-2.9.0/tests/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:35.183340 core_explore_keyword_app-2.9.0/tests/views/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:24.000000 core_explore_keyword_app-2.9.0/tests/views/user/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:35.265714 core_explore_keyword_app-2.9.0/tests/views/user/ajax/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2024-05-13 16:05:24.000000 core_explore_keyword_app-2.9.0/tests/views/user/ajax/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    12542 2024-05-13 16:05:24.000000 core_explore_keyword_app-2.9.0/tests/views/user/ajax/tests_unit.py
```

### Comparing `core_explore_keyword_app-2.8.0/LICENSE.md` & `core_explore_keyword_app-2.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.8.0/PKG-INFO` & `core_explore_keyword_app-2.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core_explore_keyword_app
-Version: 2.8.0
+Version: 2.9.0
 Summary: Exploration by keywords for the curator core project
 Home-page: https://github.com/usnistgov/core_explore_keyword_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: ========================
         Core Explore Keyword App
```

### Comparing `core_explore_keyword_app-2.8.0/README.rst` & `core_explore_keyword_app-2.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.8.0/core_explore_keyword_app/admin.py` & `core_explore_keyword_app-2.9.0/core_explore_keyword_app/admin.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.8.0/core_explore_keyword_app/apps.py` & `core_explore_keyword_app-2.9.0/core_explore_keyword_app/apps.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.8.0/core_explore_keyword_app/components/persistent_query_keyword/api.py` & `core_explore_keyword_app-2.9.0/core_explore_keyword_app/components/persistent_query_keyword/api.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.8.0/core_explore_keyword_app/components/persistent_query_keyword/models.py` & `core_explore_keyword_app-2.9.0/core_explore_keyword_app/components/persistent_query_keyword/models.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.8.0/core_explore_keyword_app/components/search_operator/api.py` & `core_explore_keyword_app-2.9.0/core_explore_keyword_app/components/search_operator/api.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.8.0/core_explore_keyword_app/components/search_operator/models.py` & `core_explore_keyword_app-2.9.0/core_explore_keyword_app/components/search_operator/models.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.8.0/core_explore_keyword_app/forms.py` & `core_explore_keyword_app-2.9.0/core_explore_keyword_app/forms.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.8.0/core_explore_keyword_app/menus.py` & `core_explore_keyword_app-2.9.0/core_explore_keyword_app/menus.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.8.0/core_explore_keyword_app/migrations/0001_initial.py` & `core_explore_keyword_app-2.9.0/core_explore_keyword_app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.8.0/core_explore_keyword_app/models.py` & `core_explore_keyword_app-2.9.0/core_explore_keyword_app/models.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.8.0/core_explore_keyword_app/permissions/discover.py` & `core_explore_keyword_app-2.9.0/core_explore_keyword_app/permissions/discover.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.8.0/core_explore_keyword_app/rest/persistent_query_keyword/serializers.py` & `core_explore_keyword_app-2.9.0/core_explore_keyword_app/rest/persistent_query_keyword/serializers.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.8.0/core_explore_keyword_app/rest/persistent_query_keyword/views.py` & `core_explore_keyword_app-2.9.0/core_explore_keyword_app/rest/persistent_query_keyword/views.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.8.0/core_explore_keyword_app/rest/search_operators/serializers.py` & `core_explore_keyword_app-2.9.0/core_explore_keyword_app/rest/search_operators/serializers.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.8.0/core_explore_keyword_app/rest/search_operators/views.py` & `core_explore_keyword_app-2.9.0/core_explore_keyword_app/rest/search_operators/views.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.8.0/core_explore_keyword_app/rest/urls.py` & `core_explore_keyword_app-2.9.0/core_explore_keyword_app/rest/urls.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.8.0/core_explore_keyword_app/static/core_explore_keyword_app/admin/js/search_ops_manager.js` & `core_explore_keyword_app-2.9.0/core_explore_keyword_app/static/core_explore_keyword_app/admin/js/search_ops_manager.js`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.8.0/core_explore_keyword_app/static/core_explore_keyword_app/admin/js/search_ops_manager_delete.js` & `core_explore_keyword_app-2.9.0/core_explore_keyword_app/static/core_explore_keyword_app/admin/js/search_ops_manager_delete.js`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.8.0/core_explore_keyword_app/static/core_explore_keyword_app/libs/stretchy/stretchy.min.js` & `core_explore_keyword_app-2.9.0/core_explore_keyword_app/static/core_explore_keyword_app/libs/stretchy/stretchy.min.js`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.8.0/core_explore_keyword_app/static/core_explore_keyword_app/libs/tag-it/2.0/css/jquery.tagit.css` & `core_explore_keyword_app-2.9.0/core_explore_keyword_app/static/core_explore_keyword_app/libs/tag-it/2.0/css/jquery.tagit.css`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.8.0/core_explore_keyword_app/static/core_explore_keyword_app/libs/tag-it/2.0/js/tag-it.js` & `core_explore_keyword_app-2.9.0/core_explore_keyword_app/static/core_explore_keyword_app/libs/tag-it/2.0/js/tag-it.js`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.8.0/core_explore_keyword_app/static/core_explore_keyword_app/user/css/search/search.css` & `core_explore_keyword_app-2.9.0/core_explore_keyword_app/static/core_explore_keyword_app/user/css/search/search.css`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.8.0/core_explore_keyword_app/static/core_explore_keyword_app/user/js/search/autocomplete_source.js` & `core_explore_keyword_app-2.9.0/core_explore_keyword_app/static/core_explore_keyword_app/user/js/search/autocomplete_source.js`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.8.0/core_explore_keyword_app/static/core_explore_keyword_app/user/js/search/search.js` & `core_explore_keyword_app-2.9.0/core_explore_keyword_app/static/core_explore_keyword_app/user/js/search/search.js`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.8.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/search_ops_manager/box.html` & `core_explore_keyword_app-2.9.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/search_ops_manager/box.html`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.8.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/search_ops_manager/modal/config/form.html` & `core_explore_keyword_app-2.9.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/search_ops_manager/modal/config/form.html`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.8.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/search_ops_manager/modal/config/modal.html` & `core_explore_keyword_app-2.9.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/search_ops_manager/modal/config/modal.html`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.8.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/search_ops_manager/modal/delete/modal.html` & `core_explore_keyword_app-2.9.0/core_explore_keyword_app/templates/core_explore_keyword_app/admin/search_ops_manager/modal/delete/modal.html`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.8.0/core_explore_keyword_app/templates/core_explore_keyword_app/user/embedded_search_bar.html` & `core_explore_keyword_app-2.9.0/core_explore_keyword_app/templates/core_explore_keyword_app/user/embedded_search_bar.html`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.8.0/core_explore_keyword_app/templates/core_explore_keyword_app/user/index.html` & `core_explore_keyword_app-2.9.0/core_explore_keyword_app/templates/core_explore_keyword_app/user/index.html`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.8.0/core_explore_keyword_app/templates/core_explore_keyword_app/user/search_bar.html` & `core_explore_keyword_app-2.9.0/core_explore_keyword_app/templates/core_explore_keyword_app/user/search_bar.html`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.8.0/core_explore_keyword_app/templates/core_explore_keyword_app/user/template_filter.html` & `core_explore_keyword_app-2.9.0/core_explore_keyword_app/templates/core_explore_keyword_app/user/template_filter.html`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.8.0/core_explore_keyword_app/templatetags/core_explore_keyword_app_search_bar.py` & `core_explore_keyword_app-2.9.0/core_explore_keyword_app/templatetags/core_explore_keyword_app_search_bar.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.8.0/core_explore_keyword_app/urls.py` & `core_explore_keyword_app-2.9.0/core_explore_keyword_app/urls.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.8.0/core_explore_keyword_app/utils/abstract_keyword_search_extras.py` & `core_explore_keyword_app-2.9.0/core_explore_keyword_app/utils/abstract_keyword_search_extras.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.8.0/core_explore_keyword_app/utils/search_operators.py` & `core_explore_keyword_app-2.9.0/core_explore_keyword_app/utils/search_operators.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.8.0/core_explore_keyword_app/views/admin/ajax.py` & `core_explore_keyword_app-2.9.0/core_explore_keyword_app/views/admin/ajax.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,15 +49,15 @@
             return render(
                 request,
                 "core_explore_keyword_app/admin/search_ops_manager/modal/config/form.html",
                 context={"form": operator_form},
             )
 
         messages.add_message(
-            request, messages.SUCCESS, "Operator successfully %s!" % action
+            request, messages.SUCCESS, "Operator  %s!" % action
         )
 
         return JsonResponse({})
 
     @staticmethod
     def get(request):
         """Method called after editing a search operator.
```

### Comparing `core_explore_keyword_app-2.8.0/core_explore_keyword_app/views/admin/forms.py` & `core_explore_keyword_app-2.9.0/core_explore_keyword_app/views/admin/forms.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.8.0/core_explore_keyword_app/views/admin/views.py` & `core_explore_keyword_app-2.9.0/core_explore_keyword_app/views/admin/views.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.8.0/core_explore_keyword_app/views/user/ajax.py` & `core_explore_keyword_app-2.9.0/core_explore_keyword_app/views/user/ajax.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.8.0/core_explore_keyword_app/views/user/views.py` & `core_explore_keyword_app-2.9.0/core_explore_keyword_app/views/user/views.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.8.0/core_explore_keyword_app.egg-info/PKG-INFO` & `core_explore_keyword_app-2.9.0/core_explore_keyword_app.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: core-explore-keyword-app
-Version: 2.8.0
+Version: 2.9.0
 Summary: Exploration by keywords for the curator core project
 Home-page: https://github.com/usnistgov/core_explore_keyword_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: ========================
         Core Explore Keyword App
```

### Comparing `core_explore_keyword_app-2.8.0/core_explore_keyword_app.egg-info/SOURCES.txt` & `core_explore_keyword_app-2.9.0/core_explore_keyword_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.8.0/docs/conf.py` & `core_explore_keyword_app-2.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.8.0/setup.py` & `core_explore_keyword_app-2.9.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_explore_keyword_app",
-    version="2.8.0",
+    version="2.9.0",
     description="Exploration by keywords for the curator core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_explore_keyword_app",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `core_explore_keyword_app-2.8.0/tests/components/persistent_query_keyword/fixtures/fixtures.py` & `core_explore_keyword_app-2.9.0/tests/components/persistent_query_keyword/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.8.0/tests/components/persistent_query_keyword/tests_int_access_control.py` & `core_explore_keyword_app-2.9.0/tests/components/persistent_query_keyword/tests_int_access_control.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.8.0/tests/components/persistent_query_keyword/tests_unit.py` & `core_explore_keyword_app-2.9.0/tests/components/persistent_query_keyword/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.8.0/tests/components/search_operator/tests_unit.py` & `core_explore_keyword_app-2.9.0/tests/components/search_operator/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.8.0/tests/forms/tests_unit.py` & `core_explore_keyword_app-2.9.0/tests/forms/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.8.0/tests/rest/persistent_query_keyword/tests_int.py` & `core_explore_keyword_app-2.9.0/tests/rest/persistent_query_keyword/tests_int.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.8.0/tests/rest/persistent_query_keyword/tests_permissions.py` & `core_explore_keyword_app-2.9.0/tests/rest/persistent_query_keyword/tests_permissions.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.8.0/tests/rest/search_operators/tests_permissions.py` & `core_explore_keyword_app-2.9.0/tests/rest/search_operators/tests_permissions.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.8.0/tests/rest/search_operators/tests_unit.py` & `core_explore_keyword_app-2.9.0/tests/rest/search_operators/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.8.0/tests/templatetags/test_unit.py` & `core_explore_keyword_app-2.9.0/tests/templatetags/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.8.0/tests/test_settings.py` & `core_explore_keyword_app-2.9.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.8.0/tests/utils/search_operators/tests_unit.py` & `core_explore_keyword_app-2.9.0/tests/utils/search_operators/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_explore_keyword_app-2.8.0/tests/views/user/ajax/tests_unit.py` & `core_explore_keyword_app-2.9.0/tests/views/user/ajax/tests_unit.py`

 * *Files identical despite different names*

