# Comparing `tmp/eomaps-8.1.1.tar.gz` & `tmp/eomaps-8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eomaps-8.1.1.tar", last modified: Tue Apr  9 17:27:31 2024, max compression
+gzip compressed data, was "eomaps-8.2.tar", last modified: Mon May 13 12:48:01 2024, max compression
```

## Comparing `eomaps-8.1.1.tar` & `eomaps-8.2.tar`

### file list

```diff
@@ -1,111 +1,112 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:27:31.129676 eomaps-8.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-09 17:27:19.000000 eomaps-8.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14165 2024-04-09 17:27:31.129676 eomaps-8.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10674 2024-04-09 17:27:19.000000 eomaps-8.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:27:31.117676 eomaps-8.1.1/eomaps/
--rw-r--r--   0 runner    (1001) docker     (127)    17356 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/NE_features.json
--rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    54506 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/_blit_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    10119 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/_containers.py
--rw-r--r--   0 runner    (1001) docker     (127)    48962 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/_data_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    50349 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/_webmap.py
--rw-r--r--   0 runner    (1001) docker     (127)    24787 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/annotation_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)    49562 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)    79214 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/cb_container.py
--rw-r--r--   0 runner    (1001) docker     (127)    57327 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/colorbar.py
--rw-r--r--   0 runner    (1001) docker     (127)    20504 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/compass.py
--rw-r--r--   0 runner    (1001) docker     (127)    28800 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/draw.py
--rw-r--r--   0 runner    (1001) docker     (127)   198736 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/eomaps.py
--rw-r--r--   0 runner    (1001) docker     (127)    35956 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/grid.py
--rw-r--r--   0 runner    (1001) docker     (127)    17589 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    16394 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/inset_maps.py
--rw-r--r--   0 runner    (1001) docker     (127)    37516 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/layout_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)    86617 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    17423 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/mapsgrid.py
--rw-r--r--   0 runner    (1001) docker     (127)    22191 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/ne_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     6045 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/projections.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:27:31.117676 eomaps-8.1.1/eomaps/qtcompanion/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/qtcompanion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6883 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/qtcompanion/app.py
--rw-r--r--   0 runner    (1001) docker     (127)    15683 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/qtcompanion/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/qtcompanion/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:27:31.125676 eomaps-8.1.1/eomaps/qtcompanion/icons/
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/qtcompanion/icons/close.png
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/qtcompanion/icons/edit_layout.png
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/qtcompanion/icons/edit_layout_active.png
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/qtcompanion/icons/edit_layout_hover.png
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/qtcompanion/icons/eye_closed.png
--rw-r--r--   0 runner    (1001) docker     (127)     5435 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/qtcompanion/icons/eye_open.png
--rw-r--r--   0 runner    (1001) docker     (127)     5680 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/qtcompanion/icons/info.png
--rw-r--r--   0 runner    (1001) docker     (127)     5962 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/qtcompanion/icons/info_checked.png
--rw-r--r--   0 runner    (1001) docker     (127)     6220 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/qtcompanion/icons/info_hoover.png
--rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/qtcompanion/icons/layers.png
--rw-r--r--   0 runner    (1001) docker     (127)     3494 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/qtcompanion/icons/layers_hover.png
--rw-r--r--   0 runner    (1001) docker     (127)    86617 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/qtcompanion/icons/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/qtcompanion/icons/maximize.png
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/qtcompanion/icons/open.png
--rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/qtcompanion/icons/open_hover.png
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/qtcompanion/icons/peek_bottom.png
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/qtcompanion/icons/peek_bottom_active.png
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/qtcompanion/icons/peek_circle.png
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/qtcompanion/icons/peek_circle_active.png
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/qtcompanion/icons/peek_ellipse.png
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/qtcompanion/icons/peek_ellipse_active.png
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/qtcompanion/icons/peek_left.png
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/qtcompanion/icons/peek_left_active.png
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/qtcompanion/icons/peek_rectangle.png
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/qtcompanion/icons/peek_rectangle_active.png
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/qtcompanion/icons/peek_right.png
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/qtcompanion/icons/peek_right_active.png
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/qtcompanion/icons/peek_square.png
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/qtcompanion/icons/peek_square_active.png
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/qtcompanion/icons/peek_top.png
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/qtcompanion/icons/peek_top_active.png
--rw-r--r--   0 runner    (1001) docker     (127)     4249 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/qtcompanion/icons/plus.png
--rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/qtcompanion/icons/plus_hoover.png
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/qtcompanion/signal_container.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:27:31.125676 eomaps-8.1.1/eomaps/qtcompanion/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/qtcompanion/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23702 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/qtcompanion/widgets/annotate.py
--rw-r--r--   0 runner    (1001) docker     (127)    19962 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/qtcompanion/widgets/click_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)    16308 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/qtcompanion/widgets/draw.py
--rw-r--r--   0 runner    (1001) docker     (127)    62338 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/qtcompanion/widgets/editor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/qtcompanion/widgets/extent.py
--rw-r--r--   0 runner    (1001) docker     (127)    46849 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/qtcompanion/widgets/files.py
--rw-r--r--   0 runner    (1001) docker     (127)    15167 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/qtcompanion/widgets/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)    20418 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/qtcompanion/widgets/peek.py
--rw-r--r--   0 runner    (1001) docker     (127)    12694 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/qtcompanion/widgets/save.py
--rw-r--r--   0 runner    (1001) docker     (127)    17052 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/qtcompanion/widgets/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    31928 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/qtcompanion/widgets/wms.py
--rw-r--r--   0 runner    (1001) docker     (127)    51631 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    56857 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/scalebar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:27:31.125676 eomaps-8.1.1/eomaps/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6308 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/scripts/open.py
--rw-r--r--   0 runner    (1001) docker     (127)    82983 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/shapes.py
--rw-r--r--   0 runner    (1001) docker     (127)    21493 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    91116 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/webmap_containers.py
--rw-r--r--   0 runner    (1001) docker     (127)    18151 2024-04-09 17:27:20.000000 eomaps-8.1.1/eomaps/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:27:31.129676 eomaps-8.1.1/eomaps.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14165 2024-04-09 17:27:31.000000 eomaps-8.1.1/eomaps.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-04-09 17:27:31.000000 eomaps-8.1.1/eomaps.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 17:27:31.000000 eomaps-8.1.1/eomaps.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-09 17:27:31.000000 eomaps-8.1.1/eomaps.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-09 17:27:31.000000 eomaps-8.1.1/eomaps.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-09 17:27:31.000000 eomaps-8.1.1/eomaps.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-04-09 17:27:20.000000 eomaps-8.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 17:27:31.129676 eomaps-8.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:27:31.129676 eomaps-8.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4795 2024-04-09 17:27:20.000000 eomaps-8.1.1/tests/test_WMS_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    44313 2024-04-09 17:27:20.000000 eomaps-8.1.1/tests/test_basic_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    29217 2024-04-09 17:27:20.000000 eomaps-8.1.1/tests/test_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-09 17:27:20.000000 eomaps-8.1.1/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-09 17:27:20.000000 eomaps-8.1.1/tests/test_doc_codeblocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-04-09 17:27:20.000000 eomaps-8.1.1/tests/test_doc_notebooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-04-09 17:27:20.000000 eomaps-8.1.1/tests/test_drawer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-09 17:27:20.000000 eomaps-8.1.1/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-04-09 17:27:20.000000 eomaps-8.1.1/tests/test_from_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     6935 2024-04-09 17:27:20.000000 eomaps-8.1.1/tests/test_layout_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-04-09 17:27:20.000000 eomaps-8.1.1/tests/test_plot_shapes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-04-09 17:27:20.000000 eomaps-8.1.1/tests/test_raster_aggregaton.py
--rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-04-09 17:27:20.000000 eomaps-8.1.1/tests/test_widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:48:01.208550 eomaps-8.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-05-13 12:47:51.000000 eomaps-8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14337 2024-05-13 12:48:01.208550 eomaps-8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10674 2024-05-13 12:47:51.000000 eomaps-8.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:48:01.192550 eomaps-8.2/eomaps/
+-rw-r--r--   0 runner    (1001) docker     (127)    17356 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/NE_features.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54662 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/_blit_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10119 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/_containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54772 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/_data_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48810 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/_maps_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50349 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/_webmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24787 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/annotation_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49570 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79174 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/cb_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57530 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/colorbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20504 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/compass.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28800 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/draw.py
+-rw-r--r--   0 runner    (1001) docker     (127)   146187 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/eomaps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36083 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18078 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16394 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/inset_maps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38892 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/layout_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86617 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17423 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/mapsgrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22191 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/ne_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6045 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/projections.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:48:01.196550 eomaps-8.2/eomaps/qtcompanion/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6883 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15683 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:48:01.200550 eomaps-8.2/eomaps/qtcompanion/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/icons/close.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/icons/edit_layout.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/icons/edit_layout_active.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/icons/edit_layout_hover.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/icons/eye_closed.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5435 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/icons/eye_open.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5680 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/icons/info.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5962 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/icons/info_checked.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6220 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/icons/info_hoover.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/icons/layers.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3494 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/icons/layers_hover.png
+-rw-r--r--   0 runner    (1001) docker     (127)    86617 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/icons/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/icons/maximize.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/icons/open.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/icons/open_hover.png
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/icons/peek_bottom.png
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/icons/peek_bottom_active.png
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/icons/peek_circle.png
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/icons/peek_circle_active.png
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/icons/peek_ellipse.png
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/icons/peek_ellipse_active.png
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/icons/peek_left.png
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/icons/peek_left_active.png
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/icons/peek_rectangle.png
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/icons/peek_rectangle_active.png
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/icons/peek_right.png
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/icons/peek_right_active.png
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/icons/peek_square.png
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/icons/peek_square_active.png
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/icons/peek_top.png
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/icons/peek_top_active.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4249 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/icons/plus.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/icons/plus_hoover.png
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/signal_container.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:48:01.204550 eomaps-8.2/eomaps/qtcompanion/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23702 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/widgets/annotate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19962 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/widgets/click_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16308 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/widgets/draw.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62338 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/widgets/editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/widgets/extent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46849 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/widgets/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15167 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/widgets/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20418 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/widgets/peek.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12694 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/widgets/save.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17052 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/widgets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31928 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/widgets/wms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51631 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57249 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/scalebar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:48:01.204550 eomaps-8.2/eomaps/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6308 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/scripts/open.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83217 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/shapes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21493 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91116 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/webmap_containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18151 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:48:01.204550 eomaps-8.2/eomaps.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14337 2024-05-13 12:48:01.000000 eomaps-8.2/eomaps.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-05-13 12:48:01.000000 eomaps-8.2/eomaps.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 12:48:01.000000 eomaps-8.2/eomaps.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-13 12:48:01.000000 eomaps-8.2/eomaps.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-13 12:48:01.000000 eomaps-8.2/eomaps.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-13 12:48:01.000000 eomaps-8.2/eomaps.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-05-13 12:47:51.000000 eomaps-8.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 12:48:01.208550 eomaps-8.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:48:01.204550 eomaps-8.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4795 2024-05-13 12:47:51.000000 eomaps-8.2/tests/test_WMS_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44313 2024-05-13 12:47:51.000000 eomaps-8.2/tests/test_basic_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29217 2024-05-13 12:47:51.000000 eomaps-8.2/tests/test_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-13 12:47:51.000000 eomaps-8.2/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-05-13 12:47:51.000000 eomaps-8.2/tests/test_doc_codeblocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-05-13 12:47:51.000000 eomaps-8.2/tests/test_doc_notebooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-05-13 12:47:51.000000 eomaps-8.2/tests/test_drawer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-13 12:47:51.000000 eomaps-8.2/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-13 12:47:51.000000 eomaps-8.2/tests/test_from_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6935 2024-05-13 12:47:51.000000 eomaps-8.2/tests/test_layout_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4550 2024-05-13 12:47:51.000000 eomaps-8.2/tests/test_plot_shapes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-05-13 12:47:51.000000 eomaps-8.2/tests/test_raster_aggregaton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-05-13 12:47:51.000000 eomaps-8.2/tests/test_widgets.py
```

### Comparing `eomaps-8.1.1/LICENSE` & `eomaps-8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `eomaps-8.1.1/PKG-INFO` & `eomaps-8.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eomaps
-Version: 8.1.1
+Version: 8.2
 Summary: A library to create interactive maps of geographical datasets.
 Author-email: Raphael Quast <raphael.quast@geo.tuwien.ac.at>
 License: BSD 3-Clause License
         
         Copyright (c) 2021, The EOmaps authors.
         
         Redistribution and use in source and binary forms, with or without
@@ -70,14 +70,18 @@
 Requires-Dist: requests; extra == "wms"
 Provides-Extra: shade
 Requires-Dist: datashader; extra == "shade"
 Requires-Dist: dask[dataframe]; extra == "shade"
 Provides-Extra: gui
 Requires-Dist: PyQt5; extra == "gui"
 Requires-Dist: qtpy; extra == "gui"
+Provides-Extra: test
+Requires-Dist: eomaps[classify,gui,io,shade,test,wms]; extra == "test"
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-mpl; extra == "test"
 
 
 <p align="center">
     <a href=https://github.com/raphaelquast/EOmaps>
     <img src="https://github.com/raphaelquast/EOmaps/blob/master/docs/_static/logo.png?raw=true" alt="EOmaps logo" width="55%">
     </a>
 </p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: eomaps Version: 8.1.1 Summary: A library to create
+Metadata-Version: 2.1 Name: eomaps Version: 8.2 Summary: A library to create
 interactive maps of geographical datasets. Author-email: Raphael Quast
 geo.tuwien.ac.at> License: BSD 3-Clause License Copyright (c) 2021, The EOmaps
 authors. Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met: 1.
 Redistributions of source code must retain the above copyright notice, this
 list of conditions and the following disclaimer. 2. Redistributions in binary
 form must reproduce the above copyright notice, this list of conditions and the
@@ -36,15 +36,17 @@
 Requires-Dist: pandas; extra == "io" Requires-Dist: geopandas; extra == "io"
 Requires-Dist: xarray; extra == "io" Requires-Dist: netcdf4; extra == "io"
 Requires-Dist: rioxarray; extra == "io" Provides-Extra: classify Requires-Dist:
 mapclassify; extra == "classify" Provides-Extra: wms Requires-Dist: owslib;
 extra == "wms" Requires-Dist: requests; extra == "wms" Provides-Extra: shade
 Requires-Dist: datashader; extra == "shade" Requires-Dist: dask[dataframe];
 extra == "shade" Provides-Extra: gui Requires-Dist: PyQt5; extra == "gui"
-Requires-Dist: qtpy; extra == "gui"
+Requires-Dist: qtpy; extra == "gui" Provides-Extra: test Requires-Dist: eomaps
+[classify,gui,io,shade,test,wms]; extra == "test" Requires-Dist: pytest; extra
+== "test" Requires-Dist: pytest-mpl; extra == "test"
                                  _[_E_O_m_a_p_s_ _l_o_g_o_]
  | Tests & Review | [![tests](https://github.com/raphaelquast/EOmaps/actions/
      workflows/testMaps.yml/badge.svg?branch=master)](https://github.com/
   raphaelquast/EOmaps/actions/workflows/testMaps.yml) | [![codecov](https://
   codecov.io/gh/raphaelquast/EOmaps/graph/badge.svg)](https://codecov.io/gh/
  raphaelquast/EOmaps) | [![pyOpenSci](https://tinyurl.com/y22nb8up)](https://
 github.com/pyOpenSci/software-submission/issues/138) | | :--------------------
```

### Comparing `eomaps-8.1.1/README.md` & `eomaps-8.2/README.md`

 * *Files identical despite different names*

### Comparing `eomaps-8.1.1/eomaps/NE_features.json` & `eomaps-8.2/eomaps/NE_features.json`

 * *Files identical despite different names*

### Comparing `eomaps-8.1.1/eomaps/__init__.py` & `eomaps-8.2/eomaps/__init__.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.1.1/eomaps/_blit_manager.py` & `eomaps-8.2/eomaps/_blit_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -264,15 +264,17 @@
         try:
             return self.canvas.get_renderer()
         except Exception:
             return None
 
     def _get_all_map_axes(self):
         maxes = {
-            m.ax for m in (self._m.parent, *self._m.parent._children) if m._new_axis_map
+            m.ax
+            for m in (self._m.parent, *self._m.parent._children)
+            if getattr(m, "_new_axis_map", False)
         }
         return maxes
 
     def _get_managed_axes(self):
         return (*self._get_all_map_axes(), *self._managed_axes)
 
     def _get_unmanaged_axes(self):
@@ -327,17 +329,17 @@
 
             # single-shot callbacks
             # (execute also if the layer is already active)
             while len(self._on_layer_change[False]) > 0:
                 try:
                     f = self._on_layer_change[False].pop(0)
                     f(layer=layer)
-                except Exception:
+                except Exception as ex:
                     _log.error(
-                        "EOmaps: Issue while executing a layer-change action",
+                        f"EOmaps: Issue during layer-change action: {ex}",
                         exc_info=_log.getEffectiveLevel() <= logging.DEBUG,
                     )
 
             sublayers, _ = self._parse_multi_layer_str(layer)
             if new:
                 for l in sublayers:
                     # individual callables executed if a specific layer is activated
@@ -348,17 +350,17 @@
             for l in sublayers:
                 # single-shot callbacks
                 single_shot_funcs = self._on_layer_activation[False].get(l, [])
                 while len(single_shot_funcs) > 0:
                     try:
                         f = single_shot_funcs.pop(0)
                         f(layer=l)
-                    except Exception:
+                    except Exception as ex:
                         _log.error(
-                            "EOmaps: Issue while executing a layer-change action",
+                            f"EOmaps: Issue during layer-change action: {ex}",
                             exc_info=_log.getEffectiveLevel() <= logging.DEBUG,
                         )
 
             # clear the list of pending webmaps once the layer has been activated
             if layer in self._pending_webmaps:
                 self._pending_webmaps.pop(layer)
 
@@ -426,15 +428,15 @@
         # a general callable to be called on every layer change
         self._do_on_layer_change(layer=val, new=new)
 
         # hide all colorbars that are not on the visible layer
         for m in [self._m.parent, *self._m.parent._children]:
             layer_visible = self._layer_is_subset(val, m.layer)
 
-            for cb in m._colorbars:
+            for cb in getattr(m, "_colorbars", []):
                 cb._hide_singular_axes()
 
                 if layer_visible:
                     if cb in self._hidden_artists:
                         self._hidden_artists.remove(cb)
                 else:
                     if cb not in self._hidden_artists:
@@ -723,16 +725,17 @@
         if "|" in layer:
             if layer not in self._bg_layers:
                 self._combine_bgs(layer)
             return
 
         # update axes spines and patches since they are used to clip artists!
         for ax in self._get_all_map_axes():
-            ax.spines["geo"]._adjust_location()
-            ax.patch._adjust_location()
+            if "geo" in ax.spines:
+                ax.spines["geo"]._adjust_location()
+                ax.patch._adjust_location()
 
         # use contextmanagers to make sure the background patches are not stored
         # in the buffer regions!
         with ExitStack() as stack:
             if layer not in ["__BG__"]:
                 # get rid of the axes background patches for all layers except
                 # the __BG__ layer
@@ -974,16 +977,19 @@
         # put all artist of inset-maps on dedicated layers
         if (
             getattr(art, "axes", None) is not None
             and art.axes.get_label() == "inset_map"
             and not layer.startswith("__inset_")
         ):
             layer = "__inset_" + str(layer)
+
         if layer in self._bg_artists and art in self._bg_artists[layer]:
-            _log.info(f"EOmaps: Background-artist '{art}' already added")
+            _log.info(
+                f"EOmaps: Background-artist '{art}' already added on layer '{layer}'"
+            )
             return
 
         art.set_animated(True)
         self._bg_artists.setdefault(layer, []).append(art)
 
         if isinstance(art, plt.Axes):
             self._managed_axes.add(art)
```

### Comparing `eomaps-8.1.1/eomaps/_containers.py` & `eomaps-8.2/eomaps/_containers.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.1.1/eomaps/_data_manager.py` & `eomaps-8.2/eomaps/_data_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -720,14 +720,161 @@
 
     def _get_current_datasize(self):
         if self._current_data:
             return self._get_datasize(**self._current_data)
         else:
             return 99
 
+    def _sel_c_transp(self, c):
+        return self._select_vals(
+            c.T if self._z_transposed else c,
+            qs=self._last_qs,
+            slices=self._last_slices,
+        )
+
+    def _handle_explicit_colors(self, color):
+        if isinstance(color, (int, float, str, np.number)):
+            # if a scalar is provided, broadcast it
+            pass
+        elif isinstance(color, (list, tuple)) and len(color) in [3, 4]:
+            if all(map(lambda i: isinstance(i, (int, float, np.number)), color)):
+                # check if a tuple of numbers is provided, and if so broadcast
+                # it as a rgb or rgba tuple
+                pass
+            elif all(map(lambda i: isinstance(i, (list, np.ndarray)), color)):
+                # check if a tuple of lists or arrays is provided, and if so,
+                # broadcast them as RGB arrays
+                color = self._sel_c_transp(
+                    np.rec.fromarrays(np.broadcast_arrays(*color))
+                )
+        elif isinstance(color, np.ndarray) and (color.shape[-1] in [3, 4]):
+            color = self._sel_c_transp(np.rec.fromarrays(color.T))
+        elif isinstance(color, np.ndarray) and (color.shape[-1] in [3, 4]):
+            color = self._sel_c_transp(np.rec.fromarrays(color.T))
+        else:
+            # still use np.asanyarray in here in case lists are provided
+            color = self._sel_c_transp(np.asanyarray(color).reshape(self.m._zshape))
+
+        return color
+
+    @staticmethod
+    def _convert_1d_to_2d(data, x, y, fill_value=np.nan):
+        """A function to convert 1D vectors + data into 2D."""
+
+        if _log.getEffectiveLevel() <= logging.DEBUG:
+            _log.debug(
+                "EOmaps: Required conversion of 1D arrays to 2D for 'raster'"
+                "shape might be slow and consume a lot of memory!"
+            )
+
+        x, y, data = map(np.asanyarray, (x, y, data))
+        assert (
+            x.size == y.size == data.size
+        ), "EOmaps: You cannot use 1D arrays with different sizes for x, y and data"
+
+        x_vals, x_idx = np.unique(x, return_inverse=True)
+        y_vals, y_idx = np.unique(y, return_inverse=True)
+        # Get output array shape
+        m, n = (x_vals.size, y_vals.size)
+
+        # Get linear indices to be used as IDs with bincount
+        lidx = np.ravel_multi_index(np.vstack((x_idx, y_idx)), (m, n))
+        idx2d = np.unravel_index(lidx, (m, n))
+
+        # Distribute data to 2D
+
+        if not np.issubdtype(data.dtype, np.integer):
+            # Integer-dtypes do not support None!
+            data2d = np.full((m, n), fill_value=fill_value, dtype=data.dtype)
+            data2d[idx2d] = data
+
+        else:
+            # use smallest possible value as fill-value
+            fill_value = np.iinfo(data.dtype).min
+            data2d = np.full((m, n), fill_value=fill_value, dtype=data.dtype)
+            data2d[idx2d] = data
+
+            mask2d = np.full((m, n), fill_value=True, dtype=bool)
+            mask2d[idx2d] = False
+
+            data2d = np.ma.masked_array(data2d, mask2d)
+
+        # Distribute coordinates to 2D
+        x_vals, y_vals = np.meshgrid(x_vals, y_vals, indexing="ij")
+
+        return data2d, x_vals, y_vals
+
+    def _get_coll(self, props, **kwargs):
+        # handle selection of explicitly provided facecolors
+        # (e.g. for rgb composites)
+
+        # allow only one of the synonyms "color", "fc" and "facecolor"
+        if (
+            np.count_nonzero(
+                [kwargs.get(i, None) is not None for i in ["color", "fc", "facecolor"]]
+            )
+            > 1
+        ):
+            raise TypeError(
+                "EOmaps: only one of 'color', 'facecolor' or 'fc' " "can be specified!"
+            )
+
+        explicit_fc = False
+        for key in ("color", "facecolor", "fc"):
+            if kwargs.get(key, None) is not None:
+                explicit_fc = True
+                kwargs[key] = self._handle_explicit_colors(kwargs[key])
+
+        # don't pass the array if explicit facecolors are set
+        if explicit_fc and self.m.shape.name not in ["contour"]:
+            args = dict(array=None, cmap=None, norm=None, **kwargs)
+        else:
+            args = dict(
+                array=props["z_data"],
+                cmap=getattr(self.m, "_cbcmap", "Reds"),
+                norm=getattr(self.m, "_norm", None),
+                **kwargs,
+            )
+
+        if (
+            self.m.shape.name in ["contour"]
+            and len(self.m._xshape) == 2
+            and len(self.m._yshape) == 2
+        ):
+            # if 2D data is provided for a contour plot, keep the data 2d!
+            coll = self.m.shape.get_coll(props["xorig"], props["yorig"], "in", **args)
+        elif self.m.shape.name in ["raster"]:
+            # if input-data is 1D, try to convert data to 2D (required for raster)
+            # TODO make an explicit data-conversion function for 2D-only shapes
+            if len(self.m._xshape) == 2 and len(self.m._yshape) == 2:
+                coll = self.m.shape.get_coll(
+                    props["xorig"], props["yorig"], "in", **args
+                )
+            else:
+                data2d, x2d, y2d = self._convert_1d_to_2d(
+                    data=props["z_data"].ravel(),
+                    x=props["x0"].ravel(),
+                    y=props["y0"].ravel(),
+                )
+
+                if args["array"] is not None:
+                    args["array"] = data2d
+
+                coll = self.m.shape.get_coll(x2d, y2d, "out", **args)
+
+        else:
+            # convert to 1D for further processing
+            if args["array"] is not None:
+                args["array"] = args["array"].ravel()
+
+            coll = self.m.shape.get_coll(
+                props["x0"].ravel(), props["y0"].ravel(), "out", **args
+            )
+        return coll
+
     def on_fetch_bg(self, layer=None, bbox=None, check_redraw=True):
         # TODO support providing a bbox as extent?
         if layer is None:
             layer = self.layer
         try:
             if check_redraw and not self.redraw_required(layer):
                 return
@@ -753,15 +900,15 @@
                 # keep original data if too low amount of data is attempted
                 # to be plotted
                 return
 
             # remove previous collection from the map
             self._remove_existing_coll()
             # draw the new collection
-            coll = self.m._get_coll(props, **self.m._coll_kwargs)
+            coll = self._get_coll(props, **self.m._coll_kwargs)
             coll.set_clim(self.m._vmin, self.m._vmax)
 
             coll.set_label("Dataset " f"({self.m.shape.name}  |  {self.z_data.shape})")
 
             if self.m.shape.name not in ["scatter_points", "contour", "hexbin"]:
                 # avoid use "autolim=True" since it can cause problems in
                 # case the data-limits are infinite (e.g. for projected
```

### Comparing `eomaps-8.1.1/eomaps/_webmap.py` & `eomaps-8.2/eomaps/_webmap.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.1.1/eomaps/annotation_editor.py` & `eomaps-8.2/eomaps/annotation_editor.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.1.1/eomaps/callbacks.py` & `eomaps-8.2/eomaps/callbacks.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,17 +172,17 @@
 
                 equal_crs = self.m.data_specs.crs == self.m._crs_plot
                 if len(parameter) > 15:
                     parameter = parameter[:15] + " ..."
                 printstr = (
                     (f"# Picked {n_ids} points\n" if multipick else "")
                     + f"{xlabel} = {x}\n"
-                    + (f"{xlabel}_plot = {x0}\n" if not equal_crs else "")
                     + f"{ylabel} = {y}\n"
-                    + (f"{ylabel}_plot = {y0}\n" if not equal_crs else "")
+                    + (f"x_plot = {x0}\n" if not equal_crs else "")
+                    + (f"y_plot = {y0}\n" if not equal_crs else "")
                     + (f"ID = {ID}\n" if ID is not None else "")
                     + (f"{parameter} = {val}" if val is not None else "")
                 )
 
             else:
                 if not crs_is_lonlat:
                     xlabel, ylabel = "x", "y"
@@ -627,15 +627,15 @@
                 "ellipses", radius=radius, radius_crs=radius_crs, n=n
             )
         elif shape == "rectangles":
             shp = self.m.set_shape._get(
                 "rectangles", radius=radius, radius_crs=radius_crs, mesh=False, n=n
             )
         elif shape == "scatter_points":
-            marker = getattr(self.m.shape, "_marker", "o")
+            marker = getattr(self.m.shape, "_marker", kwargs.pop("marker", "o"))
             shp = self.m.set_shape._get("scatter_points", _size=radius, _marker=marker)
         else:
             raise TypeError(f"EOmaps: '{shape}' is not a valid marker-shape")
 
         coll = shp.get_coll(
             np.atleast_1d(pos[0]), np.atleast_1d(pos[1]), pos_crs, **kwargs
         )
```

### Comparing `eomaps-8.1.1/eomaps/cb_container.py` & `eomaps-8.2/eomaps/cb_container.py`

 * *Files 0% similar despite different names*

```diff
@@ -575,15 +575,15 @@
         def picked_vals(self):
             """Get a list of all picked values."""
             if hasattr(self._parent.attach, "picked_vals"):
                 return self._parent.attach.picked_vals
             else:
                 _log.warning(
                     "EOmaps: No picked values found. Attach "
-                    "the 'get_vals' callback first!"
+                    "the 'get_values' callback first!"
                 )
 
         @property
         def permanent_markers(self):
             """Get a list of all permanent markers."""
             if hasattr(self._parent.attach, "permanent_markers"):
                 return self._parent.attach.permanent_markers
@@ -2300,15 +2300,14 @@
         # unattach default keymaps to avoid interaction with keypress events
         assignments = dict()
         assignments["keymap.back"] = ["c", "left"]
         assignments["keymap.forward"] = ["v", "right"]
         assignments["keymap.grid"] = ["g"]
         assignments["keymap.grid_minor"] = ["G"]
         assignments["keymap.home"] = ["h", "r"]
-        assignments["keymap.pan"] = ["p"]
         assignments["keymap.quit"] = ["q"]
         assignments["keymap.save"] = ["s"]
         assignments["keymap.xscale"] = ["k", "L"]
         assignments["keymap.yscale"] = ["l"]
 
         for key, val in assignments.items():
             for v in val:
```

### Comparing `eomaps-8.1.1/eomaps/colorbar.py` & `eomaps-8.2/eomaps/colorbar.py`

 * *Files 1% similar despite different names*

```diff
@@ -627,24 +627,29 @@
     Note
     ----
     To add a colorbar to a map, use
     :py:meth:`Maps.add_colorbar <eomaps.eomaps.Maps.add_colorbar>`.
 
     """
 
-    def __init__(self, *args, inherit_position=True, **kwargs):
+    def __init__(self, *args, inherit_position=True, layer=None, **kwargs):
         super().__init__(*args, **kwargs)
 
+        self._layer = layer
+
         self._inherit_position = inherit_position
         self._dynamic_shade_indicator = False
 
     @property
     def layer(self):
         """The layer associated with the colorbar."""
-        return self._m.layer
+        if self._layer is None:
+            return self._m.layer
+        else:
+            return self._layer
 
     def _default_cb_tick_formatter(self, x, pos, precision=None):
         """
         A formatter to format the tick-labels of the colorbar for encoded datasets.
         (used in xaxis.set_major_formatter() )
         """
         # if precision=None the shortest representation of the number is used
@@ -726,26 +731,27 @@
 
         self.ax_cb.remove()
         self.ax_cb_plot.remove()
 
     def _set_map(self, m):
         self._m = m
 
+        if self._layer is None:
+            self._layer = self._m.layer
+
         self._parent_cb = self._identify_parent_cb()
 
         self._vmin = self._m.coll.norm.vmin
         self._vmax = self._m.coll.norm.vmax
         self._norm = self._m.coll.norm
         self._cmap = self._m.coll.cmap
 
     def _add_axes_to_layer(self, dynamic):
         BM = self._m.BM
 
-        self._layer = self._m.layer
-
         # add all axes as artists
         self.ax_cb.set_navigate(False)
 
         for a in (self.ax_cb, self.ax_cb_plot):
             if a is not None:
                 if dynamic is True:
                     BM.add_artist(a, self._layer)
@@ -1355,14 +1361,15 @@
         log=False,
         label=None,
         outline=False,
         hist_kwargs=None,
         hist_label=None,
         margin=None,
         divider_linestyle=None,
+        layer=None,
         **kwargs,
     ):
         """
         Add a colorbar to the map.
 
         The colorbar always represents the data of the associated Maps-object
         that was assigned in the last call to
@@ -1557,14 +1564,15 @@
             orientation=orientation,
             tick_precision=tick_precision,
             inherit_position=inherit_position,
             extend_frac=extend_frac,
             margin=margin,
             divider_linestyle=divider_linestyle,
             hist_size=hist_size,
+            layer=layer,
         )
         cb._set_map(m)
         cb._setup_axes(pos, m.ax)
         cb._add_axes_to_layer(dynamic=dynamic_shade_indicator)
 
         cb.set_scale(log)
         cb._plot_colorbar(extend=extend, **kwargs)
```

### Comparing `eomaps-8.1.1/eomaps/compass.py` & `eomaps-8.2/eomaps/compass.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.1.1/eomaps/draw.py` & `eomaps-8.2/eomaps/draw.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.1.1/eomaps/eomaps.py` & `eomaps-8.2/eomaps/eomaps.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,117 +5,71 @@
 
 """General definition of Maps objects."""
 
 import logging
 
 _log = logging.getLogger(__name__)
 
+from contextlib import ExitStack
 from functools import lru_cache, wraps
 from itertools import repeat, chain
-import copy
-from types import SimpleNamespace
 from pathlib import Path
-import weakref
-import gc
+from types import SimpleNamespace
 from textwrap import fill
-from contextlib import contextmanager, ExitStack
+
+import copy
 import importlib.metadata
+import weakref
 
 import numpy as np
-
-from pyproj import CRS, Transformer
+from pyproj import CRS
 
 import matplotlib as mpl
 import matplotlib.pyplot as plt
-from matplotlib.gridspec import GridSpec, SubplotSpec
-
 import matplotlib.patches as mpatches
 from matplotlib.path import Path as mpath
 
 from cartopy import crs as ccrs
 
+from ._maps_base import MapsBase
 from .helpers import (
     pairwise,
     cmap_alpha,
     progressbar,
     SearchTree,
     _TransformedBoundsLocator,
-    _add_to_docstring,
     register_modules,
     _key_release_event,
+    _add_to_docstring,
 )
 
-from ._blit_manager import BlitManager
-from .layout_editor import LayoutEditor
 from .shapes import Shapes
 from .colorbar import ColorBar
-
-from ._containers import (
-    DataSpecs,
-    ClassifySpecs,
-)
-
-try:
-    from ._webmap import refetch_wms_on_size_change, _cx_refetch_wms_on_size_change
-    from .webmap_containers import WebMapContainer
-except ImportError as ex:
-    _log.error(f"EOmaps: Unable to import dependencies required for WebMaps: {ex}")
-    refetch_wms_on_size_change = None
-    _cx_refetch_wms_on_size_change = None
-    WebMapContainer = None
-
+from ._containers import DataSpecs, ClassifySpecs
 from .ne_features import NaturalEarthFeatures
-
 from .cb_container import CallbackContainer, GeoDataFramePicker
 from .scalebar import ScaleBar
 from .compass import Compass
-from .projections import Equi7Grid_projection  # import to supercharge cartopy.ccrs
 from .reader import read_file, from_file, new_layer_from_file
 from .grid import GridFactory
-
 from .utilities import Utilities
 from .draw import ShapeDrawer
 from .annotation_editor import AnnotationEditor
-
 from ._data_manager import DataManager
 
-__version__ = importlib.metadata.version("eomaps")
-
-
-def _handle_backends():
-    # make sure that the backend is activated
-    # (backends are loaded lazily and values such as plt.isinteractive() might not
-    # yet show the correct value in case the backend is not yet fully loaded)
-
-    # This is especially important for the IPython/inline backend which explicitly
-    # calls plt.ion() when the backend is loaded.
-    # (see https://github.com/matplotlib/matplotlib/issues/26221)
-    plt.install_repl_displayhook()
-
-    active_backend = plt.get_backend()
-
-    # to avoid flickering in the layout editor in jupyter notebooks
-    if active_backend in ["module://ipympl.backend_nbagg"]:
-        plt.ioff()
-    else:
-        if Maps._use_interactive_mode is True:
-            plt.ion()
-            _log.debug(
-                "EOmaps: matplotlib's interactive mode is turned on. "
-                "Maps will show up immediately and the console is NOT blocking! "
-                "To change, use Maps.config(use_interactive_mode=True/False)."
-            )
-        elif Maps._use_interactive_mode is False:
-            plt.ioff()
-            _log.debug(
-                "EOmaps: matplotlib's interactive mode is turned off. "
-                "Call `m.show()` to show the map (and block the console)! "
-                "To change, use Maps.config(use_interactive_mode=True/False)."
-            )
+try:
+    from ._webmap import refetch_wms_on_size_change, _cx_refetch_wms_on_size_change
+    from .webmap_containers import WebMapContainer
+except ImportError as ex:
+    _log.error(f"EOmaps: Unable to import dependencies required for WebMaps: {ex}")
+    refetch_wms_on_size_change = None
+    _cx_refetch_wms_on_size_change = None
+    WebMapContainer = None
 
+__version__ = importlib.metadata.version("eomaps")
 
 # hardcoded list of available mapclassify-classifiers
 # (to avoid importing it on startup)
 _CLASSIFIERS = (
     "BoxPlot",
     "EqualInterval",
     "FisherJenks",
@@ -130,99 +84,15 @@
     "Quantiles",
     "Percentiles",
     "StdMean",
     "UserDefined",
 )
 
 
-class _MapsMeta(type):
-
-    _use_interactive_mode = None
-    _always_on_top = False
-
-    _backend_warning_shown = False
-
-    def config(
-        cls,
-        snapshot_on_update=None,
-        companion_widget_key=None,
-        always_on_top=None,
-        use_interactive_mode=None,
-        log_level=None,
-    ):
-        """
-        Set global configuration parameters for figures created with EOmaps.
-
-        This function must be called before initializing any :py:class:`Maps` object!
-
-        >>> from eomaps import Maps
-        >>> Maps.config(always_on_top=True)
-
-        (parameters set to None are NOT updated!)
-
-        Parameters
-        ----------
-        snapshot_on_update : bool, optional
-            Only relevant when using an IPython console or a jupyter notebook together
-            with the `inline` backend! (e.g. using `%matplotlib inline`)
-
-            - If True, figure updates automatically trigger drawing a snapshot
-              of the current state of the figure to the active cell.
-            - If False, an explicit call to `m.show()` is required to draw the figure.
-
-            The default is True.
-        companion_widget_key : str, optional
-            The keyboard shortcut to use for activating the companion-widget.
-            The default is "w".
-        always_on_top : bool, optional
-            Only relevant if `PyQt5` is used as matplotlib backend.
-
-            - If True, the figure will be kept "always on top" of other applications.
-
-            The default is False.
-        use_interactive_mode : bool or None, optional
-            If True, matplotlibs interactive mode (`plt.ion()`) is activated by default
-            for all backends except jupyter-notebook backends (`inline` and `ipympl`).
-
-            If False, interactive mode is turned off (`plt.ioff()` and a call
-            to `m.show()` is required to trigger showing the figure!
-            Note that this will block the terminal!
-
-            If None, No changes are applied.
-
-            The default is True.
-        log_level : str or int, optional
-            The logging level.
-            If set, a StreamHandler will be attached to the logger that prints to
-            the active terminal at the specified log level.
-
-            See :py:meth:`set_loglevel` on how to customize logging format.
-
-            The default is None.
-        """
-
-        from . import set_loglevel
-
-        if companion_widget_key is not None:
-            Maps._companion_widget_key = companion_widget_key
-
-        if always_on_top is not None:
-            Maps._always_on_top = always_on_top
-
-        if snapshot_on_update is not None:
-            BlitManager._snapshot_on_update = snapshot_on_update
-
-        if use_interactive_mode is not None:
-            Maps._use_interactive_mode = use_interactive_mode
-
-        if log_level is not None:
-            set_loglevel(log_level)
-
-
-class Maps(metaclass=_MapsMeta):
+class Maps(MapsBase):
     """
     The base-class for generating plots with EOmaps.
 
     The first Maps object that is initialized will create a new matplotlib `Figure`
     and a cartopy `GeoAxes` for a map.
 
     You can then create additional `Maps` objects on the same figure with the following
@@ -367,95 +237,70 @@
         crs=None,
         layer="base",
         f=None,
         ax=None,
         preferred_wms_service="wms",
         **kwargs,
     ):
+        super().__init__(
+            crs=crs,
+            layer=layer,
+            f=f,
+            ax=ax,
+            **kwargs,
+        )
+
         self._log_on_event_messages = dict()
         self._log_on_event_cids = dict()
 
         try:
             from .qtcompanion.signal_container import _SignalContainer
 
             # initialize the signal container (MUST be done before init of the widget!)
             self._signal_container = _SignalContainer()
         except Exception:
             _log.debug("SignalContainer could not be initialized", exc_info=True)
             self._signal_container = None
 
-        # make sure the used layer-name is valid
-        layer = BlitManager._check_layer_name(layer)
-
         self._inherit_classification = None
 
-        if isinstance(ax, plt.Axes) and hasattr(ax, "figure"):
-            if isinstance(ax.figure, plt.Figure):
-                if f is not None:
-                    assert (
-                        f == ax.figure
-                    ), "EOmaps: The provided axis is in a different figure!"
-
-                self._f = ax.figure
-        else:
-            self._f = f
-
-        self._ax = None
-        self._parent = None
-        self._BM = None
         self._util = None
-        self._children = set()  # weakref.WeakSet()
-        self._after_add_child = list()
 
         self._colorbars = []
         self._coll = None  # slot for the collection created by m.plot_map()
 
-        self._layer = layer
-
-        # check if the self represents a new-layer or an object on an existing layer
-        if any(
-            i.layer == layer for i in (self.parent, *self.parent._children) if i != self
-        ):
-            self._is_sublayer = True
-        else:
-            self._is_sublayer = False
-
         self._companion_widget = None  # slot for the pyqt widget
+
         self._cid_keypress = None  # callback id for PyQt5 keypress callbacks
+        # attach a callback to show/hide the companion-widget with the "w" key
+        if self.parent._cid_keypress is None:
+            # NOTE the companion-widget is ONLY attached to the parent map
+            # since it will identify the clicked map automatically! The
+            # widget will only be initialized on Maps-objects that create
+            # NEW axes. This is required to make sure that any additional
+            # Maps-object on the same axes will then always use the
+            # same widget. (otherwise each layer would get its own widget)
+
+            self.parent._cid_keypress = self.f.canvas.mpl_connect(
+                "key_press_event", self.parent._on_keypress
+            )
+
         # a list to remember newly registered colormaps
         self._registered_cmaps = []
 
         # a list of actions that are executed whenever the widget is shown
         self._on_show_companion_widget = []
 
         # preferred way of accessing WMS services (used in the WMS container)
         assert preferred_wms_service in [
             "wms",
             "wmts",
         ], "preferred_wms_service must be either 'wms' or 'wmts' !"
         self._preferred_wms_service = preferred_wms_service
 
-        if isinstance(ax, plt.Axes):
-            # set the plot_crs only if no explicit axes is provided
-            if crs is not None:
-                raise AssertionError(
-                    "You cannot set the crs if you already provide an explicit axes!"
-                )
-            if ax.projection == Maps.CRS.PlateCarree():
-                self._crs_plot = 4326
-            else:
-                self._crs_plot = ax.projection
-        else:
-            if crs is None or crs == Maps.CRS.PlateCarree():
-                crs = 4326
-
-            self._crs_plot = crs
-
-        self._crs_plot_cartopy = self._get_cartopy_crs(self._crs_plot)
-
         # default classify specs
         self.classify_specs = ClassifySpecs(weakref.proxy(self))
 
         self.data_specs = DataSpecs(
             weakref.proxy(self),
             x=None,
             y=None,
@@ -463,58 +308,41 @@
         )
 
         # initialize the data-manager
         self._data_manager = DataManager(self._proxy(self))
         self._data_plotted = False
         self._set_extent_on_plot = True
 
-        self._layout_editor = None
-
         self.cb = self.cb(weakref.proxy(self))  # accessor for the callbacks
-        self._init_figure(ax=ax, plot_crs=crs, **kwargs)
+
+        # initialize the callbacks
+        self.cb._init_cbs()
 
         if WebMapContainer is not None:
             self.add_wms = self.add_wms(weakref.proxy(self))
 
         self._new_layer_from_file = new_layer_from_file(weakref.proxy(self))
 
         self.set_shape = self.set_shape(weakref.proxy(self))
         self._shape = None
+        # the dpi used for shade shapes
+        self._shade_dpi = None
 
         # the radius is estimated when plot_map is called
         self._estimated_radius = None
 
         # a set to hold references to the compass objects
         self._compass = set()
 
         if not hasattr(self.parent, "_wms_legend"):
             self.parent._wms_legend = dict()
 
         if not hasattr(self.parent, "_execute_callbacks"):
             self.parent._execute_callbacks = True
 
-        # Make sure the figure-background patch is on an explicit layer
-        # This is used to avoid having the background patch on each fetched
-        # background while maintaining the capability of restoring it
-        if self.f.patch not in self.BM._bg_artists.get("__BG__", []):
-            self.f.patch.set_zorder(-2)
-            self.BM.add_bg_artist(self.f.patch, layer="__BG__")
-
-        if self.ax.patch not in self.BM._bg_artists.get("__BG__", []):
-            self.ax.patch.set_zorder(-1)
-            self.BM.add_bg_artist(self.ax.patch, layer="__BG__")
-
-        # Treat cartopy geo-spines separately in the blit-manager
-        # to avoid issues with overlapping spines that are drawn on each layer
-        # if multiple layers of a map are combined.
-        # (Note: spines need to be visible on each layer in case the layer
-        # is viewed on its own, but overlapping spines cause blurry boundaries)
-        # TODO find a better way to deal with this!
-        self._handle_spines()
-
         # evaluate and cache crs boundary bounds (for extent clipping)
         self._crs_boundary_bounds = self.crs_plot.boundary.bounds
 
         # a factory to create gridlines
         if self.parent == self:
             self._grid = GridFactory(self.parent)
 
@@ -525,160 +353,14 @@
         self.draw = self.draw(weakref.proxy(self))
 
         if self.parent == self:
             self.util = Utilities(self)
         else:
             self.util = self.parent.util
 
-    def _handle_spines(self):
-        spine = self.ax.spines["geo"]
-        if spine not in self.BM._bg_artists.get("__SPINES__", []):
-            self.BM.add_bg_artist(spine, layer="__SPINES__")
-
-    def __getattribute__(self, key):
-        if key == "set_layout":
-            raise AttributeError(
-                "'Maps' object has no attribute 'set_layout'... "
-                "did you mean 'apply_layout'?"
-            )
-        else:
-            return object.__getattribute__(self, key)
-
-    def __enter__(self):
-        assert not self._is_sublayer, (
-            "EOmaps: using a Maps-object as a context-manager is only possible "
-            "if you create a NEW layer (not a Maps-object on an existing layer)!"
-        )
-
-        return self
-
-    def __exit__(self, type, value, traceback):
-        self.cleanup()
-        if self.parent == self:
-            plt.close(self.f)
-        gc.collect()
-
-    def __repr__(self):
-        try:
-            return f"<eomaps.Maps object on layer '{self.layer}'>"
-        except Exception:
-            return object.__repr__(self)
-
-    def _parse_log_level(self, level):
-        """
-        Get the numerical log-level from string (or number).
-
-        Parameters
-        ----------
-        level : str or number
-            The log level
-
-        Returns
-        -------
-        int_level : float
-            The numerical value of the log level.
-
-        """
-        from logging import getLevelNamesMapping
-
-        levels = getLevelNamesMapping()
-
-        if isinstance(level, str) and level.upper() in levels:
-            use_level = levels[level.upper()]
-        else:
-            use_level = float(level)
-
-        return use_level
-
-    def _log_on_event(self, level, msg, event):
-        """
-        Schedule a log message that will be shown on the next matplotlib event.
-
-        Identical scheduled messages are only shown once per event!
-
-        {'CRITICAL': 50, 'FATAL': 50, 'ERROR': 40, 'WARN': 30, 'WARNING': 30,
-         'INFO': 20,  'DEBUG': 10, 'NOTSET': 0}
-
-        Parameters
-        ----------
-        level : int or str
-            The logging level.
-        msg : str
-            The message.
-        event : str
-            The event name (e.g. "button_release_event")
-
-        """
-        level = self._parse_log_level(level)
-
-        messages = self._log_on_event_messages.setdefault(event, [])
-        cid = self._log_on_event_cids.setdefault(event, None)
-
-        # don't attach messages if they are already scheduled
-        if (level, msg) in messages:
-            return
-
-        messages.append((level, msg))
-
-        def log_message(*args, **kwargs):
-            cid = self._log_on_event_cids.get(event, None)
-            messages = self._log_on_event_messages.get(event, [])
-
-            if cid is not None:
-                self.f.canvas.mpl_disconnect(cid)
-                self._log_on_event_cids.pop(event, None)
-
-            while len(messages) > 0:
-                level, msg = messages.pop(0)
-                _log.log(level, msg)
-
-        if cid is None:
-            self._log_on_event_cids[event] = self.f.canvas.mpl_connect(
-                event, log_message
-            )
-
-    @property
-    def BM(self):
-        """The Blit-Manager used to dynamically update the plots."""
-        m = weakref.proxy(self)
-        if self.parent._BM is None:
-            self.parent._BM = BlitManager(m)
-            self.parent._BM._bg_layer = m.parent.layer
-        return self.parent._BM
-
-    @property
-    def layer(self):
-        """The layer-name associated with this Maps-object."""
-        return self._layer
-
-    @property
-    def all(self):
-        """
-        Get a Maps-object on the "all" layer.
-
-        Use it just as any other Maps-object. (It's the same as `Maps(layer="all")`)
-
-        >>> m.all.cb.click.attach.annotate()
-
-        """
-        if not hasattr(self, "_all"):
-            self._all = self.new_layer("all")
-        return self._all
-
-    @property
-    def ax(self):
-        """The matplotlib (cartopy) GeoAxes associated with this Maps-object."""
-        return self._ax
-
-    @property
-    def f(self):
-        """The matplotlib Figure associated with this Maps-object."""
-        # always return the figure of the parent object
-        return self._f
-
     @property
     def coll(self):
         """The collection representing the dataset plotted by m.plot_map()."""
         return self._coll
 
     @property
     def shape(self):
@@ -692,44 +374,14 @@
         """
         if self._shape is None:
             self._set_default_shape()
 
         return self._shape
 
     @property
-    def parent(self):
-        """
-        The parent-object to which this Maps-object is connected to.
-
-        If None, `self` is returned!
-        """
-        if self._parent is None:
-            self._set_parent()
-
-        return self._parent
-
-    @property
-    def _edit_annotations(self):
-        if getattr(self.parent, "_edit_annotations_parent", None) is None:
-            self.parent._edit_annotations_parent = AnnotationEditor(self.parent)
-        return self.parent._edit_annotations_parent
-
-    @property
-    def _real_self(self):
-        # workaround to obtain a non-weak reference for the parent
-        # (e.g. self.parent._real_self is a non-weak ref to parent)
-        # see https://stackoverflow.com/a/49319989/9703451
-        return self
-
-    @property
-    def crs_plot(self):
-        """The crs used for plotting."""
-        return self._crs_plot_cartopy
-
-    @property
     def colorbar(self):
         """
         Get the **most recently added** colorbar of this Maps-object.
 
         Returns
         -------
         ColorBar
@@ -744,14 +396,53 @@
         return self.data_specs.data
 
     @data.setter
     def data(self, val):
         # for downward-compatibility
         self.data_specs.data = val
 
+    @lru_cache()
+    def get_crs(self, crs="plot"):
+        """
+        Get the pyproj CRS instance of a given crs specification.
+
+        Parameters
+        ----------
+        crs : "in", "out" or a crs definition
+            the crs to return
+
+            - if "in" : the crs defined in m.data_specs.crs
+            - if "out" or "plot" : the crs used for plotting
+
+        Returns
+        -------
+        crs : pyproj.CRS
+            the pyproj CRS instance
+
+        """
+        # check for strings first to avoid expensive equality checking for CRS objects!
+        if isinstance(crs, str):
+            if crs == "in":
+                crs = self.data_specs.crs
+            elif crs == "out" or crs == "plot":
+                crs = self.crs_plot
+
+        crs = CRS.from_user_input(crs)
+        return crs
+
+    @property
+    def _edit_annotations(self):
+        if getattr(self.parent, "_edit_annotations_parent", None) is None:
+            self.parent._edit_annotations_parent = AnnotationEditor(self.parent)
+        return self.parent._edit_annotations_parent
+
+    @wraps(AnnotationEditor.__call__)
+    def edit_annotations(self, b=True, **kwargs):
+        self._edit_annotations(b, **kwargs)
+
     @property
     @wraps(new_layer_from_file)
     def new_layer_from_file(self):
         """Create a new layer from a file."""
         return self._new_layer_from_file
 
     def new_map(
@@ -1179,75 +870,14 @@
             shape=shape,
             indicate_extent=indicate_extent,
             indicator_line=indicator_line,
         )
 
         return m2
 
-    def _get_always_on_top(self):
-        if "qt" in plt.get_backend().lower():
-            from qtpy import QtCore
-
-            w = self.f.canvas.window()
-            return bool(w.windowFlags() & QtCore.Qt.WindowStaysOnTopHint)
-
-        return False
-
-    def _set_always_on_top(self, q):
-        # keep pyqt window on top
-        try:
-            from qtpy import QtCore
-
-            if q:
-                # only do this if necessary to avoid flickering
-                # see https://stackoverflow.com/a/40007740/9703451
-                if not self._get_always_on_top():
-                    # in case pyqt is used as backend, also keep the figure on top
-                    if "qt" in plt.get_backend().lower():
-                        w = self.f.canvas.window()
-                        ws = w.size()
-                        w.setWindowFlags(
-                            w.windowFlags() | QtCore.Qt.WindowStaysOnTopHint
-                        )
-                        w.resize(ws)
-                        w.show()
-
-                    # handle the widget in case it was activated (possible also for
-                    # backends other than qt)
-                    if self._companion_widget is not None:
-                        cw = self._companion_widget.window()
-                        cws = cw.size()
-                        cw.setWindowFlags(
-                            cw.windowFlags() | QtCore.Qt.WindowStaysOnTopHint
-                        )
-                        cw.resize(cws)
-                        cw.show()
-
-            else:
-                if self._get_always_on_top():
-                    if "qt" in plt.get_backend().lower():
-                        w = self.f.canvas.window()
-                        ws = w.size()
-                        w.setWindowFlags(
-                            w.windowFlags() & ~QtCore.Qt.WindowStaysOnTopHint
-                        )
-                        w.resize(ws)
-                        w.show()
-
-                    if self._companion_widget is not None:
-                        cw = self._companion_widget.window()
-                        cws = cw.size()
-                        cw.setWindowFlags(
-                            cw.windowFlags() & ~QtCore.Qt.WindowStaysOnTopHint
-                        )
-                        cw.resize(cws)
-                        cw.show()
-        except Exception:
-            pass
-
     def set_data(
         self,
         data=None,
         x=None,
         y=None,
         crs=None,
         encoding=None,
@@ -1493,14 +1123,62 @@
             kwargs passed to the call to the respective mapclassify classifier
             (dependent on the selected scheme... see above)
 
         """
         register_modules("mapclassify")
         self.classify_specs._set_scheme_and_args(scheme, **kwargs)
 
+    def inherit_data(self, m):
+        """
+        Use the data of another Maps-object (without copying).
+
+        NOTE
+        ----
+        If the data is inherited, any change in the data of the parent
+        Maps-object will be reflected in this Maps-object as well!
+
+        Parameters
+        ----------
+        m : eomaps.Maps or None
+            The Maps-object that provides the data.
+        """
+        if m is not None:
+            self.data_specs = m.data_specs
+
+            def set_data(*args, **kwargs):
+                raise AssertionError(
+                    "EOmaps: You cannot set data for a Maps object that "
+                    "inherits data!"
+                )
+
+            self.set_data = set_data
+
+    def inherit_classification(self, m):
+        """
+        Use the classification of another Maps-object when plotting the data.
+
+        NOTE
+        ----
+        If the classification is inherited, the following arguments
+        for `m.plot_map()` will have NO effect (they are inherited):
+
+            - "cmap"
+            - "vmin"
+            - "vmax"
+
+        Parameters
+        ----------
+        m : eomaps.Maps or None
+            The Maps-object that provides the classification specs.
+        """
+        if m is not None:
+            self._inherit_classification = self._proxy(m)
+        else:
+            self._inherit_classification = None
+
     def set_extent_to_location(self, location, annotate=False, user_agent=None):
         """
         Set the map-extent based on a given location query.
 
         The bounding-box is hereby resolved via the OpenStreetMap Nominatim service.
 
         Note
@@ -1558,18 +1236,122 @@
 
             self.add_annotation(
                 xy=(r["lon"], r["lat"]), xy_crs=4326, text=text, fontsize=8
             )
         else:
             _log.info(f"Centering Map to:\n    {r['display_name']}")
 
-    @staticmethod
-    def _set_clipboard_kwargs(**kwargs):
-        # use Maps to make sure InsetMaps do the same thing!
-        Maps._clipboard_kwargs = kwargs
+    def set_frame(self, rounded=0, **kwargs):
+        """
+        Set the properties of the map boundary and the background patch.
+
+        Parameters
+        ----------
+        rounded : float, optional
+            If provided, use a rectangle with rounded corners as map boundary
+            line. The corners will be rounded with respect to the provided
+            fraction (0=no rounding, 1=max. radius). The default is None.
+        kwargs :
+            Additional kwargs to style the boundary line (e.g. the spine)
+            and the background patch
+
+            Possible args for the boundary-line:
+
+            - "edgecolor" or "ec": The line color
+            - "linewidth" or "lw": The line width
+            - "linestyle" or "ls": The line style
+            - "path_effects": A list of path-effects to apply to the line
+
+            Possible args for the background-patch:
+
+            - "facecolor" or "fc": The color of the background patch
+
+        Examples
+        --------
+
+        >>> m = Maps()
+        >>> m.add_feature.preset.ocean()
+        >>> m.set_frame(fc="r", ec="b", lw=3, rounded=.2)
+
+        >>> import matplotlib.patheffects as pe
+        >>> m = Maps()
+        >>> m.add_feature.preset.ocean(fc="k")
+        >>> m.set_frame(
+        >>>     facecolor=(.8, .8, 0, .5), edgecolor="w", linewidth=2,
+        >>>     rounded=.5,
+        >>>     path_effects=[pe.withStroke(linewidth=7, foreground="m")])
+
+        """
+
+        for key in ("fc", "facecolor"):
+            if key in kwargs:
+                self.ax.patch.set_facecolor(kwargs.pop(key))
+
+        self.ax.spines["geo"].update(kwargs)
+
+        if rounded:
+            assert (
+                rounded <= 1
+            ), "EOmaps: rounded corner fraction must be between 0 and 1"
+
+            self.ax._EOmaps_rounded_spine_frac = rounded
+            theta = np.linspace(0, np.pi / 2, 50)  # use 50 intermediate points
+            s, c = np.sin(theta), np.cos(theta)
+
+            # attach a function to dynamically update the corners of the
+            # map boundary prior to fetching a background
+            # Note: this function is only attached once and the relevant
+            # properties are fetched from the axes!
+            if not getattr(self.ax, "_EOmaps_rounded_spine_attached", False):
+
+                def cb(*args, **kwargs):
+                    if self.ax._EOmaps_rounded_spine_frac == 0:
+                        return
+
+                    x0, x1, y0, y1 = self.get_extent(self.crs_plot)
+                    r = min(x1 - x0, y1 - y0) * self.ax._EOmaps_rounded_spine_frac / 2
+
+                    xs = [
+                        x0,
+                        *(x0 + r - r * c),
+                        x0 + r,
+                        x1 - r,
+                        *(x1 - r + r * s),
+                        x1,
+                        x1,
+                        *(x1 - r + r * c),
+                        x1 - r,
+                        x0 + r,
+                        *(x0 + r - r * s),
+                        x0,
+                    ]
+
+                    ys = [
+                        y1 - r,
+                        *(y1 - r + r * s),
+                        y1,
+                        y1,
+                        *(y1 - r + r * c),
+                        y1 - r,
+                        y0 + r,
+                        *(y0 + r - r * s),
+                        y0,
+                        y0,
+                        *(y0 + r - r * c),
+                        y0 + r,
+                    ]
+
+                    path = mpath(np.column_stack((xs, ys)))
+                    self.ax.set_boundary(path, transform=self.crs_plot)
+
+                self.BM._before_fetch_bg_actions.append(cb)
+                self.ax._EOmaps_rounded_spine_attached = True
+
+        self.redraw("__SPINES__")
+        self.redraw("__BG__")
 
     @staticmethod
     def set_clipboard_kwargs(**kwargs):
         """
         Set GLOBAL savefig parameters for all Maps objects on export to the clipboard.
 
         - press "control + c" to export the figure to the clipboard
@@ -1611,14 +1393,19 @@
                 m = getattr(plt.figure(i), "_EOmaps_parent", None)
                 if m is not None:
                     if m._companion_widget is not None:
                         m._emit_signal("clipboardKwargsChanged")
             except Exception:
                 _log.exception("UPS")
 
+    @staticmethod
+    def _set_clipboard_kwargs(**kwargs):
+        # use Maps to make sure InsetMaps do the same thing!
+        Maps._clipboard_kwargs = kwargs
+
     def add_title(self, title, x=0.5, y=1.01, **kwargs):
         """
         Convenience function to add a title to the map.
 
         (The title will be visible at the assigned layer.)
 
         Parameters
@@ -1645,162 +1432,14 @@
         kwargs.setdefault("fontsize", "large")
         kwargs.setdefault("horizontalalignment", "center")
         kwargs.setdefault("verticalalignment", "bottom")
         kwargs.setdefault("transform", self.ax.transAxes)
 
         self.text(x, y, title, layer=self.layer, **kwargs)
 
-    @lru_cache()
-    def get_crs(self, crs="plot"):
-        """
-        Get the pyproj CRS instance of a given crs specification.
-
-        Parameters
-        ----------
-        crs : "in", "out" or a crs definition
-            the crs to return
-
-            - if "in" : the crs defined in m.data_specs.crs
-            - if "out" or "plot" : the crs used for plotting
-
-        Returns
-        -------
-        crs : pyproj.CRS
-            the pyproj CRS instance
-
-        """
-        # check for strings first to avoid expensive equality checking for CRS objects!
-        if isinstance(crs, str):
-            if crs == "in":
-                crs = self.data_specs.crs
-            elif crs == "out" or crs == "plot":
-                crs = self.crs_plot
-
-        crs = CRS.from_user_input(crs)
-        return crs
-
-    @wraps(LayoutEditor.get_layout)
-    def get_layout(self, *args, **kwargs):
-        """Get the current layout."""
-        return self.parent._layout_editor.get_layout(*args, **kwargs)
-
-    @wraps(LayoutEditor.apply_layout)
-    def apply_layout(self, *args, **kwargs):
-        """Apply a given layout."""
-        return self.parent._layout_editor.apply_layout(*args, **kwargs)
-
-    def edit_layout(self, filepath=None):
-        """
-        Activate the "layout-editor" to quickly re-arrange the positions of subplots.
-
-        - This is the same as pressing "alt + l" on the keyboard!
-        - To exit the editor, press "escape" or "alt + l" on the keyboard!
-
-        Parameters
-        ----------
-        filepath : str, pathlib.Path or None, optional
-            A path to a file that will be used to store the layout after you exit
-            the layout-editor.
-            This file can then be used to apply the layout to the map with
-
-            >>> m.apply_layout(filepath=filepath)
-
-            NOTE: The file will be overwritten if it already exists!!
-            The default is None.
-
-        """
-        self.parent._layout_editor._make_draggable(filepath=filepath)
-
-    @wraps(AnnotationEditor.__call__)
-    def edit_annotations(self, b=True, **kwargs):
-        self._edit_annotations(b, **kwargs)
-
-    @contextmanager
-    def _disable_autoscale(self, set_extent):
-        if set_extent is False:
-            init_extent = self.get_extent()
-
-        try:
-
-            yield
-        finally:
-            if set_extent is False:
-                self.set_extent(init_extent)
-
-    def _handle_gdf(
-        self,
-        gdf,
-        val_key=None,
-        only_valid=True,
-        clip=False,
-        reproject="gpd",
-        verbose=False,
-    ):
-        (gpd,) = register_modules("geopandas")
-
-        if isinstance(gdf, (str, Path)):
-            gdf = gpd.read_file(gdf)
-
-        if only_valid:
-            gdf = gdf[gdf.is_valid]
-
-        try:
-            # explode the GeoDataFrame to avoid picking multi-part geometries
-            gdf = gdf.explode(index_parts=False)
-        except Exception:
-            # geopandas sometimes has problems exploding geometries...
-            # if it does not work, just continue with the Multi-geometries!
-            _log.error("EOmaps: Exploding geometries did not work!")
-            pass
-
-        if clip:
-            gdf = self._clip_gdf(gdf, clip)
-        if reproject == "gpd":
-            gdf = gdf.to_crs(self.crs_plot)
-        elif reproject == "cartopy":
-            # optionally use cartopy's re-projection routines to re-project
-            # geometries
-
-            cartopy_crs = self._get_cartopy_crs(gdf.crs)
-            if self.ax.projection != cartopy_crs:
-                # TODO this results in problems and sometimes masks way too much!!
-                # select only polygons that actually intersect with the CRS-boundary
-                # mask = gdf.buffer(1).intersects(
-                #     gpd.GeoDataFrame(
-                #         geometry=[self.ax.projection.domain], crs=self.ax.projection
-                #     )
-                #     .to_crs(gdf.crs)
-                #     .geometry[0]
-                # )
-                # gdf = gdf.copy()[mask]
-
-                geoms = gdf.geometry
-                if len(geoms) > 0:
-                    proj_geoms = []
-
-                    if verbose:
-                        for g in progressbar(geoms, "EOmaps: re-projecting... ", 20):
-                            proj_geoms.append(
-                                self.ax.projection.project_geometry(g, cartopy_crs)
-                            )
-                    else:
-                        for g in geoms:
-                            proj_geoms.append(
-                                self.ax.projection.project_geometry(g, cartopy_crs)
-                            )
-                    gdf = gdf.set_geometry(proj_geoms)
-                    gdf = gdf.set_crs(self.ax.projection, allow_override=True)
-                gdf = gdf[~gdf.is_empty]
-        else:
-            raise AssertionError(
-                f"EOmaps: '{reproject}' is not a valid reproject-argument."
-            )
-
-        return gdf
-
     def add_gdf(
         self,
         gdf,
         picker_name=None,
         pick_method="contains",
         val_key=None,
         layer=None,
@@ -1977,15 +1616,14 @@
                 _log.error("EOmaps: GeoDataFrame contains only invalid geometries!")
                 return
             elif n_invald > 0:
                 _log.warning(
                     "EOmaps: {n_invald} invalid GeoDataFrame geometries are ignored!"
                 )
 
-        # with self._disable_autoscale(set_extent):
         if set_extent:
             extent = np.array(
                 [
                     gdf.bounds["minx"].min(),
                     gdf.bounds["maxx"].max(),
                     gdf.bounds["miny"].min(),
                     gdf.bounds["maxy"].max(),
@@ -2061,14 +1699,187 @@
                 art.set_label(f"EOmaps GeoDataframe ({prefix.lstrip('_')}, {len(gdf)})")
                 if permanent is True:
                     self.BM.add_bg_artist(art, layer)
                 else:
                     self.BM.add_artist(art, layer)
         return artists
 
+    def _handle_gdf(
+        self,
+        gdf,
+        val_key=None,
+        only_valid=True,
+        clip=False,
+        reproject="gpd",
+        verbose=False,
+    ):
+        (gpd,) = register_modules("geopandas")
+
+        if isinstance(gdf, (str, Path)):
+            gdf = gpd.read_file(gdf)
+
+        if only_valid:
+            gdf = gdf[gdf.is_valid]
+
+        try:
+            # explode the GeoDataFrame to avoid picking multi-part geometries
+            gdf = gdf.explode(index_parts=False)
+        except Exception:
+            # geopandas sometimes has problems exploding geometries...
+            # if it does not work, just continue with the Multi-geometries!
+            _log.error("EOmaps: Exploding geometries did not work!")
+            pass
+
+        if clip:
+            gdf = self._clip_gdf(gdf, clip)
+        if reproject == "gpd":
+            gdf = gdf.to_crs(self.crs_plot)
+        elif reproject == "cartopy":
+            # optionally use cartopy's re-projection routines to re-project
+            # geometries
+
+            cartopy_crs = self._get_cartopy_crs(gdf.crs)
+            if self.ax.projection != cartopy_crs:
+                geoms = gdf.geometry
+                if len(geoms) > 0:
+                    proj_geoms = []
+
+                    if verbose:
+                        for g in progressbar(geoms, "EOmaps: re-projecting... ", 20):
+                            proj_geoms.append(
+                                self.ax.projection.project_geometry(g, cartopy_crs)
+                            )
+                    else:
+                        for g in geoms:
+                            proj_geoms.append(
+                                self.ax.projection.project_geometry(g, cartopy_crs)
+                            )
+                    gdf = gdf.set_geometry(proj_geoms)
+                    gdf = gdf.set_crs(self.ax.projection, allow_override=True)
+                gdf = gdf[~gdf.is_empty]
+        else:
+            raise AssertionError(
+                f"EOmaps: '{reproject}' is not a valid reproject-argument."
+            )
+
+        return gdf
+
+    def _clip_gdf(self, gdf, how="crs"):
+        """
+        Clip the shapes of a GeoDataFrame with respect to the given boundaries.
+
+        Parameters
+        ----------
+        gdf : geopandas.GeoDataFrame
+            The GeoDataFrame containing the geometries.
+        how : str, optional
+            Identifier how the clipping should be performed.
+
+            If a suffix "_invert" is added to the string, the polygon will be
+            inverted (via a symmetric-difference to the clip-shape)
+
+            - clipping with geopandas:
+              - "crs" : use the actual crs boundary polygon
+              - "crs_bounds" : use the boundary-envelope of the crs
+              - "extent" : use the current plot-extent
+
+            - clipping with gdal (always uses the crs domain as clip-shape):
+              - "gdal_Intersection"
+              - "gdal_SymDifference"
+              - "gdal_Difference"
+              - "gdal_Union"
+
+            The default is "crs".
+
+        Returns
+        -------
+        gdf
+            A GeoDataFrame with the clipped geometries
+        """
+        (gpd,) = register_modules("geopandas")
+
+        if how.startswith("gdal"):
+            methods = ["SymDifference", "Intersection", "Difference", "Union"]
+            # "SymDifference", "Intersection", "Difference"
+            method = how.split("_")[1]
+            assert method in methods, "EOmaps: '{how}' is not a valid clip-method"
+            try:
+                from osgeo import gdal
+                from shapely import wkt
+            except ImportError:
+                raise ImportError(
+                    "EOmaps: Missing dependency: 'osgeo'\n"
+                    + "...clipping with gdal requires 'osgeo.gdal'"
+                )
+
+            e = self.ax.projection.domain
+            e2 = gdal.ogr.CreateGeometryFromWkt(e.wkt)
+            if not e2.IsValid():
+                e2 = e2.MakeValid()
+
+            # only reproject geometries if crs cannot be identified
+            # as the initially provided (or cartopy converted) crs
+            if gdf.crs != self.crs_plot and gdf.crs != self._crs_plot:
+                gdf = gdf.to_crs(self.crs_plot)
+
+            clipgeoms = []
+            for g in gdf.geometry:
+                g2 = gdal.ogr.CreateGeometryFromWkt(g.wkt)
+
+                if g2 is None:
+                    continue
+
+                if not g2.IsValid():
+                    g2 = g2.MakeValid()
+
+                i = getattr(g2, method)(e2)
+
+                if how.endswith("_invert"):
+                    i = i.SymDifference(e2)
+
+                gclip = wkt.loads(i.ExportToWkt())
+                clipgeoms.append(gclip)
+
+            gdf = gpd.GeoDataFrame(geometry=clipgeoms, crs=self.crs_plot)
+
+            return gdf
+
+        if how == "crs" or how == "crs_invert":
+            clip_shp = gpd.GeoDataFrame(
+                geometry=[self.ax.projection.domain], crs=self.crs_plot
+            ).to_crs(gdf.crs)
+        elif how == "extent" or how == "extent_invert":
+            self.BM.update()
+            x0, x1, y0, y1 = self.get_extent()
+            clip_shp = self._make_rect_poly(x0, y0, x1, y1, self.crs_plot).to_crs(
+                gdf.crs
+            )
+        elif how == "crs_bounds" or how == "crs_bounds_invert":
+            x0, x1, y0, y1 = self.get_extent()
+            clip_shp = self._make_rect_poly(
+                *self.crs_plot.boundary.bounds, self.crs_plot
+            ).to_crs(gdf.crs)
+        else:
+            raise TypeError(f"EOmaps: '{how}' is not a valid clipping method")
+
+        clip_shp = clip_shp.buffer(0)  # use this to make sure the geometry is valid
+
+        # add 1% of the extent-diameter as buffer
+        bnd = clip_shp.boundary.bounds
+        d = np.sqrt((bnd.maxx - bnd.minx) ** 2 + (bnd.maxy - bnd.miny) ** 2)
+        clip_shp = clip_shp.buffer(d / 100)
+
+        # clip the geo-dataframe with the buffered clipping shape
+        clipgdf = gdf.clip(clip_shp)
+
+        if how.endswith("_invert"):
+            clipgdf = clipgdf.symmetric_difference(clip_shp)
+
+        return clipgdf
+
     def add_marker(
         self,
         ID=None,
         xy=None,
         xy_crs=None,
         radius=None,
         radius_crs=None,
@@ -2389,15 +2200,15 @@
             line_props=line_props,
             layer=layer,
             size_factor=size_factor,
         )
 
         # add the scalebar to the map at the desired position
         s._add_scalebar(pos=pos, azim=rotation, pickable=pickable)
-
+        self.BM.update()
         return s
 
     def add_line(
         self,
         xy,
         xy_crs=4326,
         connect="geod",
@@ -2736,190 +2547,53 @@
         return colorbar
 
     @wraps(GridFactory.add_grid)
     def add_gridlines(self, *args, **kwargs):
         """Add gridlines to the Map."""
         return self.parent._grid.add_grid(m=self, *args, **kwargs)
 
-    def _get_alpha_cmap_name(self, alpha):
-        # get a unique name for the colormap
-        try:
-            ncmaps = max(
-                [
-                    int(i.rsplit("_", 1)[1])
-                    for i in plt.colormaps()
-                    if i.startswith("EOmaps_alpha_")
-                ]
-            )
-        except Exception:
-            ncmaps = 0
-
-        return f"EOmaps_alpha_{ncmaps + 1}"
-
-    def set_extent(self, extents, crs=None):
-        """
-        Set the extent (x0, x1, y0, y1) of the map in the given coordinate system.
-
-        Parameters
-        ----------
-        extent : array-like
-            The extent in the given crs (x0, x1, y0, y1).
-        crs : a crs identifier, optional
-            The coordinate-system in which the extent is evaluated.
-
-            - if None, epsg=4326 (e.g. lon/lat projection) is used
-
-            The default is None.
-
-        """
-        # just a wrapper to make sure that previously set extents are not
-        # reset when plotting data!
-
-        # ( e.g. once .set_extent is called .plot_map does NOT set the extent!)
-        if crs is not None:
-            crs = self._get_cartopy_crs(crs)
-        else:
-            crs = Maps.CRS.PlateCarree()
-
-        self.ax.set_extent(extents, crs=crs)
-        self._set_extent_on_plot = False
-
-    def get_extent(self, crs=None):
+    def indicate_extent(self, x0, y0, x1, y1, crs=4326, npts=100, **kwargs):
         """
-        Get the extent (x0, x1, y0, y1) of the map in the given coordinate system.
+        Indicate a rectangular extent in a given crs on the map.
 
         Parameters
         ----------
-        crs : a crs identifier, optional
-            The coordinate-system in which the extent is evaluated.
-
-            - if None, the extent is provided in epsg=4326 (e.g. lon/lat projection)
-
-            The default is None.
-
-        Returns
-        -------
-        extent : The extent in the given crs (x0, x1, y0, y1).
-
+        x0, y0, y1, y1 : float
+            the boundaries of the shape
+        npts : int, optional
+            The number of points used to draw the polygon-lines.
+            (e.g. to correctly display the distortion of the extent-rectangle when
+            it is re-projected to another coordinate-system)
+            The default is 100.
+        crs : any, optional
+            A coordinate-system identifier.
+            The default is 4326 (e.g. lon/lat).
+        kwargs :
+            Additional keyword-arguments passed to `m.add_gdf()`.
         """
+        register_modules("geopandas")
 
-        # fast track if plot-crs is requested
-        if crs == self.crs_plot:
-            x0, x1, y0, y1 = (*self.ax.get_xlim(), *self.ax.get_ylim())
-
-            bnds = self._crs_boundary_bounds
-            # clip the map-extent with respect to the boundary bounds
-            # (to avoid returning values outside the crs bounds)
-            try:
-                x0, x1 = np.clip([x0, x1], bnds[0], bnds[2])
-                y0, y1 = np.clip([y0, y1], bnds[1], bnds[3])
-            except Exception:
-                _log.debug(
-                    "EOmaps: Error while trying to clip map extent", exc_info=True
-                )
-        else:
-            if crs is not None:
-                crs = self._get_cartopy_crs(crs)
-            else:
-                crs = self._get_cartopy_crs(4326)
-
-            x0, x1, y0, y1 = self.ax.get_extent(crs=crs)
-
-        return x0, x1, y0, y1
-
-    def _calc_vmin_vmax(self, vmin=None, vmax=None):
-        if self.data is None:
-            return vmin, vmax
-
-        calc_min, calc_max = vmin is None, vmax is None
-
-        # ignore fill_values when evaluating vmin/vmax on integer-encoded datasets
-        if (
-            self.data_specs.encoding is not None
-            and isinstance(self._data_manager.z_data, np.ndarray)
-            and issubclass(self._data_manager.z_data.dtype.type, np.integer)
-        ):
-
-            # note the specific way how to check for integer-dtype based on issubclass
-            # since isinstance() fails to identify all integer dtypes!!
-            #   isinstance(np.dtype("uint8"), np.integer)       (incorrect) False
-            #   issubclass(np.dtype("uint8").type, np.integer)  (correct)   True
-            # for details, see https://stackoverflow.com/a/934652/9703451
-
-            fill_value = self.data_specs.encoding.get("_FillValue", None)
-            if fill_value and any([calc_min, calc_max]):
-                # find values that are not fill-values
-                use_vals = self._data_manager.z_data[
-                    self._data_manager.z_data != fill_value
-                ]
-
-                if calc_min:
-                    vmin = np.min(use_vals)
-                if calc_max:
-                    vmax = np.max(use_vals)
-
-                return vmin, vmax
-
-        # use nanmin/nanmax for all other arrays
-        if calc_min:
-            vmin = np.nanmin(self._data_manager.z_data)
-        if calc_max:
-            vmax = np.nanmax(self._data_manager.z_data)
-
-        return vmin, vmax
-
-    def _set_vmin_vmax(self, vmin=None, vmax=None):
-        # don't encode nan-vailes to avoid setting the fill-value as vmin/vmax
-        if vmin is not None:
-            vmin = self._encode_values(vmin)
-        if vmax is not None:
-            vmax = self._encode_values(vmax)
+        gdf = self._make_rect_poly(x0, y0, x1, y1, self.get_crs(crs), npts)
+        self.add_gdf(gdf, **kwargs)
 
-        # handle inherited bounds
-        if self._inherit_classification is not None:
-            if not (vmin is None and vmax is None):
-                raise TypeError(
-                    "EOmaps: 'vmin' and 'vmax' cannot be set explicitly "
-                    "if the classification is inherited!"
-                )
+    @wraps(plt.Figure.text)
+    def text(self, *args, layer=None, **kwargs):
+        """Add text to the map."""
+        kwargs.setdefault("animated", True)
+        kwargs.setdefault("horizontalalignment", "center")
+        kwargs.setdefault("verticalalignment", "center")
 
-            # in case data is NOT inherited, warn if vmin/vmax is None
-            # (different limits might cause a different appearance of the data!)
-            if self.data_specs._m == self:
-                if self._vmin is None:
-                    _log.warning("EOmaps: Inherited value for 'vmin' is None!")
-                if self._vmax is None:
-                    _log.warning(
-                        "EOmaps: Inherited inherited value for 'vmax' is None!"
-                    )
+        a = self.f.text(*args, **kwargs)
 
-            self._vmin = self._inherit_classification._vmin
-            self._vmax = self._inherit_classification._vmax
-            return
+        if layer is None:
+            layer = self.layer
+        self.BM.add_artist(a, layer=layer)
+        self.BM.update()
 
-        if not self.shape.name.startswith("shade_"):
-            # ignore fill_values when evaluating vmin/vmax on integer-encoded datasets
-            self._vmin, self._vmax = self._calc_vmin_vmax(vmin=vmin, vmax=vmax)
-        else:
-            # get the name of the used aggretation reduction
-            aggname = self.shape.aggregator.__class__.__name__
-            if aggname in ["first", "last", "max", "min", "mean", "mode"]:
-                # set vmin/vmax in case the aggregation still represents data-values
-                self._vmin, self._vmax = self._calc_vmin_vmax(vmin=vmin, vmax=vmax)
-            else:
-                # set vmin/vmax for aggregations that do NOT represent data values
-                # allow vmin/vmax = None (e.g. autoscaling)
-                self._vmin, self._vmax = vmin, vmax
-                if "count" in aggname:
-                    # if the reduction represents a count, don't count empty pixels
-                    if vmin and vmin <= 0:
-                        _log.warning(
-                            "EOmaps: setting vmin=1 to avoid counting empty pixels..."
-                        )
-                        self._vmin = 1
+        return a
 
     def plot_map(
         self,
         layer=None,
         dynamic=False,
         set_extent=True,
         assume_sorted=True,
@@ -3142,522 +2816,403 @@
 
         self._data_plotted = True
 
         self._emit_signal("dataPlotted")
 
         self.BM.update()
 
-    def make_dataset_pickable(
+    def _plot_map(
         self,
+        layer=None,
+        dynamic=False,
+        set_extent=True,
+        assume_sorted=True,
+        **kwargs,
     ):
-        """
-        Make the associated dataset pickable **without plotting** it first.
-
-        After executing this function, `m.cb.pick` callbacks can be attached to the
-        `Maps` object.
-
-        NOTE
-        ----
-        This function is ONLY necessary if you want to use pick-callbacks **without**
-        actually plotting the data**! Otherwise a call to `m.plot_map()` is sufficient!
-
-        - Each `Maps` object can always have only one pickable dataset.
-        - The used data is always the dataset that was assigned in the last call to
-          `m.plot_map()` or `m.make_dataset_pickable()`.
-        - To get multiple pickable datasets, use an individual layer for each of the
-          datasets (e.g. first `m2 = m.new_layer()` and then assign the data to `m2`)
-
-        Examples
-        --------
-        >>> m = Maps()
-        >>> m.add_feature.preset.coastline()
-        >>> ...
-        >>> # a dataset that should be pickable but NOT visible...
-        >>> m2 = m.new_layer()
-            >>> m2.set_data(*np.linspace([0, -180,-90,], [100, 180, 90], 100).T)
-        >>> m2.make_dataset_pickable()
-        >>> m2.cb.pick.attach.annotate()  # get an annotation for the invisible dataset
-        >>> # ...call m2.plot_map() to make the dataset visible...
-        """
-        if self.coll is not None:
-            _log.error(
-                "EOmaps: There is already a dataset plotted on this Maps-object. "
-                "You MUST use a new layer (`m2 = m.new_layer()`) to use "
-                "`m2.make_dataset_pickable()`!"
-            )
-            return
-
-        # ---------------------- prepare the data
-        self._data_manager = DataManager(self._proxy(self))
-        self._data_manager.set_props(layer=self.layer, only_pick=True)
-
-        x0, x1 = self._data_manager.x0.min(), self._data_manager.x0.max()
-        y0, y1 = self._data_manager.y0.min(), self._data_manager.y0.max()
+        _log.info(
+            "EOmaps: Plotting "
+            f"{self._data_manager.z_data.size} datapoints ({self.shape.name})"
+        )
 
-        # use a transparent rectangle of the data-extent as artist for picking
-        (art,) = self.ax.fill([x0, x1, x1, x0], [y0, y0, y1, y1], fc="none", ec="none")
+        for key in ("array",):
+            assert (
+                key not in kwargs
+            ), f"The key '{key}' is assigned internally by EOmaps!"
 
-        self._coll = art
+        try:
+            self._set_extent = set_extent
 
-        self.tree = SearchTree(m=self._proxy(self))
-        self.cb.pick._set_artist(art)
-        self.cb.pick._init_cbs()
-        self.cb._methods.add("pick")
+            # ------------- plot the data
+            self._coll_kwargs = kwargs
+            self._coll_dynamic = dynamic
 
-        self._coll_kwargs = dict()
-        self._coll_dynamic = True
+            # NOTE: the actual plot is performed by the data-manager
+            # at the next call to m.BM.fetch_bg() for the corresponding layer
+            # this is called to make sure m.coll is properly set
+            self._data_manager.on_fetch_bg(check_redraw=False)
 
-        # set _data_plotted to True to trigger updates in the data-manager
-        self._data_plotted = True
+        except Exception as ex:
+            raise ex
 
-    def show_layer(self, *args, clear=True):
+    def _shade_map(
+        self,
+        layer=None,
+        dynamic=False,
+        set_extent=True,
+        assume_sorted=True,
+        **kwargs,
+    ):
         """
-        Show a single layer or (transparently) overlay multiple selected layers.
-
-        Parameters
-        ----------
-        args : str, tuple
-
-            - if str: The name of the layer to show.
-            - if tuple: A combination of a layer-name and a transparency assignment
-              ( < layer name >, < transparency [0-1] > )
-
-        Examples
-        --------
-        Show a **single layer** by providing the name of the layer as string:
-
-        >>> m.show_layer("A")
-
-        To show **multiple layers**, use one of the following options:
-
-        Provide multiple layer-names (stacking is done from left to right), e.g.:
-
-        >>> m.show_layer("A", "B", "C")
-
-        Provide the combined layer-name, e.g.:
-
-        >>> m.show_layer("A|B|C")
-
-        To **transparently overlay multiple layers**, use one of the following options:
-
-        Provide tuples of layer-names and transparency-assignments, e.g.:
-
-        >>> m.show_layer("A", ("B", 0.5), ("C", 0.25))
-
-        Provide the combined layer-name, e.g.:
-
-        >>> m.show_layer("A|B{0.5}|C{0.25}")
+        Plot the dataset using the (very fast) "datashader" library.
 
-        See Also
-        --------
-        Maps.util.layer_selector : Add a button-widget to switch layers to the map.
-        Maps.util.layer_slider : Add a slider to switch layers to the map.
+        Requires `datashader`... use `conda install -c conda-forge datashader`
 
-        """
-        name = self.BM._get_combined_layer_name(*args)
-        if not isinstance(name, str):
-            _log.info("EOmaps: All layer-names are converted to strings!")
-            name = str(name)
-
-        # check if all layers exist
-        existing_layers = self._get_layers()
-        layers_to_show, _ = self.BM._parse_multi_layer_str(name)
-
-        # don't check private layer-names
-        layers_to_show = [i for i in layers_to_show if not i.startswith("_")]
-        missing_layers = set(layers_to_show).difference(set(existing_layers))
-        if len(missing_layers) > 0:
-            lstr = " - " + "\n - ".join(map(str, existing_layers))
+        - This method is intended for extremely large datasets
+          (up to millions of datapoints)!
 
-            _log.error(
-                f"EOmaps: The layers {missing_layers} do not exist...\n"
-                + f"Use one of: \n{lstr}"
-            )
-            return
+        A dynamically updated "shaded" map will be generated.
+        Note that the datapoints in this case are NOT represented by the shapes
+        defined as `m.set_shape`!
 
-        # invoke the bg_layer setter of the blit-manager
-        self.BM.bg_layer = name
-        self.BM.update()
+        - By default, the shading is performed using a "mean"-value aggregation hook
 
-        # plot a snapshot to jupyter notebook cell if inline backend is used
-        if not self.BM._snapshot_on_update and plt.get_backend() in [
-            "module://matplotlib_inline.backend_inline"
-        ]:
-            self.snapshot(clear=clear)
+        kwargs :
+            kwargs passed to `datashader.mpl_ext.dsshow`
 
-    def show(self, clear=True):
         """
-        Show the map (only required for non-interactive matplotlib backends).
+        _log.info(
+            "EOmaps: Plotting "
+            f"{self._data_manager.z_data.size} datapoints ({self.shape.name})"
+        )
 
-        This is just a convenience function to call matplotlib's `plt.show()`!
+        ds, mpl_ext, pd, xar = register_modules(
+            "datashader", "datashader.mpl_ext", "pandas", "xarray"
+        )
 
-        To switch the currently visible layer, see :py:meth:`Maps.show_layer`
+        # remove previously fetched backgrounds for the used layer
+        if dynamic is False:
+            self.BM._refetch_layer(layer)
 
-        Parameters
-        ----------
-        clear : bool, optional
-            Only relevant if the `inline` backend is used in a jupyter-notebook
-            or an Ipython console.
+        # in case the aggregation does not represent data-values
+        # (e.g. count, std, var ... ) use an automatic "linear" normalization
 
-            If True, clear the active cell before plotting a snapshot of the figure.
-            The default is True.
-        See Also
-        --------
-        show_layer : Set the currently visible layer.
-        """
+        # get the name of the used aggretation reduction
+        aggname = self.shape.aggregator.__class__.__name__
 
-        try:
-            __IPYTHON__
-        except NameError:
-            plt.show()
+        if aggname in ["first", "last", "max", "min", "mean", "mode"]:
+            kwargs.setdefault("norm", self.classify_specs._norm)
         else:
-            active_backend = plt.get_backend()
-            # print a snapshot to the active ipython cell in case the
-            # inline-backend is used
-            if active_backend in ["module://matplotlib_inline.backend_inline"]:
-                self.snapshot(clear=clear)
-            else:
-                plt.show()
-
-    def snapshot(self, *layer, transparent=False, clear=False):
-        """
-        Print a static image of the figure to the active IPython display.
-
-        This is useful if you want to print a snapshot of the current state of the map
-        to the active Jupyter Notebook cell or the currently active IPython console
-        while using a backend that creates popup-plots (e.g. `qt` or `tkinter`)
+            kwargs.setdefault("norm", "linear")
 
-        ONLY use this if you work in an interactive IPython terminal, a Jupyter
-        Notebook or a Jupyter Lab environment!
+        zdata = self._data_manager.z_data
+        if len(zdata) == 0:
+            _log.error("EOmaps: there was no data to plot")
+            return
 
-        Parameters
-        ----------
-        *layer: str or None
-            The layer to show on the snapshot.
-            Any positional arguments are used as layer-assignments similar
-            to `m.show_layer()`
-            If None, the currently visible layer is used.
-            The default is None.
-        transparent: bool
-            Indicator if the snapshot should have a transparent background or not.
-            The default is False.
-        clear: bool
-            Indicator if the current cell-output should be cleared prior
-            to showing the snapshot or not. The default is False
+        plot_width, plot_height = self._get_shade_axis_size()
 
-        Examples
-        --------
-        >>> m = Maps(layer="base")
-        >>> m.add_feature.preset.coastline()
-        >>> m2 = m.new_layer("ocean")
-        >>> m.add_feature.preset.ocean()
-        >>> m.snapshot("base", ("ocean", .5), transparent=True)
+        # get rid of unnecessary dimensions in the numpy arrays
+        zdata = zdata.squeeze()
+        x0 = self._data_manager.x0.squeeze()
+        y0 = self._data_manager.y0.squeeze()
 
-        """
-        if getattr(self, "_snapshotting", False):
-            # this is necessary to avoid recursions with show_layer
-            # in jupyter-notebook inline backend
-            return
+        # the shape is always set after _prepare data!
+        if self.shape.name == "shade_points" and self._data_manager.x0_1D is None:
+            # fill masked-values with None to avoid issues with numba not being
+            # able to deal with numpy-arrays
+            # TODO report this to datashader to get it fixed properly?
+            if isinstance(zdata, np.ma.masked_array):
+                zdata = zdata.filled(None)
 
-        try:
-            self._snapshotting = True
+            df = pd.DataFrame(
+                dict(
+                    x=x0.ravel(),
+                    y=y0.ravel(),
+                    val=zdata.ravel(),
+                ),
+                copy=False,
+            )
 
-            from PIL import Image
+        else:
+            if len(zdata.shape) == 2:
+                if (zdata.shape == x0.shape) and (zdata.shape == y0.shape):
+                    # 2D coordinates and 2D raster
 
-            with ExitStack() as stack:
-                # don't clear on layer-changes
-                stack.enter_context(self.BM._cx_dont_clear_on_layer_change())
+                    # use a curvilinear QuadMesh
+                    if self.shape.name == "shade_raster":
+                        self.shape.glyph = ds.glyphs.QuadMeshCurvilinear(
+                            "x", "y", "val"
+                        )
 
-                if len(layer) == 0:
-                    layer = None
+                    df = xar.Dataset(
+                        data_vars=dict(val=(["xx", "yy"], zdata)),
+                        # dims=["x", "y"],
+                        coords=dict(
+                            x=(["xx", "yy"], x0),
+                            y=(["xx", "yy"], y0),
+                        ),
+                    )
 
-                # hide companion-widget indicator
-                self._indicate_companion_map(False)
+                elif (
+                    ((zdata.shape[1],) == x0.shape)
+                    and ((zdata.shape[0],) == y0.shape)
+                    and (x0.shape != y0.shape)
+                ):
+                    raise AssertionError(
+                        "EOmaps: it seems like you need to transpose your data! \n"
+                        + f"the dataset has a shape of {zdata.shape}, but the "
+                        + f"coordinates suggest ({x0.shape}, {y0.shape})"
+                    )
+                elif (zdata.T.shape == x0.shape) and (zdata.T.shape == y0.shape):
+                    raise AssertionError(
+                        "EOmaps: it seems like you need to transpose your data! \n"
+                        + f"the dataset has a shape of {zdata.shape}, but the "
+                        + f"coordinates suggest {x0.shape}"
+                    )
 
-                if layer is not None:
-                    layer = self.BM._get_combined_layer_name(*layer)
+                elif ((zdata.shape[0],) == x0.shape) and (
+                    (zdata.shape[1],) == y0.shape
+                ):
+                    # 1D coordinates and 2D data
 
-                # add the figure background patch as the bottom layer
-                initial_layer = self.BM.bg_layer
+                    # use a rectangular QuadMesh
+                    if self.shape.name == "shade_raster":
+                        self.shape.glyph = ds.glyphs.QuadMeshRectilinear(
+                            "x", "y", "val"
+                        )
 
-                if transparent is False:
-                    showlayer_name = self.BM._get_showlayer_name(layer=layer)
-                    layer_with_bg = self.BM._get_combined_layer_name(
-                        "__BG__", showlayer_name
+                    df = xar.DataArray(
+                        data=zdata,
+                        dims=["x", "y"],
+                        coords=dict(x=x0, y=y0),
+                    )
+                    df = xar.Dataset(dict(val=df))
+            else:
+                try:
+                    # try if reprojected coordinates can be used as 2d grid and if yes,
+                    # directly use a curvilinear QuadMesh based on the reprojected
+                    # coordinates to display the data
+                    idx = pd.MultiIndex.from_arrays(
+                        [x0.ravel(), y0.ravel()], names=["x", "y"]
                     )
-                    self.show_layer(layer_with_bg)
-                    sn = self._get_snapshot()
-                    # restore the previous layer
-                    self.BM._refetch_layer(layer_with_bg)
-                    self.show_layer(initial_layer)
-                else:
-                    if layer is not None:
-                        self.show_layer(layer)
-                        sn = self._get_snapshot()
-                        self.show_layer(initial_layer)
-                    else:
-                        sn = self._get_snapshot()
-            try:
-                from IPython.display import display_png, clear_output
-
-                if clear:
-                    clear_output(wait=True)
-                # use display_png to avoid issues with transparent snapshots
-                display_png(Image.fromarray(sn, "RGBA"), raw=False)
 
-            except Exception:
-                _log.exception(
-                    "Unable to display the snapshot... is the script "
-                    "running in an IPython console?",
-                    exc_info=_log.getEffectiveLevel() <= logging.DEBUG,
-                )
-        except Exception:
-            _log.exception(
-                "Encountered an error while trying to create a snapshot.",
-                exc_info=_log.getEffectiveLevel() <= logging.DEBUG,
-            )
-        finally:
-            self._snapshotting = False
+                    df = pd.DataFrame(
+                        data=dict(val=zdata.ravel()), index=idx, copy=False
+                    )
+                    df = df.to_xarray()
+                    xg, yg = np.meshgrid(df.x, df.y)
+                except Exception:
+                    # first convert original coordinates of the 1D inputs to 2D,
+                    # then reproject the grid and use a curvilinear QuadMesh to display
+                    # the data
+                    _log.warning(
+                        "EOmaps: 1D data is converted to 2D prior to reprojection... "
+                        "Consider using 'shade_points' as plot-shape instead!"
+                    )
+                    xorig = self._data_manager.xorig.ravel()
+                    yorig = self._data_manager.yorig.ravel()
 
-    @wraps(plt.Figure.text)
-    def text(self, *args, layer=None, **kwargs):
-        """Add text to the map."""
-        kwargs.setdefault("animated", True)
-        kwargs.setdefault("horizontalalignment", "center")
-        kwargs.setdefault("verticalalignment", "center")
+                    idx = pd.MultiIndex.from_arrays([xorig, yorig], names=["x", "y"])
 
-        a = self.f.text(*args, **kwargs)
+                    df = pd.DataFrame(
+                        data=dict(val=zdata.ravel()), index=idx, copy=False
+                    )
+                    df = df.to_xarray()
+                    xg, yg = np.meshgrid(df.x, df.y)
 
-        if layer is None:
-            layer = self.layer
-        self.BM.add_artist(a, layer=layer)
-        self.BM.update()
+                    # transform the grid from input-coordinates to the plot-coordinates
+                    crs1 = CRS.from_user_input(self.data_specs.crs)
+                    crs2 = CRS.from_user_input(self._crs_plot)
+                    if crs1 != crs2:
+                        transformer = self._get_transformer(
+                            crs1,
+                            crs2,
+                        )
+                        xg, yg = transformer.transform(xg, yg)
 
-        return a
+                # use a curvilinear QuadMesh
+                if self.shape.name == "shade_raster":
+                    self.shape.glyph = ds.glyphs.QuadMeshCurvilinear("x", "y", "val")
 
-    @_add_to_docstring(
-        insert={
-            "Other Parameters": (
-                "refetch_wms : bool\n"
-                "    If True, re-fetch EOmaps WebMap services with respect to "
-                "the dpi of the exported figure before exporting the image. "
-                "\n\n    NOTE: This might fail for high-dpi exports and might "
-                "result in a completely different appearance of the wms-images "
-                "in the exported file! "
-                "\n\n    See `m.refetch_wms_on_size_change()` for more details. "
-                "The default is False",
-                1,
-            )
-        }
-    )
-    @wraps(plt.savefig)
-    def savefig(self, *args, refetch_wms=False, rasterize_data=True, **kwargs):
-        """Save the figure."""
-        # get the currently visible layer (to restore it after saving is done)
-        initial_layer = self.BM.bg_layer
-
-        if plt.get_backend() == "agg":
-            # make sure that a draw-event was triggered when using the agg backend
-            # (to avoid export-issues with some shapes)
-            # TODO properly assess why this is necessary!
-            self.f.canvas.draw_idle()
+                df = xar.Dataset(
+                    data_vars=dict(val=(["xx", "yy"], df.val.values.T)),
+                    coords=dict(x=(["xx", "yy"], xg), y=(["xx", "yy"], yg)),
+                )
 
-        with ExitStack() as stack:
-            if refetch_wms is False:
-                if _cx_refetch_wms_on_size_change is not None:
-                    stack.enter_context(_cx_refetch_wms_on_size_change(refetch_wms))
+            if self.shape.name == "shade_points":
+                df = df.to_dataframe().reset_index()
 
-                # don't clear on layer-changes
-                stack.enter_context(self.BM._cx_dont_clear_on_layer_change())
+        if set_extent is True and self._set_extent_on_plot is True:
+            # convert to a numpy-array to support 2D indexing with boolean arrays
+            x, y = np.asarray(df.x), np.asarray(df.y)
+            xf, yf = np.isfinite(x), np.isfinite(y)
+            x_range = (np.nanmin(x[xf]), np.nanmax(x[xf]))
+            y_range = (np.nanmin(y[yf]), np.nanmax(y[yf]))
+        else:
+            # update here to ensure bounds are set
+            self.BM.update()
+            x0, x1, y0, y1 = self.get_extent(self.crs_plot)
+            x_range = (x0, x1)
+            y_range = (y0, y1)
 
-            # hide companion-widget indicator
-            self._indicate_companion_map(False)
+        coll = mpl_ext.dsshow(
+            df,
+            glyph=self.shape.glyph,
+            aggregator=self.shape.aggregator,
+            shade_hook=self.shape.shade_hook,
+            agg_hook=self.shape.agg_hook,
+            # norm="eq_hist",
+            # norm=plt.Normalize(vmin, vmax),
+            cmap=self._cbcmap,
+            ax=self.ax,
+            plot_width=plot_width,
+            plot_height=plot_height,
+            # x_range=(x0, x1),
+            # y_range=(y0, y1),
+            # x_range=(df.x.min(), df.x.max()),
+            # y_range=(df.y.min(), df.y.max()),
+            x_range=x_range,
+            y_range=y_range,
+            vmin=self._vmin,
+            vmax=self._vmax,
+            **kwargs,
+        )
 
-            # add the figure background patch as the bottom layer
-            transparent = kwargs.get("transparent", False)
-            if transparent is False:
-                showlayer_name = self.BM._get_showlayer_name(initial_layer)
-                layer_with_bg = self.BM._get_combined_layer_name(
-                    "__BG__", showlayer_name
-                )
-                self.show_layer(layer_with_bg)
+        coll.set_label("Dataset " f"({self.shape.name}  |  {zdata.shape})")
 
-            dpi = kwargs.get("dpi", None)
+        self._coll = coll
 
-            redraw = False
-            if dpi is not None and dpi != self.f.dpi or "bbox_inches" in kwargs:
-                redraw = True
-
-                # clear all cached background layers before saving to make sure they
-                # are re-drawn with the correct dpi-settings
-                self.BM._refetch_bg = True
+        if dynamic is True:
+            self.BM.add_artist(coll, layer)
+        else:
+            self.BM.add_bg_artist(coll, layer)
 
-                # set the shading-axis-size to reflect the used dpi setting
-                self._update_shade_axis_size(dpi=dpi)
+        if dynamic is True:
+            self.BM.update(clear=False)
 
-            # get all layer names that should be drawn
-            savelayers, alphas = self.BM._parse_multi_layer_str(
-                self.BM._get_showlayer_name(self.BM.bg_layer)
-            )
+    def set_shade_dpi(self, dpi=None):
+        """
+        Set the dpi used by "shade shapes" to aggregate datasets.
 
-            # make sure inset-maps are drawn on top of normal maps
-            savelayers.sort(key=lambda x: x.startswith("__inset_"))
+        This only affects the plot-shapes "shade_raster" and "shade_points".
 
-            for m in (self.parent, *self.parent._children):
-                # re-enable normal axis draw cycle by making axes non-animated.
-                # This is needed for backward-compatibility, since saving a figure
-                # ignores the animated attribute for axis-children but not for the axis
-                # itself. See:
-                # https://github.com/matplotlib/matplotlib/issues/26007#issuecomment-1568812089
-                stack.enter_context(m.ax._cm_set(animated=False))
+        Note
+        ----
+        If dpi=None is used (the default), datasets in exported figures will be
+        re-rendered with respect to the requested dpi of the exported image!
 
-                # handle colorbars
-                for cb in m._colorbars:
-                    for a in (cb.ax_cb, cb.ax_cb_plot):
-                        stack.enter_context(a._cm_set(animated=False))
+        Parameters
+        ----------
+        dpi : int or None, optional
+            The dpi to use for data aggregation with shade shapes.
+            If None, the figure-dpi is used.
 
-                # set if data should be rasterized on vector export
-                if m.coll is not None:
-                    stack.enter_context(m.coll._cm_set(rasterized=rasterize_data))
+            The default is None.
 
-            # explicitly set axes to non-animated to re-enable draw cycle
-            for a in m.BM._managed_axes:
-                stack.enter_context(a._cm_set(animated=False))
-
-            zorder = 0
-            for layer, alpha in zip(savelayers, alphas):
-                # get all (sorted) artists of a layer
-                if layer.startswith("__inset"):
-                    artists = self.BM.get_bg_artists(["__inset_all", layer])
-                else:
-                    if layer.startswith("__"):
-                        artists = self.BM.get_bg_artists([layer])
-                    else:
-                        artists = self.BM.get_bg_artists(["all", layer])
+        """
+        self._shade_dpi = dpi
+        self._update_shade_axis_size()
 
-                for a in artists:
-                    if isinstance(a, plt.Axes):
-                        continue
-                    zorder += 1
-                    stack.enter_context(a._cm_set(zorder=zorder, animated=False))
-
-                    if alpha < 1:
-                        current_alpha = a.get_alpha()
-                        if current_alpha is None:
-                            current_alpha = alpha
-                        else:
-                            current_alpha = current_alpha * alpha
-
-                        stack.enter_context(a._cm_set(alpha=current_alpha))
-
-            for key, val in self.BM._bg_artists.items():
-                if key not in ["all", "__inset_all", *savelayers]:
-                    for a in val:
-                        stack.enter_context(a._cm_set(visible=False, animated=True))
-
-            if any(l.startswith("__inset") for l in savelayers):
-                if "__inset_all" not in savelayers:
-                    savelayers.append("__inset_all")
-                    alphas.append(1)
-            if "all" not in savelayers:
-                savelayers.append("all")
-                alphas.append(1)
-
-            # always draw dynamic artists on top of background artists
-            for layer, alpha in zip(savelayers, alphas):
-                # get all (sorted) artists of a layer
-                artists = self.BM.get_artists([layer])
-
-                for a in artists:
-                    zorder += 1
-                    stack.enter_context(a._cm_set(zorder=zorder, animated=False))
-
-            for key, val in self.BM._artists.items():
-                if key not in savelayers:
-                    for a in val:
-                        stack.enter_context(a._cm_set(visible=False, animated=True))
-
-            # trigger a redraw of all savelayers to make sure unmanaged artists
-            # and ordinary matplotlib axes are properly drawn
-            self.redraw(*savelayers)
-            # flush events prior to savefig to avoid issues with pending draw events
-            # that cause wrong positioning of grid-labels and missing artists!
+    def _get_shade_axis_size(self, dpi=None, flush=True):
+        if flush:
+            # flush events before evaluating shade sizes to make sure axes dimensions have
+            # been properly updated
             self.f.canvas.flush_events()
-            self.f._mpl_orig_savefig(*args, **kwargs)
 
-        if redraw is True:
-            # reset the shading-axis-size to the used figure dpi
-            self._update_shade_axis_size()
+        if self._shade_dpi is not None:
+            dpi = self._shade_dpi
 
-            # restore the previous layer if background was added on save
-            if transparent is False:
-                self.show_layer(initial_layer)
+        fig_dpi = self.f.dpi
+        w, h = self.ax.bbox.width, self.ax.bbox.height
 
-            # redraw after the save to ensure that backgrounds are correctly cached
-            self.redraw()
+        # TODO for now, only handle numeric dpi-values to avoid issues.
+        # (savefig also seems to support strings like "figure" etc.)
+        if isinstance(dpi, (int, float, np.number)):
+            width = int(w / fig_dpi * dpi)
+            height = int(h / fig_dpi * dpi)
+        else:
+            width = int(w)
+            height = int(h)
+
+        return width, height
+
+    def _update_shade_axis_size(self, dpi=None, flush=True):
+        # method to update all shade-dpis
+        # NOTE: provided dpi value is only used if no explicit "_shade_dpi" is set!
+
+        # set the axis-size that is used to determine the number of pixels used
+        # when using "shade" shapes for ALL maps objects of a figure
+        for m in (self.parent, *self.parent._children):
+            if m.coll is not None and m.shape.name.startswith("shade_"):
+                w, h = m._get_shade_axis_size(dpi=dpi, flush=flush)
+                m.coll.plot_width = w
+                m.coll.plot_height = h
 
-    def fetch_layers(self, layers=None):
+    def make_dataset_pickable(
+        self,
+    ):
         """
-        Fetch (and cache) the layers of a map.
+        Make the associated dataset pickable **without plotting** it first.
 
-        This is particularly useful if you want to use sliders or buttons to quickly
-        switch between the layers (e.g. once the backgrounds are cached, switching
-        layers will be fast).
+        After executing this function, `m.cb.pick` callbacks can be attached to the
+        `Maps` object.
 
-        Note: After zooming or re-sizing the map, the cache is cleared and
-        you need to call this function again.
+        NOTE
+        ----
+        This function is ONLY necessary if you want to use pick-callbacks **without**
+        actually plotting the data**! Otherwise a call to `m.plot_map()` is sufficient!
 
-        Parameters
-        ----------
-        layers : list or None, optional
-            A list of layer-names that should be fetched.
-            If None, all layers (except the "all" layer) are fetched.
-            The default is None.
+        - Each `Maps` object can always have only one pickable dataset.
+        - The used data is always the dataset that was assigned in the last call to
+          `m.plot_map()` or `m.make_dataset_pickable()`.
+        - To get multiple pickable datasets, use an individual layer for each of the
+          datasets (e.g. first `m2 = m.new_layer()` and then assign the data to `m2`)
 
-        See Also
+        Examples
         --------
-        Maps.cb.keypress.attach.fetch_layers : use a keypress callback to fetch layers
-
+        >>> m = Maps()
+        >>> m.add_feature.preset.coastline()
+        >>> ...
+        >>> # a dataset that should be pickable but NOT visible...
+        >>> m2 = m.new_layer()
+            >>> m2.set_data(*np.linspace([0, -180,-90,], [100, 180, 90], 100).T)
+        >>> m2.make_dataset_pickable()
+        >>> m2.cb.pick.attach.annotate()  # get an annotation for the invisible dataset
+        >>> # ...call m2.plot_map() to make the dataset visible...
         """
-        active_layer = self.BM._bg_layer
-        all_layers = self._get_layers()
+        if self.coll is not None:
+            _log.error(
+                "EOmaps: There is already a dataset plotted on this Maps-object. "
+                "You MUST use a new layer (`m2 = m.new_layer()`) to use "
+                "`m2.make_dataset_pickable()`!"
+            )
+            return
 
-        if layers is None:
-            layers = all_layers
-            if "all" in layers:
-                layers.remove("all")  # don't explicitly fetch the "all" layer
-        else:
-            if not set(layers).issubset(all_layers):
-                raise AssertionError(
-                    "EOmaps: Unable to fetch the following layers:\n - "
-                    + "\n - ".join(set(layers).difference(all_layers))
-                )
+        # ---------------------- prepare the data
+        self._data_manager = DataManager(self._proxy(self))
+        self._data_manager.set_props(layer=self.layer, only_pick=True)
 
-        nlayers = len(layers)
-        assert nlayers > 0, "EOmaps: There are no layers to fetch."
+        x0, x1 = self._data_manager.x0.min(), self._data_manager.x0.max()
+        y0, y1 = self._data_manager.y0.min(), self._data_manager.y0.max()
 
-        for i, l in enumerate(layers):
-            _log.info(f"EOmaps: fetching layer {i + 1}/{nlayers}: {l}")
-            self.show_layer(l)
+        # use a transparent rectangle of the data-extent as artist for picking
+        (art,) = self.ax.fill([x0, x1, x1, x0], [y0, y0, y1, y1], fc="none", ec="none")
 
-        self.show_layer(active_layer)
-        self.BM.update()
+        self._coll = art
 
-    def join_limits(self, *args):
-        """
-        Join the x- and y- limits of the maps (crs must be equal!).
+        self.tree = SearchTree(m=self._proxy(self))
+        self.cb.pick._set_artist(art)
+        self.cb.pick._init_cbs()
+        self.cb._methods.add("pick")
 
-        Parameters
-        ----------
-        *args :
-            the axes to join.
-        """
-        for m in args:
-            if m is not self:
-                self._join_axis_limits(weakref.proxy(m))
+        self._coll_kwargs = dict()
+        self._coll_dynamic = True
+
+        # set _data_plotted to True to trigger updates in the data-manager
+        self._data_plotted = True
 
     def copy(
         self,
         data_specs=False,
         classify_specs=True,
         shape=True,
         **kwargs,
@@ -3701,162 +3256,75 @@
             classify_specs = list(self.classify_specs.keys())
             copy_cls.set_classify_specs(
                 scheme=self.classify_specs.scheme, **self.classify_specs
             )
 
         return copy_cls
 
-    def indicate_extent(self, x0, y0, x1, y1, crs=4326, npts=100, **kwargs):
-        """
-        Indicate a rectangular extent in a given crs on the map.
-
-        Parameters
-        ----------
-        x0, y0, y1, y1 : float
-            the boundaries of the shape
-        npts : int, optional
-            The number of points used to draw the polygon-lines.
-            (e.g. to correctly display the distortion of the extent-rectangle when
-            it is re-projected to another coordinate-system)
-            The default is 100.
-        crs : any, optional
-            A coordinate-system identifier.
-            The default is 4326 (e.g. lon/lat).
-        kwargs :
-            Additional keyword-arguments passed to `m.add_gdf()`.
-        """
-        register_modules("geopandas")
-
-        gdf = self._make_rect_poly(x0, y0, x1, y1, self.get_crs(crs), npts)
-        self.add_gdf(gdf, **kwargs)
-
     def redraw(self, *args):
-        """
-        Force a re-draw of cached background layers.
-
-        - Use this at the very end of your code to trigger a final re-draw
-          to make sure artists not managed by EOmaps are properly drawn!
-
-        Note
-        ----
-        Don't use this to interactively update artists on a map!
-        since it will trigger a re-draw background-layers!
-
-        To dynamically re-draw an artist whenever you interact with the map, use:
-
-        >>> m.BM.add_artist(artist)
-
-        To make an artist temporary (e.g. remove it on the next event), use
-        one of :
-
-        >>> m.cb.click.add_temporary_artist(artist)
-        >>> m.cb.pick.add_temporary_artist(artist)
-        >>> m.cb.keypress.add_temporary_artist(artist)
-        >>> m.cb.move.add_temporary_artist(artist)
-
-        Parameters
-        ----------
-        *args : str
-            Positional arguments provided to redraw are identified as layer-names
-            that should be re-drawn. If no arguments are provided, all layers
-            are re-drawn!
+        self._data_manager.last_extent = None
+        super().redraw(*args)
 
-        """
-        if len(args) == 0:
-            # in case no argument is provided, force a complete re-draw of
-            # all layers (and datasets) of the map
-            self.BM._refetch_bg = True
-            self._data_manager.last_extent = None
-        else:
-            # only re-fetch the required layers
-            for l in args:
-                self.BM._refetch_layer(l)
-
-        self.f.canvas.draw_idle()
-
-    @wraps(GridSpec.update)
-    def subplots_adjust(self, **kwargs):
-        """Adjust the margins of subplots."""
-        self.parent._gridspec.update(**kwargs)
-        # after changing margins etc. a redraw is required
-        # to fetch the updated background!
-
-        self.redraw()
-
-    def on_layer_activation(self, func, layer=None, persistent=False, **kwargs):
-        """
-        Attach a callback that is executed if the associated layer is activated.
-
-        Useful to "lazily" populate layers with features that are expensive to
-        create (e.g. fetching data from files etc.).
-
-        Parameters
-        ----------
-        func : callable
-            The callable to use.
-            The call-signature is:
-
-            >>> def func(m, **kwargs):
-            >>>    # m... the Maps-object used for calling this function
-
-            NOTE: The Maps-object that is passed to the function is determined by
-            the 'layer' argument!
-        layer : str or None, optional
-            If provided, a NEW layer will be created and passed to the execution of the
-            function. Otherwise, the calling Maps-object is used.
+    def snapshot(self, *args, **kwargs):
+        # hide companion-widget indicator
+        for m in (self.parent, *self.parent._children):
+            # hide companion-widget indicator
+            m._indicate_companion_map(False)
 
-            To clarify: The following two code-snippets are equivalent:
+        super().snapshot(*args, **kwargs)
 
-            >>> m = Maps()
-            >>> m2 = m.new_layer("my_layer")
-            >>> m2.on_layer_activation(func)
+    @_add_to_docstring(
+        insert={
+            "Other Parameters": (
+                "refetch_wms : bool\n"
+                "    If True, re-fetch EOmaps WebMap services with respect to "
+                "the dpi of the exported figure before exporting the image. "
+                "\n\n    NOTE: This might fail for high-dpi exports and might "
+                "result in a completely different appearance of the wms-images "
+                "in the exported file! "
+                "\n\n    See `m.refetch_wms_on_size_change()` for more details. "
+                "The default is False",
+                1,
+            )
+        }
+    )
+    @wraps(MapsBase.savefig)
+    def savefig(self, *args, refetch_wms=False, rasterize_data=True, **kwargs):
+        with ExitStack() as stack:
+            # re-fetch webmap servies if required
+            if refetch_wms is False:
+                if _cx_refetch_wms_on_size_change is not None:
+                    stack.enter_context(_cx_refetch_wms_on_size_change(refetch_wms))
 
-            >>> m = Maps()
-            >>> m.on_layer_activation(func, layer="my_layer")
+            for m in (self.parent, *self.parent._children):
+                # hide companion-widget indicator
+                m._indicate_companion_map(False)
 
-        persistent : bool, optional
-            Indicator if the function should be called only once (False) or if it
-            should be called each time the layer is activated (True).
-            The default is False.
-        kwargs :
-            Additional keyword-arguments passed to the call of the function.
+                # handle colorbars
+                for cb in m._colorbars:
+                    for a in (cb.ax_cb, cb.ax_cb_plot):
+                        stack.enter_context(a._cm_set(animated=False))
 
-        See Also
-        --------
-        Maps.layer : The layer-name associated with the Maps-object
-        Maps.fetch_layers : Fetch and cache all layers of the map
+                # set if data should be rasterized on vector export
+                if m.coll is not None:
+                    stack.enter_context(m.coll._cm_set(rasterized=rasterize_data))
 
-        Examples
-        --------
-        >>> m = Maps()
-        >>> m.add_feature.preset.coastline()
-        >>>
-        >>> def f(m, ocean_color, coastline_color):
-        >>>     print(f"EOmaps: creating features for the layer {m.layer}")
-        >>>     m.add_feature.preset.coastline(ec=coastline_color)
-        >>>     m.add_feature.preset.ocean(fc=ocean_color)
-        >>>
-        >>> # create a new (initially empty) layer "ocean"
-        >>> m2 = m.new_layer("ocean")
-        >>> # add features to the layer only if it is activated
-        >>> m2.on_layer_activation(f, ocean_color="b", coastline_color="r")
-        >>> s = m.util.layer_selector()
+            dpi = kwargs.get("dpi", None)
 
-        """
-        if layer is None:
-            layer = self.layer
-            m = self
-        else:
-            layer = str(layer)
-            m = self.new_layer(layer)
+            shade_dpi_changed = False
+            if dpi is not None and dpi != self.f.dpi:
+                shade_dpi_changed = True
+                # set the shading-axis-size to reflect the used dpi setting
+                self._update_shade_axis_size(dpi=dpi)
 
-        def cb(m, layer):
-            func(m=m, **kwargs)
+            super().savefig(*args, **kwargs)
 
-        self.BM.on_layer(func=cb, layer=layer, persistent=persistent, m=m)
+        if shade_dpi_changed:
+            # reset the shading-axis-size to the used figure dpi
+            self._update_shade_axis_size()
 
     def cleanup(self):
         """
         Cleanup all references to the object so that it can be safely deleted.
 
         This function is primarily used internally to clear objects if the figure
         is closed.
@@ -3864,27 +3332,24 @@
         Note
         ----
         Executing this function will remove ALL attached callbacks
         and delete all assigned datasets & pre-computed values.
 
         ONLY execute this if you do not need to do anything with the layer
         """
-        try:
-            # disconnect callback on xlim-change (only relevant for parent)
-            if not self._is_sublayer:
-                try:
-                    if hasattr(self, "_cid_xlim"):
-                        self.ax.callbacks.disconnect(self._cid_xlim)
-                        del self._cid_xlim
-                except Exception:
-                    _log.error(
-                        "EOmaps-cleanup: Problem while clearing xlim-cid",
-                        exc_info=_log.getEffectiveLevel() <= logging.DEBUG,
-                    )
 
+        # close the pyqt widget if there is one
+        if self._companion_widget is not None:
+            self._companion_widget.close()
+
+        # de-register colormaps
+        for cmap in self._registered_cmaps:
+            plt.colormaps.unregister(cmap)
+
+        try:
             # clear data-specs and all cached properties of the data
             try:
                 self._coll = None
                 self._data_manager.cleanup()
 
                 if hasattr(self, "tree"):
                     del self.tree
@@ -3902,27 +3367,22 @@
                 self.cb._clear_callbacks()
             except Exception:
                 _log.error(
                     "EOmaps-cleanup: Problem while clearing callbacks",
                     exc_info=_log.getEffectiveLevel() <= logging.DEBUG,
                 )
 
-            # cleanup all artists and cached background-layers from the blit-manager
-            if not self._is_sublayer:
-                self.BM._cleanup_layer(self.layer)
-
-            # remove the child from the parent Maps object
-            if self in self.parent._children:
-                self.parent._children.remove(self)
         except Exception:
             _log.error(
                 "EOmaps: Cleanup problem!",
                 exc_info=_log.getEffectiveLevel() <= logging.DEBUG,
             )
 
+        super().cleanup()
+
     def _save_to_clipboard(self, **kwargs):
         """
         Export the figure to the clipboard.
 
         Parameters
         ----------
         kwargs :
@@ -3937,15 +3397,16 @@
         # guess the MIME type from the provided file-extension
         fmt = kwargs.get("format", "png")
         mimetype, _ = mimetypes.guess_type(f"dummy.{fmt}")
 
         message = f"EOmaps: Exporting figure as '{fmt}' to clipboard..."
         _log.info(message)
 
-        if self._companion_widget is not None:
+        # TODO remove dependency on companion widget here
+        if getattr(self, "_companion_widget", None) is not None:
             self._companion_widget.window().statusBar().showMessage(message, 2000)
 
         with io.BytesIO() as buffer:
             self.savefig(buffer, **kwargs)
             data = QMimeData()
 
             cb = QApplication.clipboard()
@@ -3979,312 +3440,14 @@
             except Exception:
                 _log.exception(
                     "EOmaps: Encountered a problem while trying to export the figure "
                     "to the clipboard.",
                     exc_info=_log.getEffectiveLevel() <= logging.DEBUG,
                 )
 
-    def _init_figure(self, ax=None, plot_crs=None, **kwargs):
-        if self.parent.f is None:
-            # do this on any new figure since "%matpltolib inline" tries to re-activate
-            # interactive mode all the time!
-            _handle_backends()
-
-            self._f = plt.figure(**kwargs)
-            # to hide canvas header in jupyter notebooks (default figure label)
-            self._f.canvas.header_visible = False
-
-            # override Figure.savefig with Maps.savefig but keep original
-            # method accessible via Figure._mpl_orig_savefig
-            # (this ensures that using the save-buttons in the gui or pressing
-            # control+s will redirect the save process to the eomaps routine)
-            self._f._mpl_orig_savefig = self._f.savefig
-            self._f.savefig = self.savefig
-
-            _log.debug("EOmaps: New figure created")
-
-            # make sure we keep a "real" reference otherwise overwriting the
-            # variable of the parent Maps-object while keeping the figure open
-            # causes all weakrefs to be garbage-collected!
-            self.parent.f._EOmaps_parent = self.parent._real_self
-
-            newfig = True
-        else:
-            newfig = False
-            if not hasattr(self.parent.f, "_EOmaps_parent"):
-                self.parent.f._EOmaps_parent = self.parent._real_self
-            self.parent._add_child(self)
-
-        # attach a callback to show/hide the companion-widget with the "w" key
-        if self.parent._cid_keypress is None:
-            # NOTE the companion-widget is ONLY attached to the parent map
-            # since it will identify the clicked map automatically! The
-            # widget will only be initialized on Maps-objects that create
-            # NEW axes. This is required to make sure that any additional
-            # Maps-object on the same axes will then always use the
-            # same widget. (otherwise each layer would get its own widget)
-
-            self.parent._cid_keypress = self.f.canvas.mpl_connect(
-                "key_press_event", self.parent._on_keypress
-            )
-
-        if isinstance(ax, plt.Axes):
-            # check if the axis is already used by another maps-object
-            if ax not in (i.ax for i in (self.parent, *self.parent._children)):
-                newax = True
-                ax.set_animated(True)
-                # make sure axes are drawn once to properly set transforms etc.
-                # (otherwise pan/zoom, ax.contains_point etc. will not work)
-                ax.draw(self.f.canvas.get_renderer())
-
-            else:
-                newax = False
-        else:
-            newax = True
-            # create a new axis
-            if ax is None:
-                gs = GridSpec(
-                    nrows=1, ncols=1, left=0.01, right=0.99, bottom=0.05, top=0.95
-                )
-                gsspec = [gs[:]]
-            elif isinstance(ax, SubplotSpec):
-                gsspec = [ax]
-            elif isinstance(ax, (list, tuple)) and len(ax) == 4:
-                # absolute position
-                l, b, w, h = ax
-
-                gs = GridSpec(
-                    nrows=1, ncols=1, left=l, bottom=b, right=l + w, top=b + h
-                )
-                gsspec = [gs[:]]
-            elif isinstance(ax, int) and len(str(ax)) == 3:
-                gsspec = [ax]
-            elif isinstance(ax, tuple) and len(ax) == 3:
-                gsspec = ax
-            else:
-                raise TypeError("EOmaps: The provided value for 'ax' is invalid.")
-
-            projection = self._get_cartopy_crs(plot_crs)
-
-            ax = self.f.add_subplot(
-                *gsspec,
-                projection=projection,
-                aspect="equal",
-                adjustable="box",
-                label=self._get_ax_label(),
-                animated=True,
-            )
-            # make sure axes are drawn once to properly set transforms etc.
-            # (otherwise pan/zoom, ax.contains_point etc. will not work)
-            ax.draw(self.f.canvas.get_renderer())
-
-        self._ax = ax
-        self._gridspec = ax.get_gridspec()
-
-        # add support for "frameon" kwarg
-        if kwargs.get("frameon", True) is False:
-            self.ax.spines["geo"].set_edgecolor("none")
-
-        # initialize the callbacks
-        self.cb._init_cbs()
-
-        if newax:  # only if a new axis has been created
-            self._new_axis_map = True
-
-            # explicitly set initial limits to global to avoid issues if NE-features
-            # are added (and clipped) before actual limits are set
-            self.ax.set_global()
-
-            self._cid_xlim = self.ax.callbacks.connect(
-                "xlim_changed", self._on_xlims_change
-            )
-            self._cid_xlim = self.ax.callbacks.connect(
-                "ylim_changed", self._on_ylims_change
-            )
-        else:
-            self._new_axis_map = False
-
-        if self.parent == self:  # use == instead of "is" since the parent is a proxy!
-            # only attach resize- and close-callbacks if we initialize a parent
-            # Maps-object
-            # attach a callback that is executed when the figure is closed
-            self._cid_onclose = self.f.canvas.mpl_connect("close_event", self._on_close)
-            # attach a callback that is executed if the figure canvas is resized
-            self._cid_resize = self.f.canvas.mpl_connect(
-                "resize_event", self._on_resize
-            )
-
-        # if we haven't attached an axpicker so far, do it!
-        if self.parent._layout_editor is None:
-            self.parent._layout_editor = LayoutEditor(self.parent, modifier="alt+l")
-
-        active_backend = plt.get_backend()
-
-        if active_backend == "module://matplotlib_inline.backend_inline":
-            # close the figure to avoid duplicated (empty) plots created
-            # by the inline-backend manager in jupyter notebooks
-            plt.close(self.f)
-
-    def _get_ax_label(self):
-        return "map"
-
-    def _on_xlims_change(self, *args, **kwargs):
-        self.BM._refetch_bg = True
-
-    def _on_ylims_change(self, *args, **kwargs):
-        self.BM._refetch_bg = True
-
-    def _on_resize(self, event):
-        # make sure the background is re-fetched if the canvas has been resized
-        # (required for peeking layers after the canvas has been resized
-        #  and for webagg and nbagg backends to correctly re-draw the layer)
-
-        self.BM._refetch_bg = True
-        self.BM._refetch_blank = True
-
-        # update the figure dimensions in case shading is used
-        self._update_shade_axis_size()
-
-    def _update_shade_axis_size(self, dpi=None):
-        # set the axis-size that is used to determine the number of pixels used
-        # when using "shade" shapes for ALL maps objects of a figure
-        w, h = self.ax.bbox.width, self.ax.bbox.height
-        fig_dpi = self.f.dpi
-
-        for m in (self.parent, *self.parent._children):
-            if m.coll is not None and m.shape.name.startswith("shade_"):
-                # TODO for now, only handle numeric dpi-values to avoid issues.
-                # (savefig also seems to support strings like "figure" etc.)
-                if isinstance(dpi, (int, float, np.number)):
-                    m.coll.plot_width = int(w / fig_dpi * dpi)
-                    m.coll.plot_height = int(h / fig_dpi * dpi)
-                else:
-                    m.coll.plot_width = int(w)
-                    m.coll.plot_height = int(h)
-
-    def _on_close(self, event):
-        # reset attributes that might use up a lot of memory when the figure is closed
-        for m in [self.parent, *self.parent._children]:
-            if hasattr(m.f, "_EOmaps_parent"):
-                m.f._EOmaps_parent = None
-
-            m.cleanup()
-
-            # close the pyqt widget if there is one
-            if m._companion_widget is not None:
-                m._companion_widget.close()
-
-        # de-register colormaps
-        for cmap in self._registered_cmaps:
-            plt.colormaps.unregister(cmap)
-
-        # run garbage-collection to immediately free memory
-        gc.collect
-
-    def _join_axis_limits(self, m):
-        if self.ax.projection != m.ax.projection:
-            _log.warning(
-                "EOmaps: joining axis-limits is only possible for "
-                + "axes with the same projection!"
-            )
-            return
-
-        self.ax._EOmaps_joined_action = False
-        m.ax._EOmaps_joined_action = False
-
-        # Declare and register callbacks
-        def child_xlims_change(event_ax):
-            if event_ax._EOmaps_joined_action is not m.ax:
-                m.ax._EOmaps_joined_action = event_ax
-                m.ax.set_xlim(event_ax.get_xlim())
-            event_ax._EOmaps_joined_action = False
-
-        def child_ylims_change(event_ax):
-            if event_ax._EOmaps_joined_action is not m.ax:
-                m.ax._EOmaps_joined_action = event_ax
-                m.ax.set_ylim(event_ax.get_ylim())
-            event_ax._EOmaps_joined_action = False
-
-        def parent_xlims_change(event_ax):
-            if event_ax._EOmaps_joined_action is not self.ax:
-                self.ax._EOmaps_joined_action = event_ax
-                self.ax.set_xlim(event_ax.get_xlim())
-            event_ax._EOmaps_joined_action = False
-
-        def parent_ylims_change(event_ax):
-            if event_ax._EOmaps_joined_action is not self.ax:
-                self.ax._EOmaps_joined_action = event_ax
-                self.ax.set_ylim(event_ax.get_ylim())
-
-            event_ax._EOmaps_joined_action = False
-
-        self.ax.callbacks.connect("xlim_changed", child_xlims_change)
-        self.ax.callbacks.connect("ylim_changed", child_ylims_change)
-
-        m.ax.callbacks.connect("xlim_changed", parent_xlims_change)
-        m.ax.callbacks.connect("ylim_changed", parent_ylims_change)
-
-    def _add_child(self, m):
-        self.parent._children.add(m)
-
-        # execute hooks to notify the gui that a new child was added
-        for action in self._after_add_child:
-            try:
-                action()
-            except Exception:
-                _log.exception("EOmaps: Problem executing 'on_add_child' action:")
-
-    def inherit_classification(self, m):
-        """
-        Use the classification of another Maps-object when plotting the data.
-
-        NOTE
-        ----
-        If the classification is inherited, the following arguments
-        for `m.plot_map()` will have NO effect (they are inherited):
-
-            - "cmap"
-            - "vmin"
-            - "vmax"
-
-        Parameters
-        ----------
-        m : eomaps.Maps or None
-            The Maps-object that provides the classification specs.
-        """
-        if m is not None:
-            self._inherit_classification = self._proxy(m)
-        else:
-            self._inherit_classification = None
-
-    def inherit_data(self, m):
-        """
-        Use the data of another Maps-object (without copying).
-
-        NOTE
-        ----
-        If the data is inherited, any change in the data of the parent
-        Maps-object will be reflected in this Maps-object as well!
-
-        Parameters
-        ----------
-        m : eomaps.Maps or None
-            The Maps-object that provides the data.
-        """
-        if m is not None:
-            self.data_specs = m.data_specs
-
-            def set_data(*args, **kwargs):
-                raise AssertionError(
-                    "EOmaps: You cannot set data for a Maps object that "
-                    "inherits data!"
-                )
-
-            self.set_data = set_data
-
     def _classify_data(
         self,
         z_data=None,
         cmap=None,
         vmin=None,
         vmax=None,
         classify_specs=None,
@@ -4352,30 +3515,36 @@
             classified = False
             bins = None
             cbcmap = cmap
             norm = None
 
         return cbcmap, norm, bins, classified
 
-    def _set_parent(self):
-        """Identify the parent object."""
-        assert self._parent is None, "EOmaps: There is already a parent Maps object!"
-        # check if the figure to which the Maps-object is added already has a parent
-        parent = None
-        if getattr(self._f, "_EOmaps_parent", False):
-            parent = self._proxy(self._f._EOmaps_parent)
-
-        if parent is None:
-            parent = self
-
-        self._parent = self._proxy(parent)
-
-        if parent not in [self, None]:
-            # add the child to the topmost parent-object
-            self.parent._add_child(self)
+    def _get_mcl_subclass(self, s):
+        # get a subclass that inherits the docstring from the corresponding
+        # mapclassify classifier
+
+        class scheme:
+            @wraps(s)
+            def __init__(_, *args, **kwargs):
+                pass
+
+            def __new__(cls, **kwargs):
+                if "y" in kwargs:
+                    _log.error(
+                        "EOmaps: The values (e.g. the 'y' parameter) are "
+                        + "assigned internally... only provide additional "
+                        + "parameters that specify the classification scheme!"
+                    )
+                    kwargs.pop("y")
+
+                self.classify_specs._set_scheme_and_args(scheme=s.__name__, **kwargs)
+
+        scheme.__doc__ = s.__doc__
+        return scheme
 
     def _set_default_shape(self):
         if self.data is not None:
             # size = np.size(self.data)
             size = np.size(self._data_manager.z_data)
             shape = np.shape(self._data_manager.z_data)
 
@@ -4420,686 +3589,14 @@
 
         elif isinstance(ids, (list, np.ndarray)):
             mask = np.isin(ids, ID)
             ind = np.where(mask)[0]
 
         return mask, ind
 
-    def _clip_gdf(self, gdf, how="crs"):
-        """
-        Clip the shapes of a GeoDataFrame with respect to the given boundaries.
-
-        Parameters
-        ----------
-        gdf : geopandas.GeoDataFrame
-            The GeoDataFrame containing the geometries.
-        how : str, optional
-            Identifier how the clipping should be performed.
-
-            If a suffix "_invert" is added to the string, the polygon will be
-            inverted (via a symmetric-difference to the clip-shape)
-
-            - clipping with geopandas:
-              - "crs" : use the actual crs boundary polygon
-              - "crs_bounds" : use the boundary-envelope of the crs
-              - "extent" : use the current plot-extent
-
-            - clipping with gdal (always uses the crs domain as clip-shape):
-              - "gdal_Intersection"
-              - "gdal_SymDifference"
-              - "gdal_Difference"
-              - "gdal_Union"
-
-            The default is "crs".
-
-        Returns
-        -------
-        gdf
-            A GeoDataFrame with the clipped geometries
-        """
-        (gpd,) = register_modules("geopandas")
-
-        if how.startswith("gdal"):
-            methods = ["SymDifference", "Intersection", "Difference", "Union"]
-            # "SymDifference", "Intersection", "Difference"
-            method = how.split("_")[1]
-            assert method in methods, "EOmaps: '{how}' is not a valid clip-method"
-            try:
-                from osgeo import gdal
-                from shapely import wkt
-            except ImportError:
-                raise ImportError(
-                    "EOmaps: Missing dependency: 'osgeo'\n"
-                    + "...clipping with gdal requires 'osgeo.gdal'"
-                )
-
-            e = self.ax.projection.domain
-            e2 = gdal.ogr.CreateGeometryFromWkt(e.wkt)
-            if not e2.IsValid():
-                e2 = e2.MakeValid()
-
-            # only reproject geometries if crs cannot be identified
-            # as the initially provided (or cartopy converted) crs
-            if gdf.crs != self.crs_plot and gdf.crs != self._crs_plot:
-                gdf = gdf.to_crs(self.crs_plot)
-
-            clipgeoms = []
-            for g in gdf.geometry:
-                g2 = gdal.ogr.CreateGeometryFromWkt(g.wkt)
-
-                if g2 is None:
-                    continue
-
-                if not g2.IsValid():
-                    g2 = g2.MakeValid()
-
-                i = getattr(g2, method)(e2)
-
-                if how.endswith("_invert"):
-                    i = i.SymDifference(e2)
-
-                gclip = wkt.loads(i.ExportToWkt())
-                clipgeoms.append(gclip)
-
-            gdf = gpd.GeoDataFrame(geometry=clipgeoms, crs=self.crs_plot)
-
-            return gdf
-
-        if how == "crs" or how == "crs_invert":
-            clip_shp = gpd.GeoDataFrame(
-                geometry=[self.ax.projection.domain], crs=self.crs_plot
-            ).to_crs(gdf.crs)
-        elif how == "extent" or how == "extent_invert":
-            self.BM.update()
-            x0, x1, y0, y1 = self.get_extent()
-            clip_shp = self._make_rect_poly(x0, y0, x1, y1, self.crs_plot).to_crs(
-                gdf.crs
-            )
-        elif how == "crs_bounds" or how == "crs_bounds_invert":
-            x0, x1, y0, y1 = self.get_extent()
-            clip_shp = self._make_rect_poly(
-                *self.crs_plot.boundary.bounds, self.crs_plot
-            ).to_crs(gdf.crs)
-        else:
-            raise TypeError(f"EOmaps: '{how}' is not a valid clipping method")
-
-        clip_shp = clip_shp.buffer(0)  # use this to make sure the geometry is valid
-
-        # add 1% of the extent-diameter as buffer
-        bnd = clip_shp.boundary.bounds
-        d = np.sqrt((bnd.maxx - bnd.minx) ** 2 + (bnd.maxy - bnd.miny) ** 2)
-        clip_shp = clip_shp.buffer(d / 100)
-
-        # clip the geo-dataframe with the buffered clipping shape
-        clipgdf = gdf.clip(clip_shp)
-
-        if how.endswith("_invert"):
-            clipgdf = clipgdf.symmetric_difference(clip_shp)
-
-        return clipgdf
-
-    def _get_mcl_subclass(self, s):
-        # get a subclass that inherits the docstring from the corresponding
-        # mapclassify classifier
-
-        class scheme:
-            @wraps(s)
-            def __init__(_, *args, **kwargs):
-                pass
-
-            def __new__(cls, **kwargs):
-                if "y" in kwargs:
-                    _log.error(
-                        "EOmaps: The values (e.g. the 'y' parameter) are "
-                        + "assigned internally... only provide additional "
-                        + "parameters that specify the classification scheme!"
-                    )
-                    kwargs.pop("y")
-
-                self.classify_specs._set_scheme_and_args(scheme=s.__name__, **kwargs)
-
-        scheme.__doc__ = s.__doc__
-        return scheme
-
-    def _plot_map(
-        self,
-        layer=None,
-        dynamic=False,
-        set_extent=True,
-        assume_sorted=True,
-        **kwargs,
-    ):
-        _log.info(
-            "EOmaps: Plotting "
-            f"{self._data_manager.z_data.size} datapoints ({self.shape.name})"
-        )
-
-        for key in ("array",):
-            assert (
-                key not in kwargs
-            ), f"The key '{key}' is assigned internally by EOmaps!"
-
-        try:
-            self._set_extent = set_extent
-
-            # ------------- plot the data
-            self._coll_kwargs = kwargs
-            self._coll_dynamic = dynamic
-
-            # NOTE: the actual plot is performed by the data-manager
-            # at the next call to m.BM.fetch_bg() for the corresponding layer
-            # this is called to make sure m.coll is properly set
-            self._data_manager.on_fetch_bg(check_redraw=False)
-
-        except Exception as ex:
-            raise ex
-
-    def _sel_c_transp(self, c):
-        return self._data_manager._select_vals(
-            c.T if self._data_manager._z_transposed else c,
-            qs=self._data_manager._last_qs,
-            slices=self._data_manager._last_slices,
-        )
-
-    def _handle_explicit_colors(self, color):
-        if isinstance(color, (int, float, str, np.number)):
-            # if a scalar is provided, broadcast it
-            pass
-        elif isinstance(color, (list, tuple)) and len(color) in [3, 4]:
-            if all(map(lambda i: isinstance(i, (int, float, np.number)), color)):
-                # check if a tuple of numbers is provided, and if so broadcast
-                # it as a rgb or rgba tuple
-                pass
-            elif all(map(lambda i: isinstance(i, (list, np.ndarray)), color)):
-                # check if a tuple of lists or arrays is provided, and if so,
-                # broadcast them as RGB arrays
-                color = self._sel_c_transp(
-                    np.rec.fromarrays(np.broadcast_arrays(*color))
-                )
-        elif isinstance(color, np.ndarray) and (color.shape[-1] in [3, 4]):
-            color = self._sel_c_transp(np.rec.fromarrays(color.T))
-        elif isinstance(color, np.ndarray) and (color.shape[-1] in [3, 4]):
-            color = self._sel_c_transp(np.rec.fromarrays(color.T))
-        else:
-            # still use np.asanyarray in here in case lists are provided
-            color = self._sel_c_transp(np.asanyarray(color).reshape(self._zshape))
-
-        return color
-
-    @staticmethod
-    def _convert_1d_to_2d(data, x, y, fill_value=np.nan):
-        """A function to convert 1D vectors + data into 2D."""
-
-        if _log.getEffectiveLevel() <= logging.DEBUG:
-            _log.debug(
-                "EOmaps: Required conversion of 1D arrays to 2D for 'raster'"
-                "shape might be slow and consume a lot of memory!"
-            )
-
-        x, y, data = map(np.asanyarray, (x, y, data))
-        assert (
-            x.size == y.size == data.size
-        ), "EOmaps: You cannot use 1D arrays with different sizes for x, y and data"
-
-        x_vals, x_idx = np.unique(x, return_inverse=True)
-        y_vals, y_idx = np.unique(y, return_inverse=True)
-        # Get output array shape
-        m, n = (x_vals.size, y_vals.size)
-
-        # Get linear indices to be used as IDs with bincount
-        lidx = np.ravel_multi_index(np.vstack((x_idx, y_idx)), (m, n))
-        idx2d = np.unravel_index(lidx, (m, n))
-
-        # Distribute data to 2D
-
-        if not np.issubdtype(data.dtype, np.integer):
-            # Integer-dtypes do not support None!
-            data2d = np.full((m, n), fill_value=fill_value, dtype=data.dtype)
-            data2d[idx2d] = data
-
-        else:
-            # use smallest possible value as fill-value
-            fill_value = np.iinfo(data.dtype).min
-            data2d = np.full((m, n), fill_value=fill_value, dtype=data.dtype)
-            data2d[idx2d] = data
-
-            mask2d = np.full((m, n), fill_value=True, dtype=bool)
-            mask2d[idx2d] = False
-
-            data2d = np.ma.masked_array(data2d, mask2d)
-
-        # Distribute coordinates to 2D
-        x_vals, y_vals = np.meshgrid(x_vals, y_vals, indexing="ij")
-
-        return data2d, x_vals, y_vals
-
-    def _get_coll(self, props, **kwargs):
-        # handle selection of explicitly provided facecolors
-        # (e.g. for rgb composites)
-
-        # allow only one of the synonyms "color", "fc" and "facecolor"
-        if (
-            np.count_nonzero(
-                [kwargs.get(i, None) is not None for i in ["color", "fc", "facecolor"]]
-            )
-            > 1
-        ):
-            raise TypeError(
-                "EOmaps: only one of 'color', 'facecolor' or 'fc' " "can be specified!"
-            )
-
-        explicit_fc = False
-        for key in ("color", "facecolor", "fc"):
-            if kwargs.get(key, None) is not None:
-                explicit_fc = True
-                kwargs[key] = self._handle_explicit_colors(kwargs[key])
-
-        # don't pass the array if explicit facecolors are set
-        if explicit_fc and self.shape.name not in ["contour"]:
-            args = dict(array=None, cmap=None, norm=None, **kwargs)
-        else:
-            args = dict(
-                array=props["z_data"], cmap=self._cbcmap, norm=self._norm, **kwargs
-            )
-
-        if (
-            self.shape.name in ["contour"]
-            and len(self._xshape) == 2
-            and len(self._yshape) == 2
-        ):
-            # if 2D data is provided for a contour plot, keep the data 2d!
-            coll = self.shape.get_coll(props["xorig"], props["yorig"], "in", **args)
-        elif self.shape.name in ["raster"]:
-            # if input-data is 1D, try to convert data to 2D (required for raster)
-            # TODO make an explicit data-conversion function for 2D-only shapes
-            if len(self._xshape) == 2 and len(self._yshape) == 2:
-                coll = self.shape.get_coll(props["xorig"], props["yorig"], "in", **args)
-            else:
-                data2d, x2d, y2d = self._convert_1d_to_2d(
-                    data=props["z_data"].ravel(),
-                    x=props["x0"].ravel(),
-                    y=props["y0"].ravel(),
-                )
-
-                if args["array"] is not None:
-                    args["array"] = data2d
-
-                coll = self.shape.get_coll(x2d, y2d, "out", **args)
-
-        else:
-            # convert to 1D for further processing
-            if args["array"] is not None:
-                args["array"] = args["array"].ravel()
-
-            coll = self.shape.get_coll(
-                props["x0"].ravel(), props["y0"].ravel(), "out", **args
-            )
-        return coll
-
-    def _shade_map(
-        self,
-        layer=None,
-        dynamic=False,
-        set_extent=True,
-        assume_sorted=True,
-        **kwargs,
-    ):
-        """
-        Plot the dataset using the (very fast) "datashader" library.
-
-        Requires `datashader`... use `conda install -c conda-forge datashader`
-
-        - This method is intended for extremely large datasets
-          (up to millions of datapoints)!
-
-        A dynamically updated "shaded" map will be generated.
-        Note that the datapoints in this case are NOT represented by the shapes
-        defined as `m.set_shape`!
-
-        - By default, the shading is performed using a "mean"-value aggregation hook
-
-        kwargs :
-            kwargs passed to `datashader.mpl_ext.dsshow`
-
-        """
-        _log.info(
-            "EOmaps: Plotting "
-            f"{self._data_manager.z_data.size} datapoints ({self.shape.name})"
-        )
-
-        ds, mpl_ext, pd, xar = register_modules(
-            "datashader", "datashader.mpl_ext", "pandas", "xarray"
-        )
-
-        # remove previously fetched backgrounds for the used layer
-        if dynamic is False:
-            self.BM._refetch_layer(layer)
-
-        # in case the aggregation does not represent data-values
-        # (e.g. count, std, var ... ) use an automatic "linear" normalization
-
-        # get the name of the used aggretation reduction
-        aggname = self.shape.aggregator.__class__.__name__
-
-        if aggname in ["first", "last", "max", "min", "mean", "mode"]:
-            kwargs.setdefault("norm", self.classify_specs._norm)
-        else:
-            kwargs.setdefault("norm", "linear")
-
-        zdata = self._data_manager.z_data
-        if len(zdata) == 0:
-            _log.error("EOmaps: there was no data to plot")
-            return
-
-        plot_width, plot_height = int(self.ax.bbox.width), int(self.ax.bbox.height)
-
-        # get rid of unnecessary dimensions in the numpy arrays
-        zdata = zdata.squeeze()
-        x0 = self._data_manager.x0.squeeze()
-        y0 = self._data_manager.y0.squeeze()
-
-        # the shape is always set after _prepare data!
-        if self.shape.name == "shade_points" and self._data_manager.x0_1D is None:
-            # fill masked-values with None to avoid issues with numba not being
-            # able to deal with numpy-arrays
-            # TODO report this to datashader to get it fixed properly?
-            if isinstance(zdata, np.ma.masked_array):
-                zdata = zdata.filled(None)
-
-            df = pd.DataFrame(
-                dict(
-                    x=x0.ravel(),
-                    y=y0.ravel(),
-                    val=zdata.ravel(),
-                ),
-                copy=False,
-            )
-
-        else:
-            if len(zdata.shape) == 2:
-                if (zdata.shape == x0.shape) and (zdata.shape == y0.shape):
-                    # 2D coordinates and 2D raster
-
-                    # use a curvilinear QuadMesh
-                    if self.shape.name == "shade_raster":
-                        self.shape.glyph = ds.glyphs.QuadMeshCurvilinear(
-                            "x", "y", "val"
-                        )
-
-                    df = xar.Dataset(
-                        data_vars=dict(val=(["xx", "yy"], zdata)),
-                        # dims=["x", "y"],
-                        coords=dict(
-                            x=(["xx", "yy"], x0),
-                            y=(["xx", "yy"], y0),
-                        ),
-                    )
-
-                elif (
-                    ((zdata.shape[1],) == x0.shape)
-                    and ((zdata.shape[0],) == y0.shape)
-                    and (x0.shape != y0.shape)
-                ):
-                    raise AssertionError(
-                        "EOmaps: it seems like you need to transpose your data! \n"
-                        + f"the dataset has a shape of {zdata.shape}, but the "
-                        + f"coordinates suggest ({x0.shape}, {y0.shape})"
-                    )
-                elif (zdata.T.shape == x0.shape) and (zdata.T.shape == y0.shape):
-                    raise AssertionError(
-                        "EOmaps: it seems like you need to transpose your data! \n"
-                        + f"the dataset has a shape of {zdata.shape}, but the "
-                        + f"coordinates suggest {x0.shape}"
-                    )
-
-                elif ((zdata.shape[0],) == x0.shape) and (
-                    (zdata.shape[1],) == y0.shape
-                ):
-                    # 1D coordinates and 2D data
-
-                    # use a rectangular QuadMesh
-                    if self.shape.name == "shade_raster":
-                        self.shape.glyph = ds.glyphs.QuadMeshRectilinear(
-                            "x", "y", "val"
-                        )
-
-                    df = xar.DataArray(
-                        data=zdata,
-                        dims=["x", "y"],
-                        coords=dict(x=x0, y=y0),
-                    )
-                    df = xar.Dataset(dict(val=df))
-            else:
-                try:
-                    # try if reprojected coordinates can be used as 2d grid and if yes,
-                    # directly use a curvilinear QuadMesh based on the reprojected
-                    # coordinates to display the data
-                    idx = pd.MultiIndex.from_arrays(
-                        [x0.ravel(), y0.ravel()], names=["x", "y"]
-                    )
-
-                    df = pd.DataFrame(
-                        data=dict(val=zdata.ravel()), index=idx, copy=False
-                    )
-                    df = df.to_xarray()
-                    xg, yg = np.meshgrid(df.x, df.y)
-                except Exception:
-                    # first convert original coordinates of the 1D inputs to 2D,
-                    # then reproject the grid and use a curvilinear QuadMesh to display
-                    # the data
-                    _log.warning(
-                        "EOmaps: 1D data is converted to 2D prior to reprojection... "
-                        "Consider using 'shade_points' as plot-shape instead!"
-                    )
-                    xorig = self._data_manager.xorig.ravel()
-                    yorig = self._data_manager.yorig.ravel()
-
-                    idx = pd.MultiIndex.from_arrays([xorig, yorig], names=["x", "y"])
-
-                    df = pd.DataFrame(
-                        data=dict(val=zdata.ravel()), index=idx, copy=False
-                    )
-                    df = df.to_xarray()
-                    xg, yg = np.meshgrid(df.x, df.y)
-
-                    # transform the grid from input-coordinates to the plot-coordinates
-                    crs1 = CRS.from_user_input(self.data_specs.crs)
-                    crs2 = CRS.from_user_input(self._crs_plot)
-                    if crs1 != crs2:
-                        transformer = self._get_transformer(
-                            crs1,
-                            crs2,
-                        )
-                        xg, yg = transformer.transform(xg, yg)
-
-                # use a curvilinear QuadMesh
-                if self.shape.name == "shade_raster":
-                    self.shape.glyph = ds.glyphs.QuadMeshCurvilinear("x", "y", "val")
-
-                df = xar.Dataset(
-                    data_vars=dict(val=(["xx", "yy"], df.val.values.T)),
-                    coords=dict(x=(["xx", "yy"], xg), y=(["xx", "yy"], yg)),
-                )
-
-            if self.shape.name == "shade_points":
-                df = df.to_dataframe().reset_index()
-
-        if set_extent is True and self._set_extent_on_plot is True:
-            # convert to a numpy-array to support 2D indexing with boolean arrays
-            x, y = np.asarray(df.x), np.asarray(df.y)
-            xf, yf = np.isfinite(x), np.isfinite(y)
-            x_range = (np.nanmin(x[xf]), np.nanmax(x[xf]))
-            y_range = (np.nanmin(y[yf]), np.nanmax(y[yf]))
-        else:
-            # update here to ensure bounds are set
-            self.BM.update()
-            x0, x1, y0, y1 = self.get_extent(self.crs_plot)
-            x_range = (x0, x1)
-            y_range = (y0, y1)
-
-        coll = mpl_ext.dsshow(
-            df,
-            glyph=self.shape.glyph,
-            aggregator=self.shape.aggregator,
-            shade_hook=self.shape.shade_hook,
-            agg_hook=self.shape.agg_hook,
-            # norm="eq_hist",
-            # norm=plt.Normalize(vmin, vmax),
-            cmap=self._cbcmap,
-            ax=self.ax,
-            plot_width=plot_width,
-            plot_height=plot_height,
-            # x_range=(x0, x1),
-            # y_range=(y0, y1),
-            # x_range=(df.x.min(), df.x.max()),
-            # y_range=(df.y.min(), df.y.max()),
-            x_range=x_range,
-            y_range=y_range,
-            vmin=self._vmin,
-            vmax=self._vmax,
-            **kwargs,
-        )
-
-        coll.set_label("Dataset " f"({self.shape.name}  |  {zdata.shape})")
-
-        self._coll = coll
-
-        if dynamic is True:
-            self.BM.add_artist(coll, layer)
-        else:
-            self.BM.add_bg_artist(coll, layer)
-
-        if dynamic is True:
-            self.BM.update(clear=False)
-
-    def _encode_values(self, val):
-        """
-        Encode values with respect to the provided  "scale_factor" and "add_offset".
-
-        Encoding is performed via the formula:
-
-            `encoded_value = val / scale_factor - add_offset`
-
-        NOTE: the data-type is not altered!!
-        (e.g. no integer-conversion is performed, only values are adjusted)
-
-        Parameters
-        ----------
-        val : array-like
-            The data-values to encode
-
-        Returns
-        -------
-        encoded_values
-            The encoded data values
-        """
-        encoding = self.data_specs.encoding
-
-        if encoding is not None and encoding is not False:
-            try:
-                scale_factor = encoding.get("scale_factor", None)
-                add_offset = encoding.get("add_offset", None)
-                fill_value = encoding.get("_FillValue", None)
-
-                if val is None:
-                    return fill_value
-
-                if add_offset:
-                    val = val - add_offset
-                if scale_factor:
-                    val = val / scale_factor
-
-                return val
-            except Exception:
-                _log.exception(f"EOmaps: Error while trying to encode the data: {val}")
-                return val
-        else:
-            return val
-
-    def _decode_values(self, val):
-        """
-        Decode data-values with respect to the provided "scale_factor" and "add_offset".
-
-        Decoding is performed via the formula:
-
-            `actual_value = add_offset + scale_factor * val`
-
-        The encoding is defined in `m.data_specs.encoding`
-
-        Parameters
-        ----------
-        val : array-like
-            The encoded data-values
-
-        Returns
-        -------
-        decoded_values
-            The decoded data values
-        """
-        if val is None:
-            return None
-
-        encoding = self.data_specs.encoding
-        if not any(encoding is i for i in (None, False)):
-            try:
-                scale_factor = encoding.get("scale_factor", None)
-                add_offset = encoding.get("add_offset", None)
-
-                if scale_factor:
-                    val = val * scale_factor
-                if add_offset:
-                    val = val + add_offset
-
-                return val
-            except Exception:
-                _log.exception(f"EOmaps: Error while trying to decode the data {val}.")
-                return val
-        else:
-            return val
-
-    def _get_layers(self, exclude=None, exclude_private=True):
-        # return a list of all (empty and non-empty) layer-names
-        layers = set((m.layer for m in (self.parent, *self.parent._children)))
-        # add layers that are not yet activated (but have an activation
-        # method defined...)
-        layers = layers.union(set(self.BM._on_layer_activation[True]))
-        layers = layers.union(set(self.BM._on_layer_activation[False]))
-
-        # add all (possibly still invisible) layers with artists defined
-        # (ONLY do this for unique layers... skip multi-layers )
-        layers = layers.union(
-            chain(
-                *(
-                    self.BM._parse_multi_layer_str(i)[0]
-                    for i in (*self.BM._bg_artists, *self.BM._artists)
-                )
-            )
-        )
-
-        # exclude private layers
-        if exclude_private:
-            # for python <3.9 compatibility
-            def remove_prefix(text, prefix):
-                if text.startswith(prefix):
-                    return text[len(prefix) :]
-                return text
-
-            layers = {remove_prefix(i, "__inset_") for i in layers}
-            layers = {i for i in layers if not i.startswith("__")}
-
-        if exclude:
-            for i in exclude:
-                if i in layers:
-                    layers.remove(i)
-
-        # sort the layers
-        layers = sorted(layers, key=lambda x: str(x))
-
-        return layers
-
     @lru_cache()
     def _get_nominatim_response(self, q, user_agent=None):
         import requests
 
         _log.info(f"Querying {q}")
         if user_agent is None:
             user_agent = f"EOMaps v{Maps.__version__}"
@@ -5114,22 +3611,14 @@
         ).json()
 
         if len(resp) == 0:
             raise TypeError(f"Unable to resolve the location: {q}")
 
         return resp[0]
 
-    def _get_snapshot(self, layer=None):
-        if layer is None:
-            buf = self.f.canvas.print_to_buffer()
-            x = np.frombuffer(buf[0], dtype=np.uint8).reshape(buf[1][1], buf[1][0], 4)
-        else:
-            x = self.BM._get_array(layer)[::-1, ...]
-        return x
-
     def _indicate_companion_map(self, visible):
         if hasattr(self, "_companion_map_indicator"):
             self.BM.remove_artist(self._companion_map_indicator)
             try:
                 self._companion_map_indicator.remove()
             except ValueError:
                 # ignore errors resulting from the fact that the artist
@@ -5301,79 +3790,74 @@
                 _log.log(
                     1,
                     f"There was a problem while trying to emit the signal {name} "
                     f"with the args {args}",
                     exc_info=True,
                 )
 
-    @staticmethod
-    def _proxy(obj):
-        # None cannot be weak-referenced!
-        if obj is None:
-            return None
-
-        # create a proxy if the object is not yet a proxy
-        if type(obj) is not weakref.ProxyType:
-            return weakref.proxy(obj)
-        else:
-            return obj
+    def _get_always_on_top(self):
+        if "qt" in plt.get_backend().lower():
+            from qtpy import QtCore
 
-    @staticmethod
-    @lru_cache()
-    def _get_cartopy_crs(crs):
-        if isinstance(crs, Maps.CRS.CRS):  # already a cartopy CRS
-            cartopy_proj = crs
-        elif crs == 4326:
-            cartopy_proj = ccrs.PlateCarree()
-        elif crs == 3857:
-            cartopy_proj = ccrs.Mercator.GOOGLE
-        elif isinstance(crs, (int, np.integer)):
-            cartopy_proj = ccrs.epsg(crs)
-        elif isinstance(crs, CRS):  # pyproj CRS
-            cartopy_proj = None
-            for (
-                subgrid,
-                equi7crs,
-            ) in Maps.CRS.Equi7Grid_projection._pyproj_crs_generator():
-                if equi7crs == crs:
-                    cartopy_proj = Maps.CRS.Equi7Grid_projection(subgrid)
-                    break
-            if cartopy_proj is None:
-                cartopy_proj = ccrs.CRS(crs)
+            w = self.f.canvas.window()
+            return bool(w.windowFlags() & QtCore.Qt.WindowStaysOnTopHint)
 
-        else:
-            raise AssertionError(f"EOmaps: cannot identify the CRS for: {crs}")
+        return False
 
-        return cartopy_proj
+    def _set_always_on_top(self, q):
+        # keep pyqt window on top
+        try:
+            from qtpy import QtCore
 
-    @staticmethod
-    @lru_cache()
-    def _get_transformer(crs_from, crs_to):
-        # create a pyproj Transformer object and cache it for later use
-        return Transformer.from_crs(crs_from, crs_to, always_xy=True)
+            if q:
+                # only do this if necessary to avoid flickering
+                # see https://stackoverflow.com/a/40007740/9703451
+                if not self._get_always_on_top():
+                    # in case pyqt is used as backend, also keep the figure on top
+                    if "qt" in plt.get_backend().lower():
+                        w = self.f.canvas.window()
+                        ws = w.size()
+                        w.setWindowFlags(
+                            w.windowFlags() | QtCore.Qt.WindowStaysOnTopHint
+                        )
+                        w.resize(ws)
+                        w.show()
 
-    @property
-    def _transf_plot_to_lonlat(self):
-        return self._get_transformer(
-            self.crs_plot,
-            self.get_crs(self.crs_plot.as_geodetic()),
-        )
+                    # handle the widget in case it was activated (possible also for
+                    # backends other than qt)
+                    if self._companion_widget is not None:
+                        cw = self._companion_widget.window()
+                        cws = cw.size()
+                        cw.setWindowFlags(
+                            cw.windowFlags() | QtCore.Qt.WindowStaysOnTopHint
+                        )
+                        cw.resize(cws)
+                        cw.show()
 
-    @property
-    def _transf_lonlat_to_plot(self):
-        return self._get_transformer(
-            self.get_crs(self.crs_plot.as_geodetic()),
-            self.crs_plot,
-        )
+            else:
+                if self._get_always_on_top():
+                    if "qt" in plt.get_backend().lower():
+                        w = self.f.canvas.window()
+                        ws = w.size()
+                        w.setWindowFlags(
+                            w.windowFlags() & ~QtCore.Qt.WindowStaysOnTopHint
+                        )
+                        w.resize(ws)
+                        w.show()
 
-    @property
-    @lru_cache()
-    def _shape_drawer(self):
-        # initialize the shape-drawer
-        return ShapeDrawer(weakref.proxy(self))
+                    if self._companion_widget is not None:
+                        cw = self._companion_widget.window()
+                        cws = cw.size()
+                        cw.setWindowFlags(
+                            cw.windowFlags() & ~QtCore.Qt.WindowStaysOnTopHint
+                        )
+                        cw.resize(cws)
+                        cw.show()
+        except Exception:
+            pass
 
     @staticmethod
     def _make_rect_poly(x0, y0, x1, y1, crs=None, npts=100):
         """
         Return a geopandas.GeoDataFrame with a rectangle in the given crs.
 
         Parameters
@@ -5428,115 +3912,197 @@
     if refetch_wms_on_size_change is not None:
 
         @wraps(refetch_wms_on_size_change)
         def refetch_wms_on_size_change(self, *args, **kwargs):
             """Set the behavior for WebMap services on axis or figure size changes."""
             refetch_wms_on_size_change(*args, **kwargs)
 
-    def set_frame(self, rounded=0, **kwargs):
+    def _get_alpha_cmap_name(self, alpha):
+        # get a unique name for the colormap
+        try:
+            ncmaps = max(
+                [
+                    int(i.rsplit("_", 1)[1])
+                    for i in plt.colormaps()
+                    if i.startswith("EOmaps_alpha_")
+                ]
+            )
+        except Exception:
+            ncmaps = 0
+
+        return f"EOmaps_alpha_{ncmaps + 1}"
+
+    def _encode_values(self, val):
         """
-        Set the properties of the map boundary and the background patch.
+        Encode values with respect to the provided  "scale_factor" and "add_offset".
+
+        Encoding is performed via the formula:
+
+            `encoded_value = val / scale_factor - add_offset`
+
+        NOTE: the data-type is not altered!!
+        (e.g. no integer-conversion is performed, only values are adjusted)
 
         Parameters
         ----------
-        rounded : float, optional
-            If provided, use a rectangle with rounded corners as map boundary
-            line. The corners will be rounded with respect to the provided
-            fraction (0=no rounding, 1=max. radius). The default is None.
-        kwargs :
-            Additional kwargs to style the boundary line (e.g. the spine)
-            and the background patch
+        val : array-like
+            The data-values to encode
 
-            Possible args for the boundary-line:
+        Returns
+        -------
+        encoded_values
+            The encoded data values
+        """
+        encoding = self.data_specs.encoding
 
-            - "edgecolor" or "ec": The line color
-            - "linewidth" or "lw": The line width
-            - "linestyle" or "ls": The line style
-            - "path_effects": A list of path-effects to apply to the line
+        if encoding is not None and encoding is not False:
+            try:
+                scale_factor = encoding.get("scale_factor", None)
+                add_offset = encoding.get("add_offset", None)
+                fill_value = encoding.get("_FillValue", None)
 
-            Possible args for the background-patch:
+                if val is None:
+                    return fill_value
 
-            - "facecolor" or "fc": The color of the background patch
+                if add_offset:
+                    val = val - add_offset
+                if scale_factor:
+                    val = val / scale_factor
 
-        Examples
-        --------
+                return val
+            except Exception:
+                _log.exception(f"EOmaps: Error while trying to encode the data: {val}")
+                return val
+        else:
+            return val
 
-        >>> m = Maps()
-        >>> m.add_feature.preset.ocean()
-        >>> m.set_frame(fc="r", ec="b", lw=3, rounded=.2)
+    def _decode_values(self, val):
+        """
+        Decode data-values with respect to the provided "scale_factor" and "add_offset".
 
-        >>> import matplotlib.patheffects as pe
-        >>> m = Maps()
-        >>> m.add_feature.preset.ocean(fc="k")
-        >>> m.set_frame(
-        >>>     facecolor=(.8, .8, 0, .5), edgecolor="w", linewidth=2,
-        >>>     rounded=.5,
-        >>>     path_effects=[pe.withStroke(linewidth=7, foreground="m")])
+        Decoding is performed via the formula:
+
+            `actual_value = add_offset + scale_factor * val`
+
+        The encoding is defined in `m.data_specs.encoding`
 
+        Parameters
+        ----------
+        val : array-like
+            The encoded data-values
+
+        Returns
+        -------
+        decoded_values
+            The decoded data values
         """
+        if val is None:
+            return None
 
-        for key in ("fc", "facecolor"):
-            if key in kwargs:
-                self.ax.patch.set_facecolor(kwargs.pop(key))
+        encoding = self.data_specs.encoding
+        if not any(encoding is i for i in (None, False)):
+            try:
+                scale_factor = encoding.get("scale_factor", None)
+                add_offset = encoding.get("add_offset", None)
 
-        self.ax.spines["geo"].update(kwargs)
+                if scale_factor:
+                    val = val * scale_factor
+                if add_offset:
+                    val = val + add_offset
 
-        if rounded:
-            assert (
-                rounded <= 1
-            ), "EOmaps: rounded corner fraction must be between 0 and 1"
+                return val
+            except Exception:
+                _log.exception(f"EOmaps: Error while trying to decode the data {val}.")
+                return val
+        else:
+            return val
 
-            self.ax._EOmaps_rounded_spine_frac = rounded
-            theta = np.linspace(0, np.pi / 2, 50)  # use 50 intermediate points
-            s, c = np.sin(theta), np.cos(theta)
+    def _calc_vmin_vmax(self, vmin=None, vmax=None):
+        if self.data is None:
+            return vmin, vmax
 
-            # attach a function to dynamically update the corners of the
-            # map boundary prior to fetching a background
-            # Note: this function is only attached once and the relevant
-            # properties are fetched from the axes!
-            if not getattr(self.ax, "_EOmaps_rounded_spine_attached", False):
+        calc_min, calc_max = vmin is None, vmax is None
 
-                def cb(*args, **kwargs):
-                    if self.ax._EOmaps_rounded_spine_frac == 0:
-                        return
+        # ignore fill_values when evaluating vmin/vmax on integer-encoded datasets
+        if (
+            self.data_specs.encoding is not None
+            and isinstance(self._data_manager.z_data, np.ndarray)
+            and issubclass(self._data_manager.z_data.dtype.type, np.integer)
+        ):
 
-                    x0, x1, y0, y1 = self.get_extent(self.crs_plot)
-                    r = min(x1 - x0, y1 - y0) * self.ax._EOmaps_rounded_spine_frac / 2
+            # note the specific way how to check for integer-dtype based on issubclass
+            # since isinstance() fails to identify all integer dtypes!!
+            #   isinstance(np.dtype("uint8"), np.integer)       (incorrect) False
+            #   issubclass(np.dtype("uint8").type, np.integer)  (correct)   True
+            # for details, see https://stackoverflow.com/a/934652/9703451
 
-                    xs = [
-                        x0,
-                        *(x0 + r - r * c),
-                        x0 + r,
-                        x1 - r,
-                        *(x1 - r + r * s),
-                        x1,
-                        x1,
-                        *(x1 - r + r * c),
-                        x1 - r,
-                        x0 + r,
-                        *(x0 + r - r * s),
-                        x0,
-                    ]
+            fill_value = self.data_specs.encoding.get("_FillValue", None)
+            if fill_value and any([calc_min, calc_max]):
+                # find values that are not fill-values
+                use_vals = self._data_manager.z_data[
+                    self._data_manager.z_data != fill_value
+                ]
 
-                    ys = [
-                        y1 - r,
-                        *(y1 - r + r * s),
-                        y1,
-                        y1,
-                        *(y1 - r + r * c),
-                        y1 - r,
-                        y0 + r,
-                        *(y0 + r - r * s),
-                        y0,
-                        y0,
-                        *(y0 + r - r * c),
-                        y0 + r,
-                    ]
+                if calc_min:
+                    vmin = np.min(use_vals)
+                if calc_max:
+                    vmax = np.max(use_vals)
 
-                    path = mpath(np.column_stack((xs, ys)))
-                    self.ax.set_boundary(path, transform=self.crs_plot)
+                return vmin, vmax
 
-                self.BM._before_fetch_bg_actions.append(cb)
-                self.ax._EOmaps_rounded_spine_attached = True
+        # use nanmin/nanmax for all other arrays
+        if calc_min:
+            vmin = np.nanmin(self._data_manager.z_data)
+        if calc_max:
+            vmax = np.nanmax(self._data_manager.z_data)
 
-        self.redraw("__SPINES__")
-        self.redraw("__BG__")
+        return vmin, vmax
+
+    def _set_vmin_vmax(self, vmin=None, vmax=None):
+        # don't encode nan-vailes to avoid setting the fill-value as vmin/vmax
+        if vmin is not None:
+            vmin = self._encode_values(vmin)
+        if vmax is not None:
+            vmax = self._encode_values(vmax)
+
+        # handle inherited bounds
+        if self._inherit_classification is not None:
+            if not (vmin is None and vmax is None):
+                raise TypeError(
+                    "EOmaps: 'vmin' and 'vmax' cannot be set explicitly "
+                    "if the classification is inherited!"
+                )
+
+            # in case data is NOT inherited, warn if vmin/vmax is None
+            # (different limits might cause a different appearance of the data!)
+            if self.data_specs._m == self:
+                if self._vmin is None:
+                    _log.warning("EOmaps: Inherited value for 'vmin' is None!")
+                if self._vmax is None:
+                    _log.warning(
+                        "EOmaps: Inherited inherited value for 'vmax' is None!"
+                    )
+
+            self._vmin = self._inherit_classification._vmin
+            self._vmax = self._inherit_classification._vmax
+            return
+
+        if not self.shape.name.startswith("shade_"):
+            # ignore fill_values when evaluating vmin/vmax on integer-encoded datasets
+            self._vmin, self._vmax = self._calc_vmin_vmax(vmin=vmin, vmax=vmax)
+        else:
+            # get the name of the used aggretation reduction
+            aggname = self.shape.aggregator.__class__.__name__
+            if aggname in ["first", "last", "max", "min", "mean", "mode"]:
+                # set vmin/vmax in case the aggregation still represents data-values
+                self._vmin, self._vmax = self._calc_vmin_vmax(vmin=vmin, vmax=vmax)
+            else:
+                # set vmin/vmax for aggregations that do NOT represent data values
+                # allow vmin/vmax = None (e.g. autoscaling)
+                self._vmin, self._vmax = vmin, vmax
+                if "count" in aggname:
+                    # if the reduction represents a count, don't count empty pixels
+                    if vmin and vmin <= 0:
+                        _log.warning(
+                            "EOmaps: setting vmin=1 to avoid counting empty pixels..."
+                        )
+                        self._vmin = 1
```

### Comparing `eomaps-8.1.1/eomaps/grid.py` & `eomaps-8.2/eomaps/grid.py`

 * *Files 0% similar despite different names*

```diff
@@ -771,29 +771,32 @@
                 # select which lines to draw (e.g. tblr)
                 if self._where != "all":
                     if axis == 0:
                         if xt > 0.99 or xt < 0.01:
                             continue
 
                         line_in_bnds = l[:, 1].clip(bndmin[1], bndmax[1])
-                        line_center = (line_in_bnds.min() + line_in_bnds.max()) / 2
+                        line_center = (
+                            np.nanmin(line_in_bnds) + np.nanmax(line_in_bnds)
+                        ) / 2
                         top = y > line_center
                         if top:
                             if not ("t" in self._where):
                                 continue
                         else:
                             if not ("b" in self._where):
                                 continue
                     else:
                         if yt > 0.99 or yt < 0.01:
                             continue
 
                         line_in_bnds = l[:, 0].clip(bndmin[0], bndmax[0])
-                        line_center = (line_in_bnds.min() + line_in_bnds.max()) / 2
-
+                        line_center = (
+                            np.nanmin(line_in_bnds) + np.nanmax(line_in_bnds)
+                        ) / 2
                         right = x > line_center
                         if right:
                             if not ("r" in self._where):
                                 continue
                         else:
                             if not ("l" in self._where):
                                 continue
```

### Comparing `eomaps-8.1.1/eomaps/helpers.py` & `eomaps-8.2/eomaps/helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,40 @@
 from packaging import version
 
 mpl_version = version.parse(importlib.metadata.version("matplotlib"))
 
 _log = logging.getLogger(__name__)
 
 
+def _parse_log_level(level):
+    """
+    Get the numerical log-level from string (or number).
+
+    Parameters
+    ----------
+    level : str or number
+        The log level
+
+    Returns
+    -------
+    int_level : float
+        The numerical value of the log level.
+
+    """
+
+    levels = logging.getLevelNamesMapping()
+
+    if isinstance(level, str) and level.upper() in levels:
+        use_level = levels[level.upper()]
+    else:
+        use_level = float(level)
+
+    return use_level
+
+
 def _key_release_event(canvas, key, guiEvent=None):
     # copy of depreciated matplotlib functions for internal use
     s = "key_release_event"
     event = KeyEvent(s, canvas, key, guiEvent=guiEvent)
     canvas.callbacks.process(s, event)
     canvas._key = None
```

### Comparing `eomaps-8.1.1/eomaps/inset_maps.py` & `eomaps-8.2/eomaps/inset_maps.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.1.1/eomaps/layout_editor.py` & `eomaps-8.2/eomaps/layout_editor.py`

 * *Files 5% similar despite different names*

```diff
@@ -111,15 +111,16 @@
     @property
     def modifier_pressed(self):
         return self._modifier_pressed
 
     @modifier_pressed.setter
     def modifier_pressed(self, val):
         self._modifier_pressed = val
-        self.m.cb.execute_callbacks(not val)
+        if hasattr(self.m, "cb"):
+            self.m.cb.execute_callbacks(not val)
 
         if self._modifier_pressed:
             self.m.BM._disable_draw = True
             self.m.BM._disable_update = True
         else:
             self.m.BM._disable_draw = False
             self.m.BM._disable_update = False
@@ -189,16 +190,30 @@
         x0, y0 = (
             self._start_ax_position[ax][0] + (x - self._start_position[0]),
             self._start_ax_position[ax][1] + (y - self._start_position[1]),
         )
 
         if self._snap_id > 0:
             sx, sy = self._snap
-            x0 = self.roundto(x0, sx)
-            y0 = self.roundto(y0, sy)
+            x0s = self.roundto(x0, sx)
+            y0s = self.roundto(y0, sy)
+
+            # check if snap on top/right edges is closer than on bottom edges
+            x1s = self.roundto(x0 + w, sx)
+            y1s = self.roundto(y0 + h, sy)
+
+            if abs(x0s - x0) >= abs(x1s - x0 - w):
+                x0 = x1s - w
+            else:
+                x0 = x0s
+
+            if abs(y0s - y0) >= abs(y1s - y0 - h):
+                y0 = y1s - h
+            else:
+                y0 = y0s
 
         bbox = Bbox.from_bounds(x0, y0, w, h).transformed(self.f.transFigure.inverted())
 
         return bbox
 
     def _get_resize_bbox(self, ax, step):
         origw, origh = ax.bbox.width, ax.bbox.height
@@ -409,20 +424,33 @@
         if self.modifier is not None:
             if not self.modifier_pressed:
                 return False
 
         if event.button != 1:
             return
 
+        # The first picked axes is used to determine the repositioning relative to
+        # the active snap-grid. All additional axes are repositioned accordingly
+        dx, dy = None, None
         for ax in self._ax_picked:
             if ax is None:
                 return
 
-            bbox = self._get_move_bbox(ax, event.x, event.y)
-            ax.set_position(bbox)
+            if dx is None:
+                bbox = self._get_move_bbox(ax, event.x, event.y)
+                # Get the distance that the axes was shifted
+                dx, dy = bbox.x0 - ax.get_position().x0, bbox.y0 - ax.get_position().y0
+                # Reposition the axes
+                ax.set_position(bbox)
+            else:
+                # Always adjust positions of axes with respect to the first
+                # re-positioned axes (to avoid changing the relative alignment
+                # of multiple picked axes due to grid-snapping)
+                newbbox = ax.get_position().translated(dx, dy)
+                ax.set_position(newbbox)
 
         self._add_to_history()
         self._color_axes()
         self.blit_artists()
 
     def blit_artists(self):
         artists = [*self._ax_picked]
@@ -579,17 +607,21 @@
         if ax in self.m.BM._get_unmanaged_axes():
             return True
         elif ax in self.maxes:
             return True
         else:
             for layer in (self.m.BM.bg_layer, "__SPINES__", "all"):
                 # logos are put on the spines-layer to appear on top of spines!
-                if ax in self.m.BM.get_bg_artists(layer):
+                if ax in self.m.BM.get_bg_artists(
+                    self.m.BM._parse_multi_layer_str(layer)[0]
+                ):
                     return True
-                elif ax in self.m.BM.get_artists(self.m.BM.bg_layer):
+                elif ax in self.m.BM.get_artists(
+                    self.m.BM._get_active_layers_alphas[0]
+                ):
                     return True
 
         return False
 
     def _make_draggable(self, filepath=None):
         # Uncheck active pan/zoom actions of the matplotlib toolbar.
         # use a try-except block to avoid issues with ipympl in jupyter notebooks
@@ -769,15 +801,16 @@
                 p()
 
         self.modifier_pressed = False
 
         # reset the histogram-size of all colorbars to make sure previously hidden
         # axes (e.g. size=0) become visible if the size is now > 0.
         for m in self.ms:
-            for cb in m._colorbars:
+            # TODO
+            for cb in getattr(m, "_colorbars", []):
                 cb._set_hist_size(update_all=True)
 
         # remove snap-grid (if it's still visible)
         self._remove_snap_grid()
 
         self.m._emit_signal("layoutEditorDeactivated")
```

### Comparing `eomaps-8.1.1/eomaps/logo.png` & `eomaps-8.2/eomaps/logo.png`

 * *Files identical despite different names*

### Comparing `eomaps-8.1.1/eomaps/mapsgrid.py` & `eomaps-8.2/eomaps/mapsgrid.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.1.1/eomaps/ne_features.py` & `eomaps-8.2/eomaps/ne_features.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.1.1/eomaps/projections.py` & `eomaps-8.2/eomaps/projections.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.1.1/eomaps/qtcompanion/app.py` & `eomaps-8.2/eomaps/qtcompanion/app.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.1.1/eomaps/qtcompanion/base.py` & `eomaps-8.2/eomaps/qtcompanion/base.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.1.1/eomaps/qtcompanion/icons/edit_layout.png` & `eomaps-8.2/eomaps/qtcompanion/icons/edit_layout.png`

 * *Files identical despite different names*

### Comparing `eomaps-8.1.1/eomaps/qtcompanion/icons/edit_layout_active.png` & `eomaps-8.2/eomaps/qtcompanion/icons/edit_layout_active.png`

 * *Files identical despite different names*

### Comparing `eomaps-8.1.1/eomaps/qtcompanion/icons/edit_layout_hover.png` & `eomaps-8.2/eomaps/qtcompanion/icons/edit_layout_hover.png`

 * *Files identical despite different names*

### Comparing `eomaps-8.1.1/eomaps/qtcompanion/icons/eye_closed.png` & `eomaps-8.2/eomaps/qtcompanion/icons/eye_closed.png`

 * *Files identical despite different names*

### Comparing `eomaps-8.1.1/eomaps/qtcompanion/icons/eye_open.png` & `eomaps-8.2/eomaps/qtcompanion/icons/eye_open.png`

 * *Files identical despite different names*

### Comparing `eomaps-8.1.1/eomaps/qtcompanion/icons/info.png` & `eomaps-8.2/eomaps/qtcompanion/icons/info.png`

 * *Files identical despite different names*

### Comparing `eomaps-8.1.1/eomaps/qtcompanion/icons/info_checked.png` & `eomaps-8.2/eomaps/qtcompanion/icons/info_checked.png`

 * *Files identical despite different names*

### Comparing `eomaps-8.1.1/eomaps/qtcompanion/icons/info_hoover.png` & `eomaps-8.2/eomaps/qtcompanion/icons/info_hoover.png`

 * *Files identical despite different names*

### Comparing `eomaps-8.1.1/eomaps/qtcompanion/icons/layers.png` & `eomaps-8.2/eomaps/qtcompanion/icons/layers.png`

 * *Files identical despite different names*

### Comparing `eomaps-8.1.1/eomaps/qtcompanion/icons/layers_hover.png` & `eomaps-8.2/eomaps/qtcompanion/icons/layers_hover.png`

 * *Files identical despite different names*

### Comparing `eomaps-8.1.1/eomaps/qtcompanion/icons/logo.png` & `eomaps-8.2/eomaps/qtcompanion/icons/logo.png`

 * *Files identical despite different names*

### Comparing `eomaps-8.1.1/eomaps/qtcompanion/icons/open.png` & `eomaps-8.2/eomaps/qtcompanion/icons/open.png`

 * *Files identical despite different names*

### Comparing `eomaps-8.1.1/eomaps/qtcompanion/icons/open_hover.png` & `eomaps-8.2/eomaps/qtcompanion/icons/open_hover.png`

 * *Files identical despite different names*

### Comparing `eomaps-8.1.1/eomaps/qtcompanion/icons/peek_circle.png` & `eomaps-8.2/eomaps/qtcompanion/icons/peek_circle.png`

 * *Files identical despite different names*

### Comparing `eomaps-8.1.1/eomaps/qtcompanion/icons/peek_circle_active.png` & `eomaps-8.2/eomaps/qtcompanion/icons/peek_circle_active.png`

 * *Files identical despite different names*

### Comparing `eomaps-8.1.1/eomaps/qtcompanion/icons/peek_ellipse.png` & `eomaps-8.2/eomaps/qtcompanion/icons/peek_ellipse.png`

 * *Files identical despite different names*

### Comparing `eomaps-8.1.1/eomaps/qtcompanion/icons/peek_ellipse_active.png` & `eomaps-8.2/eomaps/qtcompanion/icons/peek_ellipse_active.png`

 * *Files identical despite different names*

### Comparing `eomaps-8.1.1/eomaps/qtcompanion/icons/plus.png` & `eomaps-8.2/eomaps/qtcompanion/icons/plus.png`

 * *Files identical despite different names*

### Comparing `eomaps-8.1.1/eomaps/qtcompanion/icons/plus_hoover.png` & `eomaps-8.2/eomaps/qtcompanion/icons/plus_hoover.png`

 * *Files identical despite different names*

### Comparing `eomaps-8.1.1/eomaps/qtcompanion/signal_container.py` & `eomaps-8.2/eomaps/qtcompanion/signal_container.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.1.1/eomaps/qtcompanion/widgets/annotate.py` & `eomaps-8.2/eomaps/qtcompanion/widgets/annotate.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.1.1/eomaps/qtcompanion/widgets/click_callbacks.py` & `eomaps-8.2/eomaps/qtcompanion/widgets/click_callbacks.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.1.1/eomaps/qtcompanion/widgets/draw.py` & `eomaps-8.2/eomaps/qtcompanion/widgets/draw.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.1.1/eomaps/qtcompanion/widgets/editor.py` & `eomaps-8.2/eomaps/qtcompanion/widgets/editor.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.1.1/eomaps/qtcompanion/widgets/extent.py` & `eomaps-8.2/eomaps/qtcompanion/widgets/extent.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.1.1/eomaps/qtcompanion/widgets/files.py` & `eomaps-8.2/eomaps/qtcompanion/widgets/files.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.1.1/eomaps/qtcompanion/widgets/layer.py` & `eomaps-8.2/eomaps/qtcompanion/widgets/layer.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.1.1/eomaps/qtcompanion/widgets/peek.py` & `eomaps-8.2/eomaps/qtcompanion/widgets/peek.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.1.1/eomaps/qtcompanion/widgets/save.py` & `eomaps-8.2/eomaps/qtcompanion/widgets/save.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.1.1/eomaps/qtcompanion/widgets/utils.py` & `eomaps-8.2/eomaps/qtcompanion/widgets/utils.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.1.1/eomaps/qtcompanion/widgets/wms.py` & `eomaps-8.2/eomaps/qtcompanion/widgets/wms.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.1.1/eomaps/reader.py` & `eomaps-8.2/eomaps/reader.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.1.1/eomaps/scalebar.py` & `eomaps-8.2/eomaps/scalebar.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 # See LICENSE in the root of the repository for full licensing details.
 
 """Interactive scalebar."""
 
 import logging
 from collections import OrderedDict
 from functools import lru_cache
+import importlib.metadata
+from packaging import version
 
 import numpy as np
 
 from matplotlib.collections import LineCollection
 from matplotlib.textpath import TextPath
 from matplotlib.patches import Polygon, PathPatch
 from matplotlib.transforms import Affine2D
@@ -20,14 +22,21 @@
 
 from .helpers import pairwise
 
 _picked_scalebars = set()
 
 _log = logging.getLogger(__name__)
 
+# TODO remove this once pyproj >3.5 is enforced
+pyproj_version = version.parse(importlib.metadata.version("pyproj"))
+if pyproj_version >= version.Version("3.5"):
+    _pyproj_geod_fix_args = {"return_back_azimuth": True}
+else:
+    _pyproj_geod_fix_args = {}
+
 
 class ScaleBar:
     """
     Base class for EOmaps scalebars.
 
     Note
     ----
@@ -975,14 +984,15 @@
             lon1=lon,
             lat1=lat,
             azi1=azim,
             npts=npts,
             del_s=self._current_scale,
             initial_idx=0,
             terminus_idx=0,
+            **_pyproj_geod_fix_args,
         )
 
         if isinstance(self._label_props["every"], int):
             self._every = [
                 i for i in range(pts.npts) if i % self._label_props["every"] == 0
             ]
         else:
@@ -999,14 +1009,15 @@
                 lon1=lon1,
                 lat1=lat1,
                 lon2=lon2,
                 lat2=lat2,
                 npts=self._interm_pts,
                 initial_idx=0,
                 terminus_idx=0,
+                **_pyproj_geod_fix_args,
             )
             lons.append(p.lons)
             lats.append(p.lats)
 
         # transform points to plot-crs
         pts_t = self._m._transf_lonlat_to_plot.transform(np.array(lons), np.array(lats))
         pts_t = np.stack(pts_t, axis=2)
```

### Comparing `eomaps-8.1.1/eomaps/scripts/open.py` & `eomaps-8.2/eomaps/scripts/open.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.1.1/eomaps/shapes.py` & `eomaps-8.2/eomaps/shapes.py`

 * *Files 2% similar despite different names*

```diff
@@ -457,15 +457,14 @@
                 radiusx = radiusy = radius
 
             radius = (radiusx, radiusy)
         return radius
 
     @staticmethod
     def _estimate_radius(m, radius_crs, method=np.nanmedian):
-
         assert radius_crs in [
             "in",
             "out",
         ], "radius can only be estimated if radius_crs is 'in' or 'out'!"
 
         if m._data_manager.x0_1D is not None:
             x, y = m._data_manager.x0_1D, m._data_manager.y0_1D
@@ -477,15 +476,20 @@
 
         radius = None
         # try to estimate radius for 2D datasets
         if len(x.shape) == 2 and len(y.shape) == 2:
             userange = int(np.sqrt(m.set_shape._radius_estimation_range))
 
             radiusx = method(np.diff(x[:userange, :userange], axis=1)) / 2
+            if radiusx == 0:
+                radiusx = method(np.diff(x[:userange, :userange].T, axis=1)) / 2
+
             radiusy = method(np.diff(y[:userange, :userange], axis=0)) / 2
+            if radiusy == 0:
+                radiusy = method(np.diff(y[:userange, :userange].T, axis=0)) / 2
 
             radius = (radiusx, radiusy)
 
             if not np.isfinite(radius).all() or not all(i > 0 for i in radius):
                 radius = None
 
         # for 1D datasets (or if 2D radius-estimation fails), use the median distance
@@ -571,15 +575,15 @@
         for c_key in ["fc", "facecolor", "color"]:
             color = kwargs.pop(c_key, None)
 
             if color is not None:
                 # explicit treatment for recarrays (to avoid performance issues)
                 # with matplotlib.colors.to_rgba_array()
                 # (recarrays are used to convert 3/4 arrays into an rgb(a) array
-                # in m._handle_explicit_colors() )
+                # in m._data_manager._handle_explicit_colors() )
                 if isinstance(color, np.recarray):
                     color_vals[c_key] = color[mask.reshape(color.shape)].view(
                         (float, len(color.dtype.names))
                     )  # .ravel()
                 elif isinstance(color, np.ndarray):
                     color_vals[c_key] = color[mask.reshape(color.shape)]
                 else:
```

### Comparing `eomaps-8.1.1/eomaps/utilities.py` & `eomaps-8.2/eomaps/utilities.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.1.1/eomaps/webmap_containers.py` & `eomaps-8.2/eomaps/webmap_containers.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.1.1/eomaps/widgets.py` & `eomaps-8.2/eomaps/widgets.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.1.1/eomaps.egg-info/PKG-INFO` & `eomaps-8.2/eomaps.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eomaps
-Version: 8.1.1
+Version: 8.2
 Summary: A library to create interactive maps of geographical datasets.
 Author-email: Raphael Quast <raphael.quast@geo.tuwien.ac.at>
 License: BSD 3-Clause License
         
         Copyright (c) 2021, The EOmaps authors.
         
         Redistribution and use in source and binary forms, with or without
@@ -70,14 +70,18 @@
 Requires-Dist: requests; extra == "wms"
 Provides-Extra: shade
 Requires-Dist: datashader; extra == "shade"
 Requires-Dist: dask[dataframe]; extra == "shade"
 Provides-Extra: gui
 Requires-Dist: PyQt5; extra == "gui"
 Requires-Dist: qtpy; extra == "gui"
+Provides-Extra: test
+Requires-Dist: eomaps[classify,gui,io,shade,test,wms]; extra == "test"
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-mpl; extra == "test"
 
 
 <p align="center">
     <a href=https://github.com/raphaelquast/EOmaps>
     <img src="https://github.com/raphaelquast/EOmaps/blob/master/docs/_static/logo.png?raw=true" alt="EOmaps logo" width="55%">
     </a>
 </p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: eomaps Version: 8.1.1 Summary: A library to create
+Metadata-Version: 2.1 Name: eomaps Version: 8.2 Summary: A library to create
 interactive maps of geographical datasets. Author-email: Raphael Quast
 geo.tuwien.ac.at> License: BSD 3-Clause License Copyright (c) 2021, The EOmaps
 authors. Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met: 1.
 Redistributions of source code must retain the above copyright notice, this
 list of conditions and the following disclaimer. 2. Redistributions in binary
 form must reproduce the above copyright notice, this list of conditions and the
@@ -36,15 +36,17 @@
 Requires-Dist: pandas; extra == "io" Requires-Dist: geopandas; extra == "io"
 Requires-Dist: xarray; extra == "io" Requires-Dist: netcdf4; extra == "io"
 Requires-Dist: rioxarray; extra == "io" Provides-Extra: classify Requires-Dist:
 mapclassify; extra == "classify" Provides-Extra: wms Requires-Dist: owslib;
 extra == "wms" Requires-Dist: requests; extra == "wms" Provides-Extra: shade
 Requires-Dist: datashader; extra == "shade" Requires-Dist: dask[dataframe];
 extra == "shade" Provides-Extra: gui Requires-Dist: PyQt5; extra == "gui"
-Requires-Dist: qtpy; extra == "gui"
+Requires-Dist: qtpy; extra == "gui" Provides-Extra: test Requires-Dist: eomaps
+[classify,gui,io,shade,test,wms]; extra == "test" Requires-Dist: pytest; extra
+== "test" Requires-Dist: pytest-mpl; extra == "test"
                                  _[_E_O_m_a_p_s_ _l_o_g_o_]
  | Tests & Review | [![tests](https://github.com/raphaelquast/EOmaps/actions/
      workflows/testMaps.yml/badge.svg?branch=master)](https://github.com/
   raphaelquast/EOmaps/actions/workflows/testMaps.yml) | [![codecov](https://
   codecov.io/gh/raphaelquast/EOmaps/graph/badge.svg)](https://codecov.io/gh/
  raphaelquast/EOmaps) | [![pyOpenSci](https://tinyurl.com/y22nb8up)](https://
 github.com/pyOpenSci/software-submission/issues/138) | | :--------------------
```

### Comparing `eomaps-8.1.1/eomaps.egg-info/SOURCES.txt` & `eomaps-8.2/eomaps.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 README.md
 pyproject.toml
 eomaps/NE_features.json
 eomaps/__init__.py
 eomaps/_blit_manager.py
 eomaps/_containers.py
 eomaps/_data_manager.py
+eomaps/_maps_base.py
 eomaps/_webmap.py
 eomaps/annotation_editor.py
 eomaps/callbacks.py
 eomaps/cb_container.py
 eomaps/colorbar.py
 eomaps/compass.py
 eomaps/draw.py
```

### Comparing `eomaps-8.1.1/pyproject.toml` & `eomaps-8.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 [tool.setuptools.package-data]
 eomaps = ["logo.png", "NE_features.json", "qtcompanion/icons/*"]
 
 
 [project]
 name = "eomaps"
-version = "8.1.1"
+version = "8.2"
 description = "A library to create interactive maps of geographical datasets."
 readme = "README.md"
 license = {file = "LICENSE"}
 
 requires-python = ">=3.8"
 
 authors = [
@@ -72,22 +72,31 @@
 ]
 
 gui = [
     "PyQt5",
     "qtpy"
     ]
 
+test = [
+    "eomaps[io, classify, wms, shade, gui, test]",
+    "pytest",
+    "pytest-mpl"
+]
+
 [project.scripts]
 eomaps = "eomaps.scripts.open:cli"
 
 [project.urls]
 Documentation = "https://eomaps.readthedocs.io/"
 Repository = "https://github.com/raphaelquast/eomaps"
 
 [tool.pytest.ini_options]
+mpl-use-full-test-name = "True"
+mpl-default-style = "default"
+mpl-results-path = "img_comparison_results"
 filterwarnings = [
     "ignore:Downloading*",
     "ignore:Passing a SingleBlockManager to Series is deprecated *:DeprecationWarning",
     "ignore:Passing a BlockManager to GeoDataFrame is deprecated *:DeprecationWarning",
     "ignore:Passing a SingleBlockManager to GeoSeries is deprecated *:DeprecationWarning",
     "ignore:Pyarrow will become a required dependency of pandas *:DeprecationWarning",
     "ignore:Geometry is in a geographic CRS. Results from *:UserWarning",
```

### Comparing `eomaps-8.1.1/tests/test_WMS_capabilities.py` & `eomaps-8.2/tests/test_WMS_capabilities.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.1.1/tests/test_basic_functions.py` & `eomaps-8.2/tests/test_basic_functions.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.1.1/tests/test_callbacks.py` & `eomaps-8.2/tests/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.1.1/tests/test_config.py` & `eomaps-8.2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.1.1/tests/test_doc_codeblocks.py` & `eomaps-8.2/tests/test_doc_codeblocks.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.1.1/tests/test_doc_notebooks.py` & `eomaps-8.2/tests/test_doc_notebooks.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.1.1/tests/test_drawer.py` & `eomaps-8.2/tests/test_drawer.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.1.1/tests/test_examples.py` & `eomaps-8.2/tests/test_examples.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 """Test running all python-files in docs/examples that start with 'example_' """
 from pathlib import Path
 import matplotlib.pyplot as plt
 import unittest
+import pytest
+import numpy as np
 
 
 def gen_test(name, code):
+    @pytest.mark.mpl_image_compare()
     def test(*args, **kwargs):
         try:
+            np.random.seed(0)  # make tests descriptive
             exec(code)
+
+            return locals()["m"]
         except Exception as ex:
             raise AssertionError(f"Example '{name}' failed.") from ex
         finally:
             plt.close("all")
 
     return test
```

### Comparing `eomaps-8.1.1/tests/test_layout_editor.py` & `eomaps-8.2/tests/test_layout_editor.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.1.1/tests/test_plot_shapes.py` & `eomaps-8.2/tests/test_plot_shapes.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 import pandas as pd
 import numpy as np
 import matplotlib.pyplot as plt
 
 from eomaps import Maps
 
+np.random.seed(0)
+
 # TODO add proper (extensive) tests for each shape!
 
 x, y = np.linspace(-40, 40, 50), np.linspace(-25, 30, 150)
 x2d, y2d = np.meshgrid(x, y, indexing="ij")
 data = x2d**2 + y2d**2
 
 # use an irregular sample of the data to check irregular datasets as well
@@ -35,20 +37,21 @@
 def close_all():
     yield
     plt.close("all")
 
 
 @pytest.mark.usefixtures("close_all")
 @pytest.mark.parametrize("data", testdata, ids=ids)
+@pytest.mark.mpl_image_compare()
 def test_hexbin(data):
     m = Maps(ax=221, figsize=(10, 6))
     m.set_data(**data)
     m.set_shape.hexbin(size=(10, 5))
     m.plot_map()
-    m.add_colorbar()
+    cb = m.add_colorbar()
 
     m2 = m.new_map(ax=222, inherit_data=True)
     m2.set_shape.hexbin(size=20, aggregator="median")
     m2.plot_map(cmap="RdYlBu")
     m2.add_colorbar()
 
     m3 = m.new_map(ax=223, inherit_data=True)
@@ -58,17 +61,20 @@
 
     m4 = m.new_map(ax=224, inherit_data=True)
     m4.set_shape.hexbin(size=10, aggregator="max")
     m4.set_classify.EqualInterval(k=5)
     m4.plot_map(cmap="RdYlBu")
     m4.add_colorbar()
 
+    return m
+
 
 @pytest.mark.usefixtures("close_all")
 @pytest.mark.parametrize("data", testdata, ids=ids)
+@pytest.mark.mpl_image_compare()
 def test_contour(data):
     m = Maps(ax=221, figsize=(10, 6))
     m.subplots_adjust(left=0.01, right=0.99)
     m.set_data(**data)
     m.set_shape.contour(filled=True)
     m.plot_map()
     m.add_colorbar()
@@ -83,16 +89,16 @@
     m2.set_shape.contour(filled=True)
     m2.plot_map(
         colors=["none", "r", (0, 1, 0, 0.25), "r"],
         hatches=["", "xxxx", "///", "xxxx"],
     )
 
     m3 = m.new_map(ax=224, inherit_data=True)
-    m3.set_shape.ellipses()
-    m3.plot_map(alpha=0.25)
+    m3.set_shape.voronoi_diagram()
+    m3.plot_map(alpha=0.25, lw=0.25, ec="k")
     cb3 = m3.add_colorbar()
 
     m3_1 = m3.new_layer("contours", inherit_data=True)
     m3_1.set_shape.contour(filled=False)
     m3_1.plot_map(linestyles=["--", "-", ":", "-."])
 
     cb3.indicate_contours(
@@ -118,7 +124,46 @@
     # see https://github.com/raphaelquast/EOmaps/issues/218
 
     # arts = m3_1.ax.clabel(m3_1.coll.contour_set)
     # for a in arts:
     #     m3_1.BM.add_bg_artist(a, layer=m3_1.layer)
 
     m.show_layer("base", "contours")
+
+    return m
+
+
+@pytest.mark.usefixtures("close_all")
+@pytest.mark.parametrize("data", testdata, ids=ids)
+@pytest.mark.mpl_image_compare()
+def test_shade_points(data):
+    m = Maps(ax=221, figsize=(10, 6))
+
+    m.set_data(**data)
+    m.set_shape.shade_points(aggregator="mean")
+    m.set_shade_dpi(100)
+    m.plot_map()
+    m.add_colorbar()
+
+    m2 = m.new_map(ax=222, inherit_data=True)
+    m2.set_shape.shade_points(aggregator="max")
+    m2.set_shade_dpi(30)
+    m2.plot_map(cmap="RdYlBu")
+    m2.add_colorbar()
+
+    m3 = m.new_map(ax=223, inherit_data=True)
+    m3.set_shape.shade_points(aggregator="max")
+    m3.set_shade_dpi(20)
+    m3.plot_map(cmap="RdYlBu")
+    m3.add_colorbar()
+
+    m4 = m.new_map(ax=224, inherit_data=True)
+    m4.set_shape.shade_points(aggregator="max")
+    m4.set_shade_dpi(10)
+    m4.set_classify.EqualInterval(k=5)
+    m4.plot_map(cmap="RdYlBu")
+    m4.add_colorbar()
+
+    for mi in [m, m2, m3, m4]:
+        mi.add_title(f"shade dpi = {mi._shade_dpi}")
+
+    return m
```

### Comparing `eomaps-8.1.1/tests/test_raster_aggregaton.py` & `eomaps-8.2/tests/test_raster_aggregaton.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.1.1/tests/test_widgets.py` & `eomaps-8.2/tests/test_widgets.py`

 * *Files identical despite different names*

