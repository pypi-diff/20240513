# Comparing `tmp/video-representations-extractor-1.0.0.tar.gz` & `tmp/video-representations-extractor-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "video-representations-extractor-1.0.0.tar", last modified: Mon May 13 17:51:22 2024, max compression
+gzip compressed data, was "video-representations-extractor-1.0.1.tar", last modified: Mon May 13 18:03:06 2024, max compression
```

## Comparing `video-representations-extractor-1.0.0.tar` & `video-representations-extractor-1.0.1.tar`

### file list

```diff
@@ -1,207 +1,207 @@
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 17:51:22.750004 video-representations-extractor-1.0.0/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      486 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.0/LICENSE.TXT
--rw-r--r--   0 mihai     (1000) mihai     (1000)     8135 2024-05-13 17:51:22.750004 video-representations-extractor-1.0.0/PKG-INFO
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     6979 2024-05-07 08:51:30.000000 video-representations-extractor-1.0.0/README.md
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 17:51:22.730003 video-representations-extractor-1.0.0/bin/
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)     4253 2024-05-13 17:44:45.000000 video-representations-extractor-1.0.0/bin/vre
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       38 2024-05-13 17:51:22.750004 video-representations-extractor-1.0.0/setup.cfg
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1876 2024-05-13 17:51:18.000000 video-representations-extractor-1.0.0/setup.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 17:51:22.750004 video-representations-extractor-1.0.0/video_representations_extractor.egg-info/
--rw-r--r--   0 mihai     (1000) mihai     (1000)     8135 2024-05-13 17:51:22.000000 video-representations-extractor-1.0.0/video_representations_extractor.egg-info/PKG-INFO
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    11714 2024-05-13 17:51:22.000000 video-representations-extractor-1.0.0/video_representations_extractor.egg-info/SOURCES.txt
--rw-rw-r--   0 mihai     (1000) mihai     (1000)        1 2024-05-13 17:51:22.000000 video-representations-extractor-1.0.0/video_representations_extractor.egg-info/dependency_links.txt
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      417 2024-05-13 17:51:22.000000 video-representations-extractor-1.0.0/video_representations_extractor.egg-info/requires.txt
--rw-rw-r--   0 mihai     (1000) mihai     (1000)        4 2024-05-13 17:51:22.000000 video-representations-extractor-1.0.0/video_representations_extractor.egg-info/top_level.txt
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 17:51:22.730003 video-representations-extractor-1.0.0/vre/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      215 2024-05-06 12:14:58.000000 video-representations-extractor-1.0.0/vre/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     3607 2024-05-13 17:44:45.000000 video-representations-extractor-1.0.0/vre/data_storer.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     2355 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.0/vre/logger.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     2419 2024-05-08 19:37:37.000000 video-representations-extractor-1.0.0/vre/representation.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 17:51:22.734004 video-representations-extractor-1.0.0/vre/representations/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       82 2024-05-07 08:51:30.000000 video-representations-extractor-1.0.0/vre/representations/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     5474 2024-05-09 21:06:52.000000 video-representations-extractor-1.0.0/vre/representations/build_representations.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 17:51:22.734004 video-representations-extractor-1.0.0/vre/representations/depth/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.0/vre/representations/depth/__init__.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 17:51:22.734004 video-representations-extractor-1.0.0/vre/representations/depth/dpt/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       48 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.0/vre/representations/depth/dpt/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     3880 2024-05-08 19:33:51.000000 video-representations-extractor-1.0.0/vre/representations/depth/dpt/depth_dpt.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 17:51:22.734004 video-representations-extractor-1.0.0/vre/representations/depth/dpt/dpt_impl/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.0/vre/representations/depth/dpt/dpt_impl/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      389 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.0/vre/representations/depth/dpt/dpt_impl/base_model.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     9178 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.0/vre/representations/depth/dpt/dpt_impl/blocks.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     3088 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.0/vre/representations/depth/dpt/dpt_impl/dpt_depth.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    14673 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.0/vre/representations/depth/dpt/dpt_impl/vit.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 17:51:22.734004 video-representations-extractor-1.0.0/vre/representations/depth/odo_flow/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       57 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.0/vre/representations/depth/odo_flow/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     5726 2024-05-08 19:28:49.000000 video-representations-extractor-1.0.0/vre/representations/depth/odo_flow/depth_odo_flow.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 17:51:22.734004 video-representations-extractor-1.0.0/vre/representations/depth/odo_flow/odo_flow_impl/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.0/vre/representations/depth/odo_flow/odo_flow_impl/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     2485 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.0/vre/representations/depth/odo_flow/odo_flow_impl/cam.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     3381 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.0/vre/representations/depth/odo_flow/odo_flow_impl/camera_info.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    27130 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.0/vre/representations/depth/odo_flow/odo_flow_impl/depth_from_flow.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     2996 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.0/vre/representations/depth/odo_flow/odo_flow_impl/loss.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     2552 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.0/vre/representations/depth/odo_flow/odo_flow_impl/polyfit.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    12079 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.0/vre/representations/depth/odo_flow/odo_flow_impl/utils.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    11740 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.0/vre/representations/depth/odo_flow/odo_flow_impl/utils_geometry.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1172 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.0/vre/representations/dummy_representation.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 17:51:22.734004 video-representations-extractor-1.0.0/vre/representations/edges/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.0/vre/representations/edges/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1620 2024-05-08 19:06:41.000000 video-representations-extractor-1.0.0/vre/representations/edges/canny.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 17:51:22.734004 video-representations-extractor-1.0.0/vre/representations/edges/dexined/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       45 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.0/vre/representations/edges/dexined/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     3429 2024-05-09 21:06:52.000000 video-representations-extractor-1.0.0/vre/representations/edges/dexined/dexined.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    10066 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.0/vre/representations/edges/dexined/model_dexined.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      883 2024-05-07 14:46:28.000000 video-representations-extractor-1.0.0/vre/representations/hsv.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 17:51:22.734004 video-representations-extractor-1.0.0/vre/representations/normals/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.0/vre/representations/normals/__init__.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 17:51:22.734004 video-representations-extractor-1.0.0/vre/representations/normals/depth_svd/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       63 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.0/vre/representations/normals/depth_svd/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     4088 2024-05-08 19:20:50.000000 video-representations-extractor-1.0.0/vre/representations/normals/depth_svd/depth_normals_svd.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 17:51:22.734004 video-representations-extractor-1.0.0/vre/representations/normals/depth_svd/depth_svd_impl/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.0/vre/representations/normals/depth_svd/depth_svd_impl/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     2485 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.0/vre/representations/normals/depth_svd/depth_svd_impl/cam.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     3125 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.0/vre/representations/normals/depth_svd/depth_svd_impl/utils.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 17:51:22.734004 video-representations-extractor-1.0.0/vre/representations/optical_flow/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.0/vre/representations/optical_flow/__init__.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 17:51:22.734004 video-representations-extractor-1.0.0/vre/representations/optical_flow/raft/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       48 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.0/vre/representations/optical_flow/raft/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     4983 2024-05-09 21:06:52.000000 video-representations-extractor-1.0.0/vre/representations/optical_flow/raft/flow_raft.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 17:51:22.738004 video-representations-extractor-1.0.0/vre/representations/optical_flow/raft/raft_impl/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.0/vre/representations/optical_flow/raft/raft_impl/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     3074 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.0/vre/representations/optical_flow/raft/raft_impl/corr.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     9267 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.0/vre/representations/optical_flow/raft/raft_impl/datasets.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     8869 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.0/vre/representations/optical_flow/raft/raft_impl/extractor.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     4512 2024-05-08 18:52:36.000000 video-representations-extractor-1.0.0/vre/representations/optical_flow/raft/raft_impl/raft.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     5249 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.0/vre/representations/optical_flow/raft/raft_impl/update.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     2573 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.0/vre/representations/optical_flow/raft/raft_impl/utils.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 17:51:22.738004 video-representations-extractor-1.0.0/vre/representations/optical_flow/rife/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       48 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.0/vre/representations/optical_flow/rife/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     4698 2024-05-09 21:06:52.000000 video-representations-extractor-1.0.0/vre/representations/optical_flow/rife/flow_rife.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 17:51:22.738004 video-representations-extractor-1.0.0/vre/representations/optical_flow/rife/rife_impl/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     4421 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.0/vre/representations/optical_flow/rife/rife_impl/IFNet_HD.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     3712 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.0/vre/representations/optical_flow/rife/rife_impl/IFNet_HDv2.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     8754 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.0/vre/representations/optical_flow/rife/rife_impl/RIFE_HDv2.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.0/vre/representations/optical_flow/rife/rife_impl/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     2866 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.0/vre/representations/optical_flow/rife/rife_impl/loss.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1091 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.0/vre/representations/optical_flow/rife/rife_impl/warplayer.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      804 2024-05-09 21:06:52.000000 video-representations-extractor-1.0.0/vre/representations/rgb.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 17:51:22.738004 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/__init__.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 17:51:22.738004 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/fastsam/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       45 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/fastsam/__init__.py
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)     8584 2024-05-08 15:28:20.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/fastsam/fastsam.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 17:51:22.738004 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/fastsam/fastsam_impl/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      312 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/fastsam/fastsam_impl/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     4733 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/fastsam/fastsam_impl/decoder.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     4385 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/fastsam/fastsam_impl/model.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      442 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/fastsam/fastsam_impl/predict.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    18538 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/fastsam/fastsam_impl/prompt.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     2708 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/fastsam/fastsam_impl/utils.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 17:51:22.738004 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       53 2024-04-23 19:55:41.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/__init__.py
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)    39430 2024-04-26 05:56:06.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/convert.py
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)     8143 2024-05-08 08:30:31.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 17:51:22.738004 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      138 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     7259 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/comm.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 17:51:22.738004 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/data/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       96 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/data/__init__.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 17:51:22.742004 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/data/datasets/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      318 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/data/datasets/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    52231 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/data/datasets/register_ade20k_full.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     4608 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/data/datasets/register_ade20k_instance.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    19460 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/data/datasets/register_ade20k_panoptic.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     7080 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/data/datasets/register_coco_panoptic_annos_semseg.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    13576 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/data/datasets/register_coco_stuff_10k.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    13034 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/data/datasets/register_mapillary_vistas.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    16080 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/data/datasets/register_mapillary_vistas_panoptic.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 17:51:22.742004 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      666 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     7404 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/benchmark.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    26836 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/build.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     6991 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/catalog.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    13408 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/common.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     8129 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/dataset_mapper.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 17:51:22.742004 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      545 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    10183 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/builtin.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    21863 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/builtin_meta.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    11343 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/cityscapes.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     7793 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/cityscapes_panoptic.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    22788 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/coco.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     7649 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/coco_panoptic.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     8816 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/lvis.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)   223779 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/lvis_v0_5_categories.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)   219199 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/lvis_v1_categories.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    39436 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/lvis_v1_category_image_count.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     3112 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/pascal_voc.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      191 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/register_coco.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    23182 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/detection_utils.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 17:51:22.742004 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/samplers/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      434 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/samplers/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    12251 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/samplers/distributed_sampler.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1966 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/samplers/grouped_batch_sampler.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 17:51:22.742004 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/transforms/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      352 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/transforms/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    14138 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/transforms/augmentation.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    27338 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/transforms/augmentation_impl.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    12653 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/transforms/transform.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1259 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/file_io.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 17:51:22.746003 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/layers/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      253 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/layers/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     3040 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/layers/blocks.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    16657 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/layers/deform_conv.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     9779 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/layers/norm.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      559 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/layers/shape_spec.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1388 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/layers/wrappers.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    18059 2024-04-25 06:02:24.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/maskformer_model.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 17:51:22.746003 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      238 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/__init__.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 17:51:22.746003 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/backbone/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/backbone/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    27473 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/backbone/swin.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 17:51:22.746003 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/meta_arch/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/meta_arch/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     5262 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/meta_arch/mask_former_head.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 17:51:22.746003 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/pixel_decoder/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/pixel_decoder/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    11748 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/pixel_decoder/fpn.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     7811 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/pixel_decoder/ms_deform_attn.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    15168 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/pixel_decoder/msdeformattn.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    25781 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/resnet.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 17:51:22.746003 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/transformer_decoder/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      224 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/transformer_decoder/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    17739 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/transformer_decoder/mask2former_transformer_decoder.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     6946 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/transformer_decoder/maskformer_transformer_decoder.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     2540 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/transformer_decoder/position_encoding.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    11959 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/transformer_decoder/transformer.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 17:51:22.746003 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/structures/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      410 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/structures/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    14451 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/structures/boxes.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     6697 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/structures/image_list.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     6635 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/structures/instances.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     9030 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/structures/keypoints.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    19531 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/structures/masks.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    18980 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/structures/rotated_boxes.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    54116 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/visualizer.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 17:51:22.746003 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/safeuav/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     5125 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/safeuav/Map2Map.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       45 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/safeuav/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     4155 2024-05-08 08:31:54.000000 video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/safeuav/safeuav.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 17:51:22.746003 video-representations-extractor-1.0.0/vre/representations/soft_segmentation/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.0/vre/representations/soft_segmentation/__init__.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 17:51:22.746003 video-representations-extractor-1.0.0/vre/representations/soft_segmentation/generalized_boundaries/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       74 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.0/vre/representations/soft_segmentation/generalized_boundaries/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1836 2024-05-07 15:03:35.000000 video-representations-extractor-1.0.0/vre/representations/soft_segmentation/generalized_boundaries/generalized_boundaries.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 17:51:22.750004 video-representations-extractor-1.0.0/vre/representations/soft_segmentation/halftone/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       47 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.0/vre/representations/soft_segmentation/halftone/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     7704 2024-05-07 15:05:55.000000 video-representations-extractor-1.0.0/vre/representations/soft_segmentation/halftone/halftone.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     4026 2024-05-07 14:54:13.000000 video-representations-extractor-1.0.0/vre/representations/soft_segmentation/kmeans.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 17:51:22.750004 video-representations-extractor-1.0.0/vre/utils/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      128 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.0/vre/utils/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      679 2024-05-06 09:42:54.000000 video-representations-extractor-1.0.0/vre/utils/fake_video.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1352 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.0/vre/utils/topological_sort.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     5169 2024-05-09 21:06:52.000000 video-representations-extractor-1.0.0/vre/utils/utils.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     6609 2024-05-13 17:44:45.000000 video-representations-extractor-1.0.0/vre/video_representations_extractor.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1300 2024-05-13 17:44:45.000000 video-representations-extractor-1.0.0/vre/vre_representation_mixin.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     7169 2024-05-13 17:44:45.000000 video-representations-extractor-1.0.0/vre/vre_runtime_args.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 18:03:06.162889 video-representations-extractor-1.0.1/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      486 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.1/LICENSE.TXT
+-rw-r--r--   0 mihai     (1000) mihai     (1000)     8135 2024-05-13 18:03:06.162889 video-representations-extractor-1.0.1/PKG-INFO
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     6979 2024-05-07 08:51:30.000000 video-representations-extractor-1.0.1/README.md
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 18:03:06.146889 video-representations-extractor-1.0.1/bin/
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)     4253 2024-05-13 17:44:45.000000 video-representations-extractor-1.0.1/bin/vre
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       38 2024-05-13 18:03:06.162889 video-representations-extractor-1.0.1/setup.cfg
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1340 2024-05-13 18:02:42.000000 video-representations-extractor-1.0.1/setup.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 18:03:06.162889 video-representations-extractor-1.0.1/video_representations_extractor.egg-info/
+-rw-r--r--   0 mihai     (1000) mihai     (1000)     8135 2024-05-13 18:03:06.000000 video-representations-extractor-1.0.1/video_representations_extractor.egg-info/PKG-INFO
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    11714 2024-05-13 18:03:06.000000 video-representations-extractor-1.0.1/video_representations_extractor.egg-info/SOURCES.txt
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)        1 2024-05-13 18:03:06.000000 video-representations-extractor-1.0.1/video_representations_extractor.egg-info/dependency_links.txt
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      417 2024-05-13 18:03:06.000000 video-representations-extractor-1.0.1/video_representations_extractor.egg-info/requires.txt
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)        4 2024-05-13 18:03:06.000000 video-representations-extractor-1.0.1/video_representations_extractor.egg-info/top_level.txt
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 18:03:06.146889 video-representations-extractor-1.0.1/vre/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      215 2024-05-06 12:14:58.000000 video-representations-extractor-1.0.1/vre/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     3607 2024-05-13 17:44:45.000000 video-representations-extractor-1.0.1/vre/data_storer.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     2355 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.1/vre/logger.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     2419 2024-05-08 19:37:37.000000 video-representations-extractor-1.0.1/vre/representation.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 18:03:06.150889 video-representations-extractor-1.0.1/vre/representations/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       82 2024-05-07 08:51:30.000000 video-representations-extractor-1.0.1/vre/representations/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     5474 2024-05-09 21:06:52.000000 video-representations-extractor-1.0.1/vre/representations/build_representations.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 18:03:06.150889 video-representations-extractor-1.0.1/vre/representations/depth/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.1/vre/representations/depth/__init__.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 18:03:06.150889 video-representations-extractor-1.0.1/vre/representations/depth/dpt/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       48 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.1/vre/representations/depth/dpt/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     3880 2024-05-08 19:33:51.000000 video-representations-extractor-1.0.1/vre/representations/depth/dpt/depth_dpt.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 18:03:06.150889 video-representations-extractor-1.0.1/vre/representations/depth/dpt/dpt_impl/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.1/vre/representations/depth/dpt/dpt_impl/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      389 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.1/vre/representations/depth/dpt/dpt_impl/base_model.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     9178 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.1/vre/representations/depth/dpt/dpt_impl/blocks.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     3088 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.1/vre/representations/depth/dpt/dpt_impl/dpt_depth.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    14673 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.1/vre/representations/depth/dpt/dpt_impl/vit.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 18:03:06.150889 video-representations-extractor-1.0.1/vre/representations/depth/odo_flow/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       57 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.1/vre/representations/depth/odo_flow/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     5726 2024-05-08 19:28:49.000000 video-representations-extractor-1.0.1/vre/representations/depth/odo_flow/depth_odo_flow.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 18:03:06.150889 video-representations-extractor-1.0.1/vre/representations/depth/odo_flow/odo_flow_impl/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.1/vre/representations/depth/odo_flow/odo_flow_impl/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     2485 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.1/vre/representations/depth/odo_flow/odo_flow_impl/cam.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     3381 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.1/vre/representations/depth/odo_flow/odo_flow_impl/camera_info.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    27130 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.1/vre/representations/depth/odo_flow/odo_flow_impl/depth_from_flow.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     2996 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.1/vre/representations/depth/odo_flow/odo_flow_impl/loss.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     2552 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.1/vre/representations/depth/odo_flow/odo_flow_impl/polyfit.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    12079 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.1/vre/representations/depth/odo_flow/odo_flow_impl/utils.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    11740 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.1/vre/representations/depth/odo_flow/odo_flow_impl/utils_geometry.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1172 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.1/vre/representations/dummy_representation.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 18:03:06.150889 video-representations-extractor-1.0.1/vre/representations/edges/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.1/vre/representations/edges/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1620 2024-05-08 19:06:41.000000 video-representations-extractor-1.0.1/vre/representations/edges/canny.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 18:03:06.150889 video-representations-extractor-1.0.1/vre/representations/edges/dexined/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       45 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.1/vre/representations/edges/dexined/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     3429 2024-05-09 21:06:52.000000 video-representations-extractor-1.0.1/vre/representations/edges/dexined/dexined.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    10066 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.1/vre/representations/edges/dexined/model_dexined.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      883 2024-05-07 14:46:28.000000 video-representations-extractor-1.0.1/vre/representations/hsv.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 18:03:06.150889 video-representations-extractor-1.0.1/vre/representations/normals/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.1/vre/representations/normals/__init__.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 18:03:06.150889 video-representations-extractor-1.0.1/vre/representations/normals/depth_svd/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       63 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.1/vre/representations/normals/depth_svd/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     4088 2024-05-08 19:20:50.000000 video-representations-extractor-1.0.1/vre/representations/normals/depth_svd/depth_normals_svd.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 18:03:06.150889 video-representations-extractor-1.0.1/vre/representations/normals/depth_svd/depth_svd_impl/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.1/vre/representations/normals/depth_svd/depth_svd_impl/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     2485 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.1/vre/representations/normals/depth_svd/depth_svd_impl/cam.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     3125 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.1/vre/representations/normals/depth_svd/depth_svd_impl/utils.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 18:03:06.150889 video-representations-extractor-1.0.1/vre/representations/optical_flow/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.1/vre/representations/optical_flow/__init__.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 18:03:06.150889 video-representations-extractor-1.0.1/vre/representations/optical_flow/raft/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       48 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.1/vre/representations/optical_flow/raft/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     4983 2024-05-09 21:06:52.000000 video-representations-extractor-1.0.1/vre/representations/optical_flow/raft/flow_raft.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 18:03:06.154889 video-representations-extractor-1.0.1/vre/representations/optical_flow/raft/raft_impl/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.1/vre/representations/optical_flow/raft/raft_impl/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     3074 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.1/vre/representations/optical_flow/raft/raft_impl/corr.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     9267 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.1/vre/representations/optical_flow/raft/raft_impl/datasets.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     8869 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.1/vre/representations/optical_flow/raft/raft_impl/extractor.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     4512 2024-05-08 18:52:36.000000 video-representations-extractor-1.0.1/vre/representations/optical_flow/raft/raft_impl/raft.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     5249 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.1/vre/representations/optical_flow/raft/raft_impl/update.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     2573 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.1/vre/representations/optical_flow/raft/raft_impl/utils.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 18:03:06.154889 video-representations-extractor-1.0.1/vre/representations/optical_flow/rife/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       48 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.1/vre/representations/optical_flow/rife/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     4698 2024-05-09 21:06:52.000000 video-representations-extractor-1.0.1/vre/representations/optical_flow/rife/flow_rife.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 18:03:06.154889 video-representations-extractor-1.0.1/vre/representations/optical_flow/rife/rife_impl/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     4421 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.1/vre/representations/optical_flow/rife/rife_impl/IFNet_HD.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     3712 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.1/vre/representations/optical_flow/rife/rife_impl/IFNet_HDv2.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     8754 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.1/vre/representations/optical_flow/rife/rife_impl/RIFE_HDv2.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.1/vre/representations/optical_flow/rife/rife_impl/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     2866 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.1/vre/representations/optical_flow/rife/rife_impl/loss.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1091 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.1/vre/representations/optical_flow/rife/rife_impl/warplayer.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      804 2024-05-09 21:06:52.000000 video-representations-extractor-1.0.1/vre/representations/rgb.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 18:03:06.154889 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/__init__.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 18:03:06.154889 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/fastsam/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       45 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/fastsam/__init__.py
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)     8584 2024-05-08 15:28:20.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/fastsam/fastsam.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 18:03:06.154889 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/fastsam/fastsam_impl/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      312 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/fastsam/fastsam_impl/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     4733 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/fastsam/fastsam_impl/decoder.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     4385 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/fastsam/fastsam_impl/model.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      442 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/fastsam/fastsam_impl/predict.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    18538 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/fastsam/fastsam_impl/prompt.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     2708 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/fastsam/fastsam_impl/utils.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 18:03:06.154889 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       53 2024-04-23 19:55:41.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/__init__.py
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)    39430 2024-04-26 05:56:06.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/convert.py
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)     8143 2024-05-08 08:30:31.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 18:03:06.154889 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      138 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     7259 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/comm.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 18:03:06.154889 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/data/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       96 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/data/__init__.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 18:03:06.154889 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/data/datasets/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      318 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/data/datasets/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    52231 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/data/datasets/register_ade20k_full.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     4608 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/data/datasets/register_ade20k_instance.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    19460 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/data/datasets/register_ade20k_panoptic.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     7080 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/data/datasets/register_coco_panoptic_annos_semseg.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    13576 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/data/datasets/register_coco_stuff_10k.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    13034 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/data/datasets/register_mapillary_vistas.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    16080 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/data/datasets/register_mapillary_vistas_panoptic.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 18:03:06.158889 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      666 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     7404 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/benchmark.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    26836 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/build.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     6991 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/catalog.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    13408 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/common.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     8129 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/dataset_mapper.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 18:03:06.158889 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      545 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    10183 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/builtin.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    21863 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/builtin_meta.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    11343 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/cityscapes.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     7793 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/cityscapes_panoptic.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    22788 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/coco.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     7649 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/coco_panoptic.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     8816 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/lvis.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)   223779 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/lvis_v0_5_categories.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)   219199 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/lvis_v1_categories.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    39436 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/lvis_v1_category_image_count.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     3112 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/pascal_voc.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      191 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/register_coco.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    23182 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/detection_utils.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 18:03:06.158889 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/samplers/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      434 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/samplers/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    12251 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/samplers/distributed_sampler.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1966 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/samplers/grouped_batch_sampler.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 18:03:06.158889 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/transforms/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      352 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/transforms/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    14138 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/transforms/augmentation.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    27338 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/transforms/augmentation_impl.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    12653 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/transforms/transform.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1259 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/file_io.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 18:03:06.158889 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/layers/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      253 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/layers/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     3040 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/layers/blocks.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    16657 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/layers/deform_conv.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     9779 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/layers/norm.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      559 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/layers/shape_spec.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1388 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/layers/wrappers.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    18059 2024-04-25 06:02:24.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/maskformer_model.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 18:03:06.158889 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      238 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/__init__.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 18:03:06.158889 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/backbone/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/backbone/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    27473 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/backbone/swin.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 18:03:06.162889 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/meta_arch/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/meta_arch/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     5262 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/meta_arch/mask_former_head.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 18:03:06.162889 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/pixel_decoder/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/pixel_decoder/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    11748 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/pixel_decoder/fpn.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     7811 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/pixel_decoder/ms_deform_attn.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    15168 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/pixel_decoder/msdeformattn.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    25781 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/resnet.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 18:03:06.162889 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/transformer_decoder/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      224 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/transformer_decoder/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    17739 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/transformer_decoder/mask2former_transformer_decoder.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     6946 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/transformer_decoder/maskformer_transformer_decoder.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     2540 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/transformer_decoder/position_encoding.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    11959 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/transformer_decoder/transformer.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 18:03:06.162889 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/structures/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      410 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/structures/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    14451 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/structures/boxes.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     6697 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/structures/image_list.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     6635 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/structures/instances.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     9030 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/structures/keypoints.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    19531 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/structures/masks.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    18980 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/structures/rotated_boxes.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    54116 2024-04-25 05:16:24.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/visualizer.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 18:03:06.162889 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/safeuav/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     5125 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/safeuav/Map2Map.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       45 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/safeuav/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     4155 2024-05-08 08:31:54.000000 video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/safeuav/safeuav.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 18:03:06.162889 video-representations-extractor-1.0.1/vre/representations/soft_segmentation/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.1/vre/representations/soft_segmentation/__init__.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 18:03:06.162889 video-representations-extractor-1.0.1/vre/representations/soft_segmentation/generalized_boundaries/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       74 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.1/vre/representations/soft_segmentation/generalized_boundaries/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1836 2024-05-07 15:03:35.000000 video-representations-extractor-1.0.1/vre/representations/soft_segmentation/generalized_boundaries/generalized_boundaries.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 18:03:06.162889 video-representations-extractor-1.0.1/vre/representations/soft_segmentation/halftone/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       47 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.1/vre/representations/soft_segmentation/halftone/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     7704 2024-05-07 15:05:55.000000 video-representations-extractor-1.0.1/vre/representations/soft_segmentation/halftone/halftone.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     4026 2024-05-07 14:54:13.000000 video-representations-extractor-1.0.1/vre/representations/soft_segmentation/kmeans.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-13 18:03:06.162889 video-representations-extractor-1.0.1/vre/utils/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      128 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.1/vre/utils/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      679 2024-05-06 09:42:54.000000 video-representations-extractor-1.0.1/vre/utils/fake_video.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1352 2024-04-22 18:35:19.000000 video-representations-extractor-1.0.1/vre/utils/topological_sort.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     5169 2024-05-09 21:06:52.000000 video-representations-extractor-1.0.1/vre/utils/utils.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     6609 2024-05-13 17:44:45.000000 video-representations-extractor-1.0.1/vre/video_representations_extractor.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1300 2024-05-13 17:44:45.000000 video-representations-extractor-1.0.1/vre/vre_representation_mixin.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     7169 2024-05-13 17:44:45.000000 video-representations-extractor-1.0.1/vre/vre_runtime_args.py
```

### Comparing `video-representations-extractor-1.0.0/PKG-INFO` & `video-representations-extractor-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: video-representations-extractor
-Version: 1.0.0
+Version: 1.0.1
 Summary: Video Representations Extractor (VRE) for computing algorithmic or neural representations of each frame.
 Home-page: https://gitlab.com/meehai/video-representations-extractor
 License: WTFPL
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.TXT
 Requires-Dist: numpy>=1.21.6
```

### Comparing `video-representations-extractor-1.0.0/README.md` & `video-representations-extractor-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/bin/vre` & `video-representations-extractor-1.0.1/bin/vre`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/video_representations_extractor.egg-info/PKG-INFO` & `video-representations-extractor-1.0.1/video_representations_extractor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: video-representations-extractor
-Version: 1.0.0
+Version: 1.0.1
 Summary: Video Representations Extractor (VRE) for computing algorithmic or neural representations of each frame.
 Home-page: https://gitlab.com/meehai/video-representations-extractor
 License: WTFPL
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.TXT
 Requires-Dist: numpy>=1.21.6
```

### Comparing `video-representations-extractor-1.0.0/video_representations_extractor.egg-info/SOURCES.txt` & `video-representations-extractor-1.0.1/video_representations_extractor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/data_storer.py` & `video-representations-extractor-1.0.1/vre/data_storer.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/logger.py` & `video-representations-extractor-1.0.1/vre/logger.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representation.py` & `video-representations-extractor-1.0.1/vre/representation.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/build_representations.py` & `video-representations-extractor-1.0.1/vre/representations/build_representations.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/depth/dpt/depth_dpt.py` & `video-representations-extractor-1.0.1/vre/representations/depth/dpt/depth_dpt.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/depth/dpt/dpt_impl/blocks.py` & `video-representations-extractor-1.0.1/vre/representations/depth/dpt/dpt_impl/blocks.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/depth/dpt/dpt_impl/dpt_depth.py` & `video-representations-extractor-1.0.1/vre/representations/depth/dpt/dpt_impl/dpt_depth.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/depth/dpt/dpt_impl/vit.py` & `video-representations-extractor-1.0.1/vre/representations/depth/dpt/dpt_impl/vit.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/depth/odo_flow/depth_odo_flow.py` & `video-representations-extractor-1.0.1/vre/representations/depth/odo_flow/depth_odo_flow.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/depth/odo_flow/odo_flow_impl/cam.py` & `video-representations-extractor-1.0.1/vre/representations/depth/odo_flow/odo_flow_impl/cam.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/depth/odo_flow/odo_flow_impl/camera_info.py` & `video-representations-extractor-1.0.1/vre/representations/depth/odo_flow/odo_flow_impl/camera_info.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/depth/odo_flow/odo_flow_impl/depth_from_flow.py` & `video-representations-extractor-1.0.1/vre/representations/depth/odo_flow/odo_flow_impl/depth_from_flow.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/depth/odo_flow/odo_flow_impl/loss.py` & `video-representations-extractor-1.0.1/vre/representations/depth/odo_flow/odo_flow_impl/loss.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/depth/odo_flow/odo_flow_impl/polyfit.py` & `video-representations-extractor-1.0.1/vre/representations/depth/odo_flow/odo_flow_impl/polyfit.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/depth/odo_flow/odo_flow_impl/utils.py` & `video-representations-extractor-1.0.1/vre/representations/depth/odo_flow/odo_flow_impl/utils.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/depth/odo_flow/odo_flow_impl/utils_geometry.py` & `video-representations-extractor-1.0.1/vre/representations/depth/odo_flow/odo_flow_impl/utils_geometry.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/dummy_representation.py` & `video-representations-extractor-1.0.1/vre/representations/dummy_representation.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/edges/canny.py` & `video-representations-extractor-1.0.1/vre/representations/edges/canny.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/edges/dexined/dexined.py` & `video-representations-extractor-1.0.1/vre/representations/edges/dexined/dexined.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/edges/dexined/model_dexined.py` & `video-representations-extractor-1.0.1/vre/representations/edges/dexined/model_dexined.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/hsv.py` & `video-representations-extractor-1.0.1/vre/representations/hsv.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/normals/depth_svd/depth_normals_svd.py` & `video-representations-extractor-1.0.1/vre/representations/normals/depth_svd/depth_normals_svd.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/normals/depth_svd/depth_svd_impl/cam.py` & `video-representations-extractor-1.0.1/vre/representations/normals/depth_svd/depth_svd_impl/cam.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/normals/depth_svd/depth_svd_impl/utils.py` & `video-representations-extractor-1.0.1/vre/representations/normals/depth_svd/depth_svd_impl/utils.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/optical_flow/raft/flow_raft.py` & `video-representations-extractor-1.0.1/vre/representations/optical_flow/raft/flow_raft.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/optical_flow/raft/raft_impl/corr.py` & `video-representations-extractor-1.0.1/vre/representations/optical_flow/raft/raft_impl/corr.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/optical_flow/raft/raft_impl/datasets.py` & `video-representations-extractor-1.0.1/vre/representations/optical_flow/raft/raft_impl/datasets.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/optical_flow/raft/raft_impl/extractor.py` & `video-representations-extractor-1.0.1/vre/representations/optical_flow/raft/raft_impl/extractor.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/optical_flow/raft/raft_impl/raft.py` & `video-representations-extractor-1.0.1/vre/representations/optical_flow/raft/raft_impl/raft.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/optical_flow/raft/raft_impl/update.py` & `video-representations-extractor-1.0.1/vre/representations/optical_flow/raft/raft_impl/update.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/optical_flow/raft/raft_impl/utils.py` & `video-representations-extractor-1.0.1/vre/representations/optical_flow/raft/raft_impl/utils.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/optical_flow/rife/flow_rife.py` & `video-representations-extractor-1.0.1/vre/representations/optical_flow/rife/flow_rife.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/optical_flow/rife/rife_impl/IFNet_HD.py` & `video-representations-extractor-1.0.1/vre/representations/optical_flow/rife/rife_impl/IFNet_HD.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/optical_flow/rife/rife_impl/IFNet_HDv2.py` & `video-representations-extractor-1.0.1/vre/representations/optical_flow/rife/rife_impl/IFNet_HDv2.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/optical_flow/rife/rife_impl/RIFE_HDv2.py` & `video-representations-extractor-1.0.1/vre/representations/optical_flow/rife/rife_impl/RIFE_HDv2.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/optical_flow/rife/rife_impl/loss.py` & `video-representations-extractor-1.0.1/vre/representations/optical_flow/rife/rife_impl/loss.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/optical_flow/rife/rife_impl/warplayer.py` & `video-representations-extractor-1.0.1/vre/representations/optical_flow/rife/rife_impl/warplayer.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/rgb.py` & `video-representations-extractor-1.0.1/vre/representations/rgb.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/fastsam/fastsam.py` & `video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/fastsam/fastsam.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/fastsam/fastsam_impl/decoder.py` & `video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/fastsam/fastsam_impl/decoder.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/fastsam/fastsam_impl/model.py` & `video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/fastsam/fastsam_impl/model.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/fastsam/fastsam_impl/prompt.py` & `video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/fastsam/fastsam_impl/prompt.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/fastsam/fastsam_impl/utils.py` & `video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/fastsam/fastsam_impl/utils.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/convert.py` & `video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/convert.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former.py` & `video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/comm.py` & `video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/comm.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/data/datasets/register_ade20k_full.py` & `video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/data/datasets/register_ade20k_full.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/data/datasets/register_ade20k_instance.py` & `video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/data/datasets/register_ade20k_instance.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/data/datasets/register_ade20k_panoptic.py` & `video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/data/datasets/register_ade20k_panoptic.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/data/datasets/register_coco_panoptic_annos_semseg.py` & `video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/data/datasets/register_coco_panoptic_annos_semseg.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/data/datasets/register_coco_stuff_10k.py` & `video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/data/datasets/register_coco_stuff_10k.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/data/datasets/register_mapillary_vistas.py` & `video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/data/datasets/register_mapillary_vistas.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/data/datasets/register_mapillary_vistas_panoptic.py` & `video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/data/datasets/register_mapillary_vistas_panoptic.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/__init__.py` & `video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/__init__.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/benchmark.py` & `video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/benchmark.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/build.py` & `video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/build.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/catalog.py` & `video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/catalog.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/common.py` & `video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/common.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/dataset_mapper.py` & `video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/dataset_mapper.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/__init__.py` & `video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/builtin.py` & `video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/builtin.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/builtin_meta.py` & `video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/builtin_meta.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/cityscapes.py` & `video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/cityscapes.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/cityscapes_panoptic.py` & `video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/cityscapes_panoptic.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/coco.py` & `video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/coco.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/coco_panoptic.py` & `video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/coco_panoptic.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/lvis.py` & `video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/lvis.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/lvis_v0_5_categories.py` & `video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/lvis_v0_5_categories.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/lvis_v1_categories.py` & `video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/lvis_v1_categories.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/lvis_v1_category_image_count.py` & `video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/lvis_v1_category_image_count.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/pascal_voc.py` & `video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/datasets/pascal_voc.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/detection_utils.py` & `video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/detection_utils.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/samplers/distributed_sampler.py` & `video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/samplers/distributed_sampler.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/samplers/grouped_batch_sampler.py` & `video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/samplers/grouped_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/transforms/augmentation.py` & `video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/transforms/augmentation.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/transforms/augmentation_impl.py` & `video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/transforms/augmentation_impl.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/transforms/transform.py` & `video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/det2_data/transforms/transform.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/file_io.py` & `video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/file_io.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/layers/blocks.py` & `video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/layers/blocks.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/layers/deform_conv.py` & `video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/layers/deform_conv.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/layers/norm.py` & `video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/layers/norm.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/layers/shape_spec.py` & `video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/layers/shape_spec.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/layers/wrappers.py` & `video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/layers/wrappers.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/maskformer_model.py` & `video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/maskformer_model.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/backbone/swin.py` & `video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/backbone/swin.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/meta_arch/mask_former_head.py` & `video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/meta_arch/mask_former_head.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/pixel_decoder/fpn.py` & `video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/pixel_decoder/fpn.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/pixel_decoder/ms_deform_attn.py` & `video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/pixel_decoder/ms_deform_attn.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/pixel_decoder/msdeformattn.py` & `video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/pixel_decoder/msdeformattn.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/resnet.py` & `video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/resnet.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/transformer_decoder/mask2former_transformer_decoder.py` & `video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/transformer_decoder/mask2former_transformer_decoder.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/transformer_decoder/maskformer_transformer_decoder.py` & `video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/transformer_decoder/maskformer_transformer_decoder.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/transformer_decoder/position_encoding.py` & `video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/transformer_decoder/position_encoding.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/transformer_decoder/transformer.py` & `video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/modeling/transformer_decoder/transformer.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/structures/boxes.py` & `video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/structures/boxes.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/structures/image_list.py` & `video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/structures/image_list.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/structures/instances.py` & `video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/structures/instances.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/structures/keypoints.py` & `video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/structures/keypoints.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/structures/masks.py` & `video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/structures/masks.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/structures/rotated_boxes.py` & `video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/structures/rotated_boxes.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/mask2former/mask2former_impl/visualizer.py` & `video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/mask2former/mask2former_impl/visualizer.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/safeuav/Map2Map.py` & `video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/safeuav/Map2Map.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/semantic_segmentation/safeuav/safeuav.py` & `video-representations-extractor-1.0.1/vre/representations/semantic_segmentation/safeuav/safeuav.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/soft_segmentation/generalized_boundaries/generalized_boundaries.py` & `video-representations-extractor-1.0.1/vre/representations/soft_segmentation/generalized_boundaries/generalized_boundaries.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/soft_segmentation/halftone/halftone.py` & `video-representations-extractor-1.0.1/vre/representations/soft_segmentation/halftone/halftone.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/representations/soft_segmentation/kmeans.py` & `video-representations-extractor-1.0.1/vre/representations/soft_segmentation/kmeans.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/utils/fake_video.py` & `video-representations-extractor-1.0.1/vre/utils/fake_video.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/utils/topological_sort.py` & `video-representations-extractor-1.0.1/vre/utils/topological_sort.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/utils/utils.py` & `video-representations-extractor-1.0.1/vre/utils/utils.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/video_representations_extractor.py` & `video-representations-extractor-1.0.1/vre/video_representations_extractor.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/vre_representation_mixin.py` & `video-representations-extractor-1.0.1/vre/vre_representation_mixin.py`

 * *Files identical despite different names*

### Comparing `video-representations-extractor-1.0.0/vre/vre_runtime_args.py` & `video-representations-extractor-1.0.1/vre/vre_runtime_args.py`

 * *Files identical despite different names*

