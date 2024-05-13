# Comparing `tmp/ftw.referencewidget-4.0.1.tar.gz` & `tmp/ftw.referencewidget-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ftw.referencewidget-4.0.1.tar", last modified: Fri Jun  9 16:04:37 2023, max compression
+gzip compressed data, was "ftw.referencewidget-4.0.2.tar", last modified: Mon May 13 18:58:07 2024, max compression
```

## Comparing `ftw.referencewidget-4.0.1.tar` & `ftw.referencewidget-4.0.2.tar`

### file list

```diff
@@ -1,108 +1,106 @@
-drwxr-xr-x   0 maethu     (501) staff       (20)        0 2023-06-09 16:04:37.175341 ftw.referencewidget-4.0.1/
--rw-r--r--   0 maethu     (501) staff       (20)      137 2023-06-09 16:04:36.000000 ftw.referencewidget-4.0.1/MANIFEST.in
--rw-r--r--   0 maethu     (501) staff       (20)    15715 2023-06-09 16:04:37.175160 ftw.referencewidget-4.0.1/PKG-INFO
--rw-r--r--   0 maethu     (501) staff       (20)     7085 2023-06-09 16:04:36.000000 ftw.referencewidget-4.0.1/README.rst
--rw-r--r--   0 maethu     (501) staff       (20)       71 2023-06-09 16:04:36.000000 ftw.referencewidget-4.0.1/constraints.txt
-drwxr-xr-x   0 maethu     (501) staff       (20)        0 2023-06-09 16:04:37.165124 ftw.referencewidget-4.0.1/docs/
--rw-r--r--   0 maethu     (501) staff       (20)     7872 2023-06-09 16:04:36.000000 ftw.referencewidget-4.0.1/docs/HISTORY.txt
--rw-r--r--   0 maethu     (501) staff       (20)    18092 2023-06-09 16:04:36.000000 ftw.referencewidget-4.0.1/docs/LICENSE.GPL
--rw-r--r--   0 maethu     (501) staff       (20)      721 2023-06-09 16:04:36.000000 ftw.referencewidget-4.0.1/docs/LICENSE.txt
-drwxr-xr-x   0 maethu     (501) staff       (20)        0 2023-06-09 16:04:37.165760 ftw.referencewidget-4.0.1/docs/static/
--rw-r--r--   0 maethu     (501) staff       (20)   164752 2023-06-09 16:04:36.000000 ftw.referencewidget-4.0.1/docs/static/list.png
--rw-r--r--   0 maethu     (501) staff       (20)   329017 2023-06-09 16:04:36.000000 ftw.referencewidget-4.0.1/docs/static/search.png
--rw-r--r--   0 maethu     (501) staff       (20)   136044 2023-06-09 16:04:36.000000 ftw.referencewidget-4.0.1/docs/static/selected.png
-drwxr-xr-x   0 maethu     (501) staff       (20)        0 2023-06-09 16:04:37.165953 ftw.referencewidget-4.0.1/ftw/
--rw-r--r--   0 maethu     (501) staff       (20)      244 2023-06-09 16:04:36.000000 ftw.referencewidget-4.0.1/ftw/__init__.py
-drwxr-xr-x   0 maethu     (501) staff       (20)        0 2023-06-09 16:04:37.168516 ftw.referencewidget-4.0.1/ftw/referencewidget/
-drwxr-xr-x   0 maethu     (501) staff       (20)        0 2023-06-09 16:04:37.168640 ftw.referencewidget-4.0.1/ftw/referencewidget/Extensions/
--rw-r--r--   0 maethu     (501) staff       (20)      253 2023-06-09 16:04:36.000000 ftw.referencewidget-4.0.1/ftw/referencewidget/Extensions/install.py
--rw-r--r--   0 maethu     (501) staff       (20)      177 2023-06-09 16:04:36.000000 ftw.referencewidget-4.0.1/ftw/referencewidget/__init__.py
--rw-r--r--   0 maethu     (501) staff       (20)     2881 2023-06-09 16:04:36.000000 ftw.referencewidget-4.0.1/ftw/referencewidget/behaviors.py
-drwxr-xr-x   0 maethu     (501) staff       (20)        0 2023-06-09 16:04:37.169083 ftw.referencewidget-4.0.1/ftw/referencewidget/browser/
--rw-r--r--   0 maethu     (501) staff       (20)        0 2023-06-09 16:04:36.000000 ftw.referencewidget-4.0.1/ftw/referencewidget/browser/__init__.py
--rw-r--r--   0 maethu     (501) staff       (20)      513 2023-06-09 16:04:36.000000 ftw.referencewidget-4.0.1/ftw/referencewidget/browser/configure.zcml
--rw-r--r--   0 maethu     (501) staff       (20)      162 2023-06-09 16:04:36.000000 ftw.referencewidget-4.0.1/ftw/referencewidget/browser/fake_edit.py
--rw-r--r--   0 maethu     (501) staff       (20)     4694 2023-06-09 16:04:36.000000 ftw.referencewidget-4.0.1/ftw/referencewidget/browser/utils.py
--rw-r--r--   0 maethu     (501) staff       (20)     3959 2023-06-09 16:04:36.000000 ftw.referencewidget-4.0.1/ftw/referencewidget/configure.zcml
--rw-r--r--   0 maethu     (501) staff       (20)     3699 2023-06-09 16:04:36.000000 ftw.referencewidget-4.0.1/ftw/referencewidget/converter.py
--rw-r--r--   0 maethu     (501) staff       (20)     3205 2023-06-09 16:04:36.000000 ftw.referencewidget-4.0.1/ftw/referencewidget/datagridfield.py
--rw-r--r--   0 maethu     (501) staff       (20)     1152 2023-06-09 16:04:36.000000 ftw.referencewidget-4.0.1/ftw/referencewidget/interfaces.py
-drwxr-xr-x   0 maethu     (501) staff       (20)        0 2023-06-09 16:04:37.169242 ftw.referencewidget-4.0.1/ftw/referencewidget/locales/
-drwxr-xr-x   0 maethu     (501) staff       (20)        0 2023-06-09 16:04:37.163150 ftw.referencewidget-4.0.1/ftw/referencewidget/locales/de/
-drwxr-xr-x   0 maethu     (501) staff       (20)        0 2023-06-09 16:04:37.169371 ftw.referencewidget-4.0.1/ftw/referencewidget/locales/de/LC_MESSAGES/
--rw-r--r--   0 maethu     (501) staff       (20)     3989 2023-06-09 16:04:36.000000 ftw.referencewidget-4.0.1/ftw/referencewidget/locales/de/LC_MESSAGES/ftw.referencewidget.po
--rw-r--r--   0 maethu     (501) staff       (20)     3781 2023-06-09 16:04:36.000000 ftw.referencewidget-4.0.1/ftw/referencewidget/locales/ftw.referencewidget.pot
--rw-r--r--   0 maethu     (501) staff       (20)      311 2023-06-09 16:04:36.000000 ftw.referencewidget-4.0.1/ftw/referencewidget/overrides.zcml
-drwxr-xr-x   0 maethu     (501) staff       (20)        0 2023-06-09 16:04:37.163326 ftw.referencewidget-4.0.1/ftw/referencewidget/profiles/
-drwxr-xr-x   0 maethu     (501) staff       (20)        0 2023-06-09 16:04:37.169683 ftw.referencewidget-4.0.1/ftw/referencewidget/profiles/default/
--rw-r--r--   0 maethu     (501) staff       (20)      145 2023-06-09 16:04:36.000000 ftw.referencewidget-4.0.1/ftw/referencewidget/profiles/default/metadata.xml
--rw-r--r--   0 maethu     (501) staff       (20)      123 2023-06-09 16:04:36.000000 ftw.referencewidget-4.0.1/ftw/referencewidget/profiles/default/registry.xml
-drwxr-xr-x   0 maethu     (501) staff       (20)        0 2023-06-09 16:04:37.169811 ftw.referencewidget-4.0.1/ftw/referencewidget/profiles/uninstall/
--rw-r--r--   0 maethu     (501) staff       (20)      303 2023-06-09 16:04:36.000000 ftw.referencewidget-4.0.1/ftw/referencewidget/profiles/uninstall/registry.xml
-drwxr-xr-x   0 maethu     (501) staff       (20)        0 2023-06-09 16:04:37.163480 ftw.referencewidget-4.0.1/ftw/referencewidget/resources/
-drwxr-xr-x   0 maethu     (501) staff       (20)        0 2023-06-09 16:04:37.170397 ftw.referencewidget-4.0.1/ftw/referencewidget/resources/dist/
--rw-r--r--   0 maethu     (501) staff       (20)   533956 2023-06-09 16:04:36.000000 ftw.referencewidget-4.0.1/ftw/referencewidget/resources/dist/referencewidget.es.js
--rw-r--r--   0 maethu     (501) staff       (20)   228975 2023-06-09 16:04:36.000000 ftw.referencewidget-4.0.1/ftw/referencewidget/resources/dist/referencewidget.umd.js
-drwxr-xr-x   0 maethu     (501) staff       (20)        0 2023-06-09 16:04:37.170637 ftw.referencewidget-4.0.1/ftw/referencewidget/resources/src/
--rw-r--r--   0 maethu     (501) staff       (20)     1154 2023-06-09 16:04:36.000000 ftw.referencewidget-4.0.1/ftw/referencewidget/resources/src/main.js
-drwxr-xr-x   0 maethu     (501) staff       (20)        0 2023-06-09 16:04:37.170887 ftw.referencewidget-4.0.1/ftw/referencewidget/resources/src/widget/
--rw-r--r--   0 maethu     (501) staff       (20)     6913 2023-06-09 16:04:36.000000 ftw.referencewidget-4.0.1/ftw/referencewidget/resources/src/widget/App.vue
-drwxr-xr-x   0 maethu     (501) staff       (20)        0 2023-06-09 16:04:37.171637 ftw.referencewidget-4.0.1/ftw/referencewidget/resources/src/widget/components/
--rw-r--r--   0 maethu     (501) staff       (20)     1374 2023-06-09 16:04:36.000000 ftw.referencewidget-4.0.1/ftw/referencewidget/resources/src/widget/components/Breadcrumbs.vue
--rw-r--r--   0 maethu     (501) staff       (20)     3738 2023-06-09 16:04:36.000000 ftw.referencewidget-4.0.1/ftw/referencewidget/resources/src/widget/components/ListItems.vue
--rw-r--r--   0 maethu     (501) staff       (20)     1893 2023-06-09 16:04:36.000000 ftw.referencewidget-4.0.1/ftw/referencewidget/resources/src/widget/components/Pagination.vue
--rw-r--r--   0 maethu     (501) staff       (20)      813 2023-06-09 16:04:36.000000 ftw.referencewidget-4.0.1/ftw/referencewidget/resources/src/widget/components/ResolveIcon.vue
--rw-r--r--   0 maethu     (501) staff       (20)     2586 2023-06-09 16:04:36.000000 ftw.referencewidget-4.0.1/ftw/referencewidget/resources/src/widget/components/searchForm.vue
--rw-r--r--   0 maethu     (501) staff       (20)      213 2023-06-09 16:04:36.000000 ftw.referencewidget-4.0.1/ftw/referencewidget/resources/src/widget/i18n.js
--rw-r--r--   0 maethu     (501) staff       (20)     1141 2023-06-09 16:04:36.000000 ftw.referencewidget-4.0.1/ftw/referencewidget/selectable.py
--rw-r--r--   0 maethu     (501) staff       (20)     3196 2023-06-09 16:04:36.000000 ftw.referencewidget-4.0.1/ftw/referencewidget/sources.py
-drwxr-xr-x   0 maethu     (501) staff       (20)        0 2023-06-09 16:04:37.171888 ftw.referencewidget-4.0.1/ftw/referencewidget/templates/
--rw-r--r--   0 maethu     (501) staff       (20)      610 2023-06-09 16:04:36.000000 ftw.referencewidget-4.0.1/ftw/referencewidget/templates/referencewidget_display.pt
--rw-r--r--   0 maethu     (501) staff       (20)     2110 2023-06-09 16:04:36.000000 ftw.referencewidget-4.0.1/ftw/referencewidget/templates/referencewidget_input.pt
--rw-r--r--   0 maethu     (501) staff       (20)     1907 2023-06-09 16:04:36.000000 ftw.referencewidget-4.0.1/ftw/referencewidget/testing.py
-drwxr-xr-x   0 maethu     (501) staff       (20)        0 2023-06-09 16:04:37.173394 ftw.referencewidget-4.0.1/ftw/referencewidget/tests/
--rw-r--r--   0 maethu     (501) staff       (20)     1755 2023-06-09 16:04:36.000000 ftw.referencewidget-4.0.1/ftw/referencewidget/tests/__init__.py
--rw-r--r--   0 maethu     (501) staff       (20)      386 2023-06-09 16:04:36.000000 ftw.referencewidget-4.0.1/ftw/referencewidget/tests/builders.py
--rw-r--r--   0 maethu     (501) staff       (20)     1717 2023-06-09 16:04:36.000000 ftw.referencewidget-4.0.1/ftw/referencewidget/tests/test_change_widget_config.py
--rw-r--r--   0 maethu     (501) staff       (20)     1738 2023-06-09 16:04:36.000000 ftw.referencewidget-4.0.1/ftw/referencewidget/tests/test_converter.py
--rw-r--r--   0 maethu     (501) staff       (20)     1357 2023-06-09 16:04:36.000000 ftw.referencewidget-4.0.1/ftw/referencewidget/tests/test_datagrid_field.py
--rw-r--r--   0 maethu     (501) staff       (20)     1335 2023-06-09 16:04:36.000000 ftw.referencewidget-4.0.1/ftw/referencewidget/tests/test_override.py
--rw-r--r--   0 maethu     (501) staff       (20)     4369 2023-06-09 16:04:36.000000 ftw.referencewidget-4.0.1/ftw/referencewidget/tests/test_related_items_behavior.py
--rw-r--r--   0 maethu     (501) staff       (20)     4937 2023-06-09 16:04:36.000000 ftw.referencewidget-4.0.1/ftw/referencewidget/tests/test_relation_choice.py
--rw-r--r--   0 maethu     (501) staff       (20)     3956 2023-06-09 16:04:36.000000 ftw.referencewidget-4.0.1/ftw/referencewidget/tests/test_source.py
--rw-r--r--   0 maethu     (501) staff       (20)      293 2023-06-09 16:04:36.000000 ftw.referencewidget-4.0.1/ftw/referencewidget/tests/test_uninstall.py
--rw-r--r--   0 maethu     (501) staff       (20)     2565 2023-06-09 16:04:36.000000 ftw.referencewidget-4.0.1/ftw/referencewidget/tests/test_utils.py
-drwxr-xr-x   0 maethu     (501) staff       (20)        0 2023-06-09 16:04:37.173726 ftw.referencewidget-4.0.1/ftw/referencewidget/tests/views/
--rw-r--r--   0 maethu     (501) staff       (20)        0 2023-06-09 16:04:36.000000 ftw.referencewidget-4.0.1/ftw/referencewidget/tests/views/__init__.py
--rw-r--r--   0 maethu     (501) staff       (20)      319 2023-06-09 16:04:36.000000 ftw.referencewidget-4.0.1/ftw/referencewidget/tests/views/configure.zcml
--rw-r--r--   0 maethu     (501) staff       (20)     1275 2023-06-09 16:04:36.000000 ftw.referencewidget-4.0.1/ftw/referencewidget/tests/views/form.py
--rw-r--r--   0 maethu     (501) staff       (20)     1472 2023-06-09 16:04:36.000000 ftw.referencewidget-4.0.1/ftw/referencewidget/tests/widgets.py
-drwxr-xr-x   0 maethu     (501) staff       (20)        0 2023-06-09 16:04:37.173859 ftw.referencewidget-4.0.1/ftw/referencewidget/upgrades/
-drwxr-xr-x   0 maethu     (501) staff       (20)        0 2023-06-09 16:04:37.174249 ftw.referencewidget-4.0.1/ftw/referencewidget/upgrades/20181112105705_fix_registry_field_frontend_edit/
--rw-r--r--   0 maethu     (501) staff       (20)        0 2023-06-09 16:04:36.000000 ftw.referencewidget-4.0.1/ftw/referencewidget/upgrades/20181112105705_fix_registry_field_frontend_edit/__init__.py
--rw-r--r--   0 maethu     (501) staff       (20)      122 2023-06-09 16:04:36.000000 ftw.referencewidget-4.0.1/ftw/referencewidget/upgrades/20181112105705_fix_registry_field_frontend_edit/registry.xml
--rw-r--r--   0 maethu     (501) staff       (20)      200 2023-06-09 16:04:36.000000 ftw.referencewidget-4.0.1/ftw/referencewidget/upgrades/20181112105705_fix_registry_field_frontend_edit/upgrade.py
-drwxr-xr-x   0 maethu     (501) staff       (20)        0 2023-06-09 16:04:37.174625 ftw.referencewidget-4.0.1/ftw/referencewidget/upgrades/20200115110839_restrict_handle_bars_to_authenticated_users/
--rw-r--r--   0 maethu     (501) staff       (20)        0 2023-06-09 16:04:36.000000 ftw.referencewidget-4.0.1/ftw/referencewidget/upgrades/20200115110839_restrict_handle_bars_to_authenticated_users/__init__.py
--rw-r--r--   0 maethu     (501) staff       (20)      286 2023-06-09 16:04:36.000000 ftw.referencewidget-4.0.1/ftw/referencewidget/upgrades/20200115110839_restrict_handle_bars_to_authenticated_users/jsregistry.xml
--rw-r--r--   0 maethu     (501) staff       (20)      354 2023-06-09 16:04:36.000000 ftw.referencewidget-4.0.1/ftw/referencewidget/upgrades/20200115110839_restrict_handle_bars_to_authenticated_users/upgrade.py
-drwxr-xr-x   0 maethu     (501) staff       (20)        0 2023-06-09 16:04:37.174966 ftw.referencewidget-4.0.1/ftw/referencewidget/upgrades/20201215183140_fix_js_bundle_for_plone_5/
--rw-r--r--   0 maethu     (501) staff       (20)        0 2023-06-09 16:04:36.000000 ftw.referencewidget-4.0.1/ftw/referencewidget/upgrades/20201215183140_fix_js_bundle_for_plone_5/__init__.py
--rw-r--r--   0 maethu     (501) staff       (20)      350 2023-06-09 16:04:36.000000 ftw.referencewidget-4.0.1/ftw/referencewidget/upgrades/20201215183140_fix_js_bundle_for_plone_5/registry.xml
--rw-r--r--   0 maethu     (501) staff       (20)      314 2023-06-09 16:04:36.000000 ftw.referencewidget-4.0.1/ftw/referencewidget/upgrades/20201215183140_fix_js_bundle_for_plone_5/upgrade.py
--rw-r--r--   0 maethu     (501) staff       (20)        0 2023-06-09 16:04:36.000000 ftw.referencewidget-4.0.1/ftw/referencewidget/upgrades/__init__.py
--rw-r--r--   0 maethu     (501) staff       (20)      485 2023-06-09 16:04:36.000000 ftw.referencewidget-4.0.1/ftw/referencewidget/utils.py
--rw-r--r--   0 maethu     (501) staff       (20)     8721 2023-06-09 16:04:36.000000 ftw.referencewidget-4.0.1/ftw/referencewidget/widget.py
-drwxr-xr-x   0 maethu     (501) staff       (20)        0 2023-06-09 16:04:37.166952 ftw.referencewidget-4.0.1/ftw.referencewidget.egg-info/
--rw-r--r--   0 maethu     (501) staff       (20)    15715 2023-06-09 16:04:37.000000 ftw.referencewidget-4.0.1/ftw.referencewidget.egg-info/PKG-INFO
--rw-r--r--   0 maethu     (501) staff       (20)     3673 2023-06-09 16:04:37.000000 ftw.referencewidget-4.0.1/ftw.referencewidget.egg-info/SOURCES.txt
--rw-r--r--   0 maethu     (501) staff       (20)        1 2023-06-09 16:04:37.000000 ftw.referencewidget-4.0.1/ftw.referencewidget.egg-info/dependency_links.txt
--rw-r--r--   0 maethu     (501) staff       (20)       42 2023-06-09 16:04:37.000000 ftw.referencewidget-4.0.1/ftw.referencewidget.egg-info/entry_points.txt
--rw-r--r--   0 maethu     (501) staff       (20)        4 2023-06-09 16:04:37.000000 ftw.referencewidget-4.0.1/ftw.referencewidget.egg-info/namespace_packages.txt
--rw-r--r--   0 maethu     (501) staff       (20)        1 2023-06-09 16:04:37.000000 ftw.referencewidget-4.0.1/ftw.referencewidget.egg-info/not-zip-safe
--rw-r--r--   0 maethu     (501) staff       (20)      361 2023-06-09 16:04:37.000000 ftw.referencewidget-4.0.1/ftw.referencewidget.egg-info/requires.txt
--rw-r--r--   0 maethu     (501) staff       (20)        4 2023-06-09 16:04:37.000000 ftw.referencewidget-4.0.1/ftw.referencewidget.egg-info/top_level.txt
--rw-r--r--   0 maethu     (501) staff       (20)       41 2023-06-09 16:04:36.000000 ftw.referencewidget-4.0.1/requirements.txt
--rw-r--r--   0 maethu     (501) staff       (20)      191 2023-06-09 16:04:36.000000 ftw.referencewidget-4.0.1/requirements_barebone.txt
--rw-r--r--   0 maethu     (501) staff       (20)       38 2023-06-09 16:04:37.175391 ftw.referencewidget-4.0.1/setup.cfg
--rw-r--r--   0 maethu     (501) staff       (20)     1895 2023-06-09 16:04:36.000000 ftw.referencewidget-4.0.1/setup.py
+drwxr-xr-x   0 maethu     (501) staff       (20)        0 2024-05-13 18:58:07.585541 ftw.referencewidget-4.0.2/
+-rw-r--r--   0 maethu     (501) staff       (20)      137 2024-05-13 18:58:07.000000 ftw.referencewidget-4.0.2/MANIFEST.in
+-rw-r--r--   0 maethu     (501) staff       (20)    15782 2024-05-13 18:58:07.585326 ftw.referencewidget-4.0.2/PKG-INFO
+-rw-r--r--   0 maethu     (501) staff       (20)     6954 2024-05-13 18:58:07.000000 ftw.referencewidget-4.0.2/README.rst
+-rw-r--r--   0 maethu     (501) staff       (20)       71 2024-05-13 18:58:07.000000 ftw.referencewidget-4.0.2/constraints.txt
+drwxr-xr-x   0 maethu     (501) staff       (20)        0 2024-05-13 18:58:07.575660 ftw.referencewidget-4.0.2/docs/
+-rw-r--r--   0 maethu     (501) staff       (20)     8070 2024-05-13 18:58:07.000000 ftw.referencewidget-4.0.2/docs/HISTORY.txt
+-rw-r--r--   0 maethu     (501) staff       (20)    18092 2024-05-13 18:58:07.000000 ftw.referencewidget-4.0.2/docs/LICENSE.GPL
+-rw-r--r--   0 maethu     (501) staff       (20)      721 2024-05-13 18:58:07.000000 ftw.referencewidget-4.0.2/docs/LICENSE.txt
+drwxr-xr-x   0 maethu     (501) staff       (20)        0 2024-05-13 18:58:07.576306 ftw.referencewidget-4.0.2/docs/static/
+-rw-r--r--   0 maethu     (501) staff       (20)   164752 2024-05-13 18:58:07.000000 ftw.referencewidget-4.0.2/docs/static/list.png
+-rw-r--r--   0 maethu     (501) staff       (20)   329017 2024-05-13 18:58:07.000000 ftw.referencewidget-4.0.2/docs/static/search.png
+-rw-r--r--   0 maethu     (501) staff       (20)   136044 2024-05-13 18:58:07.000000 ftw.referencewidget-4.0.2/docs/static/selected.png
+drwxr-xr-x   0 maethu     (501) staff       (20)        0 2024-05-13 18:58:07.576506 ftw.referencewidget-4.0.2/ftw/
+-rw-r--r--   0 maethu     (501) staff       (20)      244 2024-05-13 18:58:07.000000 ftw.referencewidget-4.0.2/ftw/__init__.py
+drwxr-xr-x   0 maethu     (501) staff       (20)        0 2024-05-13 18:58:07.578751 ftw.referencewidget-4.0.2/ftw/referencewidget/
+drwxr-xr-x   0 maethu     (501) staff       (20)        0 2024-05-13 18:58:07.578869 ftw.referencewidget-4.0.2/ftw/referencewidget/Extensions/
+-rw-r--r--   0 maethu     (501) staff       (20)      253 2024-05-13 18:58:07.000000 ftw.referencewidget-4.0.2/ftw/referencewidget/Extensions/install.py
+-rw-r--r--   0 maethu     (501) staff       (20)      177 2024-05-13 18:58:07.000000 ftw.referencewidget-4.0.2/ftw/referencewidget/__init__.py
+-rw-r--r--   0 maethu     (501) staff       (20)     2881 2024-05-13 18:58:07.000000 ftw.referencewidget-4.0.2/ftw/referencewidget/behaviors.py
+drwxr-xr-x   0 maethu     (501) staff       (20)        0 2024-05-13 18:58:07.579180 ftw.referencewidget-4.0.2/ftw/referencewidget/browser/
+-rw-r--r--   0 maethu     (501) staff       (20)        0 2024-05-13 18:58:07.000000 ftw.referencewidget-4.0.2/ftw/referencewidget/browser/__init__.py
+-rw-r--r--   0 maethu     (501) staff       (20)      325 2024-05-13 18:58:07.000000 ftw.referencewidget-4.0.2/ftw/referencewidget/browser/configure.zcml
+-rw-r--r--   0 maethu     (501) staff       (20)     4694 2024-05-13 18:58:07.000000 ftw.referencewidget-4.0.2/ftw/referencewidget/browser/utils.py
+-rw-r--r--   0 maethu     (501) staff       (20)     3959 2024-05-13 18:58:07.000000 ftw.referencewidget-4.0.2/ftw/referencewidget/configure.zcml
+-rw-r--r--   0 maethu     (501) staff       (20)     3699 2024-05-13 18:58:07.000000 ftw.referencewidget-4.0.2/ftw/referencewidget/converter.py
+-rw-r--r--   0 maethu     (501) staff       (20)     3205 2024-05-13 18:58:07.000000 ftw.referencewidget-4.0.2/ftw/referencewidget/datagridfield.py
+-rw-r--r--   0 maethu     (501) staff       (20)     1152 2024-05-13 18:58:07.000000 ftw.referencewidget-4.0.2/ftw/referencewidget/interfaces.py
+drwxr-xr-x   0 maethu     (501) staff       (20)        0 2024-05-13 18:58:07.579301 ftw.referencewidget-4.0.2/ftw/referencewidget/locales/
+drwxr-xr-x   0 maethu     (501) staff       (20)        0 2024-05-13 18:58:07.573763 ftw.referencewidget-4.0.2/ftw/referencewidget/locales/de/
+drwxr-xr-x   0 maethu     (501) staff       (20)        0 2024-05-13 18:58:07.579420 ftw.referencewidget-4.0.2/ftw/referencewidget/locales/de/LC_MESSAGES/
+-rw-r--r--   0 maethu     (501) staff       (20)     3989 2024-05-13 18:58:07.000000 ftw.referencewidget-4.0.2/ftw/referencewidget/locales/de/LC_MESSAGES/ftw.referencewidget.po
+-rw-r--r--   0 maethu     (501) staff       (20)     3781 2024-05-13 18:58:07.000000 ftw.referencewidget-4.0.2/ftw/referencewidget/locales/ftw.referencewidget.pot
+-rw-r--r--   0 maethu     (501) staff       (20)      311 2024-05-13 18:58:07.000000 ftw.referencewidget-4.0.2/ftw/referencewidget/overrides.zcml
+drwxr-xr-x   0 maethu     (501) staff       (20)        0 2024-05-13 18:58:07.573941 ftw.referencewidget-4.0.2/ftw/referencewidget/profiles/
+drwxr-xr-x   0 maethu     (501) staff       (20)        0 2024-05-13 18:58:07.579641 ftw.referencewidget-4.0.2/ftw/referencewidget/profiles/default/
+-rw-r--r--   0 maethu     (501) staff       (20)      145 2024-05-13 18:58:07.000000 ftw.referencewidget-4.0.2/ftw/referencewidget/profiles/default/metadata.xml
+-rw-r--r--   0 maethu     (501) staff       (20)      123 2024-05-13 18:58:07.000000 ftw.referencewidget-4.0.2/ftw/referencewidget/profiles/default/registry.xml
+drwxr-xr-x   0 maethu     (501) staff       (20)        0 2024-05-13 18:58:07.579747 ftw.referencewidget-4.0.2/ftw/referencewidget/profiles/uninstall/
+-rw-r--r--   0 maethu     (501) staff       (20)      303 2024-05-13 18:58:07.000000 ftw.referencewidget-4.0.2/ftw/referencewidget/profiles/uninstall/registry.xml
+drwxr-xr-x   0 maethu     (501) staff       (20)        0 2024-05-13 18:58:07.574118 ftw.referencewidget-4.0.2/ftw/referencewidget/resources/
+drwxr-xr-x   0 maethu     (501) staff       (20)        0 2024-05-13 18:58:07.580284 ftw.referencewidget-4.0.2/ftw/referencewidget/resources/dist/
+-rw-r--r--   0 maethu     (501) staff       (20)   533956 2024-05-13 18:58:07.000000 ftw.referencewidget-4.0.2/ftw/referencewidget/resources/dist/referencewidget.es.js
+-rw-r--r--   0 maethu     (501) staff       (20)   228975 2024-05-13 18:58:07.000000 ftw.referencewidget-4.0.2/ftw/referencewidget/resources/dist/referencewidget.umd.js
+drwxr-xr-x   0 maethu     (501) staff       (20)        0 2024-05-13 18:58:07.580554 ftw.referencewidget-4.0.2/ftw/referencewidget/resources/src/
+-rw-r--r--   0 maethu     (501) staff       (20)     1154 2024-05-13 18:58:07.000000 ftw.referencewidget-4.0.2/ftw/referencewidget/resources/src/main.js
+drwxr-xr-x   0 maethu     (501) staff       (20)        0 2024-05-13 18:58:07.580819 ftw.referencewidget-4.0.2/ftw/referencewidget/resources/src/widget/
+-rw-r--r--   0 maethu     (501) staff       (20)     6913 2024-05-13 18:58:07.000000 ftw.referencewidget-4.0.2/ftw/referencewidget/resources/src/widget/App.vue
+drwxr-xr-x   0 maethu     (501) staff       (20)        0 2024-05-13 18:58:07.581589 ftw.referencewidget-4.0.2/ftw/referencewidget/resources/src/widget/components/
+-rw-r--r--   0 maethu     (501) staff       (20)     1374 2024-05-13 18:58:07.000000 ftw.referencewidget-4.0.2/ftw/referencewidget/resources/src/widget/components/Breadcrumbs.vue
+-rw-r--r--   0 maethu     (501) staff       (20)     3738 2024-05-13 18:58:07.000000 ftw.referencewidget-4.0.2/ftw/referencewidget/resources/src/widget/components/ListItems.vue
+-rw-r--r--   0 maethu     (501) staff       (20)     1893 2024-05-13 18:58:07.000000 ftw.referencewidget-4.0.2/ftw/referencewidget/resources/src/widget/components/Pagination.vue
+-rw-r--r--   0 maethu     (501) staff       (20)      813 2024-05-13 18:58:07.000000 ftw.referencewidget-4.0.2/ftw/referencewidget/resources/src/widget/components/ResolveIcon.vue
+-rw-r--r--   0 maethu     (501) staff       (20)     2586 2024-05-13 18:58:07.000000 ftw.referencewidget-4.0.2/ftw/referencewidget/resources/src/widget/components/searchForm.vue
+-rw-r--r--   0 maethu     (501) staff       (20)      213 2024-05-13 18:58:07.000000 ftw.referencewidget-4.0.2/ftw/referencewidget/resources/src/widget/i18n.js
+-rw-r--r--   0 maethu     (501) staff       (20)     1141 2024-05-13 18:58:07.000000 ftw.referencewidget-4.0.2/ftw/referencewidget/selectable.py
+-rw-r--r--   0 maethu     (501) staff       (20)     3196 2024-05-13 18:58:07.000000 ftw.referencewidget-4.0.2/ftw/referencewidget/sources.py
+drwxr-xr-x   0 maethu     (501) staff       (20)        0 2024-05-13 18:58:07.581914 ftw.referencewidget-4.0.2/ftw/referencewidget/templates/
+-rw-r--r--   0 maethu     (501) staff       (20)      610 2024-05-13 18:58:07.000000 ftw.referencewidget-4.0.2/ftw/referencewidget/templates/referencewidget_display.pt
+-rw-r--r--   0 maethu     (501) staff       (20)     2110 2024-05-13 18:58:07.000000 ftw.referencewidget-4.0.2/ftw/referencewidget/templates/referencewidget_input.pt
+-rw-r--r--   0 maethu     (501) staff       (20)     1907 2024-05-13 18:58:07.000000 ftw.referencewidget-4.0.2/ftw/referencewidget/testing.py
+drwxr-xr-x   0 maethu     (501) staff       (20)        0 2024-05-13 18:58:07.583592 ftw.referencewidget-4.0.2/ftw/referencewidget/tests/
+-rw-r--r--   0 maethu     (501) staff       (20)     1755 2024-05-13 18:58:07.000000 ftw.referencewidget-4.0.2/ftw/referencewidget/tests/__init__.py
+-rw-r--r--   0 maethu     (501) staff       (20)      386 2024-05-13 18:58:07.000000 ftw.referencewidget-4.0.2/ftw/referencewidget/tests/builders.py
+-rw-r--r--   0 maethu     (501) staff       (20)     1717 2024-05-13 18:58:07.000000 ftw.referencewidget-4.0.2/ftw/referencewidget/tests/test_change_widget_config.py
+-rw-r--r--   0 maethu     (501) staff       (20)     1738 2024-05-13 18:58:07.000000 ftw.referencewidget-4.0.2/ftw/referencewidget/tests/test_converter.py
+-rw-r--r--   0 maethu     (501) staff       (20)     1357 2024-05-13 18:58:07.000000 ftw.referencewidget-4.0.2/ftw/referencewidget/tests/test_datagrid_field.py
+-rw-r--r--   0 maethu     (501) staff       (20)     1335 2024-05-13 18:58:07.000000 ftw.referencewidget-4.0.2/ftw/referencewidget/tests/test_override.py
+-rw-r--r--   0 maethu     (501) staff       (20)     4369 2024-05-13 18:58:07.000000 ftw.referencewidget-4.0.2/ftw/referencewidget/tests/test_related_items_behavior.py
+-rw-r--r--   0 maethu     (501) staff       (20)     4937 2024-05-13 18:58:07.000000 ftw.referencewidget-4.0.2/ftw/referencewidget/tests/test_relation_choice.py
+-rw-r--r--   0 maethu     (501) staff       (20)     3956 2024-05-13 18:58:07.000000 ftw.referencewidget-4.0.2/ftw/referencewidget/tests/test_source.py
+-rw-r--r--   0 maethu     (501) staff       (20)      293 2024-05-13 18:58:07.000000 ftw.referencewidget-4.0.2/ftw/referencewidget/tests/test_uninstall.py
+-rw-r--r--   0 maethu     (501) staff       (20)     2565 2024-05-13 18:58:07.000000 ftw.referencewidget-4.0.2/ftw/referencewidget/tests/test_utils.py
+drwxr-xr-x   0 maethu     (501) staff       (20)        0 2024-05-13 18:58:07.583932 ftw.referencewidget-4.0.2/ftw/referencewidget/tests/views/
+-rw-r--r--   0 maethu     (501) staff       (20)        0 2024-05-13 18:58:07.000000 ftw.referencewidget-4.0.2/ftw/referencewidget/tests/views/__init__.py
+-rw-r--r--   0 maethu     (501) staff       (20)      319 2024-05-13 18:58:07.000000 ftw.referencewidget-4.0.2/ftw/referencewidget/tests/views/configure.zcml
+-rw-r--r--   0 maethu     (501) staff       (20)     1275 2024-05-13 18:58:07.000000 ftw.referencewidget-4.0.2/ftw/referencewidget/tests/views/form.py
+-rw-r--r--   0 maethu     (501) staff       (20)     1472 2024-05-13 18:58:07.000000 ftw.referencewidget-4.0.2/ftw/referencewidget/tests/widgets.py
+drwxr-xr-x   0 maethu     (501) staff       (20)        0 2024-05-13 18:58:07.584044 ftw.referencewidget-4.0.2/ftw/referencewidget/upgrades/
+drwxr-xr-x   0 maethu     (501) staff       (20)        0 2024-05-13 18:58:07.584366 ftw.referencewidget-4.0.2/ftw/referencewidget/upgrades/20181112105705_fix_registry_field_frontend_edit/
+-rw-r--r--   0 maethu     (501) staff       (20)        0 2024-05-13 18:58:07.000000 ftw.referencewidget-4.0.2/ftw/referencewidget/upgrades/20181112105705_fix_registry_field_frontend_edit/__init__.py
+-rw-r--r--   0 maethu     (501) staff       (20)      122 2024-05-13 18:58:07.000000 ftw.referencewidget-4.0.2/ftw/referencewidget/upgrades/20181112105705_fix_registry_field_frontend_edit/registry.xml
+-rw-r--r--   0 maethu     (501) staff       (20)      200 2024-05-13 18:58:07.000000 ftw.referencewidget-4.0.2/ftw/referencewidget/upgrades/20181112105705_fix_registry_field_frontend_edit/upgrade.py
+drwxr-xr-x   0 maethu     (501) staff       (20)        0 2024-05-13 18:58:07.584750 ftw.referencewidget-4.0.2/ftw/referencewidget/upgrades/20200115110839_restrict_handle_bars_to_authenticated_users/
+-rw-r--r--   0 maethu     (501) staff       (20)        0 2024-05-13 18:58:07.000000 ftw.referencewidget-4.0.2/ftw/referencewidget/upgrades/20200115110839_restrict_handle_bars_to_authenticated_users/__init__.py
+-rw-r--r--   0 maethu     (501) staff       (20)      286 2024-05-13 18:58:07.000000 ftw.referencewidget-4.0.2/ftw/referencewidget/upgrades/20200115110839_restrict_handle_bars_to_authenticated_users/jsregistry.xml
+-rw-r--r--   0 maethu     (501) staff       (20)      354 2024-05-13 18:58:07.000000 ftw.referencewidget-4.0.2/ftw/referencewidget/upgrades/20200115110839_restrict_handle_bars_to_authenticated_users/upgrade.py
+drwxr-xr-x   0 maethu     (501) staff       (20)        0 2024-05-13 18:58:07.585145 ftw.referencewidget-4.0.2/ftw/referencewidget/upgrades/20201215183140_fix_js_bundle_for_plone_5/
+-rw-r--r--   0 maethu     (501) staff       (20)        0 2024-05-13 18:58:07.000000 ftw.referencewidget-4.0.2/ftw/referencewidget/upgrades/20201215183140_fix_js_bundle_for_plone_5/__init__.py
+-rw-r--r--   0 maethu     (501) staff       (20)      350 2024-05-13 18:58:07.000000 ftw.referencewidget-4.0.2/ftw/referencewidget/upgrades/20201215183140_fix_js_bundle_for_plone_5/registry.xml
+-rw-r--r--   0 maethu     (501) staff       (20)      314 2024-05-13 18:58:07.000000 ftw.referencewidget-4.0.2/ftw/referencewidget/upgrades/20201215183140_fix_js_bundle_for_plone_5/upgrade.py
+-rw-r--r--   0 maethu     (501) staff       (20)        0 2024-05-13 18:58:07.000000 ftw.referencewidget-4.0.2/ftw/referencewidget/upgrades/__init__.py
+-rw-r--r--   0 maethu     (501) staff       (20)      485 2024-05-13 18:58:07.000000 ftw.referencewidget-4.0.2/ftw/referencewidget/utils.py
+-rw-r--r--   0 maethu     (501) staff       (20)     8721 2024-05-13 18:58:07.000000 ftw.referencewidget-4.0.2/ftw/referencewidget/widget.py
+drwxr-xr-x   0 maethu     (501) staff       (20)        0 2024-05-13 18:58:07.577441 ftw.referencewidget-4.0.2/ftw.referencewidget.egg-info/
+-rw-r--r--   0 maethu     (501) staff       (20)    15782 2024-05-13 18:58:07.000000 ftw.referencewidget-4.0.2/ftw.referencewidget.egg-info/PKG-INFO
+-rw-r--r--   0 maethu     (501) staff       (20)     3615 2024-05-13 18:58:07.000000 ftw.referencewidget-4.0.2/ftw.referencewidget.egg-info/SOURCES.txt
+-rw-r--r--   0 maethu     (501) staff       (20)        1 2024-05-13 18:58:07.000000 ftw.referencewidget-4.0.2/ftw.referencewidget.egg-info/dependency_links.txt
+-rw-r--r--   0 maethu     (501) staff       (20)       42 2024-05-13 18:58:07.000000 ftw.referencewidget-4.0.2/ftw.referencewidget.egg-info/entry_points.txt
+-rw-r--r--   0 maethu     (501) staff       (20)        4 2024-05-13 18:58:07.000000 ftw.referencewidget-4.0.2/ftw.referencewidget.egg-info/namespace_packages.txt
+-rw-r--r--   0 maethu     (501) staff       (20)        1 2024-05-13 18:58:07.000000 ftw.referencewidget-4.0.2/ftw.referencewidget.egg-info/not-zip-safe
+-rw-r--r--   0 maethu     (501) staff       (20)      361 2024-05-13 18:58:07.000000 ftw.referencewidget-4.0.2/ftw.referencewidget.egg-info/requires.txt
+-rw-r--r--   0 maethu     (501) staff       (20)        4 2024-05-13 18:58:07.000000 ftw.referencewidget-4.0.2/ftw.referencewidget.egg-info/top_level.txt
+-rw-r--r--   0 maethu     (501) staff       (20)      191 2024-05-13 18:58:07.000000 ftw.referencewidget-4.0.2/requirements_barebone.txt
+-rw-r--r--   0 maethu     (501) staff       (20)       38 2024-05-13 18:58:07.585583 ftw.referencewidget-4.0.2/setup.cfg
+-rw-r--r--   0 maethu     (501) staff       (20)     1895 2024-05-13 18:58:07.000000 ftw.referencewidget-4.0.2/setup.py
```

### Comparing `ftw.referencewidget-4.0.1/PKG-INFO` & `ftw.referencewidget-4.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ftw.referencewidget
-Version: 4.0.1
+Version: 4.0.2
 Summary: A reference browser widget (Maintainer Mathias Leimgruber)
 Home-page: https://github.com/webcloud7/ftw.referencewidget
 Author: Mathias Leimgruber, webcloud7 ag
 Author-email: mailto:info@webcloud7.ch
 Maintainer: Mathias Leimgruber
 License: GPL2
 Keywords: webcloud7 widget reference browser
@@ -53,24 +53,14 @@
 - Install the default generic import profile.
 
 
 
 Installation / Development
 --------------------------
 
-Option 1 - Using buildout
-
-.. code:: sh
-
-    $ ./bootstrap.sh development.cfg
-    $ ./bin/instance fg
-
-
-Option 2 - Using Makefile
-
 .. code:: sh
 
     $ make install
     $ make run
 
 
 We support both option since the makefile approach does not support yet all the features
@@ -211,14 +201,22 @@
 
 ``ftw.referencewidget`` is licensed under GNU General Public License, version 2.
 
 Changelog
 =========
 
 
+4.0.2 (2024-05-13)
+------------------
+
+- Test against Plone 6.0.9 [mathias.leimgruber]
+- Remove buildout based setup [mathias.leimgruber]
+- Remove FakeEditView for plone root [mathias.leimgruber]
+
+
 4.0.1 (2023-06-09)
 ------------------
 
 - Fix pagination querystring duplicates [mathias.leimgruber]
 
 
 4.0.0 (2023-05-30)
```

### Comparing `ftw.referencewidget-4.0.1/README.rst` & `ftw.referencewidget-4.0.2/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -32,24 +32,14 @@
 - Install the default generic import profile.
 
 
 
 Installation / Development
 --------------------------
 
-Option 1 - Using buildout
-
-.. code:: sh
-
-    $ ./bootstrap.sh development.cfg
-    $ ./bin/instance fg
-
-
-Option 2 - Using Makefile
-
 .. code:: sh
 
     $ make install
     $ make run
 
 
 We support both option since the makefile approach does not support yet all the features
```

### Comparing `ftw.referencewidget-4.0.1/docs/HISTORY.txt` & `ftw.referencewidget-4.0.2/docs/HISTORY.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 Changelog
 =========
 
 
+4.0.2 (2024-05-13)
+------------------
+
+- Test against Plone 6.0.9 [mathias.leimgruber]
+- Remove buildout based setup [mathias.leimgruber]
+- Remove FakeEditView for plone root [mathias.leimgruber]
+
+
 4.0.1 (2023-06-09)
 ------------------
 
 - Fix pagination querystring duplicates [mathias.leimgruber]
 
 
 4.0.0 (2023-05-30)
```

### Comparing `ftw.referencewidget-4.0.1/docs/LICENSE.GPL` & `ftw.referencewidget-4.0.2/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `ftw.referencewidget-4.0.1/docs/LICENSE.txt` & `ftw.referencewidget-4.0.2/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ftw.referencewidget-4.0.1/docs/static/list.png` & `ftw.referencewidget-4.0.2/docs/static/list.png`

 * *Files identical despite different names*

### Comparing `ftw.referencewidget-4.0.1/docs/static/search.png` & `ftw.referencewidget-4.0.2/docs/static/search.png`

 * *Files identical despite different names*

### Comparing `ftw.referencewidget-4.0.1/docs/static/selected.png` & `ftw.referencewidget-4.0.2/docs/static/selected.png`

 * *Files identical despite different names*

### Comparing `ftw.referencewidget-4.0.1/ftw/referencewidget/behaviors.py` & `ftw.referencewidget-4.0.2/ftw/referencewidget/behaviors.py`

 * *Files identical despite different names*

### Comparing `ftw.referencewidget-4.0.1/ftw/referencewidget/browser/utils.py` & `ftw.referencewidget-4.0.2/ftw/referencewidget/browser/utils.py`

 * *Files identical despite different names*

### Comparing `ftw.referencewidget-4.0.1/ftw/referencewidget/configure.zcml` & `ftw.referencewidget-4.0.2/ftw/referencewidget/configure.zcml`

 * *Files identical despite different names*

### Comparing `ftw.referencewidget-4.0.1/ftw/referencewidget/converter.py` & `ftw.referencewidget-4.0.2/ftw/referencewidget/converter.py`

 * *Files identical despite different names*

### Comparing `ftw.referencewidget-4.0.1/ftw/referencewidget/datagridfield.py` & `ftw.referencewidget-4.0.2/ftw/referencewidget/datagridfield.py`

 * *Files identical despite different names*

### Comparing `ftw.referencewidget-4.0.1/ftw/referencewidget/interfaces.py` & `ftw.referencewidget-4.0.2/ftw/referencewidget/interfaces.py`

 * *Files identical despite different names*

### Comparing `ftw.referencewidget-4.0.1/ftw/referencewidget/locales/de/LC_MESSAGES/ftw.referencewidget.po` & `ftw.referencewidget-4.0.2/ftw/referencewidget/locales/de/LC_MESSAGES/ftw.referencewidget.po`

 * *Files identical despite different names*

### Comparing `ftw.referencewidget-4.0.1/ftw/referencewidget/locales/ftw.referencewidget.pot` & `ftw.referencewidget-4.0.2/ftw/referencewidget/locales/ftw.referencewidget.pot`

 * *Files identical despite different names*

### Comparing `ftw.referencewidget-4.0.1/ftw/referencewidget/resources/dist/referencewidget.es.js` & `ftw.referencewidget-4.0.2/ftw/referencewidget/resources/dist/referencewidget.es.js`

 * *Files identical despite different names*

### Comparing `ftw.referencewidget-4.0.1/ftw/referencewidget/resources/dist/referencewidget.umd.js` & `ftw.referencewidget-4.0.2/ftw/referencewidget/resources/dist/referencewidget.umd.js`

 * *Files identical despite different names*

### Comparing `ftw.referencewidget-4.0.1/ftw/referencewidget/resources/src/main.js` & `ftw.referencewidget-4.0.2/ftw/referencewidget/resources/src/main.js`

 * *Files identical despite different names*

### Comparing `ftw.referencewidget-4.0.1/ftw/referencewidget/resources/src/widget/App.vue` & `ftw.referencewidget-4.0.2/ftw/referencewidget/resources/src/widget/App.vue`

 * *Files identical despite different names*

### Comparing `ftw.referencewidget-4.0.1/ftw/referencewidget/resources/src/widget/components/Breadcrumbs.vue` & `ftw.referencewidget-4.0.2/ftw/referencewidget/resources/src/widget/components/Breadcrumbs.vue`

 * *Files identical despite different names*

### Comparing `ftw.referencewidget-4.0.1/ftw/referencewidget/resources/src/widget/components/ListItems.vue` & `ftw.referencewidget-4.0.2/ftw/referencewidget/resources/src/widget/components/ListItems.vue`

 * *Files identical despite different names*

### Comparing `ftw.referencewidget-4.0.1/ftw/referencewidget/resources/src/widget/components/Pagination.vue` & `ftw.referencewidget-4.0.2/ftw/referencewidget/resources/src/widget/components/Pagination.vue`

 * *Files identical despite different names*

### Comparing `ftw.referencewidget-4.0.1/ftw/referencewidget/resources/src/widget/components/ResolveIcon.vue` & `ftw.referencewidget-4.0.2/ftw/referencewidget/resources/src/widget/components/ResolveIcon.vue`

 * *Files identical despite different names*

### Comparing `ftw.referencewidget-4.0.1/ftw/referencewidget/resources/src/widget/components/searchForm.vue` & `ftw.referencewidget-4.0.2/ftw/referencewidget/resources/src/widget/components/searchForm.vue`

 * *Files identical despite different names*

### Comparing `ftw.referencewidget-4.0.1/ftw/referencewidget/selectable.py` & `ftw.referencewidget-4.0.2/ftw/referencewidget/selectable.py`

 * *Files identical despite different names*

### Comparing `ftw.referencewidget-4.0.1/ftw/referencewidget/sources.py` & `ftw.referencewidget-4.0.2/ftw/referencewidget/sources.py`

 * *Files identical despite different names*

### Comparing `ftw.referencewidget-4.0.1/ftw/referencewidget/templates/referencewidget_display.pt` & `ftw.referencewidget-4.0.2/ftw/referencewidget/templates/referencewidget_display.pt`

 * *Files identical despite different names*

### Comparing `ftw.referencewidget-4.0.1/ftw/referencewidget/templates/referencewidget_input.pt` & `ftw.referencewidget-4.0.2/ftw/referencewidget/templates/referencewidget_input.pt`

 * *Files identical despite different names*

### Comparing `ftw.referencewidget-4.0.1/ftw/referencewidget/testing.py` & `ftw.referencewidget-4.0.2/ftw/referencewidget/testing.py`

 * *Files identical despite different names*

### Comparing `ftw.referencewidget-4.0.1/ftw/referencewidget/tests/__init__.py` & `ftw.referencewidget-4.0.2/ftw/referencewidget/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `ftw.referencewidget-4.0.1/ftw/referencewidget/tests/test_change_widget_config.py` & `ftw.referencewidget-4.0.2/ftw/referencewidget/tests/test_change_widget_config.py`

 * *Files identical despite different names*

### Comparing `ftw.referencewidget-4.0.1/ftw/referencewidget/tests/test_converter.py` & `ftw.referencewidget-4.0.2/ftw/referencewidget/tests/test_converter.py`

 * *Files identical despite different names*

### Comparing `ftw.referencewidget-4.0.1/ftw/referencewidget/tests/test_datagrid_field.py` & `ftw.referencewidget-4.0.2/ftw/referencewidget/tests/test_datagrid_field.py`

 * *Files identical despite different names*

### Comparing `ftw.referencewidget-4.0.1/ftw/referencewidget/tests/test_override.py` & `ftw.referencewidget-4.0.2/ftw/referencewidget/tests/test_override.py`

 * *Files identical despite different names*

### Comparing `ftw.referencewidget-4.0.1/ftw/referencewidget/tests/test_related_items_behavior.py` & `ftw.referencewidget-4.0.2/ftw/referencewidget/tests/test_related_items_behavior.py`

 * *Files identical despite different names*

### Comparing `ftw.referencewidget-4.0.1/ftw/referencewidget/tests/test_relation_choice.py` & `ftw.referencewidget-4.0.2/ftw/referencewidget/tests/test_relation_choice.py`

 * *Files identical despite different names*

### Comparing `ftw.referencewidget-4.0.1/ftw/referencewidget/tests/test_source.py` & `ftw.referencewidget-4.0.2/ftw/referencewidget/tests/test_source.py`

 * *Files identical despite different names*

### Comparing `ftw.referencewidget-4.0.1/ftw/referencewidget/tests/test_utils.py` & `ftw.referencewidget-4.0.2/ftw/referencewidget/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ftw.referencewidget-4.0.1/ftw/referencewidget/tests/views/form.py` & `ftw.referencewidget-4.0.2/ftw/referencewidget/tests/views/form.py`

 * *Files identical despite different names*

### Comparing `ftw.referencewidget-4.0.1/ftw/referencewidget/tests/widgets.py` & `ftw.referencewidget-4.0.2/ftw/referencewidget/tests/widgets.py`

 * *Files identical despite different names*

### Comparing `ftw.referencewidget-4.0.1/ftw/referencewidget/widget.py` & `ftw.referencewidget-4.0.2/ftw/referencewidget/widget.py`

 * *Files identical despite different names*

### Comparing `ftw.referencewidget-4.0.1/ftw.referencewidget.egg-info/PKG-INFO` & `ftw.referencewidget-4.0.2/ftw.referencewidget.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ftw.referencewidget
-Version: 4.0.1
+Version: 4.0.2
 Summary: A reference browser widget (Maintainer Mathias Leimgruber)
 Home-page: https://github.com/webcloud7/ftw.referencewidget
 Author: Mathias Leimgruber, webcloud7 ag
 Author-email: mailto:info@webcloud7.ch
 Maintainer: Mathias Leimgruber
 License: GPL2
 Keywords: webcloud7 widget reference browser
@@ -53,24 +53,14 @@
 - Install the default generic import profile.
 
 
 
 Installation / Development
 --------------------------
 
-Option 1 - Using buildout
-
-.. code:: sh
-
-    $ ./bootstrap.sh development.cfg
-    $ ./bin/instance fg
-
-
-Option 2 - Using Makefile
-
 .. code:: sh
 
     $ make install
     $ make run
 
 
 We support both option since the makefile approach does not support yet all the features
@@ -211,14 +201,22 @@
 
 ``ftw.referencewidget`` is licensed under GNU General Public License, version 2.
 
 Changelog
 =========
 
 
+4.0.2 (2024-05-13)
+------------------
+
+- Test against Plone 6.0.9 [mathias.leimgruber]
+- Remove buildout based setup [mathias.leimgruber]
+- Remove FakeEditView for plone root [mathias.leimgruber]
+
+
 4.0.1 (2023-06-09)
 ------------------
 
 - Fix pagination querystring duplicates [mathias.leimgruber]
 
 
 4.0.0 (2023-05-30)
```

### Comparing `ftw.referencewidget-4.0.1/ftw.referencewidget.egg-info/SOURCES.txt` & `ftw.referencewidget-4.0.2/ftw.referencewidget.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 MANIFEST.in
 README.rst
 constraints.txt
-requirements.txt
 requirements_barebone.txt
 setup.py
 docs/HISTORY.txt
 docs/LICENSE.GPL
 docs/LICENSE.txt
 docs/static/list.png
 docs/static/search.png
@@ -30,15 +29,14 @@
 ftw/referencewidget/sources.py
 ftw/referencewidget/testing.py
 ftw/referencewidget/utils.py
 ftw/referencewidget/widget.py
 ftw/referencewidget/Extensions/install.py
 ftw/referencewidget/browser/__init__.py
 ftw/referencewidget/browser/configure.zcml
-ftw/referencewidget/browser/fake_edit.py
 ftw/referencewidget/browser/utils.py
 ftw/referencewidget/locales/ftw.referencewidget.pot
 ftw/referencewidget/locales/de/LC_MESSAGES/ftw.referencewidget.po
 ftw/referencewidget/profiles/default/metadata.xml
 ftw/referencewidget/profiles/default/registry.xml
 ftw/referencewidget/profiles/uninstall/registry.xml
 ftw/referencewidget/resources/dist/referencewidget.es.js
```

### Comparing `ftw.referencewidget-4.0.1/setup.py` & `ftw.referencewidget-4.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 import os
 
-version = '4.0.1'
+version = '4.0.2'
 maintainer = 'Mathias Leimgruber'
 
 tests_require = [
     'collective.z3cform.datagridfield',
     'plone.app.testing',
     'ftw.builder',
     'ftw.testing',
```

