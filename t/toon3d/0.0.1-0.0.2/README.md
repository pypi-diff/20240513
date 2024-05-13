# Comparing `tmp/toon3d-0.0.1.tar.gz` & `tmp/toon3d-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toon3d-0.0.1.tar", last modified: Sat Feb 24 05:19:28 2024, max compression
+gzip compressed data, was "toon3d-0.0.2.tar", last modified: Mon May 13 05:32:20 2024, max compression
```

## Comparing `toon3d-0.0.1.tar` & `toon3d-0.0.2.tar`

### file list

```diff
@@ -1,54 +1,65 @@
-drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-02-24 05:19:28.024814 toon3d-0.0.1/
--rw-r--r--   0 ethanweber (1000282) users    (1000001)      826 2024-02-24 05:19:28.024814 toon3d-0.0.1/PKG-INFO
--rw-r--r--   0 ethanweber (1000282) users    (1000001)     4891 2024-02-24 05:12:30.000000 toon3d-0.0.1/README.md
--rw-r--r--   0 ethanweber (1000282) users    (1000001)      810 2024-02-24 05:19:12.000000 toon3d-0.0.1/pyproject.toml
--rw-r--r--   0 ethanweber (1000282) users    (1000001)       38 2024-02-24 05:19:28.024814 toon3d-0.0.1/setup.cfg
-drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-02-24 05:19:28.020815 toon3d-0.0.1/tests/
--rw-r--r--   0 ethanweber (1000282) users    (1000001)      344 2024-02-24 05:12:30.000000 toon3d-0.0.1/tests/test_finetune.py
-drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-02-24 05:19:28.020815 toon3d-0.0.1/toon3d/
--rw-r--r--   0 ethanweber (1000282) users    (1000001)       42 2024-02-24 05:14:10.000000 toon3d-0.0.1/toon3d/temp.py
-drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-02-24 05:19:28.020815 toon3d-0.0.1/toon3d-current/
--rw-r--r--   0 ethanweber (1000282) users    (1000001)        0 2023-11-29 02:41:20.000000 toon3d-0.0.1/toon3d-current/__init__.py
--rw-r--r--   0 ethanweber (1000282) users    (1000001)     1728 2024-01-02 05:18:16.000000 toon3d-0.0.1/toon3d-current/color_palette.py
-drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-02-24 05:19:28.020815 toon3d-0.0.1/toon3d-current/configs/
--rw-r--r--   0 ethanweber (1000282) users    (1000001)     1475 2024-02-05 20:08:58.000000 toon3d-0.0.1/toon3d-current/configs/prompts.py
-drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-02-24 05:19:28.020815 toon3d-0.0.1/toon3d-current/generative/
--rw-r--r--   0 ethanweber (1000282) users    (1000001)    14001 2024-02-24 04:24:41.000000 toon3d-0.0.1/toon3d-current/generative/ldm3d.py
--rw-r--r--   0 ethanweber (1000282) users    (1000001)    10358 2024-01-31 00:44:40.000000 toon3d-0.0.1/toon3d-current/generative/marigold.py
-drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-02-24 05:19:28.020815 toon3d-0.0.1/toon3d-current/scripts/
--rw-r--r--   0 ethanweber (1000282) users    (1000001)     6596 2024-02-20 00:38:40.000000 toon3d-0.0.1/toon3d-current/scripts/download_data.py
--rw-r--r--   0 ethanweber (1000282) users    (1000001)    19820 2024-02-24 05:12:30.000000 toon3d-0.0.1/toon3d-current/scripts/finetune.py
--rw-r--r--   0 ethanweber (1000282) users    (1000001)     3207 2024-02-24 05:12:30.000000 toon3d-0.0.1/toon3d-current/scripts/process_data.py
--rw-r--r--   0 ethanweber (1000282) users    (1000001)    24887 2024-02-24 05:12:30.000000 toon3d-0.0.1/toon3d-current/scripts/render.py
--rw-r--r--   0 ethanweber (1000282) users    (1000001)    33570 2024-02-24 05:12:30.000000 toon3d-0.0.1/toon3d-current/scripts/run.py
--rw-r--r--   0 ethanweber (1000282) users    (1000001)     1185 2024-02-11 21:30:36.000000 toon3d-0.0.1/toon3d-current/scripts/server.py
--rw-r--r--   0 ethanweber (1000282) users    (1000001)     2915 2024-02-24 05:12:30.000000 toon3d-0.0.1/toon3d-current/tooned_config.py
--rw-r--r--   0 ethanweber (1000282) users    (1000001)     5939 2024-02-24 05:12:30.000000 toon3d-0.0.1/toon3d-current/tooned_datamanager.py
--rw-r--r--   0 ethanweber (1000282) users    (1000001)     2290 2024-02-24 05:12:30.000000 toon3d-0.0.1/toon3d-current/tooned_dataparser.py
--rw-r--r--   0 ethanweber (1000282) users    (1000001)    16299 2024-02-24 05:12:30.000000 toon3d-0.0.1/toon3d-current/tooned_model.py
--rw-r--r--   0 ethanweber (1000282) users    (1000001)     4624 2024-02-24 05:12:30.000000 toon3d-0.0.1/toon3d-current/tooned_pipeline.py
--rw-r--r--   0 ethanweber (1000282) users    (1000001)        0 2023-12-04 21:16:52.000000 toon3d-0.0.1/toon3d-current/tooned_process_data.py
-drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-02-24 05:19:28.024814 toon3d-0.0.1/toon3d-current/utils/
--rw-r--r--   0 ethanweber (1000282) users    (1000001)     2331 2024-02-20 00:51:55.000000 toon3d-0.0.1/toon3d-current/utils/camera_utils.py
--rw-r--r--   0 ethanweber (1000282) users    (1000001)     1514 2024-01-02 05:18:16.000000 toon3d-0.0.1/toon3d-current/utils/convert_points.py
--rw-r--r--   0 ethanweber (1000282) users    (1000001)      997 2024-02-24 04:24:41.000000 toon3d-0.0.1/toon3d-current/utils/depth_utils.py
--rw-r--r--   0 ethanweber (1000282) users    (1000001)     2699 2024-01-02 05:18:16.000000 toon3d-0.0.1/toon3d-current/utils/draw_utils.py
--rw-r--r--   0 ethanweber (1000282) users    (1000001)     3047 2024-02-24 05:12:30.000000 toon3d-0.0.1/toon3d-current/utils/image_processing_utils.py
--rw-r--r--   0 ethanweber (1000282) users    (1000001)      416 2024-02-24 05:11:20.000000 toon3d-0.0.1/toon3d-current/utils/json_utils.py
--rw-r--r--   0 ethanweber (1000282) users    (1000001)     2108 2024-01-31 00:44:40.000000 toon3d-0.0.1/toon3d-current/utils/losses.py
--rw-r--r--   0 ethanweber (1000282) users    (1000001)     1767 2024-02-07 22:42:32.000000 toon3d-0.0.1/toon3d-current/utils/novel_view_samplers.py
-drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-02-24 05:19:28.024814 toon3d-0.0.1/toon3d-current/utils/pytorch_arap/
--rw-r--r--   0 ethanweber (1000282) users    (1000001)    23448 2024-01-02 05:18:16.000000 toon3d-0.0.1/toon3d-current/utils/pytorch_arap/arap.py
--rw-r--r--   0 ethanweber (1000282) users    (1000001)     8227 2024-01-02 05:18:16.000000 toon3d-0.0.1/toon3d-current/utils/pytorch_arap/arap_utils.py
-drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-02-24 05:19:28.024814 toon3d-0.0.1/toon3d-current/warp/
--rw-r--r--   0 ethanweber (1000282) users    (1000001)      814 2024-02-20 00:51:55.000000 toon3d-0.0.1/toon3d-current/warp/arap_utils.py
--rw-r--r--   0 ethanweber (1000282) users    (1000001)     4744 2024-02-20 00:51:55.000000 toon3d-0.0.1/toon3d-current/warp/tri_rasterize.py
--rw-r--r--   0 ethanweber (1000282) users    (1000001)     2689 2024-02-24 05:12:30.000000 toon3d-0.0.1/toon3d-current/warp/warp_losses.py
--rw-r--r--   0 ethanweber (1000282) users    (1000001)    20337 2024-02-24 05:12:30.000000 toon3d-0.0.1/toon3d-current/warp/warp_mesh.py
--rw-r--r--   0 ethanweber (1000282) users    (1000001)     7403 2024-02-24 05:12:30.000000 toon3d-0.0.1/toon3d-current/warp_model.py
-drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-02-24 05:19:28.024814 toon3d-0.0.1/toon3d.egg-info/
--rw-r--r--   0 ethanweber (1000282) users    (1000001)      826 2024-02-24 05:19:28.000000 toon3d-0.0.1/toon3d.egg-info/PKG-INFO
--rw-r--r--   0 ethanweber (1000282) users    (1000001)     1357 2024-02-24 05:19:28.000000 toon3d-0.0.1/toon3d.egg-info/SOURCES.txt
--rw-r--r--   0 ethanweber (1000282) users    (1000001)        1 2024-02-24 05:19:28.000000 toon3d-0.0.1/toon3d.egg-info/dependency_links.txt
--rw-r--r--   0 ethanweber (1000282) users    (1000001)      280 2024-02-24 05:19:28.000000 toon3d-0.0.1/toon3d.egg-info/requires.txt
--rw-r--r--   0 ethanweber (1000282) users    (1000001)       22 2024-02-24 05:19:28.000000 toon3d-0.0.1/toon3d.egg-info/top_level.txt
+drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-05-13 05:32:20.454004 toon3d-0.0.2/
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)      826 2024-05-13 05:32:20.454004 toon3d-0.0.2/PKG-INFO
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     5785 2024-05-12 06:19:19.000000 toon3d-0.0.2/README.md
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     1240 2024-05-13 05:31:47.000000 toon3d-0.0.2/pyproject.toml
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)       38 2024-05-13 05:32:20.454004 toon3d-0.0.2/setup.cfg
+drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-05-13 05:32:20.450004 toon3d-0.0.2/tests/
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)      344 2024-03-15 01:48:57.000000 toon3d-0.0.2/tests/test_finetune.py
+drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-05-13 05:32:20.450004 toon3d-0.0.2/toon3d/
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)        0 2024-03-15 01:48:57.000000 toon3d-0.0.2/toon3d/__init__.py
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     1728 2024-03-15 01:48:57.000000 toon3d-0.0.2/toon3d/color_palette.py
+drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-05-13 05:32:20.450004 toon3d-0.0.2/toon3d/configs/
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     1475 2024-03-15 01:48:57.000000 toon3d-0.0.2/toon3d/configs/prompts.py
+drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-05-13 05:32:20.450004 toon3d-0.0.2/toon3d/generative/
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)    14001 2024-03-15 01:48:57.000000 toon3d-0.0.2/toon3d/generative/ldm3d.py
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)    10358 2024-03-15 01:48:57.000000 toon3d-0.0.2/toon3d/generative/marigold.py
+drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-05-13 05:32:20.454004 toon3d-0.0.2/toon3d/scripts/
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     4646 2024-05-10 20:12:48.000000 toon3d-0.0.2/toon3d/scripts/colmap_with_corrs.py
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     6596 2024-03-15 01:48:57.000000 toon3d-0.0.2/toon3d/scripts/download_data.py
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)    19820 2024-03-15 01:48:57.000000 toon3d-0.0.2/toon3d/scripts/finetune.py
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     8611 2024-05-10 21:53:19.000000 toon3d-0.0.2/toon3d/scripts/process_data.py
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)    34172 2024-03-29 05:06:36.000000 toon3d-0.0.2/toon3d/scripts/render.py
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)    37741 2024-05-12 17:37:52.000000 toon3d-0.0.2/toon3d/scripts/run.py
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     1185 2024-03-15 01:48:57.000000 toon3d-0.0.2/toon3d/scripts/server.py
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     4685 2024-05-13 05:11:25.000000 toon3d-0.0.2/toon3d/scripts/viser_vis.py
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     2847 2024-03-15 01:48:57.000000 toon3d-0.0.2/toon3d/toon3d_config.py
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     5939 2024-03-15 01:48:57.000000 toon3d-0.0.2/toon3d/toon3d_datamanager.py
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     2290 2024-03-15 01:48:57.000000 toon3d-0.0.2/toon3d/toon3d_dataparser.py
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)    17776 2024-03-15 01:48:57.000000 toon3d-0.0.2/toon3d/toon3d_model.py
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     5605 2024-03-15 01:48:57.000000 toon3d-0.0.2/toon3d/toon3d_pipeline.py
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)        0 2024-03-15 01:48:57.000000 toon3d-0.0.2/toon3d/toon3d_process_data.py
+drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-05-13 05:32:20.454004 toon3d-0.0.2/toon3d/utils/
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     3376 2024-03-15 01:48:57.000000 toon3d-0.0.2/toon3d/utils/camera_utils.py
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)    12545 2024-03-15 01:48:57.000000 toon3d-0.0.2/toon3d/utils/colmap_database.py
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     1514 2024-03-15 01:48:57.000000 toon3d-0.0.2/toon3d/utils/convert_points.py
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     3008 2024-03-15 01:48:57.000000 toon3d-0.0.2/toon3d/utils/depth_utils.py
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     2699 2024-03-15 01:48:57.000000 toon3d-0.0.2/toon3d/utils/draw_utils.py
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     4322 2024-05-10 21:50:37.000000 toon3d-0.0.2/toon3d/utils/image_processing_utils.py
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     2108 2024-03-15 01:48:57.000000 toon3d-0.0.2/toon3d/utils/losses.py
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     9203 2024-03-15 01:48:57.000000 toon3d-0.0.2/toon3d/utils/mesh_utils.py
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     1767 2024-03-15 01:48:57.000000 toon3d-0.0.2/toon3d/utils/novel_view_samplers.py
+drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-05-13 05:32:20.454004 toon3d-0.0.2/toon3d/utils/pytorch_arap/
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)    23448 2024-03-15 01:48:57.000000 toon3d-0.0.2/toon3d/utils/pytorch_arap/arap.py
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     8227 2024-03-15 01:48:57.000000 toon3d-0.0.2/toon3d/utils/pytorch_arap/arap_utils.py
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     2675 2024-03-15 01:48:57.000000 toon3d-0.0.2/toon3d/utils/tsdf_utils.py
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     3316 2024-03-26 21:11:46.000000 toon3d-0.0.2/toon3d/utils/viser_utils.py
+drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-05-13 05:32:20.454004 toon3d-0.0.2/toon3d/warp/
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     3415 2024-04-12 21:13:30.000000 toon3d-0.0.2/toon3d/warp/arap_utils.py
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     4744 2024-03-15 01:48:57.000000 toon3d-0.0.2/toon3d/warp/tri_rasterize.py
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)    10060 2024-04-12 21:13:30.000000 toon3d-0.0.2/toon3d/warp/warp_mesh.py
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     7403 2024-03-15 01:48:57.000000 toon3d-0.0.2/toon3d/warp_model.py
+drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-05-13 05:32:20.450004 toon3d-0.0.2/toon3d-labeler/
+drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-05-13 05:32:20.450004 toon3d-0.0.2/toon3d-labeler/node_modules/
+drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-05-13 05:32:20.450004 toon3d-0.0.2/toon3d-labeler/node_modules/flatted/
+drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-05-13 05:32:20.450004 toon3d-0.0.2/toon3d-labeler/node_modules/flatted/python/
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     3879 2024-04-30 22:25:05.000000 toon3d-0.0.2/toon3d-labeler/node_modules/flatted/python/flatted.py
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     2129 2024-04-30 22:25:05.000000 toon3d-0.0.2/toon3d-labeler/node_modules/flatted/python/test.py
+drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-05-13 05:32:20.450004 toon3d-0.0.2/toon3d-spaces/
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)    10976 2024-05-13 05:21:40.000000 toon3d-0.0.2/toon3d-spaces/app.py
+drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-05-13 05:32:20.454004 toon3d-0.0.2/toon3d.egg-info/
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)      826 2024-05-13 05:32:19.000000 toon3d-0.0.2/toon3d.egg-info/PKG-INFO
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     1369 2024-05-13 05:32:20.000000 toon3d-0.0.2/toon3d.egg-info/SOURCES.txt
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)        1 2024-05-13 05:32:19.000000 toon3d-0.0.2/toon3d.egg-info/dependency_links.txt
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)      393 2024-05-13 05:32:19.000000 toon3d-0.0.2/toon3d.egg-info/entry_points.txt
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)      280 2024-05-13 05:32:19.000000 toon3d-0.0.2/toon3d.egg-info/requires.txt
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)       56 2024-05-13 05:32:19.000000 toon3d-0.0.2/toon3d.egg-info/top_level.txt
```

### Comparing `toon3d-0.0.1/PKG-INFO` & `toon3d-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toon3d
-Version: 0.0.1
+Version: 0.0.2
 Summary: toon3d package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Requires-Python: >=3.7.3
 Requires-Dist: black
 Requires-Dist: h5py
 Requires-Dist: mediapy
```

### Comparing `toon3d-0.0.1/README.md` & `toon3d-0.0.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-# toon3d
+# Toon3D
 
-This project enables 3D reconstruction of non-geometric scenes, such as cartoons. _We can take a few images from a cartoon and reconstruct it in 3D._
+This project enables 3D reconstruction of non-geometrically consistent scenes, such as cartoons. _We take a few images from a cartoon and reconstruct it in 3D._
 
 |   Image 1   |   Image 2   |   Image 3   |
 | :------------------------: | :--------------------------: | :-------------------------: |
-| ![](media/randm_left.jpeg) | ![](media/randm_center.jpeg) | ![](media/randm_right.jpeg) |
+| ![](toon3d/assets/randm_left.jpeg) | ![](toon3d/assets/randm_center.jpeg) | ![](toon3d/assets/randm_right.jpeg) |
 
 # Setting up the environment
 
 Create a conda environment. 
 
 1. Install the latest nerfstudio package.
 
@@ -77,45 +77,52 @@
 This step runs depth estimation and Segment Anything (SAM).
 
 Download [SAM](https://github.com/facebookresearch/segment-anything) weights with `tnd-download-data sam`.
 
 Now, you can run
 
 ```bash
-tnd-process-data --dataset [dataset] --input_path [input_path]
+tnd-process-data initialize --dataset [dataset] --input_path [input_path]
 ```
 
 Where the `input_path` is the source folder of your images while `dataset` is the name of the dataset that will be output to `data/processed/[dataset]`
 
 For example,
 
 ```bash
-tnd-process-data --dataset bobs-burgers-dining --input_path data/images/bobs-burgers-dining
+tnd-process-data initialize --dataset bobs-burgers-dining --input_path data/images/bobs-burgers-dining
 ```
 
-## Label images
-
-You can use [toon3d.studio](https://toon3d.studio/), or, if you want to make edits locally then run the following.
+If you want to add more images to your dataset, run this
 
 ```bash
-cd labeler
-nvm use 20
-npm install
-npm start
+tnd-process-data add --dataset bobs-burgers-dining --input_path data/images/more-bobs-burgers-dining-photos
 ```
 
+## Label images
+
+You can use [labeler.toon3d.studio](https://labeler.toon3d.studio/).
+
+You have two ways of getting your data in the viewer.
+
+(1) **Uploading ZIP folders**
+
+You can either upload a zipped process-data folder or simply a selection of images. If just images, you'll have more limited functionality (no depth images or SAM masks).
+
+(2) **No-upload version for faster development**
+
 Expose your processed data to a public URL. Here is an example with our script with CORS allowed for any origin. You can change the port or the relative directory from which to host the files from.
 
 ```bash
 tnd-server --path data/processed --port 8000
 ```
 
 Now, open your processed dataset and annotate.
 
-Navigate to https://toon3d.studio/?path=http://localhost:8000/bobs-burgers-dining in our case. Or, if you are developing locally then http://localhost:3000/?path=http://localhost:8000/bobs-burgers-dining.
+Navigate to https://labeler.toon3d.studio/?path=http://localhost:8000/bobs-burgers-dining in our case. Or, if you are developing locally then http://localhost:3000/?path=http://localhost:8000/bobs-burgers-dining.
 
 ## Run structure from motion!
 
 Now we can run our method to get a dense 3D reconstruction for novel-view synthesis.
 
 ```bash
 tnd-run --help
@@ -131,14 +138,25 @@
 
 For example,
 
 ```bash
 ns-train toon3d --data data/nerfstudio/bobs-burgers-dining
 ```
 
+To train a depth-nerfacto, run the following:
+
+```bash
+ns-train depth-nerfacto --data data/nerfstudio/bobs-burgers-dining \
+    --pipeline.use_visibility_loss True \
+    --pipeline.visibility_min_views 1 \
+    --pipeline.model.is_euclidean_depth True \
+    nerfstudio-data \
+    --depth_unit_scale_factor 1.0
+```
+
 <details>
 <summary><strong>(Optional) Regularize with a fine-tuned diffusion model</strong></summary>
 <br>
 
 <blockquote style="margin: 0 0 0 20px; border-left: 3px solid #4CAF50; padding: 0 10px;">
 
 We can fine-tune a diffusion model on our data, and then we can apply it while optimizing the 3D model. Check out the wandb logs to see training progress.
@@ -165,14 +183,20 @@
 
 Render a camera path that you created
 
 ```bash
 tnd-render camera-path --load-config [load-config] --camera-path-filename [camera-path-filename] --output-path [output-path].mp4
 ```
 
+Render videos between training views
+
+```bash
+tnd-render interpolate --load-config [load-config] --output-path [output-path]
+``` 
+
 # Test cases
 
 ```bash
 pytest tests
 ```
 
 # Project structure
```

### Comparing `toon3d-0.0.1/toon3d-current/color_palette.py` & `toon3d-0.0.2/toon3d/color_palette.py`

 * *Files identical despite different names*

### Comparing `toon3d-0.0.1/toon3d-current/configs/prompts.py` & `toon3d-0.0.2/toon3d/configs/prompts.py`

 * *Files identical despite different names*

### Comparing `toon3d-0.0.1/toon3d-current/generative/ldm3d.py` & `toon3d-0.0.2/toon3d/generative/ldm3d.py`

 * *Files identical despite different names*

### Comparing `toon3d-0.0.1/toon3d-current/generative/marigold.py` & `toon3d-0.0.2/toon3d/generative/marigold.py`

 * *Files identical despite different names*

### Comparing `toon3d-0.0.1/toon3d-current/scripts/download_data.py` & `toon3d-0.0.2/toon3d/scripts/download_data.py`

 * *Files identical despite different names*

### Comparing `toon3d-0.0.1/toon3d-current/scripts/finetune.py` & `toon3d-0.0.2/toon3d/scripts/finetune.py`

 * *Files identical despite different names*

### Comparing `toon3d-0.0.1/toon3d-current/scripts/run.py` & `toon3d-0.0.2/toon3d/scripts/run.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,102 +3,38 @@
 """
 
 from pathlib import Path
 import json
 from datetime import datetime
 import io
 
+import cv2 
+import kornia
 import mediapy
 import numpy as np
 import plotly.graph_objects as go
 import torch
 import torch.nn as nn
 from tqdm import tqdm
 import shutil
 import cv2
 
 import tyro
 import viser
 from toon3d.utils.draw_utils import get_images_with_keypoints
+from toon3d.utils.viser_utils import view_pcs_cameras
 from toon3d.utils.camera_utils import Cameras
-from toon3d.warp.warp_mesh import WarpMesh, draw_tris, draw_points, create_triangulations
-from toon3d.warp.warp_losses import constant_triangulation_loss
-from toon3d.warp.arap_utils import face_verts_arap_loss
-from toon3d.warp.tri_rasterize import rasterize_texture
+from toon3d.warp.warp_mesh import WarpMesh, draw_tris, draw_points, FrameMeshes, get_simplices
+from toon3d.warp.arap_utils import face_verts_arap_loss, calc_area_loss, signed_areas
+from toon3d.utils.depth_utils import create_discontinuity_mask
+from toon3d.utils.mesh_utils import get_mesh, save_mesh
 
+from nerfstudio.utils.colormaps import apply_depth_colormap
 from nerfstudio.utils.rich_utils import CONSOLE
 
-def optimize_mesh(
-    mesh,
-    iters=400,
-    split_iters=200,
-    tri_loss_mult=1,
-    tri_reg_mult=1,
-    lr=0.5,
-    num_fixed_points=None,
-    split_faces=True,
-    flip_edges=True,
-    show_triangulation=True,
-):
-    if not num_fixed_points:
-        num_fixed_points = mesh.num_fixed_points
-    optim = torch.optim.Adam([mesh.points], lr=lr)
-
-    image_np = mesh.image[0].detach().cpu().numpy()
-
-    frames = []
-    error_frames = []
-    wire_frames = []
-
-    pbar = tqdm(range(iters))
-    for p in pbar:
-        optim.zero_grad()
-
-        # photometric loss
-        if show_triangulation:
-            tri_loss, to_split, tri_image = constant_triangulation_loss(mesh, return_image=True)
-
-            tri_image = tri_image.cpu().detach().numpy()
-            ref_image = mesh.image[0].cpu().detach().numpy()
-
-            frames.append(draw_tris(mesh, image=tri_image))
-            error_frames.append((tri_image - ref_image) ** 2)
-            wire_frames.append(draw_tris(mesh, image=image_np))
-        else:
-            tri_loss, to_split = constant_triangulation_loss(mesh, return_image=False)
-
-        # regularization
-        tri_reg = mesh.laplacian_smoothing_loss()
-
-        loss = tri_loss_mult * tri_loss + tri_reg_mult * tri_reg
-        loss.backward()
-
-        # mask grad for corners
-        # print(mesh.points.grad)
-        mesh.points.grad[:52] = 0
-        optim.step()
-
-        with torch.no_grad():
-            if p < split_iters and split_faces and len(to_split) > 0:
-                mesh.split_face(to_split[0])
-                optim.param_groups[0]["params"][0] = mesh.points
-
-            mesh.points[mesh.points < 0] = 0
-            mesh.points[:, 0][mesh.points[:, 0] > mesh.width - 1] = mesh.width - 1
-            mesh.points[:, 1][mesh.points[:, 1] > mesh.height - 1] = mesh.height - 1
-
-            if flip_edges:
-                while (to_flip := mesh.find_edge_flips()) and to_flip > -1:
-                    mesh.flip_edge(to_flip)
-
-        pbar.set_description(f"loss: {loss:.2e}, tri_loss: {tri_loss:.2e}, tri_reg: {tri_reg:.2e}", refresh=True)
-
-    if show_triangulation:
-        return frames, error_frames, wire_frames
-
 
 def make_transforms_json(fxs, fys, Rs, ts, widths, heights):
     fxs, fys, Rs, ts = fxs.detach().cpu(), fys.detach().cpu(), Rs.detach().cpu(), ts.detach().cpu()
     transforms = {
         "camera_model": "OPENCV",
         "ply_file_path": "plys/all.ply",
         "points": "points/points.pt",
@@ -135,29 +71,54 @@
     return transforms
 
 def make_dense_points_3d(cameras, depths, factor=4):
     dense_points_3d = []
 
     for ndx, depth_map in enumerate(depths): 
         height, width = depth_map.shape
-        xs = torch.arange(width)
-        ys = torch.arange(height)
+        xs = torch.arange(width).to(depth_map.device)
+        ys = torch.arange(height).to(depth_map.device)
         grid_x, grid_y = torch.meshgrid(xs, ys, indexing="ij")
 
         grid_x = (grid_x / (width - 1) * 2) - 1
         grid_y = (grid_y / (height - 1) * 2) - 1
 
         x = grid_x[::factor, ::factor].flatten()
         y = grid_y[::factor, ::factor].flatten()
         z = depth_map[::factor, ::factor].T.flatten()
 
         dense_points_3d.append(cameras(x, y, z)[ndx])
 
     return dense_points_3d
 
+def make_dense_points_3d_no_flatten(cameras, depths, factor=1):
+    dense_points_3d = []
+
+    for ndx, depth_map in enumerate(depths): 
+        height, width = depth_map.shape
+        xs = torch.arange(width).to(depth_map.device)
+        ys = torch.arange(height).to(depth_map.device)
+        grid_x, grid_y = torch.meshgrid(xs, ys, indexing="ij")
+
+        grid_x = (grid_x / (width - 1) * 2) - 1
+        grid_y = (grid_y / (height - 1) * 2) - 1
+
+        x = grid_x
+        y = grid_y
+        z = depth_map.T
+
+        shape = x.shape
+
+        points = cameras(x.flatten(), y.flatten(), z.flatten())[ndx]
+        points = points.reshape(shape + (3,))
+
+        dense_points_3d.append(points)
+
+    return dense_points_3d
+
 
 def make_plys(images_colors, points_3d):
     n = len(images_colors)
     plys = []
     for i in range(n):
         image_colors = images_colors[i]
         ply_points = points_3d[i]
@@ -180,189 +141,175 @@
             ply.write(f"{x:8f} {y:8f} {z:8f} {r} {g} {b}\n")
 
         plys.append(ply.getvalue())
         ply.close()
 
     return plys
 
-def load_dataset(data_prefix, dataset):
+def load_dataset(data_prefix, dataset, device="cpu", dilate_mask_iters=4, dilate_lines_thresh=0.05, dilate_lines_iters=3, min_valid_points=3):
     images_path = data_prefix / f"{dataset}/images"
     metadata_path = data_prefix / f"{dataset}/metadata.json"
     points_path = data_prefix / f"{dataset}/points.json"
     depths_path = data_prefix / f"{dataset}/depths"
 
     metadata_json = json.loads(metadata_path.read_text())
 
     points_json = json.loads(points_path.read_text())
     valid_images = points_json["validImages"]
     points_list = [[[p["x"], p["y"]] for p in points] for points in points_json["points"]]
     valid_points_list = points_json["validPoints"]
+    # update valid_images based on valid_points_list and min_valid_points
+    valid_images = [valid_images[i] and sum(valid_points_list[i]) >= min_valid_points for i in range(len(valid_images))]
     valid_polygons = points_json["polygons"]
     image_filenames = sorted(list(images_path.glob("*.png")))
 
     # only keep the valid indices, based on valid_images
     metadata_json["frames"] = [
         metadata_json["frames"][i] for i in range(len(metadata_json["frames"])) if valid_images[i]
     ]
     points_list = [points_list[i] for i in range(len(points_list)) if valid_images[i]]
     valid_points_list = [valid_points_list[i] for i in range(len(valid_points_list)) if valid_images[i]]
     valid_polygons = [valid_polygons[i] for i in range(len(valid_polygons)) if valid_images[i]]
     image_filenames = [image_filenames[i] for i in range(len(image_filenames)) if valid_images[i]]
 
     images = [torch.from_numpy(mediapy.read_image(imf)[:, :, :3] / 255.0).float() for imf in image_filenames]
     n = len(images)
-    heights = torch.tensor([image.shape[0] for image in images])
-    widths = torch.tensor([image.shape[1] for image in images])
+    heights = torch.tensor([image.shape[0] for image in images]).to(device)
+    widths = torch.tensor([image.shape[1] for image in images]).to(device)
 
     m = max([len(p) for p in points_list])
 
-    points = torch.full([n, m, 2], -1)
+    points = torch.full([n, m, 2], -1).float().to(device)
     for i in range(n):
         for j in range(len(points_list[i])):
             points[i, j, 0] = points_list[i][j][0]
             points[i, j, 1] = points_list[i][j][1]
 
     # points_mask padded with False
     points_mask = torch.zeros_like(points[:, :, 0]) == 1
     for i in range(n):
         for j in range(len(points_list[i])):
             points_mask[i, j] = valid_points_list[i][j]
 
+    # remove points that have no pair
+    points_mask.T[(points_mask * 1).sum(0) < 2][:] = False
+
     depths = []
     for i in range(len(valid_images)):
-        depths.append(torch.load(depths_path / f"{i:05d}.pt").squeeze())
+        depths.append(torch.load(depths_path / f"{i:05d}.pt").squeeze().to(device))
     # only keep the valid indices, based on valid_images
     depths = [depths[i] for i in range(len(depths)) if valid_images[i]]
     max_depth = max([torch.max(depth) for depth in depths])
     depths = [depth / max_depth for depth in depths]
 
     masks = []
     for i in range(n):
         mask_image = np.ones((heights[i], widths[i]), dtype=np.uint8) * 255
         for j in range(len(metadata_json["frames"][i]["masks"])):
             mask = metadata_json["frames"][i]["masks"][j]
             for k in range(len(mask["polygons"])):
                 contour = np.array(mask["polygons"][k]).reshape(-1, 2).astype(np.int32)
+                temp_mask_image = np.zeros((heights[i], widths[i]), dtype=np.uint8)
                 if valid_polygons[i][j][k]:
-                    cv2.fillPoly(mask_image, [contour], 0)
+                    cv2.fillPoly(temp_mask_image, [contour], 1)
+                temp_mask_image = cv2.dilate(temp_mask_image, np.ones((5, 5), np.uint8), iterations=dilate_mask_iters)
+                mask_image[temp_mask_image == 1] = 0
         masks.append(mask_image)
 
-    shapes = torch.cat([widths[:, None], heights[:, None]], -1).unsqueeze(1).repeat(1, m, 1)
+    # mask out parts of the depth map where they are big discontinuities
+    for i in range(n):
+        depth_mask = 1 - create_discontinuity_mask(depths[i][None], dilate_lines_thresh, dilate_lines_iters)[0].float()
+        masks[i] *= depth_mask.cpu().numpy().astype(np.uint8)
+
+    shapes = torch.cat([widths[:, None], heights[:, None]], -1).unsqueeze(1).repeat(1, m, 1).to(device)
     points_normed = (points / shapes) * 2 - 1
 
     return images, heights, widths, points, points_normed, points_mask, depths, masks
 
 
-def view_pcs_cameras(server,
-                     images, # images
-                     cameras,
-                     dense_points_3d, # dense pc
-                     images_colors, 
-                     sparse_points_3d, # sparse pc
-                     point_colors, 
-                     mesh_verts_list, # mesh
-                     simplices_list,
-                     mesh_colors,
-                     prefix="data"):
-
-    heights = torch.tensor([image.shape[0] for image in images])
-
-    # from our coords to viser coords X, Y, Z -> -Z, X, -Y
-    flip = torch.tensor([[0, 0, -1], [1, 0, 0], [0, -1, 0]]).float()
-    for ndx in range(len(images)):
-        server.add_mesh_simple(
-            f"{prefix}/mesh/img-{ndx}/fill",
-            vertices=5 * (flip @ mesh_verts_list[ndx].T).T.cpu().detach().numpy(),
-            faces=simplices_list[ndx].cpu().detach().numpy(),
-            color=mesh_colors[ndx],
-            wxyz=viser.transforms.SO3.from_x_radians(0).wxyz,
-            opacity=0.4,
-            flat_shading=True,
-            side='double',
-            visible=False,
-        )
-
-        #wireframe
-        server.add_mesh_simple(
-            f"{prefix}/mesh/img-{ndx}/wireframe",
-            vertices=5 * (flip @ mesh_verts_list[ndx].T).T.cpu().detach().numpy(),
-            faces=simplices_list[ndx].cpu().detach().numpy(),
-            wireframe=True,
-            color=(0, 0, 0),
-            wxyz=viser.transforms.SO3.from_x_radians(0).wxyz,
-            visible=False,
-        )
-
-        server.add_point_cloud(
-            f"{prefix}/dense-pc/img-{ndx}",
-            colors=images_colors[ndx].detach().numpy(),
-            points=5 * (flip @ dense_points_3d[ndx].T).T.cpu().detach().numpy(),
-            point_size=0.05,
-        )
-
-        server.add_point_cloud(
-            f"{prefix}/sparse-pc/img-{ndx}",
-            colors=point_colors[ndx].detach().numpy(),
-            points=5 * (flip @ sparse_points_3d[ndx].T).T.detach().numpy(),
-            point_size=0.1,
-        )
-
-        server.add_camera_frustum(
-            f"{prefix}/cameras/img-{ndx}",
-            fov=np.arctan2(heights[ndx] / 2, cameras.fxs[ndx].item()),
-            aspect=cameras.fys[ndx].item() / cameras.fxs[ndx].item(),
-            scale=0.1,
-            wxyz=viser.transforms.SO3.from_matrix(flip @ cameras.Rs[ndx].detach().numpy()).wxyz,
-            position=5 * ((flip @ cameras.ts[ndx].flatten().detach().numpy())),
-            image=images[ndx].numpy(),
-        )
-
-
 def main(
     data_prefix: Path = Path("data/processed"),
     dataset: str = "rick-house",
     device: str = "cpu",
     niters: int = 5000,
     lr: float = 0.01,
-    affine_loss_mult: float = 1.0,
+    affine_loss_mult: float = 1000.0,
     scale_loss_mult: float = 1e3,
+    scale_loss_target: float = 1.0,
     offset_loss_mult: float = 1e3,
-    quat_norm_mult: float = 1.0,
     focal_mag_mult: float = 1e-3,
-    focal_fix_mult: float = 1e-3,
-    arap_mult: float = 1, 
-    refine_depths_mult: float = 1e-3,
-    refine_points_mult: float = 1e-2, 
-    refine_pose_mult: float = 1,
+    aspect_mult: float = 1,
+    up_mult: float = 0,
+    niters_warp: int = 2000,
+    lr_warp: float = 0.01,
+    arap_mult: float = 1e3, 
+    zs_diff_mult: float = 0.0,
     output_prefix: Path = Path("outputs"),
+    output_method: Path = Path("run"),
     nerfstudio_folder: Path = Path("data/nerfstudio"),
-    ply_downscale_factor: int = 8,
+    ply_downscale_factor: int = 4,
     view_point_cloud: bool = True,
+    make_video: bool = False,
+    coarse_camera_params: torch.Tensor = None,
+    dzs: torch.Tensor = None,
+    szs: torch.Tensor = None,
+    save_geometry: bool = True,
+    write_to_nerfstudio: bool = True,
+    mask_random_points: int = 0,
+    port: int = 8080,
 ):
     """Script to run our SfM on cartoons."""
 
-    output_folder = output_prefix / dataset / "run" / datetime.now().strftime("%Y-%m-%d_%H%M%S")
+    output_folder = output_prefix / dataset / output_method / datetime.now().strftime("%Y-%m-%d_%H%M%S")
     output_folder.mkdir(parents=True)
 
-    images, heights, widths, points, points_normed, points_mask, depths, masks = load_dataset(data_prefix, dataset)
+    images, heights, widths, points, points_normed, points_mask, depths, masks = load_dataset(data_prefix, dataset, device)
     n, m = points.shape[:2]
+    
+    # for hold-out evaluation
+    original_points_mask = points_mask.clone()
+    mask_random_points_indices = None
+    if mask_random_points > 0:
+        # set a seed
+        torch.manual_seed(0)
+        mask_random_points_indices = torch.randperm(m)[:mask_random_points]
+        points_mask[:, mask_random_points_indices] = False
+
+    depth_offset = 0.2
+    depths = [depths[i] + depth_offset for i in range(n)]
+
+    # set all depths to depth_offset
+    depths = [torch.ones_like(depth) for depth in depths]
 
     # draw keypoints on image
-    point_colors = torch.rand((m, 3))
-    colors = point_colors[None].repeat(n, 1, 1).to(device)
-    colors[~points_mask] = torch.tensor([1, 1, 1]).to(device).float()
+    point_colors = torch.rand((m, 3)).to(device)
+    colors = point_colors[None].repeat(n, 1, 1)
+    colors[~points_mask] = torch.tensor([1, 1, 1]).float().to(device)
     output_images_dir = Path(output_folder / "images")
     output_images_dir.mkdir(parents=True)
     for i in range(n):
         keypoint_image = get_images_with_keypoints(
-            images[i].permute(2, 0, 1)[None], points_normed[i][None], colors[i][None], keypoint_size=5
+            images[i].permute(2, 0, 1)[None], points_normed[i][None].cpu(), colors[i][None], keypoint_size=5
         )[0].permute(1, 2, 0)
         
         mediapy.write_image(output_images_dir / f"{i:02d}.png", keypoint_image)
 
+    # make borders
+    border_masks = []
+    for ndx in range(n):
+        pts = points[ndx][points_mask[ndx]]
+        spls = get_simplices(pts)
+
+        mask_mesh = WarpMesh(pts, spls, heights[ndx], widths[ndx], pts, device=device)
+        border_mask = (mask_mesh.rasterize().pix_to_face[0,...,0] > -1) * 1.0
+        border_mask = border_mask.cpu().numpy()
+
+        masks[ndx] = masks[ndx] * border_mask
+        border_masks.append(border_mask)
+
     ########################################
     ###### coarse camera optimization ######
     ########################################
     CONSOLE.print("[bold green] Camera optimization")
 
     # make pairs for comparison in optimization
     pairs = []
@@ -379,475 +326,557 @@
     vs = points[..., 1].int()
 
     us_normed = us / (widths[..., None] - 1) * 2 - 1
     vs_normed = vs / (heights[..., None] - 1) * 2 - 1
 
     zs = torch.stack([depths[ndx][vs[ndx], us[ndx]] for ndx in range(n)])
 
-    dzs = nn.Parameter(torch.zeros([n]).float()) # delta zs
-    szs = nn.Parameter(torch.ones([n]).float()) # scale zs
+    dzs = nn.Parameter(torch.zeros([n]).float().to(device)) # delta zs
+    szs = nn.Parameter(torch.ones([n]).float().to(device)) # scale zs
 
     # make cameras and optimizer
-    coarse_cameras = Cameras(n)
-    optimizer = torch.optim.Adam(list(coarse_cameras.parameters()) + [szs, dzs], lr=lr)
-
-    # optimization loop
-    pbar = tqdm(range(niters))
-
-    for i in pbar:
-
-        new_zs = zs * szs[...,None] + dzs[...,None]
-        points_3d = coarse_cameras(us_normed, vs_normed, new_zs)
-
-        paired_points = points_3d[pairs]
-
-        affine_loss = affine_loss_mult * torch.mean(((paired_points[0] - paired_points[1]) ** 2) * pairs_mask)
-
-        scale_loss = scale_loss_mult * ((torch.mean(szs) - 1) ** 2)
-
-        offset_loss = offset_loss_mult * torch.mean(torch.relu(-dzs) ** 2)
-
-        quat_norm = quat_norm_mult * torch.mean((torch.sum(coarse_cameras.quats**2, 1) - 1) ** 2)
-
-        focal_mag = focal_mag_mult * (torch.mean(coarse_cameras.fxs) + torch.mean(coarse_cameras.fys))
-
-        focal_fix = focal_fix_mult * torch.mean((coarse_cameras.fys / coarse_cameras.fxs - widths / heights) ** 2)
-
-        loss = affine_loss + scale_loss + offset_loss + quat_norm + focal_mag + focal_fix
-
-        optimizer.zero_grad()
-        loss.backward()
-        optimizer.step()
-
-        # keep first point cloud fixed
-        with torch.no_grad():
-            coarse_cameras.quats[0] = torch.tensor([1, 0, 0, 0])
-            coarse_cameras.ts[0] = torch.zeros([3])
-
-            pbar.set_description(f"Loss: {affine_loss:.2e}", refresh=True)
+    coarse_cameras = Cameras(n).to(device)
 
-    # rescale depth maps
+    # load cameras if exist
+    if coarse_camera_params is not None:
+        coarse_cameras.load_state_dict(coarse_camera_params)
+    else:
+        optimizer = torch.optim.Adam(list(coarse_cameras.parameters()) + [szs, dzs], lr=lr)
+
+        # optimization loop
+        pbar = tqdm(range(niters))
+
+        for i in pbar:
+
+            new_zs = zs * szs[...,None] + dzs[...,None]
+            points_3d = coarse_cameras(us_normed, vs_normed, new_zs)
+            paired_points = points_3d[pairs]
+            affine_loss = affine_loss_mult * torch.mean(((paired_points[0] - paired_points[1]) ** 2) * pairs_mask)
+
+            scale_loss = scale_loss_mult * ((torch.mean(szs) - scale_loss_target) ** 2 + torch.mean(torch.relu(-szs) ** 2))
+            offset_loss = offset_loss_mult * torch.mean(torch.relu(-dzs) ** 2)
+            focal_mag = focal_mag_mult * (torch.mean(coarse_cameras.fxs) + torch.mean(coarse_cameras.fys))
+            focal_fix = aspect_mult * torch.mean((coarse_cameras.fys / coarse_cameras.fxs - widths / heights) ** 2)
+            up_loss = up_mult * torch.mean((torch.abs((coarse_cameras.Rs @ torch.tensor([0, 1, 0]).float().to(device))[:,1] - 1)))
+            loss = affine_loss + scale_loss + offset_loss + focal_mag + focal_fix + up_loss
+
+            optimizer.zero_grad()
+            loss.backward()
+            optimizer.step()
+
+            # keep first point cloud fixed
+            with torch.no_grad():
+                coarse_cameras.quats[0] = torch.tensor([1, 0, 0, 0])
+                coarse_cameras.ts[0] = torch.zeros([3])
+
+                pbar.set_description(f"Loss: {loss:.2e}, 3D: {affine_loss:.2e}", refresh=True)
+
+                # unbounded scale and offset
+                if scale_loss_mult == 0:
+                    szs[:] = 1
+                if offset_loss_mult == 0:
+                    dzs[:] = 0
 
     # make new cameras
-
     refined_cameras = Cameras(n, 
-                              coarse_cameras.fxs.detach().clone(), 
-                              coarse_cameras.fys.detach().clone(), 
-                              coarse_cameras.quats.detach().clone(), 
-                              coarse_cameras.ts.detach().clone())
+                            coarse_cameras.fxs.detach().clone(), 
+                            coarse_cameras.fys.detach().clone(), 
+                            coarse_cameras.quats.detach().clone(), 
+                            coarse_cameras.ts.detach().clone()).to(device)
+
+    new_zs = zs * szs[...,None] + dzs[...,None]
 
     ################################
     ###### make triangulation ######
     ################################
     CONSOLE.print("[bold green] Image triangulation")
 
-    corr_points_list, boundary_points_list, inner_points_list, simplices_list = create_triangulations(points, points_mask, widths, heights)
-    edges_list = [torch.unique(torch.stack((simplices[:, [0, 1]], simplices[:, [1, 2]], simplices[:, [2, 0]]), dim=0).flatten(0, 1).sort(1).values, dim=0).T for simplices in simplices_list]
+    frame_meshes = FrameMeshes(points, points_mask, depths, heights, widths)
 
-    # number of corr, boundary, and inner points per mesh
-    num_corrs_per_mesh = [len(cp) for cp in corr_points_list]
-    num_boundary_pts_per_mesh = [len(bp) for bp in boundary_points_list]
-    num_inner_pts_per_mesh = [len(ip) for ip in inner_points_list]
-
-    # make original mesh points
-    original_mesh_points_list = [torch.cat(omp_triple) for omp_triple in zip(corr_points_list, boundary_points_list, inner_points_list)]
-    original_mesh_points_packed = torch.cat(original_mesh_points_list)
-    num_points_per_mesh = torch.tensor([len(omp) for omp in original_mesh_points_list])
-
-    # make simplices
-    simplices_shifts = torch.cat([torch.tensor([0]), num_points_per_mesh.cumsum(0)[:-1]])
-    simplices_shifted_list = [simplices + shift for simplices, shift in zip(simplices_list, simplices_shifts)]
-    simplices_shifted_packed = torch.cat(simplices_shifted_list)
-
-    # original face verts
-    original_face_verts_packed = original_mesh_points_packed[simplices_shifted_packed].mT
-
-    # make warped points
-    warped_boundary_points_list = [nn.Parameter(bp.detach().clone()) for bp in boundary_points_list]
-    warped_inner_points_list = [nn.Parameter(ip.detach().clone()) for ip in inner_points_list]
-    
-    mesh_us_list = []
-    mesh_vs_list = []
-    mesh_zs_list = []
-    zs_diff_list = []
-
-    for ndx in range(n):
-        original_mesh_points = original_mesh_points_list[ndx]
-
-        mesh_us = original_mesh_points[...,0].int()
-        mesh_vs = original_mesh_points[...,1].int()
-
-        mesh_zs = depths[ndx][mesh_vs, mesh_us].detach()
-
-        edges = edges_list[ndx]
-
-        mesh_us_list.append(mesh_us)
-        mesh_vs_list.append(mesh_vs)
-        mesh_zs_list.append(mesh_zs)
-
-        zs_diff_list.append(mesh_zs[edges[0]] - mesh_zs[edges[1]])
+    # face verts for ARAP
+    face_verts_packed = frame_meshes.points_packed[frame_meshes.simplices_packed].mT
 
     ###################################
     ###### epipolar optimization ######
     ###################################
     CONSOLE.print("[bold green] Image Warping")
 
-    # set up optimizer
-    dus = nn.Parameter(torch.zeros_like(us).float())
-    dvs = nn.Parameter(torch.zeros_like(vs).float())
+    dzs_warp = nn.Parameter(dzs.detach().clone()) # delta zs
+    szs_warp = nn.Parameter(szs.detach().clone()) # scale zs
 
-    pzs = nn.Parameter(torch.zeros_like(zs)) # perturbation zs
-    vert_pzs_list = [nn.Parameter(torch.zeros_like(mesh_zs[num_corrs:].detach())) for mesh_zs, num_corrs in zip(mesh_zs_list, num_corrs_per_mesh)]
+    # set up optimizer
+    optimizer = torch.optim.Adam(list(frame_meshes.parameters()) + list(refined_cameras.parameters()) + [szs_warp, dzs_warp], lr=lr_warp)
+    # optimizer = torch.optim.Adam(frame_meshes.parameters(), lr=lr_warp)
+    video_warped_mesh_points = [[] for _ in range(n)]
 
-    optimizer = torch.optim.Adam([pzs, dus, dvs] + [bp for bp in warped_boundary_points_list] + [ip for ip in warped_inner_points_list] + [vp for vp in vert_pzs_list], lr=lr)
-    # optimizer = torch.optim.Adam(list(refined_cameras.parameters()) + [pzs, dus, dvs]  + [bp for bp in warped_boundary_points_list] + [ip for ip in warped_inner_points_list], lr=lr)
-    
     # optimization loop
-    pbar = tqdm(range(niters//2))
+    pbar = tqdm(range(niters_warp))
 
-    # import pdb; pdb.set_trace()
+    tri_areas = signed_areas(face_verts_packed)
 
     for i in pbar:
 
         # arap loss
-        warped_us_packed = (us + dus)[points_mask]
-        warped_vs_packed = (vs + dvs)[points_mask]
-
-        warped_corr_points_packed = torch.stack([warped_us_packed, warped_vs_packed]).T.detach() # (sum(all_valid_corrs), 2)
-        warped_corr_points_list = warped_corr_points_packed.split(num_corrs_per_mesh) # (n, tensor(valid_corrs, 2))
+        warped_face_verts_packed = frame_meshes.warped_points_packed[frame_meshes.simplices_packed].mT
+        arap_loss = arap_mult * face_verts_arap_loss(face_verts_packed, warped_face_verts_packed)
 
-        warped_mesh_points_list = [torch.cat(wmp_triple) for wmp_triple in zip(warped_corr_points_list, warped_boundary_points_list, warped_inner_points_list)]
-        warped_mesh_points_packed = torch.cat(warped_mesh_points_list)
+        # area loss
+        area_loss = calc_area_loss(warped_face_verts_packed, min_area=tri_areas * 0.1)
 
-        warped_face_verts_packed = warped_mesh_points_packed[simplices_shifted_packed].mT
-
-        arap_loss = face_verts_arap_loss(original_face_verts_packed, warped_face_verts_packed)
-
-        # 3D arap loss
-
-        # import pdb; pdb.set_trace();
-        zs_diff_loss = torch.tensor(0.0)
-        for ndx in range(n):
-            corr_pzs = pzs[ndx][points_mask[ndx]].detach() # stop gradient
-            vert_pzs = vert_pzs_list[ndx]
-
-            mesh_zs = mesh_zs_list[ndx]
-            mesh_pzs = torch.cat([corr_pzs, vert_pzs])
-            mesh_zs_pzs = (mesh_zs + mesh_pzs) * szs[ndx] + dzs[ndx]
-
-            edges = edges_list[ndx]
-            zs_diff = zs_diff_list[ndx] * szs[ndx]
-            zs_pzs_diff = mesh_zs_pzs[edges[0]] - mesh_zs_pzs[edges[1]]
-
-            zs_diff_loss += torch.mean((zs_diff - zs_pzs_diff) ** 2) / n
+        # szs, dzs packed for depth_ranking
+        szs_warp_packed = szs_warp.repeat_interleave(torch.tensor(frame_meshes.num_points_per_mesh).to(device)).detach()
+        dzs_warp_packed = dzs_warp.repeat_interleave(torch.tensor(frame_meshes.num_points_per_mesh).to(device)).detach()
+
+        # z_diff_loss
+        zs_packed = frame_meshes.zs_packed * szs_warp_packed + dzs_warp_packed
+        warped_zs_packed = frame_meshes.warped_zs_packed * szs_warp_packed + dzs_warp_packed
+        zs_diff_loss = zs_diff_mult * torch.mean((zs_packed - warped_zs_packed).abs())
 
         # affine loss
-        dus_normed = dus / (widths[..., None] - 1) * 2
-        dvs_normed = dvs / (heights[..., None] - 1) * 2
-        
-        new_zs = (zs + pzs) * szs[...,None] + dzs[...,None]
-        points_3d = refined_cameras(us_normed + dus_normed, vs_normed + dvs_normed, new_zs)
+        warped_us = frame_meshes.warped_corr_points_padded[...,0]
+        warped_vs = frame_meshes.warped_corr_points_padded[...,1]
+        warped_us_normed = warped_us / (widths[..., None] - 1) * 2 - 1
+        warped_vs_normed = warped_vs / (heights[..., None] - 1) * 2 - 1
+        warped_zs = frame_meshes.warped_corr_zs_padded * szs_warp[...,None] + dzs_warp[...,None]
 
+        points_3d = refined_cameras(warped_us_normed, warped_vs_normed, warped_zs)
         paired_points = points_3d[pairs]
+        affine_loss = affine_loss_mult * torch.mean(((paired_points[0] - paired_points[1]) ** 2) * pairs_mask)
 
-        affine_loss = torch.mean(((paired_points[0] - paired_points[1]) ** 2) * pairs_mask)
-
-        # regularizations
-        refine_depths_reg = refine_depths_mult * torch.mean(pzs ** 2)
-        refine_points_reg = refine_points_mult * torch.mean(dus_normed ** 2 + dvs_normed ** 2)
-
-        ts_reg = torch.mean((refined_cameras.ts - coarse_cameras.ts) ** 2)
-        fxs_reg = torch.mean((refined_cameras.fxs - coarse_cameras.fxs) ** 2)
-        fys_reg = torch.mean((refined_cameras.fys - coarse_cameras.fys) ** 2)
-
-        refine_pose_reg = refine_pose_mult * (ts_reg + fxs_reg + fys_reg)
-        
-        loss = affine_loss + arap_mult * arap_loss + refine_depths_reg + refine_points_reg + refine_pose_reg + zs_diff_loss
+        scale_loss = scale_loss_mult * ((torch.mean(szs_warp) - scale_loss_target) ** 2 + torch.mean(torch.relu(-szs_warp) ** 2))
+        offset_loss = offset_loss_mult * torch.mean(torch.relu(-dzs_warp) ** 2)
+        focal_mag = focal_mag_mult * (torch.mean(refined_cameras.fxs) + torch.mean(refined_cameras.fys))
+        focal_fix = aspect_mult * torch.mean((refined_cameras.fys / refined_cameras.fxs - widths / heights) ** 2)
+        up_loss = up_mult * torch.mean((torch.abs((refined_cameras.Rs @ torch.tensor([0, 1, 0]).float().to(device))[:,1] - 1)))
+
+        loss = 0.0
+        loss += affine_loss + scale_loss + offset_loss + focal_mag + focal_fix
+        loss += arap_loss + area_loss + zs_diff_loss + up_loss
 
         optimizer.zero_grad()
         loss.backward()
         optimizer.step()
 
         with torch.no_grad():
             refined_cameras.quats[0] = torch.tensor([1, 0, 0, 0])
             refined_cameras.ts[0] = torch.zeros([3])
-            for ndx in range(n):
-                # keep boundaries outside of frame
-                
-                    pts_at_zero = boundary_points_list[ndx] == 0
-                    pts_at_width = boundary_points_list[ndx] == (widths[ndx] - 1)
-                    pts_at_height = boundary_points_list[ndx] == (heights[ndx] - 1)
-
-                    pt_gthan_zero = warped_boundary_points_list[ndx] > 0
-                    pts_lthan_widths = warped_boundary_points_list[ndx] < widths[ndx] - 1
-                    pts_lthan_height = warped_boundary_points_list[ndx] < heights[ndx] - 1
-
-                    warped_boundary_points_list[ndx][torch.logical_and(pts_at_zero, pt_gthan_zero)] = 0
-                    warped_boundary_points_list[ndx][torch.logical_and(pts_at_width, pts_lthan_widths)] = (widths[ndx] - 1)
-                    warped_boundary_points_list[ndx][torch.logical_and(pts_at_height, pts_lthan_height)] = (heights[ndx] - 1)
 
-        pbar.set_description(f"Loss: {affine_loss:.2e}, arap: {arap_loss:.2e}, zs_diff_loss: {zs_diff_loss:.2e}", refresh=True)
+            # unbounded scale and offset
+            if scale_loss_mult == 0:
+                szs_warp[:] = 1
 
-    ### create meshes for warping ###
+            if offset_loss_mult == 0:
+                dzs_warp[:] = 0
 
-    warped_us_packed = (us + dus)[points_mask]
-    warped_vs_packed = (vs + dvs)[points_mask]
+            corrs_lthan_min = frame_meshes.corr_zs_padded + frame_meshes.delta_corr_zs_padded < 0.1
+            if torch.any(corrs_lthan_min):
+                frame_meshes.delta_corr_zs_padded[corrs_lthan_min] = 0.1 - frame_meshes.corr_zs_padded[corrs_lthan_min]
 
-    warped_corr_points_packed = torch.stack([warped_us_packed, warped_vs_packed]).T.detach() # (sum(all_valid_corrs), 2)
-    warped_corr_points_list = warped_corr_points_packed.split(num_corrs_per_mesh) # (n, tensor(valid_corrs, 2))
+            if make_video and i % 20 == 0:
+                for ndx in range(n):
+                        video_warped_mesh_points[ndx].append(frame_meshes.warped_corr_points_list[ndx].clone())
 
-    warped_mesh_points_list = [torch.cat(wmp_triple) for wmp_triple in zip(warped_corr_points_list, warped_boundary_points_list, warped_inner_points_list)]
-    
+
+        pbar.set_description(f"Loss: {loss:.2e}, 3D: {affine_loss:.2e}, ARAP: {arap_loss:.2e}, Z: {zs_diff_loss:.2e}", refresh=True)
+
+    ### create meshes for warping ###
     all_meshes = []
 
     for ndx in range(n):
-        uv_points = original_mesh_points_list[ndx]
-        warped_mesh_points = warped_mesh_points_list[ndx]
-        simplices = simplices_list[ndx]
+        warped_mesh_points = frame_meshes.warped_points_list[ndx]
+        uv_points = frame_meshes.points_list[ndx]
+        simplices = frame_meshes.simplices_list[ndx]
 
         mesh = WarpMesh(warped_mesh_points, simplices, heights[ndx], widths[ndx], uv_points, device=device)
 
         all_meshes.append(mesh)
 
     # warp images and depths
-    
-    # rescale depths
-    depths = [(depth_map * sz[...,None]) + dz[...,None] for depth_map, dz, sz in zip(depths, dzs, szs)]
-        
     warped_images = []
     warped_depths = []
     warped_masks = []
 
-    output_warped_images_dir = Path(output_folder / "warped_images")
-    output_warped_depths_dir = Path(output_folder / "warped_depths")
-    output_warped_masks_dir = Path(output_folder / "warped_masks")
+    warp_visuals_dir = output_folder / "visuals_warp"
+    output_warped_images_dir = Path(warp_visuals_dir / "warped_images")
+    output_warped_depths_dir = Path(warp_visuals_dir / "warped_depths")
+    output_warped_masks_dir = Path(warp_visuals_dir / "warped_masks")
+    output_warp_colormap_dir = Path(warp_visuals_dir / "warp_colormaps")
 
+    warp_visuals_dir.mkdir(parents=True, exist_ok=True)
     output_warped_images_dir.mkdir(parents=True)
     output_warped_depths_dir.mkdir(parents=True)
     output_warped_masks_dir.mkdir(parents=True)
+    output_warp_colormap_dir.mkdir(parents=True)
+
+    CONSOLE.print("[bold green] Rendering Images")
 
     for ndx in range(len(all_meshes)):
         mesh = all_meshes[ndx]
         image = images[ndx]
         depth_map = depths[ndx]
         mask = torch.from_numpy(masks[ndx]).float()
 
+        mesh.pzs = frame_meshes.delta_zs_list[ndx]
+
         fragments = mesh.rasterize()
-        warped_image = mesh.render(image, fragments)
+        warped_pdepth = (fragments.zbuf[0,...,0] - mesh.z_offset)
+        warped_image = mesh.render(image, fragments).cpu().detach()
         warped_depth = mesh.render(depth_map, fragments)
+
         warped_mask = mesh.render(mask, fragments)
+        warped_mask[warped_mask < 100] = 0
 
-        warped_image = warped_image.cpu().detach()
-        warped_depth = warped_depth.cpu().detach()[...,0]
+        warped_depth = warped_depth.cpu().detach()[...,0] + warped_pdepth.cpu().detach()
         warped_mask = warped_mask.cpu().detach()[...,0].to(torch.uint8).numpy()
 
         wire_img = draw_tris(mesh, image = warped_image.numpy())
-        points_img = draw_points(mesh, image=wire_img, points=warped_corr_points_list[ndx], colors=point_colors[points_mask[ndx]].tolist())
+        points_img = draw_points(mesh, image=wire_img, points=frame_meshes.warped_corr_points_list[ndx], colors=point_colors[points_mask[ndx]].tolist())
+
+        border_mask = border_masks[ndx]
+        image[border_mask == 0] = 1
+        warp_transition = ((warped_image * 0.5) + (image * 0.5)).numpy()
+
+        warp_transition = draw_tris(mesh, points= mesh.uv_points, image = warp_transition, color = (0.5, 0.5, 0.5)) # draw old verts
+        warp_transition = draw_points(mesh, image=warp_transition, points=frame_meshes.corr_points_list[ndx], colors=((1+point_colors[points_mask[ndx]])/2).tolist())
+
+        warp_transition = draw_tris(mesh, image = warp_transition)
+        warp_transition = draw_points(mesh, image=warp_transition, points=frame_meshes.warped_corr_points_list[ndx], colors=point_colors[points_mask[ndx]].tolist())
+        
+        colors_ = ((1+point_colors[points_mask[ndx]])/2).tolist()
+        for old_point, new_point, color_ in zip(mesh.uv_points, mesh.points, colors_):
+            x0, y0 = old_point[0].int().item(), old_point[1].int().item()
+            x1, y1 = new_point[0].int().item(), new_point[1].int().item()
+
+            warp_transition = cv2.arrowedLine(warp_transition, (x0, y0), (x1, y1), color_, 2) 
+
+        mediapy.write_image(output_warp_colormap_dir / f"{ndx:02d}.png", warp_transition)
 
         # save warps to outputs
-        mediapy.write_image(output_warped_images_dir / f"{ndx:02d}.png", np.concatenate([warped_image.numpy(), points_img], axis=1))
+        mediapy.write_image(output_warped_images_dir / f"{ndx:02d}.png", warped_image.numpy())
+        mediapy.write_image(output_warped_images_dir / f"wire_{ndx:02d}.png", points_img)
+        mediapy.write_image(output_warped_images_dir / f"duo_{ndx:02d}.png", np.concatenate([warped_image.numpy(), points_img], axis=1))
+
         mediapy.write_image(output_warped_depths_dir / f"{ndx:02d}.png", warped_depth)
+        mediapy.write_image(output_warped_depths_dir / f"pdepth_{ndx:02d}.png", warped_pdepth.cpu().detach().numpy())
         mediapy.write_image(output_warped_masks_dir / f"{ndx:02d}.png", warped_mask)
-    
+
         warped_images.append(warped_image)
         warped_depths.append(warped_depth)
         warped_masks.append(warped_mask)
 
-    # import pdb; pdb.set_trace();
+    if make_video:
+        CONSOLE.print("[bold green] Rendering Videos")
+        pbar = tqdm(range(n))
+        for ndx in pbar:
+            warped_mesh_points_frames = video_warped_mesh_points[ndx]
+            
+            uv_points = frame_meshes.points_list[ndx]
+            simplices = frame_meshes.simplices_list[ndx]
+
+            video_frames = []
+
+            mesh = WarpMesh(warped_mesh_points, simplices, heights[ndx], widths[ndx], uv_points, device=device)
+
+            for warped_mesh_points in warped_mesh_points_frames:
+                mesh.points = warped_mesh_points.to(mesh.device).float()
+                image = images[ndx]
+
+                warped_image = mesh.render(image).cpu().detach()
+                wire_img = draw_tris(mesh, image = warped_image.numpy())
+                points_img = draw_points(mesh, image=wire_img, points=warped_mesh_points[:frame_meshes.num_corrs_per_mesh[ndx]], colors=point_colors[points_mask[ndx]].tolist())
+                video_frames.append(np.concatenate([warped_image.numpy(), points_img], axis=1))
+
+            mediapy.write_video(output_warped_images_dir / f"{ndx:02d}.mp4", video_frames)
+
+
+    # rescale depths
+    depths = [(depth_map * sz[...,None]) + dz[...,None] for depth_map, dz, sz in zip(depths, dzs, szs)]
+    warped_depths = [(depth_map.to(device) * sz[...,None]) + dz[...,None] for depth_map, dz, sz in zip(warped_depths, dzs_warp, szs_warp)]
 
 
     #######################
     ###### make json ######
     #######################
 
     nerfstudio_dir = output_folder / "nerfstudio"
     nerfstudio_images_dir = nerfstudio_dir / "images"
     nerfstudio_depths_dir = nerfstudio_dir / "depths"
     nerfstudio_masks_dir = nerfstudio_dir / "masks"
     nerfstudio_points_dir = nerfstudio_dir / "points"
     nerfstudio_meshes_dir = nerfstudio_dir / "meshes"
     nerfstudio_plys_dir = nerfstudio_dir / "plys"
+    nerfstudio_objs_dir = nerfstudio_dir / "objs"
 
     nerfstudio_dir.mkdir(parents=True, exist_ok=True)
     nerfstudio_images_dir.mkdir(parents=True, exist_ok=True)
     nerfstudio_depths_dir.mkdir(parents=True, exist_ok=True)
     nerfstudio_masks_dir.mkdir(parents=True, exist_ok=True)
     nerfstudio_points_dir.mkdir(parents=True, exist_ok=True)
     nerfstudio_meshes_dir.mkdir(parents=True, exist_ok=True)
     nerfstudio_plys_dir.mkdir(parents=True, exist_ok=True)
+    nerfstudio_objs_dir.mkdir(parents=True, exist_ok=True)
 
     # store mesh points
     
-    meshes_points_dict = {"corr_points": corr_points_list, 
-                    "boundary_points":boundary_points_list, 
-                    "inner_points": inner_points_list}
-
-    warped_meshes_points_dict = {"corr_points": warped_corr_points_list, 
-                            "boundary_points":warped_boundary_points_list, # grad still attached to boundary_points
-                            "inner_points": warped_inner_points_list} # grad still attached to inner_points
+    meshes_points_dict = {"corr_points": frame_meshes.corr_points_list, 
+                    "boundary_points": [], 
+                    "inner_points": [],
+                    "points": frame_meshes.points_list}
+
+    warped_meshes_points_dict = {"corr_points": frame_meshes.warped_corr_points_list, 
+                            "boundary_points": [], # grad still attached to boundary_points
+                            "inner_points": [], # grad still attached to inner_points
+                            "points": frame_meshes.warped_points_list
+                            }
 
     # json
     transforms = make_transforms_json(
         refined_cameras.fxs,
         refined_cameras.fys,
         refined_cameras.Rs,
         refined_cameras.ts,
         widths,
         heights,
     )
     with open(nerfstudio_dir / "transforms.json", "w", encoding="utf-8") as f:
         json.dump(transforms, f, indent=4)
 
+    # points
+    torch.save(points, output_folder / "nerfstudio" / "points/points.pt")
+    torch.save(points_mask, output_folder / "nerfstudio" / "points/points_mask.pt")
+
+    # mesh points
+    torch.save(meshes_points_dict, output_folder / "nerfstudio" / "meshes/meshes_points.pt")
+    torch.save(warped_meshes_points_dict, output_folder / "nerfstudio" / "meshes/warped_meshes_points.pt")
+    torch.save(frame_meshes.simplices_list, output_folder / "nerfstudio" / "meshes/simplices.pt")
+
     # images
     for i, img in enumerate(images):
-        mediapy.write_image(nerfstudio_images_dir / f"{i:05}.png", img.cpu().numpy())
+        mediapy.write_image(nerfstudio_images_dir / f"{i:05}.png", warped_images[i].cpu().numpy())
 
     # depths
     for i in range(n):
-        np.save(nerfstudio_depths_dir / f"{i:05d}", depths[i][..., None].cpu().detach().numpy())
+        np.save(nerfstudio_depths_dir / f"{i:05d}", warped_depths[i][..., None].cpu().detach().numpy())
 
     # masks
     for i in range(n):
-        mediapy.write_image(nerfstudio_masks_dir / f"{i:05}.png", masks[i])
+        mediapy.write_image(nerfstudio_masks_dir / f"{i:05}.png", warped_masks[i])
 
-    # points
-    torch.save(points, output_folder / "nerfstudio" / "points/points.pt")
-    torch.save(points_mask, output_folder / "nerfstudio" / "points/points_mask.pt")
+    # camera params and szs/dzs
+    camera_params_dir = output_folder / "camera_params"
+    output_cameras_dir = Path(camera_params_dir / "cameras")
+    output_szs_dir = Path(camera_params_dir / "szs")
+    output_dzs_dir = Path(camera_params_dir / "dzs")
+
+    camera_params_dir.mkdir(parents=True)
+    output_cameras_dir.mkdir(parents=True)
+    output_szs_dir.mkdir(parents=True)
+    output_dzs_dir.mkdir(parents=True)
 
-    # mesh points
-    torch.save(meshes_points_dict, output_folder / "nerfstudio" / "meshes/meshes_points.pt")
-    torch.save(warped_meshes_points_dict, output_folder / "nerfstudio" / "meshes/warped_meshes_points.pt")
-    torch.save(simplices_list, output_folder / "nerfstudio" / "meshes/simplices.pt")
+    torch.save(coarse_cameras.state_dict(), output_cameras_dir / "coarse_cameras.pt")
+    torch.save(refined_cameras.state_dict(), output_cameras_dir / "refined_cameras.pt")
 
+    torch.save(szs, output_szs_dir / "szs.pt")
+    torch.save(szs_warp, output_szs_dir / "szs_warp.pt")
 
-    #######################
-    ###### make plys ######
-    #######################
+    torch.save(dzs, output_dzs_dir / "dzs.pt")
+    torch.save(dzs_warp, output_dzs_dir / "dzs_warp.pt")
 
+    
     # coarse
     valid_points_3d = [mask[::ply_downscale_factor, ::ply_downscale_factor].T.flatten() != 0 for mask in masks]
-    
     coarse_dense_points_3d = make_dense_points_3d(coarse_cameras, depths, ply_downscale_factor)
     coarse_dense_points_3d = [coarse_dense_points_3d[ndx][valid_points_3d[ndx]] for ndx in range(n)]
-    
     images_colors = [image.permute(1, 0, 2)[::ply_downscale_factor, ::ply_downscale_factor].cpu().flatten(0, 1) for image in images]
     images_colors = [images_colors[ndx][valid_points_3d[ndx]] for ndx in range(n)]
 
     # refined
-    warped_valid_points_3d = [mask[::ply_downscale_factor, ::ply_downscale_factor].T.flatten() != 0 for mask in warped_masks]
-
+    warped_valid_points_3d = [mask[::ply_downscale_factor, ::ply_downscale_factor].T.flatten() > 0.1 for mask in warped_masks]
+    warped_dense_points_3d = make_dense_points_3d(refined_cameras, warped_depths, ply_downscale_factor)
+    warped_dense_points_3d = [warped_dense_points_3d[ndx][warped_valid_points_3d[ndx]] for ndx in range(n)]
     warped_images_colors = [image.permute(1, 0, 2)[::ply_downscale_factor, ::ply_downscale_factor].cpu().flatten(0, 1) for image in warped_images]
     warped_images_colors = [warped_images_colors[ndx][warped_valid_points_3d[ndx]] for ndx in range(n)]
     
-    warped_dense_points_3d = make_dense_points_3d(refined_cameras, warped_depths, ply_downscale_factor)
-    warped_dense_points_3d = [warped_dense_points_3d[ndx][warped_valid_points_3d[ndx]] for ndx in range(n)] 
-
-
-    plys = make_plys(warped_images_colors, warped_dense_points_3d)
-
-    for i, ply in enumerate(plys):
-        with open(output_folder / "nerfstudio" / "plys" / f"{i:05d}.ply", "w") as f:
-            f.write(ply)
-
-    # make a point cloud ply with all the plys combined ...
-    with open(output_folder / "nerfstudio" / "plys" / "all.ply", "w") as f:
-        f.write("ply\n")
-        f.write("format ascii 1.0\n")
-        f.write(f"element vertex {sum([len(ply.splitlines()) - 14 for ply in plys])}\n")
-        f.write("property float x\n")
-        f.write("property float y\n")
-        f.write("property float z\n")
-        f.write("property uint8 red\n")
-        f.write("property uint8 green\n")
-        f.write("property uint8 blue\n")
-        f.write("end_header\n")
-
-        for ply in plys:
-            for line in ply.splitlines()[14:]:
-                f.write(line + "\n")
-
-    # remove folder if exists
-    if (nerfstudio_folder / dataset).exists():
-        shutil.rmtree(nerfstudio_folder / dataset)
-    shutil.copytree(output_folder / "nerfstudio", nerfstudio_folder / dataset)
-
-    if view_point_cloud:
-
-        mesh_verts_list = []
-        warped_mesh_verts_list = []
-
-        coarse_sparse_points_3d = []
-        refined_sparse_points_3d = []
 
-        for ndx in range(n):
-            original_mesh_points = original_mesh_points_list[ndx]
-            warped_mesh_points = warped_mesh_points_list[ndx]
-            simplices = simplices_list[ndx]
+    # verts and sparse points
+    mesh_verts_list = []
+    warped_mesh_verts_list = []
 
-            mesh_us = original_mesh_points[...,0].int()
-            mesh_vs = original_mesh_points[...,1].int()
+    coarse_corrs_3d = []
+    refined_corrs_3d = []
 
-            mesh_us_normed = mesh_us / (widths[ndx] - 1) * 2 - 1
-            mesh_vs_normed = mesh_vs / (heights[ndx] - 1) * 2 - 1
-
-            mesh_zs = mesh_zs_list[ndx] * szs[ndx] + dzs[ndx]
+    for ndx in range(n):
+        us = frame_meshes.points_list[ndx][...,0]
+        vs = frame_meshes.points_list[ndx][...,1]
+        us_normed = us / (widths[ndx] - 1) * 2 - 1
+        vs_normed = vs / (heights[ndx] - 1) * 2 - 1
+        zs = frame_meshes.zs_list[ndx] * szs[ndx] + dzs[ndx]
+        points_3d = coarse_cameras(us_normed, vs_normed, zs)[ndx]
+
+        mesh_verts_list.append(points_3d)
+        coarse_corrs_3d.append(points_3d[:frame_meshes.num_corrs_per_mesh[ndx]])
+
+        warped_us = frame_meshes.warped_points_list[ndx][...,0]
+        warped_vs = frame_meshes.warped_points_list[ndx][...,1]
+        warped_us_normed = warped_us / (widths[ndx] - 1) * 2 - 1
+        warped_vs_normed = warped_vs / (heights[ndx] - 1) * 2 - 1
+        warped_zs = frame_meshes.warped_zs_list[ndx] * szs_warp[ndx] + dzs_warp[ndx]
+        warped_points_3d = refined_cameras(warped_us_normed, warped_vs_normed, warped_zs)[ndx]
+
+        warped_mesh_verts_list.append(warped_points_3d)
+        refined_corrs_3d.append(warped_points_3d[:frame_meshes.num_corrs_per_mesh[ndx]])
+
+
+    visuals_3d_dir = output_folder / "visuals_3d"
+    output_verts_dir = visuals_3d_dir / "verts"
+    output_corrs_dir = visuals_3d_dir / "corrs"
+    output_dense_points_dir = visuals_3d_dir / "dense_points"
+    output_img_colors_dir = visuals_3d_dir / "img_colors"
+
+    visuals_3d_dir.mkdir(parents=True, exist_ok=True)
+    output_corrs_dir.mkdir(parents=True, exist_ok=True)
+    output_verts_dir.mkdir(parents=True, exist_ok=True)
+    output_dense_points_dir.mkdir(parents=True, exist_ok=True)
+    output_img_colors_dir.mkdir(parents=True, exist_ok=True)
 
-            warped_mesh_us = warped_mesh_points[..., 0].int().clamp(0, widths[ndx] - 1)
-            warped_mesh_vs = warped_mesh_points[..., 1].int().clamp(0, heights[ndx] - 1)
+    torch.save(mesh_verts_list, output_verts_dir / "verts.pt")
+    torch.save(warped_mesh_verts_list, output_verts_dir / "warped_verts.pt")
 
-            warped_mesh_us_normed = warped_mesh_us / (widths[ndx] - 1) * 2 - 1
-            warped_mesh_vs_normed = warped_mesh_vs / (heights[ndx] - 1) * 2 - 1
+    torch.save(coarse_corrs_3d, output_corrs_dir / "corrs.pt")
+    torch.save(refined_corrs_3d, output_corrs_dir / "warped_corrs.pt")
+    
+    torch.save(coarse_dense_points_3d, output_dense_points_dir / "dense_points.pt")
+    torch.save(warped_dense_points_3d, output_dense_points_dir / "warped_dense_points.pt")
 
-            corr_pzs = pzs[ndx][points_mask[ndx]].detach() # stop gradient
-            vert_pzs = vert_pzs_list[ndx]
+    torch.save(images_colors, output_img_colors_dir / "img_colors.pt")
+    torch.save(warped_images_colors, output_img_colors_dir / "warped_img_colors.pt")
 
-            mesh_pzs = torch.cat([corr_pzs, vert_pzs])
-            warped_mesh_zs = mesh_zs + (mesh_pzs * szs[ndx])
+    if mask_random_points_indices is not None:
+        # #############################
+        # ###### compute metrics ######
+        # #############################
+        with torch.no_grad():
+            warped_us = frame_meshes.warped_corr_points_padded[...,0]
+            warped_vs = frame_meshes.warped_corr_points_padded[...,1]
 
-            mesh_verts = coarse_cameras(mesh_us_normed[None], mesh_vs_normed[None], mesh_zs[None])[ndx]
-            mesh_verts_list.append(mesh_verts)
-            coarse_sparse_points_3d.append(mesh_verts[:num_corrs_per_mesh[ndx]])
+            warped_us_normed = warped_us / (widths[..., None] - 1) * 2 - 1
+            warped_vs_normed = warped_vs / (heights[..., None] - 1) * 2 - 1
+            warped_zs = frame_meshes.warped_corr_zs_padded * szs_warp[...,None] + dzs_warp[...,None]
+
+            points_3d = refined_cameras(warped_us_normed, warped_vs_normed, warped_zs)
+            paired_points = points_3d[pairs][:, :, mask_random_points_indices]
+            loss_3d = torch.mean((paired_points[0] - paired_points[1]) ** 2)
+            metrics = {"3D": loss_3d.item(), "mask_random_points_indices": mask_random_points_indices.tolist()}
+            with open(output_folder / "metrics.json", "w", encoding="utf-8") as f:
+                json.dump(metrics, f, indent=4)
+        CONSOLE.print(f"[bold green] Metrics: {metrics}")
+    else:
+        metrics = None
+
+
+    if save_geometry:
+        # #######################
+        # ###### make plys ######
+        # #######################
+        CONSOLE.print("[bold green] Writing objs and plys")
+
+        # create plys (point clouds)
+        plys = make_plys(warped_images_colors, warped_dense_points_3d)
+        for i, ply in enumerate(plys):
+            with open(output_folder / "nerfstudio" / "plys" / f"{i:05d}.ply", "w") as f:
+                f.write(ply)
+
+        # make a point cloud ply with all the plys combined ...
+        with open(output_folder / "nerfstudio" / "plys" / "all.ply", "w") as f:
+            f.write("ply\n")
+            f.write("format ascii 1.0\n")
+            f.write(f"element vertex {sum([len(ply.splitlines()) - 14 for ply in plys])}\n")
+            f.write("property float x\n")
+            f.write("property float y\n")
+            f.write("property float z\n")
+            f.write("property uint8 red\n")
+            f.write("property uint8 green\n")
+            f.write("property uint8 blue\n")
+            f.write("end_header\n")
+
+            for ply in plys:
+                for line in ply.splitlines()[14:]:
+                    f.write(line + "\n")
+
+        # TODO: move a lot of this code to functions
+        # create objs (meshes, i.e., connected point clouds)
+        obj_colors = [image.permute(1, 0, 2).cpu() for image in images]
+        obj_points = make_dense_points_3d_no_flatten(refined_cameras, warped_depths)
+        obj_all_vertices = []
+        obj_all_vertex_colors = []
+        obj_all_faces = []
+        all_vertices_count = 0
+        for i in range(len(obj_points)):
+            temp_masks = torch.from_numpy(masks[i]).permute(1, 0)[None]
+            temp_images = obj_colors[i].permute(2, 0, 1)[None]
+            temp_vertices = obj_points[i].permute(2, 0, 1)[None].cpu()
+            temp_masks = temp_masks[..., ::ply_downscale_factor, ::ply_downscale_factor]
+            temp_images = temp_images[..., ::ply_downscale_factor, ::ply_downscale_factor]
+            temp_vertices = temp_vertices[..., ::ply_downscale_factor, ::ply_downscale_factor]
+            vertices, vertex_colors, faces, faces_mask = get_mesh(images=temp_images, vertices=temp_vertices, masks=temp_masks, distance_threshold=0.5)
+            faces = faces[faces_mask] # remove faces that are masked out
+            save_mesh(vertices, vertex_colors, faces, filename=str(output_folder / "nerfstudio" / "objs" / f"{i:05d}.obj"))
+            obj_all_vertices.append(vertices)
+            obj_all_vertex_colors.append(vertex_colors)
+            obj_all_faces.append(faces + all_vertices_count)
+            all_vertices_count += vertices.shape[0]
+        obj_all_vertices = torch.cat(obj_all_vertices)
+        obj_all_vertex_colors = torch.cat(obj_all_vertex_colors)
+        obj_all_faces = torch.cat(obj_all_faces)
+        save_mesh(obj_all_vertices, obj_all_vertex_colors, obj_all_faces, filename=str(output_folder / "nerfstudio" / "objs" / "all.obj"))
+
+    if write_to_nerfstudio:
+        # remove folder if exists
+        if nerfstudio_folder:
+            if (nerfstudio_folder / dataset).exists():
+                shutil.rmtree(nerfstudio_folder / dataset)
+            shutil.copytree(output_folder / "nerfstudio", nerfstudio_folder / dataset)
 
-            warped_mesh_verts = coarse_cameras(warped_mesh_us_normed[None], warped_mesh_vs_normed[None], warped_mesh_zs[None])[ndx]
-            warped_mesh_verts_list.append(warped_mesh_verts)
-            refined_sparse_points_3d.append(warped_mesh_verts[:num_corrs_per_mesh[ndx]])
+    if view_point_cloud:
 
         sparse_point_colors = [point_colors[points_mask[ndx]] for ndx in range(n)]
         mesh_colors = [np.random.rand(3) for _ in range(n)]
         
-        server = viser.ViserServer()
+        server = viser.ViserServer(request_share_url=True, port=port)
 
-        view_pcs_cameras(server, 
-                         images, # cameras
-                         coarse_cameras,
-                         coarse_dense_points_3d, # dense pc
-                         images_colors, 
-                         coarse_sparse_points_3d, # sparse pc
-                         sparse_point_colors,
-                         mesh_verts_list, # mesh
-                         simplices_list,
-                         mesh_colors,
-                         prefix="coarse")
+        # view_pcs_cameras(server, 
+        #                  images, # cameras
+        #                  coarse_cameras,
+        #                  coarse_dense_points_3d, # dense pc
+        #                  images_colors, 
+        #                  coarse_corrs_3d, # sparse pc
+        #                  sparse_point_colors,
+        #                  mesh_verts_list, # mesh
+        #                  frame_meshes.simplices_list,
+        #                  mesh_colors,
+        #                  prefix="coarse")
         
         view_pcs_cameras(server, 
                          warped_images, # cameras
                          refined_cameras,
                          warped_dense_points_3d, # dense pc
                          warped_images_colors, 
-                         refined_sparse_points_3d, # sparse pc
+                         refined_corrs_3d, # sparse pc
                          sparse_point_colors,
                          warped_mesh_verts_list, # mesh
-                         simplices_list,
+                         frame_meshes.simplices_list,
                          mesh_colors,
                          prefix="refined")
         
         # import pdb; pdb.set_trace()
         while True:
             pass
 
+    return metrics
+
 
 def entrypoint():
     """Entrypoint for use with pyproject scripts."""
     tyro.extras.set_accent_color("bright_yellow")
     tyro.cli(main)
```

### Comparing `toon3d-0.0.1/toon3d-current/scripts/server.py` & `toon3d-0.0.2/toon3d/scripts/server.py`

 * *Files identical despite different names*

### Comparing `toon3d-0.0.1/toon3d-current/tooned_config.py` & `toon3d-0.0.2/toon3d/toon3d_config.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,70 +7,68 @@
 from nerfstudio.configs.base_config import ViewerConfig
 
 from nerfstudio.engine.optimizers import AdamOptimizerConfig
 from nerfstudio.engine.schedulers import (
     ExponentialDecaySchedulerConfig,
 )
 from nerfstudio.engine.trainer import TrainerConfig
-from toon3d.toon3d_model import toon3dModelConfig
-from toon3d.toon3d_pipeline import toon3dPipelineConfig
-from toon3d.toon3d_datamanager import toon3dDataManagerConfig
-from toon3d.toon3d_dataparser import toon3dDataParserConfig
+from toon3d.toon3d_model import Toon3DModelConfig
+from toon3d.toon3d_pipeline import Toon3DPipelineConfig
+from toon3d.toon3d_datamanager import Toon3DDataManagerConfig
+from toon3d.toon3d_dataparser import Toon3DDataParserConfig
 
 from nerfstudio.plugins.types import MethodSpecification
 
 toon3d_config = MethodSpecification(
     TrainerConfig(
         method_name="toon3d",
-        steps_per_eval_image=100,
-        steps_per_eval_batch=100,
-        steps_per_save=2000,
+        steps_per_eval_image=100000,
+        steps_per_eval_batch=100000,
         steps_per_eval_all_images=100000,
-        max_num_iterations=30000,
+        steps_per_save=500,
+        max_num_iterations=2000,
         mixed_precision=False,
         gradient_accumulation_steps={"camera_opt": 100},
-        pipeline=toon3dPipelineConfig(
-            datamanager=toon3dDataManagerConfig(
-                dataparser=toon3dDataParserConfig(eval_mode="all", load_3D_points=True, depth_unit_scale_factor=1.0)
+        pipeline=Toon3DPipelineConfig(
+            datamanager=Toon3DDataManagerConfig(
+                dataparser=Toon3DDataParserConfig(eval_mode="all", load_3D_points=True, depth_unit_scale_factor=1.0)
             ),
-            model=toon3dModelConfig(
-                warmup_length=0,
-                sh_degree=0,
-                num_downscales=0,
-                use_scale_regularization=True,
-                max_gauss_ratio=1.0,
-                scale_reg_mult=10.0,
+            model=Toon3DModelConfig(
+                # sh_degree=0,
+                # warmup_length=0,
+                # cull_scale_thresh=0.1,
+                sh_degree_interval=1,
                 output_depth_during_training=True,
             ),
         ),
         optimizers={
-            "xyz": {
+            "means": {
                 "optimizer": AdamOptimizerConfig(lr=1.6e-4, eps=1e-15),
                 "scheduler": ExponentialDecaySchedulerConfig(
                     lr_final=1.6e-6,
                     max_steps=30000,
                 ),
             },
             "features_dc": {
                 "optimizer": AdamOptimizerConfig(lr=0.0025, eps=1e-15),
                 "scheduler": None,
             },
             "features_rest": {
                 "optimizer": AdamOptimizerConfig(lr=0.0025 / 20, eps=1e-15),
                 "scheduler": None,
             },
-            "opacity": {
+            "opacities": {
                 "optimizer": AdamOptimizerConfig(lr=0.05, eps=1e-15),
                 "scheduler": None,
             },
-            "scaling": {
+            "scales": {
                 "optimizer": AdamOptimizerConfig(lr=0.005, eps=1e-15),
                 "scheduler": None,
             },
-            "rotation": {"optimizer": AdamOptimizerConfig(lr=0.001, eps=1e-15), "scheduler": None},
+            "quats": {"optimizer": AdamOptimizerConfig(lr=0.001, eps=1e-15), "scheduler": None},
             "camera_opt": {
                 "optimizer": AdamOptimizerConfig(lr=1e-3, eps=1e-15),
                 "scheduler": ExponentialDecaySchedulerConfig(lr_final=5e-5, max_steps=30000),
             },
         },
         viewer=ViewerConfig(num_rays_per_chunk=1 << 15, camera_frustum_scale=0.5, default_composite_depth=False),
         vis="viewer",
```

### Comparing `toon3d-0.0.1/toon3d-current/tooned_datamanager.py` & `toon3d-0.0.2/toon3d/toon3d_datamanager.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,39 +12,39 @@
 import mediapy
 from toon3d.color_palette import color_cluster_kmeans
 from kornia.color import rgb_to_lab, lab_to_rgb, rgb_to_hsv, hsv_to_rgb
 from nerfstudio.data.datasets.depth_dataset import DepthDataset
 
 
 @dataclass
-class toon3dDataManagerConfig(FullImageDatamanagerConfig):
-    """toon3d DataManager Config
+class Toon3DDataManagerConfig(FullImageDatamanagerConfig):
+    """Toon3D DataManager Config
 
     Add your custom datamanager config parameters here.
     """
 
     # color palette parameters
     use_color_palette: bool = False
     palette_type: str = "hsv_kmeans"
     color_palette_downscale: float = 1
     num_colors: int = 8
 
-    _target: Type = field(default_factory=lambda: toon3dDataManager)
+    _target: Type = field(default_factory=lambda: Toon3DDataManager)
 
 
-class toon3dDataManager(FullImageDatamanager[DepthDataset]):
-    """toon3d DataManager
+class Toon3DDataManager(FullImageDatamanager[DepthDataset]):
+    """Toon3D DataManager
 
     Args:
-        config: the toon3dDataManager used to instantiate class
+        config: the Toon3DDataManager used to instantiate class
     """
 
-    config: toon3dDataManagerConfig
+    config: Toon3DDataManagerConfig
 
-    def __init__(self, config: toon3dDataManagerConfig, **kwargs):
+    def __init__(self, config: Toon3DDataManagerConfig, **kwargs):
         self.color_palette = None
         super().__init__(config)
 
     def setup_train(self):
         """Setup the train dataloader."""
         self.device = "cuda:0"
```

### Comparing `toon3d-0.0.1/toon3d-current/tooned_dataparser.py` & `toon3d-0.0.2/toon3d/toon3d_dataparser.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,26 +22,26 @@
 import torch
 
 from nerfstudio.data.dataparsers.nerfstudio_dataparser import Nerfstudio, NerfstudioDataParserConfig
 from nerfstudio.utils.io import load_from_json
 
 
 @dataclass
-class toon3dDataParserConfig(NerfstudioDataParserConfig):
-    """toon3d dataset config"""
+class Toon3DDataParserConfig(NerfstudioDataParserConfig):
+    """Toon3D dataset config"""
 
-    _target: Type = field(default_factory=lambda: toon3d)
+    _target: Type = field(default_factory=lambda: Toon3D)
     """target class to instantiate"""
 
 
 @dataclass
-class toon3d(Nerfstudio):
-    """toon3d DatasetParser"""
+class Toon3D(Nerfstudio):
+    """Toon3D DatasetParser"""
 
-    config: toon3dDataParserConfig
+    config: Toon3DDataParserConfig
 
     def _generate_dataparser_outputs(self, split="train"):
         dataparser_outputs = super()._generate_dataparser_outputs(split=split)
 
         if self.config.data.suffix == ".json":
             meta = load_from_json(self.config.data)
             data_dir = self.config.data.parent
```

### Comparing `toon3d-0.0.1/toon3d-current/tooned_model.py` & `toon3d-0.0.2/toon3d/toon3d_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-toon3d model.
+Toon3D model.
 """
 
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 from typing import Dict, List, Type
 import torch
@@ -47,24 +47,27 @@
 from nerfstudio.utils.colormaps import apply_depth_colormap
 
 from toon3d.generative.ldm3d import LDM3D
 import mediapy
 from toon3d.configs.prompts import get_prompts
 from toon3d.utils.novel_view_samplers import sample_interpolated_camera
 from toon3d.utils.depth_utils import depth_to_disparity
+from pytorch3d.loss.chamfer import chamfer_distance
+from nerfstudio.viewer.viewer_elements import ViewerControl
+from nerfstudio.viewer.viewer import VISER_NERFSTUDIO_SCALE_RATIO
 
 
 @dataclass
-class toon3dModelConfig(SplatfactoModelConfig):
+class Toon3DModelConfig(SplatfactoModelConfig):
     """Config for the toon3d model."""
 
-    _target: Type = field(default_factory=lambda: toon3dModel)
+    _target: Type = field(default_factory=lambda: Toon3DModel)
 
     # warp parameters
-    warp_images: bool = True
+    warp_images: bool = False
     """Warp input images"""
 
     # color palette parameters
     use_color_palette: bool = False
     """Whether to use the color palette for the toon3d model."""
     color_palette_project_before_render: bool = False
     """Whether to project nd dim with the color palette before rendering."""
@@ -72,17 +75,17 @@
     """Whether to use the color palette as the rgb output of the model."""
     color_palette_mult: float = 1.0
     """Multiplier for the color palette loss, when using it as a regularizer (not rgb)."""
     color_palette_rend_consistency_mult: float = 1.0
     """Multiplier for the color palette rendered consistency loss, when using it as a regularizer (not rgb)."""
 
     # depth regularization parameters
-    use_tv_loss: bool = False
+    use_tv_loss: bool = True
     """Whether to use the total variation loss."""
-    tv_loss_mult: float = 1.0
+    tv_loss_mult: float = 100.0
     """Multiplier for the total variation loss."""
     tv_loss_strides: List[int] = field(default_factory=lambda: [1])
     """Downscale strides to use for the total variation loss."""
     use_tv_in_novel_views: bool = True
     """Whether to use the total variation loss in novel views."""
     tv_in_novel_views_loss_mult: float = 100.0
     """Multiplier for the total variation loss in novel views."""
@@ -113,33 +116,50 @@
     sds_guidance_scale: float = 10.0
     """Guidance scale for sds loss."""
     sds_dataset: Optional[str] = None
     """Dataset for sds model."""
     sds_lora_weights_path: Optional[str] = None
     """Path to the lora weights for sds model."""
 
-    # scale regularization parameters
-    scale_reg_mult: float = 0.1
-    """Multiplier for the scale regularization loss."""
+    use_chamfer_loss: bool = False
+    """Whether to use the chamfer loss."""
+    chamfer_loss_mult: float = 1.0
+    """Multiplier for the chamfer loss."""
+    chamfer_loss_num_points: int = 10000
+    """Number of points to use for the chamfer loss."""
+
+    use_isotropic_loss: bool = False
+    """Whether to use the isotropic loss."""
+    isotropic_ratio_mult: float = 1e6
+    """Multiplier for the isotropic ratio loss."""
+
+    use_ratio_loss: bool = True
+    """Whether to use the ratio loss."""
+    ratio_loss_mult: float = 1e6
+    """Multiplier for the ratio loss."""
+    max_ratio_ratio: float = 10.0
+    """threshold of ratio of gaussian max to min scale before applying regularization
+    loss from the PhysGaussian paper
+    """
 
-
-class toon3dModel(SplatfactoModel):
+class Toon3DModel(SplatfactoModel):
     """Model for toon3d."""
 
-    config: toon3dModelConfig
+    config: Toon3DModelConfig
 
     def __init__(self, *args, **kwargs):
         self.color_palette = kwargs["color_palette"]
         self.images = kwargs["images"]
         self.points = kwargs["points"]
         self.points_mask = kwargs["points_mask"]
         self.mesh_points = kwargs["mesh_points"]
         self.warped_mesh_points = kwargs["warped_mesh_points"]
         self.simplices_list = kwargs["simplices"]
         self.cameras = kwargs["cameras"]
+        self.points3D_xyz = kwargs["points3D_xyz"]
         self.devic = kwargs["device"] # would be device but otherwise get a AttributeError: can't set attribute
         super().__init__(*args, **kwargs)
 
     def populate_modules(self):
         """Required for our custom models."""
 
         # modify the config for nd attributes
@@ -303,18 +323,19 @@
                     rgbd,
                     guidance_scale=self.config.sds_guidance_scale,
                 )
                 loss_dict["sds"] = sds_loss.to(self.device)
             if self.config.use_tv_in_novel_views:
                 pred_depth = outputs["depth"]
                 for stride in self.config.tv_in_novel_views_loss_strides:
-                    loss_dict[f"depth_tv_in_novel_views_loss_stride-{stride}"] = (
-                        self.config.tv_in_novel_views_loss_mult
-                        * tv_loss(pred_depth.permute(2, 0, 1)[None, :, ::stride, ::stride])
-                    )
+                    l = self.config.tv_in_novel_views_loss_mult * tv_loss(pred_depth.permute(2, 0, 1)[None, :, ::stride, ::stride])
+                    if l > 0:
+                        loss_dict[f"depth_tv_in_novel_views_loss_stride-{stride}"] = l
+            # hack to avoid having no gradients for backprop
+            loss_dict["hack"] = (self.xys * 0).sum()
             return loss_dict
 
         # dense warp for image
         image_idx = batch["image_idx"]
         image = batch["image"] # (height, width, 3)
         mask = batch["mask"].to(image.device)[..., 0] # (height, width)
         depth = batch["depth_image"] # (height, width, 1)
@@ -384,20 +405,29 @@
             )
 
         if self.config.use_depth_loss:
             pred_depth = outputs["depth"]
             gt_depth = depth.to(pred_depth.device)
             loss_dict["depth_loss"] = self.config.depth_loss_mult * torch.abs(pred_depth[mask] - gt_depth[mask]).mean()
 
-        if self.config.use_scale_regularization and self.step % 10 == 0:
+        if self.config.use_chamfer_loss:
+            indices = torch.randperm(self.points3D_xyz.shape[0])[:self.config.chamfer_loss_num_points]
+            points3D_xyz = self.points3D_xyz[indices].to(self.means.device)
+            chamfer_loss = chamfer_distance(self.means[None], points3D_xyz[None], single_directional=True)[0]
+            loss_dict["chamfer_loss"] = self.config.chamfer_loss_mult * chamfer_loss
+
+        if self.config.use_isotropic_loss:
+            scale_var = torch.mean(torch.var(self.scales, dim=1))
+            loss_dict["isotropic_loss"] = self.config.isotropic_ratio_mult * scale_var
+
+        if self.config.use_ratio_loss:
             scale_exp = torch.exp(self.scales)
             scale_reg = (
                 torch.maximum(
                     scale_exp.amax(dim=-1) / scale_exp.amin(dim=-1),
-                    torch.tensor(self.config.max_gauss_ratio),
+                    torch.tensor(self.config.max_ratio_ratio),
                 )
-                - self.config.max_gauss_ratio
+                - self.config.max_ratio_ratio
             )
-            scale_reg = self.config.scale_reg_mult * scale_reg.mean()
-            loss_dict["scale_reg"] = scale_reg
+            scale_reg = self.config.ratio_loss_mult * scale_reg.mean()
 
         return loss_dict
```

### Comparing `toon3d-0.0.1/toon3d-current/tooned_pipeline.py` & `toon3d-0.0.2/toon3d/toon3d_pipeline.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,43 +8,45 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""toon3d pipeline."""
+"""Toon3D pipeline."""
 
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 from typing import Optional, Type
 import torch
 from torch.cuda.amp.grad_scaler import GradScaler
 from typing_extensions import Literal
 from nerfstudio.pipelines.base_pipeline import VanillaPipeline, VanillaPipelineConfig
-from toon3d.toon3d_model import toon3dModelConfig
+from toon3d.toon3d_model import Toon3DModelConfig
+from toon3d.utils.tsdf_utils import export_tsdf_mesh
+from pathlib import Path
 
 
 @dataclass
-class toon3dPipelineConfig(VanillaPipelineConfig):
+class Toon3DPipelineConfig(VanillaPipelineConfig):
     """Configuration for pipeline instantiation"""
 
-    _target: Type = field(default_factory=lambda: toon3dPipeline)
+    _target: Type = field(default_factory=lambda: Toon3DPipeline)
     """target class to instantiate"""
 
 
-class toon3dPipeline(VanillaPipeline):
+class Toon3DPipeline(VanillaPipeline):
     """InstructNeRF2NeRF pipeline"""
 
-    config: toon3dPipelineConfig
+    config: Toon3DPipelineConfig
 
     def __init__(
         self,
-        config: toon3dPipelineConfig,
+        config: Toon3DPipelineConfig,
         device: str,
         test_mode: Literal["test", "val", "inference"] = "val",
         world_size: int = 1,
         local_rank: int = 0,
         grad_scaler: Optional[GradScaler] = None,
     ):
         super(VanillaPipeline, self).__init__()
@@ -69,24 +71,42 @@
             pts = self.datamanager.train_dataparser_outputs.metadata["points3D_xyz"]
             pts_rgb = self.datamanager.train_dataparser_outputs.metadata["points3D_rgb"]
             seed_pts = (pts, pts_rgb)
         self.datamanager.to(device)
         # TODO(ethan): get rid of scene_bounds from the model
         assert self.datamanager.train_dataset is not None, "Missing input dataset"
 
-        assert isinstance(config.model, toon3dModelConfig), "Model config must be toon3dModelConfg"
+        assert isinstance(config.model, Toon3DModelConfig), "Model config must be Toon3DModelConfg"
 
         color_palette = self.datamanager.color_palette
         images = [self.datamanager.cached_train[i]["image"] for i in range(len(self.datamanager.cached_train))]
         points = self.datamanager.train_dataparser_outputs.metadata["points"]
         points_mask = self.datamanager.train_dataparser_outputs.metadata["points_mask"]
         mesh_points = self.datamanager.train_dataparser_outputs.metadata["mesh_points"]
         warped_mesh_points = self.datamanager.train_dataparser_outputs.metadata["warped_mesh_points"]
         simplices = self.datamanager.train_dataparser_outputs.metadata["simplices"]
         cameras = self.datamanager.train_dataparser_outputs.cameras
+        points3D_xyz = self.datamanager.train_dataparser_outputs.metadata["points3D_xyz"]
+
+        # compute the TSDF
+        # depth_images = [self.datamanager.cached_train[i]["depth_image"] for i in range(len(self.datamanager.cached_train))]
+        # color_images = [self.datamanager.cached_train[i]["image"] for i in range(len(self.datamanager.cached_train))]
+        # res = 512
+        # scale = 2.0
+        # bounding_box_min = (-scale, -scale, -scale)
+        # bounding_box_max = (scale, scale, scale)
+        # tsdf = export_tsdf_mesh(
+        #     cameras=cameras,
+        #     depth_images=depth_images,
+        #     color_images=color_images,
+        #     output_dir=Path('.'),
+        #     device=device,
+        #     resolution=[res, res, res],
+        #     bounding_box_min=bounding_box_min,
+        #     bounding_box_max=bounding_box_max)
 
         # import pdb; pdb.set_trace();
         self._model = config.model.setup(
             scene_box=self.datamanager.train_dataset.scene_box,
             num_train_data=len(self.datamanager.train_dataset),
             metadata=self.datamanager.train_dataset.metadata,
             device=device,
@@ -96,14 +116,15 @@
             images=images,
             points=points,
             points_mask=points_mask,
             mesh_points=mesh_points,
             warped_mesh_points=warped_mesh_points,
             simplices=simplices,
             cameras=cameras,
+            points3D_xyz=points3D_xyz,
         )
         self.model.to(device)
         if self.model.config.use_sds:
             # TODO(ethan): this is hacky and should be fixed
             self.model.diffusion_model.to(self.model.config.sds_device)
 
         self.world_size = world_size
```

### Comparing `toon3d-0.0.1/toon3d-current/utils/camera_utils.py` & `toon3d-0.0.2/toon3d/utils/camera_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -24,15 +24,16 @@
         if ts is None: ts = torch.zeros([self.n, 3], dtype=torch.float32)
 
         self.quats = nn.Parameter(quats)
         self.ts = nn.Parameter(ts)
         
     @property
     def Rs(self):
-        qr, qi, qj, qk = self.quats.split(1, -1)
+        quats = self.quats / torch.norm(self.quats, dim=1)[...,None]
+        qr, qi, qj, qk = quats.split(1, -1)
 
         Rs = (
             torch.stack(
                 [
                     torch.stack([0.5 - (qj**2 + qk**2), (qi * qj) - (qr * qk), (qi * qk) + (qr * qj)], -1),
                     torch.stack([(qi * qj) + (qr * qk), 0.5 - (qi**2 + qk**2), (qj * qk) - (qr * qi)], -1),
                     torch.stack([(qi * qk) - (qr * qj), (qj * qk) + (qr * qi), 0.5 - (qi**2 + qj**2)], -1),
@@ -40,33 +41,53 @@
                 -1,
             ).mT
             * 2
         )
 
         return Rs.squeeze(1)
 
-    def forward(self, us, vs, zs):
+    def forward(self, us, vs, zs, ndx=None):
         """
         us (batch, num_pts)
         vs (batch, num_pts)
         zs (batch, num_pts)
 
         returns points_3d (batch, num_points, 3)
         """
-        points_backprojected = self.backproject(us, vs, zs).permute(0, 2, 1) # (batch, 3, num_points)
-        points_3d = (self.Rs @ points_backprojected) + self.ts[...,None]  # (batch, 3, num_points)
+        if ndx is None:
+            points_backprojected = self.backproject(us, vs, zs).permute(0, 2, 1) # (batch, 3, num_points)
+            points_3d = (self.Rs @ points_backprojected) + self.ts[...,None]  # (batch, 3, num_points)
+            points_3d = points_3d.permute(0, 2, 1)  # (batch, num_points, 3)
+        
+        else:
+            points_backprojected = self.backproject(us, vs, zs, ndx).permute(1, 0) # (3, num_points)
+            points_3d = (self.Rs[ndx] @ points_backprojected) + self.ts[ndx,...,None]  # (3, num_points)
+            points_3d =  points_3d.permute(1, 0) # (num_points, 3)
+
+        return points_3d
 
-        return points_3d.permute(0, 2, 1)  # (batch, num_points, 3)
-    
-    def backproject(self, us, vs, zs):
+    def backproject(self, us, vs, zs, ndx=None):
         """
         us (batch, num_pts)
         vs (batch, num_pts)
         zs (batch, num_pts)
 
+        or
+
+        ndx = int
+        us (num_pts)
+        vs (num_pts)
+        zs (num_pts)
+
         returns points_backprojected (batch, num_points, 3)
         """
-        points_intrinsics = torch.stack([us / self.fxs[...,None], vs / self.fys[...,None]], -1) # (batch, num_points, 2)
-        points_homogenous = nn.functional.pad(points_intrinsics, (0, 1, 0, 0), mode="constant", value=1) # (batch, num_points, 3)
-        points_backprojected = points_homogenous * zs[...,None] # (batch, num_points, 3)
+        assert us.shape == vs.shape and vs.shape == zs.shape, f"us ({us.shape}), vs ({vs.shape}), zs ({zs.shape}) must all be same shape"
+        if ndx is None:
+            points_intrinsics = torch.stack([us / self.fxs[...,None], vs / self.fys[...,None]], -1) # (batch, num_points, 2)
+            points_homogenous = nn.functional.pad(points_intrinsics, (0, 1, 0, 0), mode="constant", value=1) # (batch, num_points, 3)
+            points_backprojected = points_homogenous * zs[...,None] # (batch, num_points, 3)
+        else:
+            points_intrinsics = torch.stack([us / self.fxs[ndx], vs / self.fys[ndx]], -1) # (num_points, 2)
+            points_homogenous = nn.functional.pad(points_intrinsics, (0, 1, 0, 0), mode="constant", value=1) # (num_points, 3)
+            points_backprojected = points_homogenous * zs[...,None] # (num_points, 3)
 
         return points_backprojected
```

### Comparing `toon3d-0.0.1/toon3d-current/utils/convert_points.py` & `toon3d-0.0.2/toon3d/utils/convert_points.py`

 * *Files identical despite different names*

### Comparing `toon3d-0.0.1/toon3d-current/utils/draw_utils.py` & `toon3d-0.0.2/toon3d/utils/draw_utils.py`

 * *Files identical despite different names*

### Comparing `toon3d-0.0.1/toon3d-current/utils/image_processing_utils.py` & `toon3d-0.0.2/toon3d/utils/image_processing_utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,57 @@
 import sys
 import os
 
 from pycocotools import mask as cocomask
 import cv2
 import torch
 from segment_anything import sam_model_registry, SamAutomaticMaskGenerator
+import kornia as K
+import kornia.feature as KF
 
 from nerfstudio.utils.rich_utils import CONSOLE
 from PIL import Image
+from transformers import pipeline
 
 
 def generate_depths(images, method="marigold", device="cpu"):
     if method == "marigold":
         from toon3d.generative.marigold import Marigold
 
         marigold = Marigold(device=device)
     elif method == "zoedepth":
         torch.hub.help("intel-isl/MiDaS", "DPT_BEiT_L_384", force_reload=False)  # Triggers fresh download of MiDaS repo
         zoe = torch.hub.load("isl-org/ZoeDepth", "ZoeD_NK", pretrained=True, _verbose=False).to(device)
+    elif method == "depth-anything":
+        pipe = pipeline(task="depth-estimation", model="LiheYoung/depth-anything-small-hf")
     else:
         CONSOLE.log(f"[bold red]Invalid depth method: {method}")
         sys.exit(1)
 
     depths = []
     for i, image in enumerate(images):
         image_tensor = (torch.from_numpy(images[i]).permute(2, 0, 1).to(device).unsqueeze(0) / 255.0).float()
         if method == "marigold":
             depth_tensor = torch.from_numpy(marigold.pipe(Image.fromarray(image)).depth_np)[..., None]
         elif method == "zoedepth":
             depth_tensor = zoe.infer(image_tensor).detach().cpu()[0].permute(1, 2, 0)
+        elif method == "depth-anything":
+            pil_image = Image.fromarray(image)
+            depth_tensor = pipe(pil_image)["predicted_depth"]
+            depth_tensor = torch.nn.functional.interpolate(
+                depth_tensor.unsqueeze(0), size=image_tensor.shape[2:], mode="bicubic", align_corners=False)[0]
+            depth_tensor = -depth_tensor.permute(1, 2, 0)
+            depth_tensor = depth_tensor - depth_tensor.min()
         depths.append(depth_tensor)
 
     return depths
 
 
-def generate_segments(images, device="cpu"):
-    sam_checkpoint = "data/sam-checkpoints/sam_vit_b_01ec64.pth"
+def generate_segments(images, device="cpu", sam_checkpoint_prefix="data/sam-checkpoints"):
+    sam_checkpoint = os.path.join(sam_checkpoint_prefix, "sam_vit_b_01ec64.pth")
     model_type = "vit_b"
 
     if not os.path.exists(sam_checkpoint):
         CONSOLE.log(f"[bold yellow]File not found: {sam_checkpoint}")
         CONSOLE.log(f"[bold yellow]Downloading `vit_b` from https://github.com/facebookresearch/segment-anything")
         os.system(
             "wget https://dl.fbaipublicfiles.com/segment_anything/sam_vit_b_01ec64.pth && mkdir data/sam-checkpoints/ && mv sam_vit_b_01ec64.pth data/sam-checkpoints/"
@@ -50,31 +62,47 @@
     except FileNotFoundError as e:
         CONSOLE.log(f"[bold red]{e}")
         CONSOLE.log(f"[bold red]Problem Downloading `vit_b` from https://github.com/facebookresearch/segment-anything")
         sys.exit(1)
 
     mask_generator = SamAutomaticMaskGenerator(
         model=sam,
-        points_per_side=64,
+        points_per_side=128,
         pred_iou_thresh=0.85,
         stability_score_thresh=0.88,
         stability_score_offset=1,
         box_nms_thresh=0.9,
         output_mode="coco_rle",
     )
 
     image_segments = []
-    for image in images:
+    for i, image in enumerate(images):
+        print(f"Processing image {i+1} of {len(images)}")
         segments = mask_generator.generate(image)
 
         for idx in range(len(segments)):
             mask_array = cocomask.decode(segments[idx]["segmentation"])
             contours, _ = cv2.findContours(mask_array, cv2.RETR_TREE, cv2.CHAIN_APPROX_SIMPLE)
             polygons = []
             for contour in contours:
                 if contour.size >= 6:
                     polygon = [point[0] for point in contour.tolist()]
                     polygons.append(polygon)
             segments[idx]["polygons"] = polygons
 
         image_segments.append(segments)
     return image_segments
+
+def generate_lines(images, device="cpu"):
+    torch_ims = []
+    for im in images:
+        torch_ims.append(K.color.rgb_to_grayscale(K.image_to_tensor(im).to(device).unsqueeze(0)/255.0))
+    
+    sold2 = KF.SOLD2(pretrained=True, config=None).to(device)
+    
+    outputs = []
+    with torch.no_grad():
+        for im in torch_ims:
+            outputs.append(sold2(im))
+    
+    lines = [outputs[i]["line_segments"][0].cpu().numpy().tolist() for i in range(len(outputs))]
+    return lines
```

### Comparing `toon3d-0.0.1/toon3d-current/utils/losses.py` & `toon3d-0.0.2/toon3d/utils/losses.py`

 * *Files identical despite different names*

### Comparing `toon3d-0.0.1/toon3d-current/utils/novel_view_samplers.py` & `toon3d-0.0.2/toon3d/utils/novel_view_samplers.py`

 * *Files identical despite different names*

### Comparing `toon3d-0.0.1/toon3d-current/utils/pytorch_arap/arap.py` & `toon3d-0.0.2/toon3d/utils/pytorch_arap/arap.py`

 * *Files identical despite different names*

### Comparing `toon3d-0.0.1/toon3d-current/utils/pytorch_arap/arap_utils.py` & `toon3d-0.0.2/toon3d/utils/pytorch_arap/arap_utils.py`

 * *Files identical despite different names*

### Comparing `toon3d-0.0.1/toon3d-current/warp/tri_rasterize.py` & `toon3d-0.0.2/toon3d/warp/tri_rasterize.py`

 * *Files identical despite different names*

### Comparing `toon3d-0.0.1/toon3d-current/warp_model.py` & `toon3d-0.0.2/toon3d/warp_model.py`

 * *Files identical despite different names*

### Comparing `toon3d-0.0.1/toon3d.egg-info/PKG-INFO` & `toon3d-0.0.2/toon3d.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toon3d
-Version: 0.0.1
+Version: 0.0.2
 Summary: toon3d package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Requires-Python: >=3.7.3
 Requires-Dist: black
 Requires-Dist: h5py
 Requires-Dist: mediapy
```

