# Comparing `tmp/netbox_inventory-2.0.0.tar.gz` & `tmp/netbox_inventory-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox_inventory-2.0.0.tar", last modified: Thu May  9 15:09:56 2024, max compression
+gzip compressed data, was "netbox_inventory-2.0.1.tar", last modified: Mon May 13 10:29:30 2024, max compression
```

## Comparing `netbox_inventory-2.0.0.tar` & `netbox_inventory-2.0.1.tar`

### file list

```diff
@@ -1,121 +1,115 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:09:56.930429 netbox_inventory-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9497 2024-05-09 15:09:56.930429 netbox_inventory-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8918 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:09:56.918429 netbox_inventory-2.0.0/netbox_inventory/
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/analyzers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:09:56.918429 netbox_inventory-2.0.0/netbox_inventory/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/api/nested_serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6882 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/api/views.py
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/choices.py
--rw-r--r--   0 runner    (1001) docker     (127)    15610 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/filtersets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:09:56.918429 netbox_inventory-2.0.0/netbox_inventory/forms/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7030 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/forms/assign.py
--rw-r--r--   0 runner    (1001) docker     (127)    22130 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/forms/bulk.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/forms/bulk_add.py
--rw-r--r--   0 runner    (1001) docker     (127)     4770 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/forms/create.py
--rw-r--r--   0 runner    (1001) docker     (127)    11075 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/forms/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     8479 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/forms/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     8756 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/forms/reassign.py
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/graphql.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:09:56.914429 netbox_inventory-2.0.0/netbox_inventory/management/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:09:56.922429 netbox_inventory-2.0.0/netbox_inventory/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/management/commands/check_asset_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:09:56.922429 netbox_inventory-2.0.0/netbox_inventory/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     6962 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/migrations/0001_initial_prod.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/migrations/0002_alter_asset_serial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/migrations/0003_add_inventoryitemgroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/migrations/0004_inventoryitemgroup_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/migrations/0005_delivery_asset_delivery.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/migrations/0006_purchase_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/migrations/0007_alter_asset_unique_together_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19653 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4771 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/navigation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/signals.py
--rw-r--r--   0 runner    (1001) docker     (127)    14414 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     6977 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/template_content.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:09:56.914429 netbox_inventory-2.0.0/netbox_inventory/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:09:56.922429 netbox_inventory-2.0.0/netbox_inventory/templates/netbox_inventory/
--rw-r--r--   0 runner    (1001) docker     (127)     7390 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/templates/netbox_inventory/asset.html
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/templates/netbox_inventory/asset_assign.html
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/templates/netbox_inventory/asset_bulk_add.html
--rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/templates/netbox_inventory/asset_bulk_import.html
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/templates/netbox_inventory/asset_create.html
--rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/templates/netbox_inventory/asset_edit.html
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/templates/netbox_inventory/asset_reassign.html
--rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/templates/netbox_inventory/delivery.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:09:56.926429 netbox_inventory-2.0.0/netbox_inventory/templates/netbox_inventory/inc/
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/templates/netbox_inventory/inc/asset_edit_header.html
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/templates/netbox_inventory/inc/asset_info.html
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/templates/netbox_inventory/inc/asset_stats_counts.html
--rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/templates/netbox_inventory/inventoryitemgroup.html
--rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/templates/netbox_inventory/inventoryitemtype.html
--rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/templates/netbox_inventory/purchase.html
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/templates/netbox_inventory/supplier.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:09:56.926429 netbox_inventory-2.0.0/netbox_inventory/templates/netbox_inventory/tabs/
--rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/templates/netbox_inventory/tabs/located_assets_base.html
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/templates/netbox_inventory/tabs/located_assets_location.html
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/templates/netbox_inventory/tabs/located_assets_rack.html
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/templates/netbox_inventory/tabs/located_assets_site.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:09:56.926429 netbox_inventory-2.0.0/netbox_inventory/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:09:56.926429 netbox_inventory-2.0.0/netbox_inventory/tests/asset/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/tests/asset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7853 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/tests/asset/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7738 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/tests/asset/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     7311 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/tests/asset/test_views.py
--rw-r--r--   0 runner    (1001) docker     (127)     7709 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/tests/asset/test_views_create.py
--rw-r--r--   0 runner    (1001) docker     (127)    11317 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/tests/asset/test_views_reassign.py
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/tests/custom.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:09:56.926429 netbox_inventory-2.0.0/netbox_inventory/tests/delivery/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/tests/delivery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/tests/delivery/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/tests/delivery/test_views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:09:56.926429 netbox_inventory-2.0.0/netbox_inventory/tests/inventoryitem_group/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/tests/inventoryitem_group/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/tests/inventoryitem_group/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/tests/inventoryitem_group/test_views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:09:56.926429 netbox_inventory-2.0.0/netbox_inventory/tests/inventoryitem_type/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/tests/inventoryitem_type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/tests/inventoryitem_type/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/tests/inventoryitem_type/test_views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:09:56.930429 netbox_inventory-2.0.0/netbox_inventory/tests/purchase/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/tests/purchase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/tests/purchase/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/tests/purchase/test_views.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/tests/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:09:56.930429 netbox_inventory-2.0.0/netbox_inventory/tests/supplier/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/tests/supplier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/tests/supplier/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4538 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/tests/supplier/test_views.py
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/tests/test_load.py
--rw-r--r--   0 runner    (1001) docker     (127)     6987 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     6357 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:09:56.930429 netbox_inventory-2.0.0/netbox_inventory/views/
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8881 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/views/asset.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/views/asset_assign.py
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/views/asset_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/views/asset_reassign.py
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/views/delivery.py
--rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/views/inventoryitem_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/views/inventoryitem_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/views/purchase.py
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/views/supplier.py
--rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/views/tabs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:09:56.930429 netbox_inventory-2.0.0/netbox_inventory.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9497 2024-05-09 15:09:56.000000 netbox_inventory-2.0.0/netbox_inventory.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4357 2024-05-09 15:09:56.000000 netbox_inventory-2.0.0/netbox_inventory.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 15:09:56.000000 netbox_inventory-2.0.0/netbox_inventory.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-09 15:09:56.000000 netbox_inventory-2.0.0/netbox_inventory.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 15:09:56.930429 netbox_inventory-2.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:29:30.746802 netbox_inventory-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9497 2024-05-13 10:29:30.746802 netbox_inventory-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8918 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:29:30.734802 netbox_inventory-2.0.1/netbox_inventory/
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/analyzers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:29:30.734802 netbox_inventory-2.0.1/netbox_inventory/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/api/nested_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6882 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/choices.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15821 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/filtersets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:29:30.734802 netbox_inventory-2.0.1/netbox_inventory/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6978 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/forms/assign.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22130 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/forms/bulk.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/forms/bulk_add.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4770 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/forms/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11075 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/forms/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8479 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/forms/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8756 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/forms/reassign.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/graphql.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:29:30.730801 netbox_inventory-2.0.1/netbox_inventory/management/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:29:30.738802 netbox_inventory-2.0.1/netbox_inventory/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/management/commands/check_asset_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:29:30.738802 netbox_inventory-2.0.1/netbox_inventory/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     6962 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/migrations/0001_initial_prod.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/migrations/0002_alter_asset_serial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/migrations/0003_add_inventoryitemgroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/migrations/0004_inventoryitemgroup_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/migrations/0005_delivery_asset_delivery.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/migrations/0006_purchase_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/migrations/0007_alter_asset_unique_together_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19653 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4771 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/navigation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14414 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9228 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/template_content.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:29:30.730801 netbox_inventory-2.0.1/netbox_inventory/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:29:30.738802 netbox_inventory-2.0.1/netbox_inventory/templates/netbox_inventory/
+-rw-r--r--   0 runner    (1001) docker     (127)     7390 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/templates/netbox_inventory/asset.html
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/templates/netbox_inventory/asset_assign.html
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/templates/netbox_inventory/asset_bulk_add.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/templates/netbox_inventory/asset_bulk_import.html
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/templates/netbox_inventory/asset_create.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/templates/netbox_inventory/asset_edit.html
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/templates/netbox_inventory/asset_reassign.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/templates/netbox_inventory/delivery.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:29:30.738802 netbox_inventory-2.0.1/netbox_inventory/templates/netbox_inventory/inc/
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/templates/netbox_inventory/inc/asset_edit_header.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/templates/netbox_inventory/inc/asset_info.html
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/templates/netbox_inventory/inc/asset_stats_counts.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/templates/netbox_inventory/inventoryitemgroup.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/templates/netbox_inventory/inventoryitemtype.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/templates/netbox_inventory/purchase.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/templates/netbox_inventory/supplier.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:29:30.742802 netbox_inventory-2.0.1/netbox_inventory/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:29:30.742802 netbox_inventory-2.0.1/netbox_inventory/tests/asset/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/tests/asset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7853 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/tests/asset/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7738 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/tests/asset/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7311 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/tests/asset/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7709 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/tests/asset/test_views_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11317 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/tests/asset/test_views_reassign.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/tests/custom.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:29:30.742802 netbox_inventory-2.0.1/netbox_inventory/tests/delivery/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/tests/delivery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/tests/delivery/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/tests/delivery/test_views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:29:30.742802 netbox_inventory-2.0.1/netbox_inventory/tests/inventoryitem_group/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/tests/inventoryitem_group/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/tests/inventoryitem_group/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/tests/inventoryitem_group/test_views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:29:30.742802 netbox_inventory-2.0.1/netbox_inventory/tests/inventoryitem_type/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/tests/inventoryitem_type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/tests/inventoryitem_type/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/tests/inventoryitem_type/test_views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:29:30.742802 netbox_inventory-2.0.1/netbox_inventory/tests/purchase/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/tests/purchase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/tests/purchase/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/tests/purchase/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/tests/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:29:30.746802 netbox_inventory-2.0.1/netbox_inventory/tests/supplier/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/tests/supplier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/tests/supplier/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4538 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/tests/supplier/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/tests/test_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6987 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6357 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:29:30.746802 netbox_inventory-2.0.1/netbox_inventory/views/
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8881 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/views/asset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/views/asset_assign.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/views/asset_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/views/asset_reassign.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/views/delivery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/views/inventoryitem_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/views/inventoryitem_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/views/purchase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/netbox_inventory/views/supplier.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:29:30.746802 netbox_inventory-2.0.1/netbox_inventory.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9497 2024-05-13 10:29:30.000000 netbox_inventory-2.0.1/netbox_inventory.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4026 2024-05-13 10:29:30.000000 netbox_inventory-2.0.1/netbox_inventory.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 10:29:30.000000 netbox_inventory-2.0.1/netbox_inventory.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-13 10:29:30.000000 netbox_inventory-2.0.1/netbox_inventory.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-13 10:29:18.000000 netbox_inventory-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 10:29:30.746802 netbox_inventory-2.0.1/setup.cfg
```

### Comparing `netbox_inventory-2.0.0/LICENSE` & `netbox_inventory-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox_inventory-2.0.0/PKG-INFO` & `netbox_inventory-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-inventory
-Version: 2.0.0
+Version: 2.0.1
 Summary: Inventory asset management in NetBox
 Author-email: Matej Vadnjal <matej.vadnjal@arnes.si>
 Project-URL: Homepage, https://github.com/ArnesSI/netbox-inventory/
 Project-URL: Bug Tracker, https://github.com/ArnesSI/netbox-inventory/issues/
 Keywords: netbox,netbox-plugin,inventory
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `netbox_inventory-2.0.0/README.md` & `netbox_inventory-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `netbox_inventory-2.0.0/netbox_inventory/__init__.py` & `netbox_inventory-2.0.1/netbox_inventory/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-2.0.0/netbox_inventory/analyzers.py` & `netbox_inventory-2.0.1/netbox_inventory/analyzers.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-2.0.0/netbox_inventory/api/nested_serializers.py` & `netbox_inventory-2.0.1/netbox_inventory/api/nested_serializers.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-2.0.0/netbox_inventory/api/serializers.py` & `netbox_inventory-2.0.1/netbox_inventory/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-2.0.0/netbox_inventory/api/urls.py` & `netbox_inventory-2.0.1/netbox_inventory/api/urls.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-2.0.0/netbox_inventory/api/views.py` & `netbox_inventory-2.0.1/netbox_inventory/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-2.0.0/netbox_inventory/choices.py` & `netbox_inventory-2.0.1/netbox_inventory/choices.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-2.0.0/netbox_inventory/filtersets.py` & `netbox_inventory-2.0.1/netbox_inventory/filtersets.py`

 * *Files 1% similar despite different names*

```diff
@@ -420,14 +420,20 @@
 
 
 class InventoryItemGroupFilterSet(NetBoxModelFilterSet):
     parent_id = django_filters.ModelMultipleChoiceFilter(
         queryset=InventoryItemGroup.objects.all(),
         label='Parent group (ID)',
     )
+    ancestor_id = filters.TreeNodeMultipleChoiceFilter(
+        queryset=InventoryItemGroup.objects.all(),
+        field_name='parent',
+        lookup_expr='in',
+        label='Inventory item group (ID)',
+    )
 
     class Meta:
         model = InventoryItemGroup
         fields = (
             'id', 'name'
         )
```

### Comparing `netbox_inventory-2.0.0/netbox_inventory/forms/assign.py` & `netbox_inventory-2.0.1/netbox_inventory/forms/assign.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
             attrs={
                 'data-static-params': '[{"queryParam":"has_asset_assigned","queryValue":"false"}]',
             },
         )
     )
 
     fieldsets = (
-        FieldSet('device_type', 'name', name='Asset'),
+        FieldSet('name', name='Asset'),
         FieldSet('site', 'device', name='Device'),
         FieldSet('tenant', 'contact', name='Assigned to'),
     )
 
     class Meta:
         model = Asset
         fields = ('device_type', 'name', 'site', 'device', 'tenant', 'contact')
@@ -128,15 +128,15 @@
             attrs={
                 'data-static-params': '[{"queryParam":"has_asset_assigned","queryValue":"false"}]',
             },
         )
     )
 
     fieldsets = (
-        FieldSet('module_type', 'name', name='Asset'),
+        FieldSet('name', name='Asset'),
         FieldSet('device', 'module', name='Module'),
         FieldSet('tenant', 'contact', name='Tenancy'),
     )
 
     class Meta:
         model = Asset
         fields = ('module_type', 'name', 'device', 'module', 'tenant', 'contact')
@@ -172,15 +172,15 @@
             attrs={
                 'data-static-params': '[{"queryParam":"has_asset_assigned","queryValue":"false"}]',
             },
         )
     )
 
     fieldsets = (
-        FieldSet('inventoryitem_type', 'name', name='Asset'),
+        FieldSet('name', name='Asset'),
         FieldSet('device', 'inventoryitem', name='Inventory Item'),
         FieldSet('tenant', 'contact', name='Tenancy'),
     )
 
     class Meta:
         model = Asset
         fields = ('inventoryitem_type', 'name', 'device', 'inventoryitem', 'tenant', 'contact')
```

### Comparing `netbox_inventory-2.0.0/netbox_inventory/forms/bulk.py` & `netbox_inventory-2.0.1/netbox_inventory/forms/bulk.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-2.0.0/netbox_inventory/forms/bulk_add.py` & `netbox_inventory-2.0.1/netbox_inventory/forms/bulk_add.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-2.0.0/netbox_inventory/forms/create.py` & `netbox_inventory-2.0.1/netbox_inventory/forms/create.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-2.0.0/netbox_inventory/forms/filters.py` & `netbox_inventory-2.0.1/netbox_inventory/forms/filters.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-2.0.0/netbox_inventory/forms/models.py` & `netbox_inventory-2.0.1/netbox_inventory/forms/models.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-2.0.0/netbox_inventory/forms/reassign.py` & `netbox_inventory-2.0.1/netbox_inventory/forms/reassign.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-2.0.0/netbox_inventory/graphql.py` & `netbox_inventory-2.0.1/netbox_inventory/graphql.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-2.0.0/netbox_inventory/management/commands/check_asset_tags.py` & `netbox_inventory-2.0.1/netbox_inventory/management/commands/check_asset_tags.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-2.0.0/netbox_inventory/migrations/0001_initial_prod.py` & `netbox_inventory-2.0.1/netbox_inventory/migrations/0001_initial_prod.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-2.0.0/netbox_inventory/migrations/0003_add_inventoryitemgroup.py` & `netbox_inventory-2.0.1/netbox_inventory/migrations/0003_add_inventoryitemgroup.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-2.0.0/netbox_inventory/migrations/0004_inventoryitemgroup_tree.py` & `netbox_inventory-2.0.1/netbox_inventory/migrations/0004_inventoryitemgroup_tree.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-2.0.0/netbox_inventory/migrations/0005_delivery_asset_delivery.py` & `netbox_inventory-2.0.1/netbox_inventory/migrations/0005_delivery_asset_delivery.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-2.0.0/netbox_inventory/migrations/0007_alter_asset_unique_together_and_more.py` & `netbox_inventory-2.0.1/netbox_inventory/migrations/0007_alter_asset_unique_together_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-2.0.0/netbox_inventory/models.py` & `netbox_inventory-2.0.1/netbox_inventory/models.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-2.0.0/netbox_inventory/navigation.py` & `netbox_inventory-2.0.1/netbox_inventory/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-2.0.0/netbox_inventory/search.py` & `netbox_inventory-2.0.1/netbox_inventory/search.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-2.0.0/netbox_inventory/signals.py` & `netbox_inventory-2.0.1/netbox_inventory/signals.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-2.0.0/netbox_inventory/tables.py` & `netbox_inventory-2.0.1/netbox_inventory/tables.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-2.0.0/netbox_inventory/template_content.py` & `netbox_inventory-2.0.1/netbox_inventory/template_content.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from django.template import Template
 from netbox.plugins import PluginTemplateExtension
 
 from .models import Asset
+from .utils import query_located
 
 
 WARRANTY_PROGRESSBAR = '''
 {% with record.warranty_progress as wp %}
 {% with record.warranty_remaining as wr %}
 {% with settings.PLUGINS_CONFIG.netbox_inventory.asset_warranty_expire_warning_days as wthresh %}
 
@@ -74,14 +75,43 @@
                     'count': Asset.objects.restrict(user, 'view').filter(**{self.kind:object}).count(),
                 },
             ],
         }
         return self.render('netbox_inventory/inc/asset_stats_counts.html', extra_context=context)
 
 
+class AssetLocationStats(PluginTemplateExtension):
+    def right_page(self):
+        object = self.context.get('object')
+        user = self.context['request'].user
+        assets_qs = Asset.objects.restrict(user, 'view')
+        count_installed = query_located(assets_qs, self.location_type, [object.pk], assets_shown='installed').count()
+        count_stored = query_located(assets_qs, self.location_type, [object.pk], assets_shown='stored').count()
+        context = {
+            'asset_stats': [
+                {
+                    'label': 'Installed',
+                    'filter_field': f'installed_{self.location_type}_id',
+                    'count': count_installed,
+                },
+                {
+                    'label': 'Stored',
+                    'filter_field': f'storage_{self.location_type}_id',
+                    'count': count_stored,
+                },
+                {
+                    'label': 'Total',
+                    'filter_field': f'located_{self.location_type}_id',
+                    'count': count_installed + count_stored,
+                },
+            ],
+        }
+        return self.render('netbox_inventory/inc/asset_stats_counts.html', extra_context=context)
+
+
 class DeviceAssetInfo(AssetInfoExtension):
     model = 'dcim.device'
     kind = 'device'
 
 
 class ModuleAssetInfo(AssetInfoExtension):
     model = 'dcim.module'
@@ -137,14 +167,44 @@
                     'count': count_device + count_module + count_inventoryitem,
                 },
             ],
         }
         return self.render('netbox_inventory/inc/asset_stats_counts.html', extra_context=context)
 
 
+class SiteAssetInfo(AssetLocationStats):
+    model = 'dcim.site'
+    location_type='site'
+
+
+class LocationAssetInfo(AssetLocationStats):
+    model = 'dcim.location'
+    location_type='location'
+
+
+class RackAssetInfo(PluginTemplateExtension):
+    # rack cannot have stored assets so we can't use AssetLocationStats
+    model = 'dcim.rack'
+    def right_page(self):
+        object = self.context.get('object')
+        user = self.context['request'].user
+        assets_qs = Asset.objects.restrict(user, 'view')
+        assets_qs = query_located(assets_qs, 'rack', [object.pk])
+        context = {
+            'asset_stats': [
+                {
+                    'label': 'Installed',
+                    'filter_field': 'installed_rack_id',
+                    'count': assets_qs.count(),
+                },
+            ],
+        }
+        return self.render('netbox_inventory/inc/asset_stats_counts.html', extra_context=context)
+
+
 class TenantAssetInfo(PluginTemplateExtension):
     model = 'tenancy.tenant'
     def right_page(self):
         object = self.context.get('object')
         user = self.context['request'].user
         context = {
             'asset_stats': [
@@ -183,10 +243,13 @@
 template_extensions = (
     DeviceAssetInfo,
     ModuleAssetInfo,
     InventoryItemAssetInfo,
     DeviceTypeAssetInfo,
     ModuleTypeAssetInfo,
     ManufacturerAssetInfo,
+    SiteAssetInfo,
+    LocationAssetInfo,
+    RackAssetInfo,
     TenantAssetInfo,
     ContactAssetInfo,
 )
```

### Comparing `netbox_inventory-2.0.0/netbox_inventory/templates/netbox_inventory/asset.html` & `netbox_inventory-2.0.1/netbox_inventory/templates/netbox_inventory/asset.html`

 * *Files identical despite different names*

### Comparing `netbox_inventory-2.0.0/netbox_inventory/templates/netbox_inventory/asset_bulk_import.html` & `netbox_inventory-2.0.1/netbox_inventory/templates/netbox_inventory/asset_bulk_import.html`

 * *Files identical despite different names*

### Comparing `netbox_inventory-2.0.0/netbox_inventory/templates/netbox_inventory/asset_edit.html` & `netbox_inventory-2.0.1/netbox_inventory/templates/netbox_inventory/asset_edit.html`

 * *Files identical despite different names*

### Comparing `netbox_inventory-2.0.0/netbox_inventory/templates/netbox_inventory/asset_reassign.html` & `netbox_inventory-2.0.1/netbox_inventory/templates/netbox_inventory/asset_reassign.html`

 * *Files identical despite different names*

### Comparing `netbox_inventory-2.0.0/netbox_inventory/templates/netbox_inventory/delivery.html` & `netbox_inventory-2.0.1/netbox_inventory/templates/netbox_inventory/delivery.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 {% extends 'generic/object.html' %}
 {% load helpers %}
 {% load plugins %}
-{% load render_table from django_tables2 %}
 
 {% block breadcrumbs %}
   {{ block.super }}
   <li class="breadcrumb-item">
     <a href="{% url 'plugins:netbox_inventory:delivery_list' %}?supplier_id={{ object.purchase.supplier.pk }}">{{ object.purchase.supplier }}</a>
   </li>
   <li class="breadcrumb-item">
```

#### html2text {}

```diff
@@ -1,10 +1,9 @@
 {% extends 'generic/object.html' %} {% load helpers %} {% load plugins %} {%
-load render_table from django_tables2 %} {% block breadcrumbs %} {{ block.super
-}}
+block breadcrumbs %} {{ block.super }}
 _{_{_ _o_b_j_e_c_t_._p_u_r_c_h_a_s_e_._s_u_p_p_l_i_e_r_ _}_}
 _{_{_ _o_b_j_e_c_t_._p_u_r_c_h_a_s_e_ _}_}
 {% endblock %} {% block content %}
 **** DDeelliivveerryy ****
 NNaammee              {{ object.name }}
 PPuurrcchhaassee          {{ object.purchase|linkify }}
 RReecceeiivviinngg CCoonnttaacctt {{ object.receiving_contact|linkify|placeholder }}
```

### Comparing `netbox_inventory-2.0.0/netbox_inventory/templates/netbox_inventory/inc/asset_edit_header.html` & `netbox_inventory-2.0.1/netbox_inventory/templates/netbox_inventory/inc/asset_edit_header.html`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 {% load helpers %}
+{# renders tab navbar for asset form #}
 
 <ul class="nav nav-tabs px-3">
   <li class="nav-item">
       <a
           class="nav-link {% if active_tab == 'add' %}active{% endif %}"
           href="{% url 'plugins:netbox_inventory:asset_add' %}{% querystring request %}"
       >
```

### Comparing `netbox_inventory-2.0.0/netbox_inventory/templates/netbox_inventory/inc/asset_info.html` & `netbox_inventory-2.0.1/netbox_inventory/templates/netbox_inventory/inc/asset_info.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 {% load helpers %}
+{# renders panel on object (device, module, inventory_item) with asset info assigned to it #}
 
 <div class="card">
   <h5 class="card-header">
     Asset
     {# only show reassign button if user has change permissions on asset #}
     {% if perms.netbox_inventory.change_asset %}
       <div class="card-actions">
```

#### html2text {}

```diff
@@ -1,8 +1,9 @@
-{% load helpers %}
+{% load helpers %} {# renders panel on object (device, module, inventory_item)
+with asset info assigned to it #}
 AAsssseett {{## oonnllyy sshhooww rreeaassssiiggnn bbuuttttoonn iiff uusseerr hhaass cchhaannggee ppeerrmmiissssiioonnss oonn aasssseett ##}}
 {{%% iiff ppeerrmmss..nneettbbooxx__iinnvveennttoorryy..cchhaannggee__aasssseett %%}}
 {{%% wwiitthh oobbjjeecctt||mmeettaa::""mmooddeell__nnaammee"" aass oobbjjeecctt__ttyyppee %%}} {{%% iiff oobbjjeecctt__ttyyppee ====
 ""ddeevviiccee"" %%}}
 _{{_%%_ _ee_ll_ii_ff_ _oo_bb_jj_ee_cc_tt____tt_yy_pp_ee_ _==_==_ _""_mm_oo_dd_uu_ll_ee_""_ _%%_}}
 _{{_%%_ _ee_ll_ii_ff_ _oo_bb_jj_ee_cc_tt____tt_yy_pp_ee_ _==_==_ _""_ii_nn_vv_ee_nn_tt_oo_rr_yy_ii_tt_ee_mm_""_ _%%_}}
 _{{_%%_ _ee_nn_dd_ii_ff_ _%%_}}_ _{{_%%_ _ee_nn_dd_ww_ii_tt_hh_ _%%_}}_ _EE_dd_ii_tt_ _AA_ss_ss_ii_gg_nn_mm_ee_nn_tt
```

### Comparing `netbox_inventory-2.0.0/netbox_inventory/templates/netbox_inventory/inc/asset_stats_counts.html` & `netbox_inventory-2.0.1/netbox_inventory/templates/netbox_inventory/inc/asset_stats_counts.html`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 {% load helpers %}
+{# renders panel simmilar to Related Objects with counts of assets related to object #}
 
 <div class="card">
   <h5 class="card-header">Assets</h5>
   <ul class="list-group list-group-flush">
     {% for asset_stat in asset_stats %}
       <a href="{% url 'plugins:netbox_inventory:asset_list' %}?{{ asset_stat.filter_field }}={{ object.pk }}{{ asset_stat.extra_filter }}" class="list-group-item list-group-item-action d-flex justify-content-between">
         {{ asset_stat.label|bettertitle }}
```

#### html2text {}

```diff
@@ -1,5 +1,6 @@
-{% load helpers %}
+{% load helpers %} {# renders panel simmilar to Related Objects with counts of
+assets related to object #}
 **** AAsssseettss ****
     * {% for asset_stat in asset_stats %} _{_{_ _a_s_s_e_t___s_t_a_t_._l_a_b_e_l_|_b_e_t_t_e_r_t_i_t_l_e_ _}_}_ _{_%
       _i_f_ _a_s_s_e_t___s_t_a_t_._c_o_u_n_t_ _%_}_ _{_{_ _a_s_s_e_t___s_t_a_t_._c_o_u_n_t_ _}_}_ _{_%_ _e_l_s_e_ _%_}_ _—_ _{_%_ _e_n_d_i_f_ _%_}
 {% endfor %}
```

### Comparing `netbox_inventory-2.0.0/netbox_inventory/templates/netbox_inventory/inventoryitemgroup.html` & `netbox_inventory-2.0.1/netbox_inventory/templates/netbox_inventory/inventoryitemgroup.html`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 {% extends 'generic/object.html' %}
 {% load helpers %}
 {% load plugins %}
-{% load render_table from django_tables2 %}
 
 {% block breadcrumbs %}
   {{ block.super }}
   {% for group in object.get_ancestors %}
     <li class="breadcrumb-item"><a href="{% url 'plugins:netbox_inventory:inventoryitemgroup' group.pk %}">{{ group }}</a></li>
   {% endfor %}
 {% endblock %}
@@ -112,25 +111,24 @@
             <div class="card-actions">
               <a href="{% url 'plugins:netbox_inventory:inventoryitemgroup_add' %}?parent={{ object.pk }}&return_url={{ object.get_absolute_url }}" class="btn btn-ghost-primary btn-sm">
                 <i class="mdi mdi-plus-thick" aria-hidden="true"></i> Add Group
               </a>
             </div>
           {% endif %}
         </h5>
-        {% render_table child_groups_table 'inc/table.html' %}
+        {% htmx_table 'plugins:netbox_inventory:inventoryitemgroup_list' ancestor_id=object.pk %}
       </div>
       {% include 'inc/panels/tags.html' %}
       {% include 'inc/panels/comments.html' %}
       {% plugin_right_page object %}
     </div>
   </div>
   <div class="row mb-3">
     <div class="col col-md-12">
       <div class="card">
         <h5 class="card-header">Assets</h5>
-        {% render_table asset_table 'inc/table.html' %}
-        {% include 'inc/paginator.html' with paginator=asset_table.paginator page=asset_table.page %}
+        {% htmx_table 'plugins:netbox_inventory:asset_list' inventoryitem_group_id=object.pk %}
       </div>
       {% plugin_full_width_page object %}
     </div>
   </div>
 {% endblock content %}
```

#### html2text {}

```diff
@@ -1,10 +1,9 @@
 {% extends 'generic/object.html' %} {% load helpers %} {% load plugins %} {%
-load render_table from django_tables2 %} {% block breadcrumbs %} {{ block.super
-}} {% for group in object.get_ancestors %}
+block breadcrumbs %} {{ block.super }} {% for group in object.get_ancestors %}
 _{_{_ _g_r_o_u_p_ _}_}
 {% endfor %} {% endblock %} {% block extra_controls %} {% if
 perms.netbox_inventory.add_inventoryitemtype %}
 _A_d_d_ _i_n_v_e_n_t_o_r_y_ _i_t_e_m_ _t_y_p_e
 {% endif %} {% endblock extra_controls %} {% block content %}
 **** IInnvveennttoorryy IItteemm GGrroouupp ****
 NNaammee   {{ object.name }}
@@ -23,15 +22,16 @@
 _}_}_ _{_{_ _t_s_c_._i_n_v_e_n_t_o_r_y_i_t_e_m___t_y_p_e_____m_o_d_e_l_ _}_}     _b_g___c_o_l_o_r_=_s_t_a_t_u_s_._c_o_l_o_r_|_a_d_d_:_'_ _w_-_1_0_0_'
                                            _%_}_ {% endfor %}
 â No assets found â
 {% plugin_left_page object %}
 CChhiilldd GGrroouuppss {{%% iiff ppeerrmmss..nneettbbooxx__iinnvveennttoorryy..aadddd__iinnvveennttoorryyiitteemmggrroouupp %%}}
 _AA_dd_dd_ _GG_rr_oo_uu_pp
 {{%% eennddiiff %%}}
-{% render_table child_groups_table 'inc/table.html' %}
+{% htmx_table 'plugins:netbox_inventory:inventoryitemgroup_list'
+ancestor_id=object.pk %}
 {% include 'inc/panels/tags.html' %} {% include 'inc/panels/comments.html' %}
 {% plugin_right_page object %}
 **** AAsssseettss ****
-{% render_table asset_table 'inc/table.html' %} {% include 'inc/paginator.html'
-with paginator=asset_table.paginator page=asset_table.page %}
+{% htmx_table 'plugins:netbox_inventory:asset_list'
+inventoryitem_group_id=object.pk %}
 {% plugin_full_width_page object %}
 {% endblock content %}
```

### Comparing `netbox_inventory-2.0.0/netbox_inventory/templates/netbox_inventory/inventoryitemtype.html` & `netbox_inventory-2.0.1/netbox_inventory/templates/netbox_inventory/inventoryitemtype.html`

 * *Files identical despite different names*

### Comparing `netbox_inventory-2.0.0/netbox_inventory/templates/netbox_inventory/purchase.html` & `netbox_inventory-2.0.1/netbox_inventory/templates/netbox_inventory/purchase.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 {% extends 'generic/object.html' %}
 {% load helpers %}
 {% load plugins %}
-{% load render_table from django_tables2 %}
 
 {% block breadcrumbs %}
   {{ block.super }}
   <li class="breadcrumb-item">
     <a href="{% url 'plugins:netbox_inventory:purchase_list' %}?supplier_id={{ object.supplier.pk }}">{{ object.supplier }}</a>
   </li>
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,10 +1,9 @@
 {% extends 'generic/object.html' %} {% load helpers %} {% load plugins %} {%
-load render_table from django_tables2 %} {% block breadcrumbs %} {{ block.super
-}}
+block breadcrumbs %} {{ block.super }}
 _{_{_ _o_b_j_e_c_t_._s_u_p_p_l_i_e_r_ _}_}
 {% endblock %} {% block content %}
 **** PPuurrcchhaassee ****
 NNaammee        {{ object.name }}
 SSuupppplliieerr    {{ object.supplier|linkify }}
 SSttaattuuss      {% badge object.get_status_display bg_color=object.get_status_color
             %}
```

### Comparing `netbox_inventory-2.0.0/netbox_inventory/templates/netbox_inventory/supplier.html` & `netbox_inventory-2.0.1/netbox_inventory/templates/netbox_inventory/supplier.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 {% extends 'generic/object.html' %}
 {% load plugins %}
-{% load render_table from django_tables2 %}
 
 {% block breadcrumbs %}
   <li class="breadcrumb-item"><a href="{% url 'plugins:netbox_inventory:supplier_list' %}">Suppliers</a></li>
 {% endblock %}
 
 {% block extra_controls %}
   {% if perms.netbox_inventory.add_purchase %}
```

#### html2text {}

```diff
@@ -1,9 +1,8 @@
-{% extends 'generic/object.html' %} {% load plugins %} {% load render_table
-from django_tables2 %} {% block breadcrumbs %}
+{% extends 'generic/object.html' %} {% load plugins %} {% block breadcrumbs %}
 _S_u_p_p_l_i_e_r_s
 {% endblock %} {% block extra_controls %} {% if
 perms.netbox_inventory.add_purchase %}
 _A_d_d_ _p_u_r_c_h_a_s_e
 {% endif %} {% endblock extra_controls %} {% block content %}
 **** SSuupppplliieerr ****
 NNaammee        {{ object.name }}
```

### Comparing `netbox_inventory-2.0.0/netbox_inventory/tests/asset/test_api.py` & `netbox_inventory-2.0.1/netbox_inventory/tests/asset/test_api.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-2.0.0/netbox_inventory/tests/asset/test_models.py` & `netbox_inventory-2.0.1/netbox_inventory/tests/asset/test_models.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-2.0.0/netbox_inventory/tests/asset/test_views.py` & `netbox_inventory-2.0.1/netbox_inventory/tests/asset/test_views.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-2.0.0/netbox_inventory/tests/asset/test_views_create.py` & `netbox_inventory-2.0.1/netbox_inventory/tests/asset/test_views_create.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-2.0.0/netbox_inventory/tests/asset/test_views_reassign.py` & `netbox_inventory-2.0.1/netbox_inventory/tests/asset/test_views_reassign.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-2.0.0/netbox_inventory/tests/custom.py` & `netbox_inventory-2.0.1/netbox_inventory/tests/custom.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-2.0.0/netbox_inventory/tests/delivery/test_api.py` & `netbox_inventory-2.0.1/netbox_inventory/tests/delivery/test_api.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-2.0.0/netbox_inventory/tests/delivery/test_views.py` & `netbox_inventory-2.0.1/netbox_inventory/tests/delivery/test_views.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-2.0.0/netbox_inventory/tests/inventoryitem_group/test_api.py` & `netbox_inventory-2.0.1/netbox_inventory/tests/inventoryitem_group/test_api.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-2.0.0/netbox_inventory/tests/inventoryitem_group/test_views.py` & `netbox_inventory-2.0.1/netbox_inventory/tests/inventoryitem_group/test_views.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-2.0.0/netbox_inventory/tests/inventoryitem_type/test_api.py` & `netbox_inventory-2.0.1/netbox_inventory/tests/inventoryitem_type/test_api.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-2.0.0/netbox_inventory/tests/inventoryitem_type/test_views.py` & `netbox_inventory-2.0.1/netbox_inventory/tests/inventoryitem_type/test_views.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-2.0.0/netbox_inventory/tests/purchase/test_api.py` & `netbox_inventory-2.0.1/netbox_inventory/tests/purchase/test_api.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-2.0.0/netbox_inventory/tests/purchase/test_views.py` & `netbox_inventory-2.0.1/netbox_inventory/tests/purchase/test_views.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-2.0.0/netbox_inventory/tests/settings.py` & `netbox_inventory-2.0.1/netbox_inventory/tests/settings.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-2.0.0/netbox_inventory/tests/supplier/test_api.py` & `netbox_inventory-2.0.1/netbox_inventory/tests/supplier/test_api.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-2.0.0/netbox_inventory/tests/supplier/test_views.py` & `netbox_inventory-2.0.1/netbox_inventory/tests/supplier/test_views.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-2.0.0/netbox_inventory/tests/test_load.py` & `netbox_inventory-2.0.1/netbox_inventory/tests/test_load.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 class NetboxInventoryVersionTestCase(SimpleTestCase):
     """
     Test for netbox_inventory package
     """
 
     def test_version(self):
-        assert __version__ == "2.0.0"
+        assert __version__ == "2.0.1"
 
 
 class AppTest(APITestCase):
     """
     Test the availability of the plugin API root
     """
```

### Comparing `netbox_inventory-2.0.0/netbox_inventory/urls.py` & `netbox_inventory-2.0.1/netbox_inventory/urls.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-2.0.0/netbox_inventory/utils.py` & `netbox_inventory-2.0.1/netbox_inventory/utils.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-2.0.0/netbox_inventory/views/asset.py` & `netbox_inventory-2.0.1/netbox_inventory/views/asset.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-2.0.0/netbox_inventory/views/asset_assign.py` & `netbox_inventory-2.0.1/netbox_inventory/views/asset_assign.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-2.0.0/netbox_inventory/views/asset_create.py` & `netbox_inventory-2.0.1/netbox_inventory/views/asset_create.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-2.0.0/netbox_inventory/views/asset_reassign.py` & `netbox_inventory-2.0.1/netbox_inventory/views/asset_reassign.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-2.0.0/netbox_inventory/views/delivery.py` & `netbox_inventory-2.0.1/netbox_inventory/views/delivery.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-2.0.0/netbox_inventory/views/inventoryitem_group.py` & `netbox_inventory-2.0.1/netbox_inventory/views/inventoryitem_group.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-2.0.0/netbox_inventory/views/inventoryitem_type.py` & `netbox_inventory-2.0.1/netbox_inventory/views/inventoryitem_type.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-2.0.0/netbox_inventory/views/purchase.py` & `netbox_inventory-2.0.1/netbox_inventory/views/purchase.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-2.0.0/netbox_inventory/views/supplier.py` & `netbox_inventory-2.0.1/netbox_inventory/views/supplier.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-2.0.0/netbox_inventory.egg-info/PKG-INFO` & `netbox_inventory-2.0.1/netbox_inventory.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-inventory
-Version: 2.0.0
+Version: 2.0.1
 Summary: Inventory asset management in NetBox
 Author-email: Matej Vadnjal <matej.vadnjal@arnes.si>
 Project-URL: Homepage, https://github.com/ArnesSI/netbox-inventory/
 Project-URL: Bug Tracker, https://github.com/ArnesSI/netbox-inventory/issues/
 Keywords: netbox,netbox-plugin,inventory
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `netbox_inventory-2.0.0/netbox_inventory.egg-info/SOURCES.txt` & `netbox_inventory-2.0.1/netbox_inventory.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -53,18 +53,14 @@
 netbox_inventory/templates/netbox_inventory/inventoryitemgroup.html
 netbox_inventory/templates/netbox_inventory/inventoryitemtype.html
 netbox_inventory/templates/netbox_inventory/purchase.html
 netbox_inventory/templates/netbox_inventory/supplier.html
 netbox_inventory/templates/netbox_inventory/inc/asset_edit_header.html
 netbox_inventory/templates/netbox_inventory/inc/asset_info.html
 netbox_inventory/templates/netbox_inventory/inc/asset_stats_counts.html
-netbox_inventory/templates/netbox_inventory/tabs/located_assets_base.html
-netbox_inventory/templates/netbox_inventory/tabs/located_assets_location.html
-netbox_inventory/templates/netbox_inventory/tabs/located_assets_rack.html
-netbox_inventory/templates/netbox_inventory/tabs/located_assets_site.html
 netbox_inventory/tests/__init__.py
 netbox_inventory/tests/custom.py
 netbox_inventory/tests/settings.py
 netbox_inventory/tests/test_load.py
 netbox_inventory/tests/asset/__init__.py
 netbox_inventory/tests/asset/test_api.py
 netbox_inventory/tests/asset/test_models.py
@@ -91,9 +87,8 @@
 netbox_inventory/views/asset_assign.py
 netbox_inventory/views/asset_create.py
 netbox_inventory/views/asset_reassign.py
 netbox_inventory/views/delivery.py
 netbox_inventory/views/inventoryitem_group.py
 netbox_inventory/views/inventoryitem_type.py
 netbox_inventory/views/purchase.py
-netbox_inventory/views/supplier.py
-netbox_inventory/views/tabs.py
+netbox_inventory/views/supplier.py
```

### Comparing `netbox_inventory-2.0.0/pyproject.toml` & `netbox_inventory-2.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "netbox-inventory"
-version = "2.0.0"
+version = "2.0.1"
 authors = [
   { name="Matej Vadnjal", email="matej.vadnjal@arnes.si" },
 ]
 description = "Inventory asset management in NetBox"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

