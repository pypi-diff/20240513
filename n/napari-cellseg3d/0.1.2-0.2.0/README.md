# Comparing `tmp/napari_cellseg3d-0.1.2.tar.gz` & `tmp/napari_cellseg3d-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari_cellseg3d-0.1.2.tar", last modified: Tue Apr  2 08:55:46 2024, max compression
+gzip compressed data, was "napari_cellseg3d-0.2.0.tar", last modified: Mon May 13 08:58:23 2024, max compression
```

## Comparing `napari_cellseg3d-0.1.2.tar` & `napari_cellseg3d-0.2.0.tar`

### file list

```diff
@@ -1,102 +1,103 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:55:46.183704 napari_cellseg3d-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9462 2024-04-02 08:55:46.183704 napari_cellseg3d-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6795 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:55:46.167704 napari_cellseg3d-0.1.2/napari_cellseg3d/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:55:46.171704 napari_cellseg3d-0.1.2/napari_cellseg3d/_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/_tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/_tests/fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:55:46.171704 napari_cellseg3d-0.1.2/napari_cellseg3d/_tests/res/
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/_tests/res/test.png
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/_tests/test_base_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/_tests/test_dock_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/_tests/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/_tests/test_inference.py
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/_tests/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/_tests/test_labels_correction.py
--rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/_tests/test_model_framework.py
--rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/_tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/_tests/test_plugin_inference.py
--rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/_tests/test_plugin_training.py
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/_tests/test_plugin_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/_tests/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/_tests/test_review.py
--rw-r--r--   0 runner    (1001) docker     (127)     4316 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/_tests/test_training.py
--rw-r--r--   0 runner    (1001) docker     (127)     7335 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/_tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/_tests/test_weight_download.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/_tests/test_wnet_training.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:55:46.175704 napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9598 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/crf.py
--rw-r--r--   0 runner    (1001) docker     (127)    30959 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/instance_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)    13712 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/model_framework.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:55:46.175704 napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/models/
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/models/TEMPLATE_model.py
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/models/model_SegResNet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/models/model_SwinUNetR.py
--rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/models/model_TRAILMAP.py
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/models/model_TRAILMAP_MS.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/models/model_VNet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/models/model_WNet.py
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/models/model_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:55:46.175704 napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/models/pretrained/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/models/pretrained/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/models/pretrained/pretrained_model_urls.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:55:46.175704 napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/models/unet/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/models/unet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19683 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/models/unet/buildingblocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6032 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/models/unet/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:55:46.175704 napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/models/wnet/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/models/wnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9105 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/models/wnet/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5065 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/models/wnet/soft_Ncuts.py
--rw-r--r--   0 runner    (1001) docker     (127)    37497 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/worker_inference.py
--rw-r--r--   0 runner    (1001) docker     (127)    68486 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/worker_training.py
--rw-r--r--   0 runner    (1001) docker     (127)    11149 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/workers_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:55:46.179704 napari_cellseg3d-0.1.2/napari_cellseg3d/code_plugins/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/code_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18865 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/code_plugins/plugin_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    27266 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/code_plugins/plugin_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)    10606 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/code_plugins/plugin_crf.py
--rw-r--r--   0 runner    (1001) docker     (127)    23870 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/code_plugins/plugin_crop.py
--rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/code_plugins/plugin_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    10859 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/code_plugins/plugin_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    36530 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/code_plugins/plugin_model_inference.py
--rw-r--r--   0 runner    (1001) docker     (127)    61986 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/code_plugins/plugin_model_training.py
--rw-r--r--   0 runner    (1001) docker     (127)    16713 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/code_plugins/plugin_review.py
--rw-r--r--   0 runner    (1001) docker     (127)    10102 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/code_plugins/plugin_review_dock.py
--rw-r--r--   0 runner    (1001) docker     (127)     7700 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/code_plugins/plugin_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    12482 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:55:46.179704 napari_cellseg3d-0.1.2/napari_cellseg3d/dev_scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/dev_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14359 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/dev_scripts/artefact_labeling.py
--rw-r--r--   0 runner    (1001) docker     (127)    29173 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/dev_scripts/colab_training.py
--rw-r--r--   0 runner    (1001) docker     (127)    12203 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/dev_scripts/correct_labels.py
--rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/dev_scripts/crop_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    11993 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/dev_scripts/evaluate_labels.py
--rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/dev_scripts/remote_training.py
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/dev_scripts/sliding_window_voronoi.py
--rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/dev_scripts/thread_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/dev_scripts/whole_brain_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    53880 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/napari.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:55:46.179704 napari_cellseg3d-0.1.2/napari_cellseg3d/res/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/res/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   495510 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/res/logo_alpha.png
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    21552 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:55:46.183704 napari_cellseg3d-0.1.2/napari_cellseg3d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9462 2024-04-02 08:55:46.000000 napari_cellseg3d-0.1.2/napari_cellseg3d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3915 2024-04-02 08:55:46.000000 napari_cellseg3d-0.1.2/napari_cellseg3d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 08:55:46.000000 napari_cellseg3d-0.1.2/napari_cellseg3d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-02 08:55:46.000000 napari_cellseg3d-0.1.2/napari_cellseg3d.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-02 08:55:46.000000 napari_cellseg3d-0.1.2/napari_cellseg3d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-02 08:55:46.000000 napari_cellseg3d-0.1.2/napari_cellseg3d.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-02 08:55:46.183704 napari_cellseg3d-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:58:23.473503 napari_cellseg3d-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10497 2024-05-13 08:58:23.473503 napari_cellseg3d-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7635 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:58:23.453503 napari_cellseg3d-0.2.0/napari_cellseg3d/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/napari_cellseg3d/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:58:23.457502 napari_cellseg3d-0.2.0/napari_cellseg3d/_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/napari_cellseg3d/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/napari_cellseg3d/_tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/napari_cellseg3d/_tests/fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:58:23.457502 napari_cellseg3d-0.2.0/napari_cellseg3d/_tests/res/
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/napari_cellseg3d/_tests/res/test.png
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/napari_cellseg3d/_tests/test_base_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/napari_cellseg3d/_tests/test_dock_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/napari_cellseg3d/_tests/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/napari_cellseg3d/_tests/test_inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/napari_cellseg3d/_tests/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/napari_cellseg3d/_tests/test_labels_correction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/napari_cellseg3d/_tests/test_model_framework.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/napari_cellseg3d/_tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/napari_cellseg3d/_tests/test_plugin_inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4127 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/napari_cellseg3d/_tests/test_plugin_training.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/napari_cellseg3d/_tests/test_plugin_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/napari_cellseg3d/_tests/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/napari_cellseg3d/_tests/test_review.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4318 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/napari_cellseg3d/_tests/test_training.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7335 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/napari_cellseg3d/_tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/napari_cellseg3d/_tests/test_weight_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/napari_cellseg3d/_tests/test_wnet_training.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:58:23.457502 napari_cellseg3d-0.2.0/napari_cellseg3d/code_models/
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/napari_cellseg3d/code_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9598 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/napari_cellseg3d/code_models/crf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30959 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/napari_cellseg3d/code_models/instance_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13712 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/napari_cellseg3d/code_models/model_framework.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:58:23.461502 napari_cellseg3d-0.2.0/napari_cellseg3d/code_models/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/napari_cellseg3d/code_models/models/TEMPLATE_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/napari_cellseg3d/code_models/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/napari_cellseg3d/code_models/models/model_SegResNet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/napari_cellseg3d/code_models/models/model_SwinUNetR.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/napari_cellseg3d/code_models/models/model_TRAILMAP.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/napari_cellseg3d/code_models/models/model_TRAILMAP_MS.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/napari_cellseg3d/code_models/models/model_VNet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/napari_cellseg3d/code_models/models/model_WNet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/napari_cellseg3d/code_models/models/model_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:58:23.461502 napari_cellseg3d-0.2.0/napari_cellseg3d/code_models/models/pretrained/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/napari_cellseg3d/code_models/models/pretrained/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/napari_cellseg3d/code_models/models/pretrained/pretrained_model_urls.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:58:23.461502 napari_cellseg3d-0.2.0/napari_cellseg3d/code_models/models/unet/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/napari_cellseg3d/code_models/models/unet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19683 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/napari_cellseg3d/code_models/models/unet/buildingblocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6032 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/napari_cellseg3d/code_models/models/unet/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:58:23.461502 napari_cellseg3d-0.2.0/napari_cellseg3d/code_models/models/wnet/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/napari_cellseg3d/code_models/models/wnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9107 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/napari_cellseg3d/code_models/models/wnet/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5065 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/napari_cellseg3d/code_models/models/wnet/soft_Ncuts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37499 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/napari_cellseg3d/code_models/worker_inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69600 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/napari_cellseg3d/code_models/worker_training.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11149 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/napari_cellseg3d/code_models/workers_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:58:23.465503 napari_cellseg3d-0.2.0/napari_cellseg3d/code_plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/napari_cellseg3d/code_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18865 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/napari_cellseg3d/code_plugins/plugin_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27266 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/napari_cellseg3d/code_plugins/plugin_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10606 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/napari_cellseg3d/code_plugins/plugin_crf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23870 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/napari_cellseg3d/code_plugins/plugin_crop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/napari_cellseg3d/code_plugins/plugin_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10859 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/napari_cellseg3d/code_plugins/plugin_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36534 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/napari_cellseg3d/code_plugins/plugin_model_inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62865 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/napari_cellseg3d/code_plugins/plugin_model_training.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16713 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/napari_cellseg3d/code_plugins/plugin_review.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10102 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/napari_cellseg3d/code_plugins/plugin_review_dock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7700 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/napari_cellseg3d/code_plugins/plugin_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12497 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/napari_cellseg3d/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:58:23.465503 napari_cellseg3d-0.2.0/napari_cellseg3d/dev_scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/napari_cellseg3d/dev_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14359 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/napari_cellseg3d/dev_scripts/artefact_labeling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29181 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/napari_cellseg3d/dev_scripts/colab_training.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12203 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/napari_cellseg3d/dev_scripts/correct_labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/napari_cellseg3d/dev_scripts/crop_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11993 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/napari_cellseg3d/dev_scripts/evaluate_labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6008 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/napari_cellseg3d/dev_scripts/remote_inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/napari_cellseg3d/dev_scripts/remote_training.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/napari_cellseg3d/dev_scripts/sliding_window_voronoi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/napari_cellseg3d/dev_scripts/thread_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/napari_cellseg3d/dev_scripts/whole_brain_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53880 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/napari_cellseg3d/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/napari_cellseg3d/napari.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/napari_cellseg3d/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:58:23.465503 napari_cellseg3d-0.2.0/napari_cellseg3d/res/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/napari_cellseg3d/res/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   495510 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/napari_cellseg3d/res/logo_alpha.png
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/napari_cellseg3d/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21552 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/napari_cellseg3d/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:58:23.469503 napari_cellseg3d-0.2.0/napari_cellseg3d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10497 2024-05-13 08:58:23.000000 napari_cellseg3d-0.2.0/napari_cellseg3d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-05-13 08:58:23.000000 napari_cellseg3d-0.2.0/napari_cellseg3d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 08:58:23.000000 napari_cellseg3d-0.2.0/napari_cellseg3d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-13 08:58:23.000000 napari_cellseg3d-0.2.0/napari_cellseg3d.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-13 08:58:23.000000 napari_cellseg3d-0.2.0/napari_cellseg3d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-13 08:58:23.000000 napari_cellseg3d-0.2.0/napari_cellseg3d.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-13 08:58:10.000000 napari_cellseg3d-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-13 08:58:23.473503 napari_cellseg3d-0.2.0/setup.cfg
```

### Comparing `napari_cellseg3d-0.1.2/LICENSE` & `napari_cellseg3d-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.2/PKG-INFO` & `napari_cellseg3d-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: napari_cellseg3d
-Version: 0.1.2
+Version: 0.2.0
 Summary: Plugin for cell segmentation in 3D
 Author-email: Cyril Achard <cyril.achard@epfl.ch>, Maxime Vidal <maxime.vidal@epfl.ch>, Mackenzie Mathis <mackenzie@post.harvard.edu>
 License: MIT
-Project-URL: Homepage, https://github.com/AdaptiveMotorControlLab/CellSeg3d
+Project-URL: Homepage, https://github.com/AdaptiveMotorControlLab/CellSeg3D
 Project-URL: Documentation, https://adaptivemotorcontrollab.github.io/cellseg3d-docs/res/welcome.html
-Project-URL: Issues, https://github.com/AdaptiveMotorControlLab/CellSeg3d/issues
+Project-URL: Issues, https://github.com/AdaptiveMotorControlLab/CellSeg3D/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Framework :: napari
 Classifier: Topic :: Software Development :: Testing
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -34,14 +34,20 @@
 Requires-Dist: torch>=1.11
 Requires-Dist: monai[einops,nibabel]>=0.9.0
 Requires-Dist: itk
 Requires-Dist: tqdm
 Requires-Dist: pyclesperanto-prototype
 Requires-Dist: tqdm
 Requires-Dist: matplotlib
+Provides-Extra: pyqt5
+Requires-Dist: pyqt5; extra == "pyqt5"
+Provides-Extra: pyside2
+Requires-Dist: pyside2; extra == "pyside2"
+Provides-Extra: pyside6
+Requires-Dist: pyside6; extra == "pyside6"
 Provides-Extra: onnx-cpu
 Requires-Dist: onnx; extra == "onnx-cpu"
 Requires-Dist: onnxruntime; extra == "onnx-cpu"
 Provides-Extra: onnx-gpu
 Requires-Dist: onnx; extra == "onnx-gpu"
 Requires-Dist: onnxruntime-gpu; extra == "onnx-gpu"
 Provides-Extra: wandb
@@ -61,112 +67,125 @@
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: coverage; extra == "test"
 Requires-Dist: tox; extra == "test"
 Requires-Dist: twine; extra == "test"
 Requires-Dist: onnx; extra == "test"
 Requires-Dist: onnxruntime; extra == "test"
 
-# napari-cellseg3D: a napari plug-in for direct 3D cell segmentation with deep learning
-
+# CellSeg3D: self-supervised (and supervised) 3D cell segmentation
 <img src="https://images.squarespace-cdn.com/content/v1/57f6d51c9f74566f55ecf271/838605d0-9723-4e43-83cd-6dbfe4adf36b/cellseg-logo.png?format=1500w" title="cellseg3d" alt="cellseg3d logo" width="350" align="right" vspace = "80"/>
 
 <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
-[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/AdaptiveMotorControlLab/CellSeg3d/raw/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/napari-cellseg3d.svg?color=green)](https://pypi.org/project/napari-cellseg3d)
+[![Downloads](https://static.pepy.tech/badge/napari-cellseg3d)](https://pepy.tech/project/napari-cellseg3d)
+[![Downloads](https://static.pepy.tech/badge/napari-cellseg3d/month)](https://pepy.tech/project/napari-cellseg3d)
+[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/AdaptiveMotorControlLab/CellSeg3D/raw/main/LICENSE)
 [![Python Version](https://img.shields.io/pypi/pyversions/napari-cellseg-annotator.svg?color=green)](https://python.org)
-[![codecov](https://codecov.io/gh/AdaptiveMotorControlLab/CellSeg3d/branch/main/graph/badge.svg?token=hzUcn3XN8F)](https://codecov.io/gh/AdaptiveMotorControlLab/CellSeg3d)
+[![codecov](https://codecov.io/gh/AdaptiveMotorControlLab/CellSeg3D/branch/main/graph/badge.svg?token=hzUcn3XN8F)](https://codecov.io/gh/AdaptiveMotorControlLab/CellSeg3D)
 [![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-cellseg3d)](https://www.napari-hub.org/plugins/napari-cellseg3d)
 
-A napari plugin for 3D cell segmentation: training, inference, and data review. In particular, this project was developed for analysis of mesoSPIM-acquired (cleared tissue + lightsheet) datasets.
+- A napari plugin for 3D cell segmentation: training, inference, and data review. In particular, this project was developed for analysis of mesoSPIM-acquired (cleared tissue + lightsheet) datasets.
 
-**Help us make the code better by reporting issues and adding your feature requests!**
+![demo](https://images.squarespace-cdn.com/content/v1/57f6d51c9f74566f55ecf271/0d16a71b-3ff2-477a-9d83-18d96cb1ce28/full_demo.gif?format=500w)
+
+## Installation
+
+ 💻 See the [Installation page] in the documentation for detailed instructions.
+
+## Documentation
+
+📚 A lot of documentation is available at https://AdaptiveMotorControlLab.github.io/CellSeg3D
+
+You can also generate docs by running ``make html`` in the docs/ folder.
+
+## Quick Start
 
-----------------------------------
+To use the plugin, please run:
+```
+napari
+```
+Then go into Plugins > napari-cellseg3d, and choose which tool to use.
+
+- **Review (label)**: This module allows you to review your labels, from predictions or manual labeling, and correct them if needed. It then saves the status of each file in a csv, for easier monitoring.
+- **Inference**: This module allows you to use pre-trained segmentation algorithms on volumes to automatically label cells and compute statistics.
+- **Train**:  This module allows you to train segmentation algorithms from labeled volumes.
+- **Utilities**: This module allows you to perform several actions like cropping your volumes and labels dynamically, by selecting a fixed size volume and moving it around the image; fragment images into smaller cubes for training; or converting labels from instance to segmentation and the opposite.
 
 ## News
 
-**New version : v0.1.2**
+**New version : v0.2.0**
 
-- Fixed manifest issue for PyPi
+- Changed project name to "napari_cellseg3d" to avoid setuptools deprecation
+- Small API changes for training/inference from a script
+- Some fixes to WandB integration ad csv saving after training
 
 Previous additions :
 
+- v0.1.2 :Fixed manifest issue for PyPi
 - Improved training interface
-- Unsupervised model : WNet
-  - Generate labels directly from raw data !
-  - Can be trained in napari directly or in Colab
+- Unsupervised model : WNet3D
+  - Generate labels directly from raw data!
+  - Can be trained in napari directly or in Google Colab
   - Pretrained weights for mesoSPIM whole-brain cell segmentation
 - WandB support (install wandb and login to use automatically when training)
 - Remade and improved documentation
   - Moved to Jupyter Book
   - Dedicated installation page, and working ARM64 install for macOS Silicon users
 - New utilities
 - Many small improvements and many bug fixes
 
-## Demo
-
-![demo](https://images.squarespace-cdn.com/content/v1/57f6d51c9f74566f55ecf271/0d16a71b-3ff2-477a-9d83-18d96cb1ce28/full_demo.gif?format=500w)
-
-## Installation
 
-See the [Installation page] in the documentation for detailed instructions.
 
-### M1 Mac users
+### Install note for ARM64 (Silicon) Mac users
 
 To avoid issues when installing on the ARM64 architecture, please follow these steps.
 
-1) Create a new conda env using the provided conda/napari_cellseg3d_m1.yml file :
+1) Create a new conda env using the provided conda/napari_CellSeg3D_ARM64.yml file :
 
         git clone https://github.com/AdaptiveMotorControlLab/CellSeg3d.git
         cd CellSeg3d
-        conda env create -f conda/napari_cellseg3d_m1.yml
-        conda activate napari_cellseg3d_m1
+        conda env create -f conda/CellSeg3D_ARM64.yml
+        conda activate napari_CellSeg3D_ARM64
 
-2) Install the plugin.
-   From repository root folder, run :
 
-        pip install -e .
-   OR directly via PyPi :
+2) Install a Qt backend (PySide or PyQt5)
+3) Launch napari, the plugin should be available in the plugins menu.
 
-        pip install napari-cellseg3d
 
-   OR directly via [napari-hub] (see Installation section above)
-
-## Documentation
-
-Available at https://AdaptiveMotorControlLab.github.io/CellSeg3d
-
-You can also generate docs by running ``make html`` in the docs/ folder.
-
-## Usage
-
-To use the plugin, please run:
-```
-napari
-```
-Then go into Plugins > napari-cellseg3d, and choose which tool to use.
-
-- **Review**: This module allows you to review your labels, from predictions or manual labeling, and correct them if needed. It then saves the status of each file in a csv, for easier monitoring.
-- **Inference**: This module allows you to use pre-trained segmentation algorithms on volumes to automatically label cells and compute statistics.
-- **Train**:  This module allows you to train segmentation algorithms from labeled volumes.
-- **Utilities**: This module allows you to perform several actions like cropping your volumes and labels dynamically, by selecting a fixed size volume and moving it around the image; computing prediction scores from ground truth and predicition labels; or converting labels from instance to segmentation and the opposite.
 
 ## Requirements
 
 **Python 3.8 or 3.9 required.**
 Requires **[napari]**, **[PyTorch]** and **[MONAI]**.
+Compatible with Windows, MacOS and Linux.
+Installation should not take more than 30 minutes, depending on your internet connection.
 
 For PyTorch, please see [the PyTorch website for installation instructions].
 
 A CUDA-capable GPU is not needed but very strongly recommended, especially for training.
 
 If you get errors from MONAI regarding missing readers, please see [MONAI's optional dependencies] page for instructions on getting the readers required by your images.
 
+## Quick demo
+
+After installation, you can run the plugin by running:
+
+        napari
+
+and launching the plugin from the Plugins menu.
+You may use the test volume in the `examples` folder to test the inference and review tools.
+This should run in far less than five minutes on a modern computer.
+
+You may also find a demo Colab notebook in the `notebooks` folder.
+
 ## Issues
 
+**Help us make the code better by reporting issues and adding your feature requests!**
+
+
 If you encounter any problems, please [file an issue] along with a detailed description.
 
 ## Testing
 
 Before testing, install all requirements using ``pip install napari-cellseg3d[test]``.
 
 ``pydensecrf`` is also required for testing.
@@ -193,31 +212,31 @@
 
 Distributed under the terms of the [MIT] license.
 
 "napari-cellseg3d" is free and open source software.
 
 [napari-hub]: https://www.napari-hub.org/plugins/napari-cellseg3d
 
-[file an issue]: https://github.com/AdaptiveMotorControlLab/CellSeg3d/issues
+[file an issue]: https://github.com/AdaptiveMotorControlLab/CellSeg3D/issues
 [napari]: https://github.com/napari/napari
 [Cookiecutter]: https://github.com/audreyr/cookiecutter
 [@napari]: https://github.com/napari
 [MIT]: http://opensource.org/licenses/MIT
 [cookiecutter-napari-plugin]: https://github.com/napari/cookiecutter-napari-plugin
 [tox]: https://tox.readthedocs.io/en/latest/
 [pip]: https://pypi.org/project/pip/
 [PyPI]: https://pypi.org/
-[Installation page]: https://adaptivemotorcontrollab.github.io/CellSeg3d/source/guides/installation_guide.html
+[Installation page]: https://adaptivemotorcontrollab.github.io/CellSeg3D/source/guides/installation_guide.html
 [the PyTorch website for installation instructions]: https://pytorch.org/get-started/locally/
 [PyTorch]: https://pytorch.org/get-started/locally/
 [MONAI's optional dependencies]: https://docs.monai.io/en/stable/installation.html#installing-the-recommended-dependencies
 [MONAI]: https://docs.monai.io/en/stable/installation.html#installing-the-recommended-dependencies
 
 ## Acknowledgements
 
-This plugin was developed by Cyril Achard, Maxime Vidal, Mackenzie Mathis.
-This work was funded, in part, from the Wyss Center to the [Mathis Laboratory of Adaptive Motor Control](https://www.mackenziemathislab.org/).
+This plugin was developed by originally Cyril Achard, Maxime Vidal, Mackenzie Mathis.
+This work was funded, in part, from the Wyss Center to the [Mathis Laboratory of Adaptive Intelligence](https://www.mackenziemathislab.org/).
 Please refer to the documentation for full acknowledgements.
 
 ## Plugin base
 
 This [napari] plugin was generated with [Cookiecutter] using [@napari]'s [cookiecutter-napari-plugin] template.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: napari_cellseg3d Version: 0.1.2 Summary: Plugin for
+Metadata-Version: 2.1 Name: napari_cellseg3d Version: 0.2.0 Summary: Plugin for
 cell segmentation in 3D Author-email: Cyril Achard
 epfl.ch>, Maxime Vidal
 epfl.ch>, Mackenzie Mathis
 post.harvard.edu> License: MIT Project-URL: Homepage, https://github.com/
-AdaptiveMotorControlLab/CellSeg3d Project-URL: Documentation, https://
+AdaptiveMotorControlLab/CellSeg3D Project-URL: Documentation, https://
 adaptivemotorcontrollab.github.io/cellseg3d-docs/res/welcome.html Project-URL:
-Issues, https://github.com/AdaptiveMotorControlLab/CellSeg3d/issues Classifier:
+Issues, https://github.com/AdaptiveMotorControlLab/CellSeg3D/issues Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Science/
 Research Classifier: Framework :: napari Classifier: Topic :: Software
 Development :: Testing Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Operating System :: OS
 Independent Classifier: License :: OSI Approved :: MIT License Classifier:
@@ -18,104 +18,117 @@
 Engineering :: Visualization Requires-Python: >=3.8 Description-Content-Type:
 text/markdown License-File: LICENSE Requires-Dist: numpy Requires-Dist: napari
 [all]>=0.4.14 Requires-Dist: QtPy Requires-Dist: scikit-image>=0.19.2 Requires-
 Dist: matplotlib>=3.4.1 Requires-Dist: tifffile>=2022.2.9 Requires-Dist:
 imagecodecs>=2023.3.16 Requires-Dist: torch>=1.11 Requires-Dist: monai
 [einops,nibabel]>=0.9.0 Requires-Dist: itk Requires-Dist: tqdm Requires-Dist:
 pyclesperanto-prototype Requires-Dist: tqdm Requires-Dist: matplotlib Provides-
-Extra: onnx-cpu Requires-Dist: onnx; extra == "onnx-cpu" Requires-Dist:
-onnxruntime; extra == "onnx-cpu" Provides-Extra: onnx-gpu Requires-Dist: onnx;
-extra == "onnx-gpu" Requires-Dist: onnxruntime-gpu; extra == "onnx-gpu"
-Provides-Extra: wandb Requires-Dist: wandb; extra == "wandb" Provides-Extra:
-dev Requires-Dist: isort; extra == "dev" Requires-Dist: black; extra == "dev"
-Requires-Dist: ruff; extra == "dev" Requires-Dist: pre-commit; extra == "dev"
-Requires-Dist: tuna; extra == "dev" Requires-Dist: twine; extra == "dev"
-Provides-Extra: docs Requires-Dist: jupyter-book; extra == "docs" Provides-
-Extra: test Requires-Dist: pytest; extra == "test" Requires-Dist: pytest_qt;
-extra == "test" Requires-Dist: pytest-cov; extra == "test" Requires-Dist:
-coverage; extra == "test" Requires-Dist: tox; extra == "test" Requires-Dist:
-twine; extra == "test" Requires-Dist: onnx; extra == "test" Requires-Dist:
-onnxruntime; extra == "test" # napari-cellseg3D: a napari plug-in for direct 3D
-cell segmentation with deep learning [cellseg3d logo]_[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_][!
-[License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://
-github.com/AdaptiveMotorControlLab/CellSeg3d/raw/main/LICENSE) [![PyPI](https:/
-/img.shields.io/pypi/v/napari-cellseg3d.svg?color=green)](https://pypi.org/
-project/napari-cellseg3d) [![Python Version](https://img.shields.io/pypi/
-pyversions/napari-cellseg-annotator.svg?color=green)](https://python.org) [!
-[codecov](https://codecov.io/gh/AdaptiveMotorControlLab/CellSeg3d/branch/main/
-graph/badge.svg?token=hzUcn3XN8F)](https://codecov.io/gh/
-AdaptiveMotorControlLab/CellSeg3d) [![napari hub](https://img.shields.io/
+Extra: pyqt5 Requires-Dist: pyqt5; extra == "pyqt5" Provides-Extra: pyside2
+Requires-Dist: pyside2; extra == "pyside2" Provides-Extra: pyside6 Requires-
+Dist: pyside6; extra == "pyside6" Provides-Extra: onnx-cpu Requires-Dist: onnx;
+extra == "onnx-cpu" Requires-Dist: onnxruntime; extra == "onnx-cpu" Provides-
+Extra: onnx-gpu Requires-Dist: onnx; extra == "onnx-gpu" Requires-Dist:
+onnxruntime-gpu; extra == "onnx-gpu" Provides-Extra: wandb Requires-Dist:
+wandb; extra == "wandb" Provides-Extra: dev Requires-Dist: isort; extra ==
+"dev" Requires-Dist: black; extra == "dev" Requires-Dist: ruff; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev" Requires-Dist: tuna; extra == "dev"
+Requires-Dist: twine; extra == "dev" Provides-Extra: docs Requires-Dist:
+jupyter-book; extra == "docs" Provides-Extra: test Requires-Dist: pytest; extra
+== "test" Requires-Dist: pytest_qt; extra == "test" Requires-Dist: pytest-cov;
+extra == "test" Requires-Dist: coverage; extra == "test" Requires-Dist: tox;
+extra == "test" Requires-Dist: twine; extra == "test" Requires-Dist: onnx;
+extra == "test" Requires-Dist: onnxruntime; extra == "test" # CellSeg3D: self-
+supervised (and supervised) 3D cell segmentation [cellseg3d logo]_[_C_o_d_e_ _s_t_y_l_e_:
+_b_l_a_c_k_][![PyPI](https://img.shields.io/pypi/v/napari-cellseg3d.svg?color=green)]
+(https://pypi.org/project/napari-cellseg3d) [![Downloads](https://
+static.pepy.tech/badge/napari-cellseg3d)](https://pepy.tech/project/napari-
+cellseg3d) [![Downloads](https://static.pepy.tech/badge/napari-cellseg3d/
+month)](https://pepy.tech/project/napari-cellseg3d) [![License: MIT](https://
+img.shields.io/badge/License-MIT-blue.svg)](https://github.com/
+AdaptiveMotorControlLab/CellSeg3D/raw/main/LICENSE) [![Python Version](https://
+img.shields.io/pypi/pyversions/napari-cellseg-annotator.svg?color=green)]
+(https://python.org) [![codecov](https://codecov.io/gh/AdaptiveMotorControlLab/
+CellSeg3D/branch/main/graph/badge.svg?token=hzUcn3XN8F)](https://codecov.io/gh/
+AdaptiveMotorControlLab/CellSeg3D) [![napari hub](https://img.shields.io/
 endpoint?url=https://api.napari-hub.org/shields/napari-cellseg3d)](https://
-www.napari-hub.org/plugins/napari-cellseg3d) A napari plugin for 3D cell
+www.napari-hub.org/plugins/napari-cellseg3d) - A napari plugin for 3D cell
 segmentation: training, inference, and data review. In particular, this project
 was developed for analysis of mesoSPIM-acquired (cleared tissue + lightsheet)
-datasets. **Help us make the code better by reporting issues and adding your
-feature requests!** ---------------------------------- ## News **New version :
-v0.1.2** - Fixed manifest issue for PyPi Previous additions : - Improved
-training interface - Unsupervised model : WNet - Generate labels directly from
-raw data ! - Can be trained in napari directly or in Colab - Pretrained weights
-for mesoSPIM whole-brain cell segmentation - WandB support (install wandb and
-login to use automatically when training) - Remade and improved documentation -
-Moved to Jupyter Book - Dedicated installation page, and working ARM64 install
-for macOS Silicon users - New utilities - Many small improvements and many bug
-fixes ## Demo ![demo](https://images.squarespace-cdn.com/content/v1/
+datasets. ![demo](https://images.squarespace-cdn.com/content/v1/
 57f6d51c9f74566f55ecf271/0d16a71b-3ff2-477a-9d83-18d96cb1ce28/
-full_demo.gif?format=500w) ## Installation See the [Installation page] in the
-documentation for detailed instructions. ### M1 Mac users To avoid issues when
-installing on the ARM64 architecture, please follow these steps. 1) Create a
-new conda env using the provided conda/napari_cellseg3d_m1.yml file : git clone
-https://github.com/AdaptiveMotorControlLab/CellSeg3d.git cd CellSeg3d conda env
-create -f conda/napari_cellseg3d_m1.yml conda activate napari_cellseg3d_m1 2)
-Install the plugin. From repository root folder, run : pip install -e . OR
-directly via PyPi : pip install napari-cellseg3d OR directly via [napari-hub]
-(see Installation section above) ## Documentation Available at https://
-AdaptiveMotorControlLab.github.io/CellSeg3d You can also generate docs by
-running ``make html`` in the docs/ folder. ## Usage To use the plugin, please
-run: ``` napari ``` Then go into Plugins > napari-cellseg3d, and choose which
-tool to use. - **Review**: This module allows you to review your labels, from
-predictions or manual labeling, and correct them if needed. It then saves the
-status of each file in a csv, for easier monitoring. - **Inference**: This
-module allows you to use pre-trained segmentation algorithms on volumes to
-automatically label cells and compute statistics. - **Train**: This module
-allows you to train segmentation algorithms from labeled volumes. -
-**Utilities**: This module allows you to perform several actions like cropping
-your volumes and labels dynamically, by selecting a fixed size volume and
-moving it around the image; computing prediction scores from ground truth and
-predicition labels; or converting labels from instance to segmentation and the
-opposite. ## Requirements **Python 3.8 or 3.9 required.** Requires **
-[napari]**, **[PyTorch]** and **[MONAI]**. For PyTorch, please see [the PyTorch
-website for installation instructions]. A CUDA-capable GPU is not needed but
-very strongly recommended, especially for training. If you get errors from
-MONAI regarding missing readers, please see [MONAI's optional dependencies]
-page for instructions on getting the readers required by your images. ## Issues
-If you encounter any problems, please [file an issue] along with a detailed
-description. ## Testing Before testing, install all requirements using ``pip
-install napari-cellseg3d[test]``. ``pydensecrf`` is also required for testing.
-To run tests locally: - Locally : run ``pytest`` in the plugin folder - Locally
-with coverage : In the plugin folder, run ``coverage run --
-source=napari_cellseg3d -m pytest`` then ``coverage xml`` to generate a .xml
-coverage file. - With tox : run ``tox`` in the plugin folder (will simulate
-tests with several python and OS configs, requires substantial storage space)
-## Contributing Contributions are very welcome. Please ensure the coverage at
-least stays the same before you submit a pull request. For local installation
-from Github cloning, please run: ``` pip install -e . ``` ## License
-Distributed under the terms of the [MIT] license. "napari-cellseg3d" is free
-and open source software. [napari-hub]: https://www.napari-hub.org/plugins/
-napari-cellseg3d [file an issue]: https://github.com/AdaptiveMotorControlLab/
-CellSeg3d/issues [napari]: https://github.com/napari/napari [Cookiecutter]:
-https://github.com/audreyr/cookiecutter [@napari]: https://github.com/napari
-[MIT]: http://opensource.org/licenses/MIT [cookiecutter-napari-plugin]: https:/
-/github.com/napari/cookiecutter-napari-plugin [tox]: https://
-tox.readthedocs.io/en/latest/ [pip]: https://pypi.org/project/pip/ [PyPI]:
-https://pypi.org/ [Installation page]: https://
-adaptivemotorcontrollab.github.io/CellSeg3d/source/guides/
+full_demo.gif?format=500w) ## Installation ð» See the [Installation page] in
+the documentation for detailed instructions. ## Documentation ð A lot of
+documentation is available at https://AdaptiveMotorControlLab.github.io/
+CellSeg3D You can also generate docs by running ``make html`` in the docs/
+folder. ## Quick Start To use the plugin, please run: ``` napari ``` Then go
+into Plugins > napari-cellseg3d, and choose which tool to use. - **Review
+(label)**: This module allows you to review your labels, from predictions or
+manual labeling, and correct them if needed. It then saves the status of each
+file in a csv, for easier monitoring. - **Inference**: This module allows you
+to use pre-trained segmentation algorithms on volumes to automatically label
+cells and compute statistics. - **Train**: This module allows you to train
+segmentation algorithms from labeled volumes. - **Utilities**: This module
+allows you to perform several actions like cropping your volumes and labels
+dynamically, by selecting a fixed size volume and moving it around the image;
+fragment images into smaller cubes for training; or converting labels from
+instance to segmentation and the opposite. ## News **New version : v0.2.0** -
+Changed project name to "napari_cellseg3d" to avoid setuptools deprecation -
+Small API changes for training/inference from a script - Some fixes to WandB
+integration ad csv saving after training Previous additions : - v0.1.2 :Fixed
+manifest issue for PyPi - Improved training interface - Unsupervised model :
+WNet3D - Generate labels directly from raw data! - Can be trained in napari
+directly or in Google Colab - Pretrained weights for mesoSPIM whole-brain cell
+segmentation - WandB support (install wandb and login to use automatically when
+training) - Remade and improved documentation - Moved to Jupyter Book -
+Dedicated installation page, and working ARM64 install for macOS Silicon users
+- New utilities - Many small improvements and many bug fixes ### Install note
+for ARM64 (Silicon) Mac users To avoid issues when installing on the ARM64
+architecture, please follow these steps. 1) Create a new conda env using the
+provided conda/napari_CellSeg3D_ARM64.yml file : git clone https://github.com/
+AdaptiveMotorControlLab/CellSeg3d.git cd CellSeg3d conda env create -f conda/
+CellSeg3D_ARM64.yml conda activate napari_CellSeg3D_ARM64 2) Install a Qt
+backend (PySide or PyQt5) 3) Launch napari, the plugin should be available in
+the plugins menu. ## Requirements **Python 3.8 or 3.9 required.** Requires **
+[napari]**, **[PyTorch]** and **[MONAI]**. Compatible with Windows, MacOS and
+Linux. Installation should not take more than 30 minutes, depending on your
+internet connection. For PyTorch, please see [the PyTorch website for
+installation instructions]. A CUDA-capable GPU is not needed but very strongly
+recommended, especially for training. If you get errors from MONAI regarding
+missing readers, please see [MONAI's optional dependencies] page for
+instructions on getting the readers required by your images. ## Quick demo
+After installation, you can run the plugin by running: napari and launching the
+plugin from the Plugins menu. You may use the test volume in the `examples`
+folder to test the inference and review tools. This should run in far less than
+five minutes on a modern computer. You may also find a demo Colab notebook in
+the `notebooks` folder. ## Issues **Help us make the code better by reporting
+issues and adding your feature requests!** If you encounter any problems,
+please [file an issue] along with a detailed description. ## Testing Before
+testing, install all requirements using ``pip install napari-cellseg3d[test]``.
+``pydensecrf`` is also required for testing. To run tests locally: - Locally :
+run ``pytest`` in the plugin folder - Locally with coverage : In the plugin
+folder, run ``coverage run --source=napari_cellseg3d -m pytest`` then
+``coverage xml`` to generate a .xml coverage file. - With tox : run ``tox`` in
+the plugin folder (will simulate tests with several python and OS configs,
+requires substantial storage space) ## Contributing Contributions are very
+welcome. Please ensure the coverage at least stays the same before you submit a
+pull request. For local installation from Github cloning, please run: ``` pip
+install -e . ``` ## License Distributed under the terms of the [MIT] license.
+"napari-cellseg3d" is free and open source software. [napari-hub]: https://
+www.napari-hub.org/plugins/napari-cellseg3d [file an issue]: https://
+github.com/AdaptiveMotorControlLab/CellSeg3D/issues [napari]: https://
+github.com/napari/napari [Cookiecutter]: https://github.com/audreyr/
+cookiecutter [@napari]: https://github.com/napari [MIT]: http://opensource.org/
+licenses/MIT [cookiecutter-napari-plugin]: https://github.com/napari/
+cookiecutter-napari-plugin [tox]: https://tox.readthedocs.io/en/latest/ [pip]:
+https://pypi.org/project/pip/ [PyPI]: https://pypi.org/ [Installation page]:
+https://adaptivemotorcontrollab.github.io/CellSeg3D/source/guides/
 installation_guide.html [the PyTorch website for installation instructions]:
 https://pytorch.org/get-started/locally/ [PyTorch]: https://pytorch.org/get-
 started/locally/ [MONAI's optional dependencies]: https://docs.monai.io/en/
 stable/installation.html#installing-the-recommended-dependencies [MONAI]:
 https://docs.monai.io/en/stable/installation.html#installing-the-recommended-
-dependencies ## Acknowledgements This plugin was developed by Cyril Achard,
-Maxime Vidal, Mackenzie Mathis. This work was funded, in part, from the Wyss
-Center to the [Mathis Laboratory of Adaptive Motor Control](https://
+dependencies ## Acknowledgements This plugin was developed by originally Cyril
+Achard, Maxime Vidal, Mackenzie Mathis. This work was funded, in part, from the
+Wyss Center to the [Mathis Laboratory of Adaptive Intelligence](https://
 www.mackenziemathislab.org/). Please refer to the documentation for full
 acknowledgements. ## Plugin base This [napari] plugin was generated with
 [Cookiecutter] using [@napari]'s [cookiecutter-napari-plugin] template.
```

### Comparing `napari_cellseg3d-0.1.2/README.md` & `napari_cellseg3d-0.2.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,105 +1,118 @@
-# napari-cellseg3D: a napari plug-in for direct 3D cell segmentation with deep learning
-
+# CellSeg3D: self-supervised (and supervised) 3D cell segmentation
 <img src="https://images.squarespace-cdn.com/content/v1/57f6d51c9f74566f55ecf271/838605d0-9723-4e43-83cd-6dbfe4adf36b/cellseg-logo.png?format=1500w" title="cellseg3d" alt="cellseg3d logo" width="350" align="right" vspace = "80"/>
 
 <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
-[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/AdaptiveMotorControlLab/CellSeg3d/raw/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/napari-cellseg3d.svg?color=green)](https://pypi.org/project/napari-cellseg3d)
+[![Downloads](https://static.pepy.tech/badge/napari-cellseg3d)](https://pepy.tech/project/napari-cellseg3d)
+[![Downloads](https://static.pepy.tech/badge/napari-cellseg3d/month)](https://pepy.tech/project/napari-cellseg3d)
+[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/AdaptiveMotorControlLab/CellSeg3D/raw/main/LICENSE)
 [![Python Version](https://img.shields.io/pypi/pyversions/napari-cellseg-annotator.svg?color=green)](https://python.org)
-[![codecov](https://codecov.io/gh/AdaptiveMotorControlLab/CellSeg3d/branch/main/graph/badge.svg?token=hzUcn3XN8F)](https://codecov.io/gh/AdaptiveMotorControlLab/CellSeg3d)
+[![codecov](https://codecov.io/gh/AdaptiveMotorControlLab/CellSeg3D/branch/main/graph/badge.svg?token=hzUcn3XN8F)](https://codecov.io/gh/AdaptiveMotorControlLab/CellSeg3D)
 [![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-cellseg3d)](https://www.napari-hub.org/plugins/napari-cellseg3d)
 
-A napari plugin for 3D cell segmentation: training, inference, and data review. In particular, this project was developed for analysis of mesoSPIM-acquired (cleared tissue + lightsheet) datasets.
+- A napari plugin for 3D cell segmentation: training, inference, and data review. In particular, this project was developed for analysis of mesoSPIM-acquired (cleared tissue + lightsheet) datasets.
 
-**Help us make the code better by reporting issues and adding your feature requests!**
+![demo](https://images.squarespace-cdn.com/content/v1/57f6d51c9f74566f55ecf271/0d16a71b-3ff2-477a-9d83-18d96cb1ce28/full_demo.gif?format=500w)
+
+## Installation
+
+ 💻 See the [Installation page] in the documentation for detailed instructions.
+
+## Documentation
+
+📚 A lot of documentation is available at https://AdaptiveMotorControlLab.github.io/CellSeg3D
+
+You can also generate docs by running ``make html`` in the docs/ folder.
+
+## Quick Start
 
-----------------------------------
+To use the plugin, please run:
+```
+napari
+```
+Then go into Plugins > napari-cellseg3d, and choose which tool to use.
+
+- **Review (label)**: This module allows you to review your labels, from predictions or manual labeling, and correct them if needed. It then saves the status of each file in a csv, for easier monitoring.
+- **Inference**: This module allows you to use pre-trained segmentation algorithms on volumes to automatically label cells and compute statistics.
+- **Train**:  This module allows you to train segmentation algorithms from labeled volumes.
+- **Utilities**: This module allows you to perform several actions like cropping your volumes and labels dynamically, by selecting a fixed size volume and moving it around the image; fragment images into smaller cubes for training; or converting labels from instance to segmentation and the opposite.
 
 ## News
 
-**New version : v0.1.2**
+**New version : v0.2.0**
 
-- Fixed manifest issue for PyPi
+- Changed project name to "napari_cellseg3d" to avoid setuptools deprecation
+- Small API changes for training/inference from a script
+- Some fixes to WandB integration ad csv saving after training
 
 Previous additions :
 
+- v0.1.2 :Fixed manifest issue for PyPi
 - Improved training interface
-- Unsupervised model : WNet
-  - Generate labels directly from raw data !
-  - Can be trained in napari directly or in Colab
+- Unsupervised model : WNet3D
+  - Generate labels directly from raw data!
+  - Can be trained in napari directly or in Google Colab
   - Pretrained weights for mesoSPIM whole-brain cell segmentation
 - WandB support (install wandb and login to use automatically when training)
 - Remade and improved documentation
   - Moved to Jupyter Book
   - Dedicated installation page, and working ARM64 install for macOS Silicon users
 - New utilities
 - Many small improvements and many bug fixes
 
-## Demo
-
-![demo](https://images.squarespace-cdn.com/content/v1/57f6d51c9f74566f55ecf271/0d16a71b-3ff2-477a-9d83-18d96cb1ce28/full_demo.gif?format=500w)
-
-## Installation
 
-See the [Installation page] in the documentation for detailed instructions.
 
-### M1 Mac users
+### Install note for ARM64 (Silicon) Mac users
 
 To avoid issues when installing on the ARM64 architecture, please follow these steps.
 
-1) Create a new conda env using the provided conda/napari_cellseg3d_m1.yml file :
+1) Create a new conda env using the provided conda/napari_CellSeg3D_ARM64.yml file :
 
         git clone https://github.com/AdaptiveMotorControlLab/CellSeg3d.git
         cd CellSeg3d
-        conda env create -f conda/napari_cellseg3d_m1.yml
-        conda activate napari_cellseg3d_m1
+        conda env create -f conda/CellSeg3D_ARM64.yml
+        conda activate napari_CellSeg3D_ARM64
 
-2) Install the plugin.
-   From repository root folder, run :
 
-        pip install -e .
-   OR directly via PyPi :
+2) Install a Qt backend (PySide or PyQt5)
+3) Launch napari, the plugin should be available in the plugins menu.
 
-        pip install napari-cellseg3d
 
-   OR directly via [napari-hub] (see Installation section above)
-
-## Documentation
-
-Available at https://AdaptiveMotorControlLab.github.io/CellSeg3d
-
-You can also generate docs by running ``make html`` in the docs/ folder.
-
-## Usage
-
-To use the plugin, please run:
-```
-napari
-```
-Then go into Plugins > napari-cellseg3d, and choose which tool to use.
-
-- **Review**: This module allows you to review your labels, from predictions or manual labeling, and correct them if needed. It then saves the status of each file in a csv, for easier monitoring.
-- **Inference**: This module allows you to use pre-trained segmentation algorithms on volumes to automatically label cells and compute statistics.
-- **Train**:  This module allows you to train segmentation algorithms from labeled volumes.
-- **Utilities**: This module allows you to perform several actions like cropping your volumes and labels dynamically, by selecting a fixed size volume and moving it around the image; computing prediction scores from ground truth and predicition labels; or converting labels from instance to segmentation and the opposite.
 
 ## Requirements
 
 **Python 3.8 or 3.9 required.**
 Requires **[napari]**, **[PyTorch]** and **[MONAI]**.
+Compatible with Windows, MacOS and Linux.
+Installation should not take more than 30 minutes, depending on your internet connection.
 
 For PyTorch, please see [the PyTorch website for installation instructions].
 
 A CUDA-capable GPU is not needed but very strongly recommended, especially for training.
 
 If you get errors from MONAI regarding missing readers, please see [MONAI's optional dependencies] page for instructions on getting the readers required by your images.
 
+## Quick demo
+
+After installation, you can run the plugin by running:
+
+        napari
+
+and launching the plugin from the Plugins menu.
+You may use the test volume in the `examples` folder to test the inference and review tools.
+This should run in far less than five minutes on a modern computer.
+
+You may also find a demo Colab notebook in the `notebooks` folder.
+
 ## Issues
 
+**Help us make the code better by reporting issues and adding your feature requests!**
+
+
 If you encounter any problems, please [file an issue] along with a detailed description.
 
 ## Testing
 
 Before testing, install all requirements using ``pip install napari-cellseg3d[test]``.
 
 ``pydensecrf`` is also required for testing.
@@ -126,31 +139,31 @@
 
 Distributed under the terms of the [MIT] license.
 
 "napari-cellseg3d" is free and open source software.
 
 [napari-hub]: https://www.napari-hub.org/plugins/napari-cellseg3d
 
-[file an issue]: https://github.com/AdaptiveMotorControlLab/CellSeg3d/issues
+[file an issue]: https://github.com/AdaptiveMotorControlLab/CellSeg3D/issues
 [napari]: https://github.com/napari/napari
 [Cookiecutter]: https://github.com/audreyr/cookiecutter
 [@napari]: https://github.com/napari
 [MIT]: http://opensource.org/licenses/MIT
 [cookiecutter-napari-plugin]: https://github.com/napari/cookiecutter-napari-plugin
 [tox]: https://tox.readthedocs.io/en/latest/
 [pip]: https://pypi.org/project/pip/
 [PyPI]: https://pypi.org/
-[Installation page]: https://adaptivemotorcontrollab.github.io/CellSeg3d/source/guides/installation_guide.html
+[Installation page]: https://adaptivemotorcontrollab.github.io/CellSeg3D/source/guides/installation_guide.html
 [the PyTorch website for installation instructions]: https://pytorch.org/get-started/locally/
 [PyTorch]: https://pytorch.org/get-started/locally/
 [MONAI's optional dependencies]: https://docs.monai.io/en/stable/installation.html#installing-the-recommended-dependencies
 [MONAI]: https://docs.monai.io/en/stable/installation.html#installing-the-recommended-dependencies
 
 ## Acknowledgements
 
-This plugin was developed by Cyril Achard, Maxime Vidal, Mackenzie Mathis.
-This work was funded, in part, from the Wyss Center to the [Mathis Laboratory of Adaptive Motor Control](https://www.mackenziemathislab.org/).
+This plugin was developed by originally Cyril Achard, Maxime Vidal, Mackenzie Mathis.
+This work was funded, in part, from the Wyss Center to the [Mathis Laboratory of Adaptive Intelligence](https://www.mackenziemathislab.org/).
 Please refer to the documentation for full acknowledgements.
 
 ## Plugin base
 
 This [napari] plugin was generated with [Cookiecutter] using [@napari]'s [cookiecutter-napari-plugin] template.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,85 +1,96 @@
-# napari-cellseg3D: a napari plug-in for direct 3D cell segmentation with deep
-learning [cellseg3d logo]_[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_][![License: MIT](https://
-img.shields.io/badge/License-MIT-blue.svg)](https://github.com/
-AdaptiveMotorControlLab/CellSeg3d/raw/main/LICENSE) [![PyPI](https://
-img.shields.io/pypi/v/napari-cellseg3d.svg?color=green)](https://pypi.org/
-project/napari-cellseg3d) [![Python Version](https://img.shields.io/pypi/
-pyversions/napari-cellseg-annotator.svg?color=green)](https://python.org) [!
-[codecov](https://codecov.io/gh/AdaptiveMotorControlLab/CellSeg3d/branch/main/
-graph/badge.svg?token=hzUcn3XN8F)](https://codecov.io/gh/
-AdaptiveMotorControlLab/CellSeg3d) [![napari hub](https://img.shields.io/
-endpoint?url=https://api.napari-hub.org/shields/napari-cellseg3d)](https://
-www.napari-hub.org/plugins/napari-cellseg3d) A napari plugin for 3D cell
-segmentation: training, inference, and data review. In particular, this project
-was developed for analysis of mesoSPIM-acquired (cleared tissue + lightsheet)
-datasets. **Help us make the code better by reporting issues and adding your
-feature requests!** ---------------------------------- ## News **New version :
-v0.1.2** - Fixed manifest issue for PyPi Previous additions : - Improved
-training interface - Unsupervised model : WNet - Generate labels directly from
-raw data ! - Can be trained in napari directly or in Colab - Pretrained weights
-for mesoSPIM whole-brain cell segmentation - WandB support (install wandb and
-login to use automatically when training) - Remade and improved documentation -
-Moved to Jupyter Book - Dedicated installation page, and working ARM64 install
-for macOS Silicon users - New utilities - Many small improvements and many bug
-fixes ## Demo ![demo](https://images.squarespace-cdn.com/content/v1/
-57f6d51c9f74566f55ecf271/0d16a71b-3ff2-477a-9d83-18d96cb1ce28/
-full_demo.gif?format=500w) ## Installation See the [Installation page] in the
-documentation for detailed instructions. ### M1 Mac users To avoid issues when
-installing on the ARM64 architecture, please follow these steps. 1) Create a
-new conda env using the provided conda/napari_cellseg3d_m1.yml file : git clone
-https://github.com/AdaptiveMotorControlLab/CellSeg3d.git cd CellSeg3d conda env
-create -f conda/napari_cellseg3d_m1.yml conda activate napari_cellseg3d_m1 2)
-Install the plugin. From repository root folder, run : pip install -e . OR
-directly via PyPi : pip install napari-cellseg3d OR directly via [napari-hub]
-(see Installation section above) ## Documentation Available at https://
-AdaptiveMotorControlLab.github.io/CellSeg3d You can also generate docs by
-running ``make html`` in the docs/ folder. ## Usage To use the plugin, please
-run: ``` napari ``` Then go into Plugins > napari-cellseg3d, and choose which
-tool to use. - **Review**: This module allows you to review your labels, from
-predictions or manual labeling, and correct them if needed. It then saves the
-status of each file in a csv, for easier monitoring. - **Inference**: This
-module allows you to use pre-trained segmentation algorithms on volumes to
-automatically label cells and compute statistics. - **Train**: This module
-allows you to train segmentation algorithms from labeled volumes. -
-**Utilities**: This module allows you to perform several actions like cropping
-your volumes and labels dynamically, by selecting a fixed size volume and
-moving it around the image; computing prediction scores from ground truth and
-predicition labels; or converting labels from instance to segmentation and the
-opposite. ## Requirements **Python 3.8 or 3.9 required.** Requires **
-[napari]**, **[PyTorch]** and **[MONAI]**. For PyTorch, please see [the PyTorch
-website for installation instructions]. A CUDA-capable GPU is not needed but
-very strongly recommended, especially for training. If you get errors from
-MONAI regarding missing readers, please see [MONAI's optional dependencies]
-page for instructions on getting the readers required by your images. ## Issues
-If you encounter any problems, please [file an issue] along with a detailed
-description. ## Testing Before testing, install all requirements using ``pip
-install napari-cellseg3d[test]``. ``pydensecrf`` is also required for testing.
-To run tests locally: - Locally : run ``pytest`` in the plugin folder - Locally
-with coverage : In the plugin folder, run ``coverage run --
-source=napari_cellseg3d -m pytest`` then ``coverage xml`` to generate a .xml
-coverage file. - With tox : run ``tox`` in the plugin folder (will simulate
-tests with several python and OS configs, requires substantial storage space)
-## Contributing Contributions are very welcome. Please ensure the coverage at
-least stays the same before you submit a pull request. For local installation
-from Github cloning, please run: ``` pip install -e . ``` ## License
-Distributed under the terms of the [MIT] license. "napari-cellseg3d" is free
-and open source software. [napari-hub]: https://www.napari-hub.org/plugins/
-napari-cellseg3d [file an issue]: https://github.com/AdaptiveMotorControlLab/
-CellSeg3d/issues [napari]: https://github.com/napari/napari [Cookiecutter]:
-https://github.com/audreyr/cookiecutter [@napari]: https://github.com/napari
-[MIT]: http://opensource.org/licenses/MIT [cookiecutter-napari-plugin]: https:/
-/github.com/napari/cookiecutter-napari-plugin [tox]: https://
-tox.readthedocs.io/en/latest/ [pip]: https://pypi.org/project/pip/ [PyPI]:
-https://pypi.org/ [Installation page]: https://
-adaptivemotorcontrollab.github.io/CellSeg3d/source/guides/
+# CellSeg3D: self-supervised (and supervised) 3D cell segmentation [cellseg3d
+logo]_[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_][![PyPI](https://img.shields.io/pypi/v/napari-
+cellseg3d.svg?color=green)](https://pypi.org/project/napari-cellseg3d) [!
+[Downloads](https://static.pepy.tech/badge/napari-cellseg3d)](https://
+pepy.tech/project/napari-cellseg3d) [![Downloads](https://static.pepy.tech/
+badge/napari-cellseg3d/month)](https://pepy.tech/project/napari-cellseg3d) [!
+[License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://
+github.com/AdaptiveMotorControlLab/CellSeg3D/raw/main/LICENSE) [![Python
+Version](https://img.shields.io/pypi/pyversions/napari-cellseg-
+annotator.svg?color=green)](https://python.org) [![codecov](https://codecov.io/
+gh/AdaptiveMotorControlLab/CellSeg3D/branch/main/graph/
+badge.svg?token=hzUcn3XN8F)](https://codecov.io/gh/AdaptiveMotorControlLab/
+CellSeg3D) [![napari hub](https://img.shields.io/endpoint?url=https://
+api.napari-hub.org/shields/napari-cellseg3d)](https://www.napari-hub.org/
+plugins/napari-cellseg3d) - A napari plugin for 3D cell segmentation: training,
+inference, and data review. In particular, this project was developed for
+analysis of mesoSPIM-acquired (cleared tissue + lightsheet) datasets. ![demo]
+(https://images.squarespace-cdn.com/content/v1/57f6d51c9f74566f55ecf271/
+0d16a71b-3ff2-477a-9d83-18d96cb1ce28/full_demo.gif?format=500w) ## Installation
+ð» See the [Installation page] in the documentation for detailed
+instructions. ## Documentation ð A lot of documentation is available at
+https://AdaptiveMotorControlLab.github.io/CellSeg3D You can also generate docs
+by running ``make html`` in the docs/ folder. ## Quick Start To use the plugin,
+please run: ``` napari ``` Then go into Plugins > napari-cellseg3d, and choose
+which tool to use. - **Review (label)**: This module allows you to review your
+labels, from predictions or manual labeling, and correct them if needed. It
+then saves the status of each file in a csv, for easier monitoring. -
+**Inference**: This module allows you to use pre-trained segmentation
+algorithms on volumes to automatically label cells and compute statistics. -
+**Train**: This module allows you to train segmentation algorithms from labeled
+volumes. - **Utilities**: This module allows you to perform several actions
+like cropping your volumes and labels dynamically, by selecting a fixed size
+volume and moving it around the image; fragment images into smaller cubes for
+training; or converting labels from instance to segmentation and the opposite.
+## News **New version : v0.2.0** - Changed project name to "napari_cellseg3d"
+to avoid setuptools deprecation - Small API changes for training/inference from
+a script - Some fixes to WandB integration ad csv saving after training
+Previous additions : - v0.1.2 :Fixed manifest issue for PyPi - Improved
+training interface - Unsupervised model : WNet3D - Generate labels directly
+from raw data! - Can be trained in napari directly or in Google Colab -
+Pretrained weights for mesoSPIM whole-brain cell segmentation - WandB support
+(install wandb and login to use automatically when training) - Remade and
+improved documentation - Moved to Jupyter Book - Dedicated installation page,
+and working ARM64 install for macOS Silicon users - New utilities - Many small
+improvements and many bug fixes ### Install note for ARM64 (Silicon) Mac users
+To avoid issues when installing on the ARM64 architecture, please follow these
+steps. 1) Create a new conda env using the provided conda/
+napari_CellSeg3D_ARM64.yml file : git clone https://github.com/
+AdaptiveMotorControlLab/CellSeg3d.git cd CellSeg3d conda env create -f conda/
+CellSeg3D_ARM64.yml conda activate napari_CellSeg3D_ARM64 2) Install a Qt
+backend (PySide or PyQt5) 3) Launch napari, the plugin should be available in
+the plugins menu. ## Requirements **Python 3.8 or 3.9 required.** Requires **
+[napari]**, **[PyTorch]** and **[MONAI]**. Compatible with Windows, MacOS and
+Linux. Installation should not take more than 30 minutes, depending on your
+internet connection. For PyTorch, please see [the PyTorch website for
+installation instructions]. A CUDA-capable GPU is not needed but very strongly
+recommended, especially for training. If you get errors from MONAI regarding
+missing readers, please see [MONAI's optional dependencies] page for
+instructions on getting the readers required by your images. ## Quick demo
+After installation, you can run the plugin by running: napari and launching the
+plugin from the Plugins menu. You may use the test volume in the `examples`
+folder to test the inference and review tools. This should run in far less than
+five minutes on a modern computer. You may also find a demo Colab notebook in
+the `notebooks` folder. ## Issues **Help us make the code better by reporting
+issues and adding your feature requests!** If you encounter any problems,
+please [file an issue] along with a detailed description. ## Testing Before
+testing, install all requirements using ``pip install napari-cellseg3d[test]``.
+``pydensecrf`` is also required for testing. To run tests locally: - Locally :
+run ``pytest`` in the plugin folder - Locally with coverage : In the plugin
+folder, run ``coverage run --source=napari_cellseg3d -m pytest`` then
+``coverage xml`` to generate a .xml coverage file. - With tox : run ``tox`` in
+the plugin folder (will simulate tests with several python and OS configs,
+requires substantial storage space) ## Contributing Contributions are very
+welcome. Please ensure the coverage at least stays the same before you submit a
+pull request. For local installation from Github cloning, please run: ``` pip
+install -e . ``` ## License Distributed under the terms of the [MIT] license.
+"napari-cellseg3d" is free and open source software. [napari-hub]: https://
+www.napari-hub.org/plugins/napari-cellseg3d [file an issue]: https://
+github.com/AdaptiveMotorControlLab/CellSeg3D/issues [napari]: https://
+github.com/napari/napari [Cookiecutter]: https://github.com/audreyr/
+cookiecutter [@napari]: https://github.com/napari [MIT]: http://opensource.org/
+licenses/MIT [cookiecutter-napari-plugin]: https://github.com/napari/
+cookiecutter-napari-plugin [tox]: https://tox.readthedocs.io/en/latest/ [pip]:
+https://pypi.org/project/pip/ [PyPI]: https://pypi.org/ [Installation page]:
+https://adaptivemotorcontrollab.github.io/CellSeg3D/source/guides/
 installation_guide.html [the PyTorch website for installation instructions]:
 https://pytorch.org/get-started/locally/ [PyTorch]: https://pytorch.org/get-
 started/locally/ [MONAI's optional dependencies]: https://docs.monai.io/en/
 stable/installation.html#installing-the-recommended-dependencies [MONAI]:
 https://docs.monai.io/en/stable/installation.html#installing-the-recommended-
-dependencies ## Acknowledgements This plugin was developed by Cyril Achard,
-Maxime Vidal, Mackenzie Mathis. This work was funded, in part, from the Wyss
-Center to the [Mathis Laboratory of Adaptive Motor Control](https://
+dependencies ## Acknowledgements This plugin was developed by originally Cyril
+Achard, Maxime Vidal, Mackenzie Mathis. This work was funded, in part, from the
+Wyss Center to the [Mathis Laboratory of Adaptive Intelligence](https://
 www.mackenziemathislab.org/). Please refer to the documentation for full
 acknowledgements. ## Plugin base This [napari] plugin was generated with
 [Cookiecutter] using [@napari]'s [cookiecutter-napari-plugin] template.
```

### Comparing `napari_cellseg3d-0.1.2/napari_cellseg3d/_tests/fixtures.py` & `napari_cellseg3d-0.2.0/napari_cellseg3d/_tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.2/napari_cellseg3d/_tests/test_base_plugin.py` & `napari_cellseg3d-0.2.0/napari_cellseg3d/_tests/test_base_plugin.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.2/napari_cellseg3d/_tests/test_dock_widget.py` & `napari_cellseg3d-0.2.0/napari_cellseg3d/_tests/test_dock_widget.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.2/napari_cellseg3d/_tests/test_inference.py` & `napari_cellseg3d-0.2.0/napari_cellseg3d/_tests/test_inference.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.2/napari_cellseg3d/_tests/test_labels_correction.py` & `napari_cellseg3d-0.2.0/napari_cellseg3d/_tests/test_labels_correction.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.2/napari_cellseg3d/_tests/test_model_framework.py` & `napari_cellseg3d-0.2.0/napari_cellseg3d/_tests/test_model_framework.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.2/napari_cellseg3d/_tests/test_models.py` & `napari_cellseg3d-0.2.0/napari_cellseg3d/_tests/test_models.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.2/napari_cellseg3d/_tests/test_plugin_inference.py` & `napari_cellseg3d-0.2.0/napari_cellseg3d/_tests/test_plugin_inference.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
     widget.use_window_choice.setChecked(True)
     widget.window_overlap_slider.setValue(0)
     widget.keep_data_on_cpu_box.setChecked(True)
 
     assert widget.check_ready()
 
-    widget.model_choice.setCurrentText("WNet")
+    widget.model_choice.setCurrentText("WNet3D")
     widget._restrict_window_size_for_model()
     assert widget.use_window_choice.isChecked()
     assert widget.window_size_choice.currentText() == "64"
 
     test_model_name = "test"
     MODEL_LIST[test_model_name] = TestModel
     widget.model_choice.addItem(test_model_name)
```

### Comparing `napari_cellseg3d-0.1.2/napari_cellseg3d/_tests/test_plugin_training.py` & `napari_cellseg3d-0.2.0/napari_cellseg3d/_tests/test_plugin_training.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     ]
     for attr in dir(default_config):
         if not attr.startswith("__") and attr not in excluded:
             assert getattr(default_config, attr) == getattr(
                 worker.config, attr
             )
     # test unsupervised config and worker
-    widget.model_choice.setCurrentText("WNet")
+    widget.model_choice.setCurrentText("WNet3D")
     widget._toggle_unsupervised_mode(enabled=True)
     default_config = config.WNetTrainingWorkerConfig()
     worker = widget._create_worker(additional_results_description="TEST_1")
     excluded = ["results_path_folder", "sample_size", "weights_info"]
     for attr in dir(default_config):
         if not attr.startswith("__") and attr not in excluded:
             assert getattr(default_config, attr) == getattr(
```

### Comparing `napari_cellseg3d-0.1.2/napari_cellseg3d/_tests/test_plugin_utils.py` & `napari_cellseg3d-0.2.0/napari_cellseg3d/_tests/test_plugin_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         widget.utils_widgets[i]._start()
 
 
 def test_crop_widget(make_napari_viewer_proxy):
     view = make_napari_viewer_proxy()
     widget = Cropping(view)
 
-    image = rand_gen.random((10, 10, 10)).astype(np.uint8)
+    image = rand_gen.random((10, 10, 10)).astype(np.int8)
     image_layer_1 = view.add_image(image, name="image")
     image_layer_2 = view.add_labels(image, name="image2")
 
     view.window.add_dock_widget(widget)
     view.dims.ndisplay = 3
     assert len(image_layer_1.data.shape) == 3
     assert len(image_layer_2.data.shape) == 3
```

### Comparing `napari_cellseg3d-0.1.2/napari_cellseg3d/_tests/test_plugins.py` & `napari_cellseg3d-0.2.0/napari_cellseg3d/_tests/test_plugins.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.2/napari_cellseg3d/_tests/test_review.py` & `napari_cellseg3d-0.2.0/napari_cellseg3d/_tests/test_review.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.2/napari_cellseg3d/_tests/test_training.py` & `napari_cellseg3d-0.2.0/napari_cellseg3d/_tests/test_training.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,16 +82,16 @@
 
 
 def test_unsupervised_training(make_napari_viewer_proxy):
     viewer = make_napari_viewer_proxy()
     widget = Trainer(viewer)
     widget.log = LogFixture()
     widget.worker = None
+    widget.model_choice.setCurrentText("WNet3D")
     widget._toggle_unsupervised_mode(enabled=True)
-    widget.model_choice.setCurrentText("WNet")
 
     widget.patch_choice.setChecked(True)
     [w.setValue(4) for w in widget.patch_size_widgets]
 
     widget.unsupervised_images_filewidget.text_field.setText(
         str((im_path.parent / "wnet_test").resolve())
     )
```

### Comparing `napari_cellseg3d-0.1.2/napari_cellseg3d/_tests/test_utils.py` & `napari_cellseg3d-0.2.0/napari_cellseg3d/_tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/__init__.py` & `napari_cellseg3d-0.2.0/napari_cellseg3d/code_models/__init__.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/crf.py` & `napari_cellseg3d-0.2.0/napari_cellseg3d/code_models/crf.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/instance_segmentation.py` & `napari_cellseg3d-0.2.0/napari_cellseg3d/code_models/instance_segmentation.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/model_framework.py` & `napari_cellseg3d-0.2.0/napari_cellseg3d/code_models/model_framework.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/models/TEMPLATE_model.py` & `napari_cellseg3d-0.2.0/napari_cellseg3d/code_models/models/TEMPLATE_model.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/models/model_SegResNet.py` & `napari_cellseg3d-0.2.0/napari_cellseg3d/code_models/models/model_SegResNet.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/models/model_SwinUNetR.py` & `napari_cellseg3d-0.2.0/napari_cellseg3d/code_models/models/model_SwinUNetR.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/models/model_TRAILMAP.py` & `napari_cellseg3d-0.2.0/napari_cellseg3d/code_models/models/model_TRAILMAP.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/models/model_TRAILMAP_MS.py` & `napari_cellseg3d-0.2.0/napari_cellseg3d/code_models/models/model_TRAILMAP_MS.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/models/model_VNet.py` & `napari_cellseg3d-0.2.0/napari_cellseg3d/code_models/models/model_VNet.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/models/model_WNet.py` & `napari_cellseg3d-0.2.0/napari_cellseg3d/code_models/models/model_WNet.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/models/model_test.py` & `napari_cellseg3d-0.2.0/napari_cellseg3d/code_models/models/model_test.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/models/pretrained/pretrained_model_urls.json` & `napari_cellseg3d-0.2.0/napari_cellseg3d/code_models/models/pretrained/pretrained_model_urls.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.875%*

 * *Differences: {"'WNet3D'": "'https://huggingface.co/C-Achard/cellseg3d/resolve/main/wnet_latest.tar.gz'"}*

```diff
@@ -1,9 +1,10 @@
 {
     "SegResNet": "https://huggingface.co/C-Achard/cellseg3d/resolve/main/SegResNet_latest.tar.gz",
     "SwinUNetR": "https://huggingface.co/C-Achard/cellseg3d/resolve/main/SwinUNetR_latest.tar.gz",
     "TRAILMAP_MS": "https://huggingface.co/C-Achard/cellseg3d/resolve/main/TRAILMAP_latest.tar.gz",
     "VNet": "https://huggingface.co/C-Achard/cellseg3d/resolve/main/VNet_latest.tar.gz",
     "WNet": "https://huggingface.co/C-Achard/cellseg3d/resolve/main/wnet_latest.tar.gz",
+    "WNet3D": "https://huggingface.co/C-Achard/cellseg3d/resolve/main/wnet_latest.tar.gz",
     "WNet_ONNX": "https://huggingface.co/C-Achard/cellseg3d/resolve/main/wnet_onnx.tar.gz",
     "test": "https://huggingface.co/C-Achard/cellseg3d/resolve/main/test.tar.gz"
 }
```

### Comparing `napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/models/unet/buildingblocks.py` & `napari_cellseg3d-0.2.0/napari_cellseg3d/code_models/models/unet/buildingblocks.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/models/unet/model.py` & `napari_cellseg3d-0.2.0/napari_cellseg3d/code_models/models/unet/model.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/models/wnet/model.py` & `napari_cellseg3d-0.2.0/napari_cellseg3d/code_models/models/wnet/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     "Xide Xia",
     "Brian Kulis",
 ]
 NUM_GROUPS = 4
 
 
 class WNet_encoder(nn.Module):
-    """WNet with encoder only."""
+    """WNet3D with encoder only."""
 
     def __init__(
         self,
         in_channels=1,
         out_channels=2,
         # num_classes=2,
         softmax=True,
```

### Comparing `napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/models/wnet/soft_Ncuts.py` & `napari_cellseg3d-0.2.0/napari_cellseg3d/code_models/models/wnet/soft_Ncuts.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/worker_inference.py` & `napari_cellseg3d-0.2.0/napari_cellseg3d/code_models/worker_inference.py`

 * *Files 0% similar despite different names*

```diff
@@ -273,15 +273,15 @@
         dims_check = volume.shape
 
         logger.debug(volume.shape)
         logger.debug(volume.dtype)
 
         normalization = (
             QuantileNormalization()
-            if self.config.model_info.name != "WNet"
+            if self.config.model_info.name != "WNet3D"
             else lambda x: x
         )
         volume = np.reshape(volume, newshape=(1, *volume.shape))
         if self.config.sliding_window_config.is_enabled():
             load_transforms = Compose(
                 [
                     # QuantileNormalization(),
```

### Comparing `napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/worker_training.py` & `napari_cellseg3d-0.2.0/napari_cellseg3d/code_models/worker_training.py`

 * *Files 2% similar despite different names*

```diff
@@ -384,15 +384,15 @@
         self.log(
             f"Weighted sum : {self.config.n_cuts_weight}*NCuts + {self.config.rec_loss_weight}*Reconstruction"
         )
         ##############
         self.log("-- Data --")
         self.log("Training data :\n")
         [
-            self.log(f"{v}")
+            self.log(f"{Path(v).stem}")
             for d in self.config.train_data_dict
             for k, v in d.items()
         ]
         if self.config.eval_volume_dict is not None:
             self.log("\nValidation data :\n")
             [
                 self.log(f"{k}: {v}")
@@ -419,20 +419,25 @@
             ##############
             # disable metadata tracking in MONAI
             set_track_meta(False)
             ##############
             if WANDB_INSTALLED:
                 config_dict = self.config.__dict__
                 logger.debug(f"wandb config : {config_dict}")
+                if wandb.run is not None:
+                    logger.warning(
+                        "A previous wandb run is still active. It will be stopped before starting a new one."
+                    )
+                    wandb.finish()
                 wandb.init(
                     config=config_dict,
-                    project="CellSeg3D - WNet",
-                    name=f"WNet_training - {utils.get_date_time()}",
+                    project="CellSeg3D - WNet3D",
+                    name=f"WNet3D_training - {utils.get_date_time()}",
                     mode=self.wandb_config.mode,
-                    tags=["WNet", "training"],
+                    tags=["WNet3D", "training"],
                 )
 
             set_determinism(seed=self.config.deterministic_config.seed)
             torch.use_deterministic_algorithms(True, warn_only=True)
 
             device = self.config.device
 
@@ -468,21 +473,29 @@
                             max=self.config.clipping,
                         )
                     )
 
             if WANDB_INSTALLED:
                 wandb.watch(model, log_freq=100)
 
-            if self.config.weights_info.use_custom:
+            if (
+                self.config.weights_info.use_pretrained
+                or self.config.weights_info.use_custom
+            ):
                 if self.config.weights_info.use_pretrained:
-                    weights_file = "wnet.pth"
-                    self.downloader.download_weights("WNet", weights_file)
-                    weights = PRETRAINED_WEIGHTS_DIR / Path(weights_file)
+                    from napari_cellseg3d.code_models.models.model_WNet import (
+                        WNet_,
+                    )
+
+                    weights_file = WNet_.weights_file
+                    self.downloader.download_weights("WNet3D", weights_file)
+                    weights = str(PRETRAINED_WEIGHTS_DIR / Path(weights_file))
                     self.config.weights_info.path = weights
-                else:
+
+                if self.config.weights_info.use_custom:
                     weights = str(Path(self.config.weights_info.path))
 
                 try:
                     model.load_state_dict(
                         torch.load(
                             weights,
                             map_location=self.config.device,
@@ -620,14 +633,17 @@
                         del optimizer
                         criterionE = None
                         del criterionE
                         criterionW = None
                         del criterionW
                         torch.cuda.empty_cache()
 
+                        if WANDB_INSTALLED:
+                            wandb.finish()
+
                 self.ncuts_losses.append(
                     epoch_ncuts_loss / len(self.dataloader)
                 )
                 self.rec_losses.append(epoch_rec_loss / len(self.dataloader))
                 self.total_losses.append(epoch_loss / len(self.dataloader))
 
                 if self.eval_dataloader is None:
@@ -638,17 +654,15 @@
 
                         images_dict = {
                             "Encoder output": {
                                 "data": enc_out,
                                 "cmap": "turbo",
                             },
                             "Encoder output (discrete)": {
-                                "data": AsDiscrete(threshold=0.5)(
-                                    enc_out
-                                ).numpy(),
+                                "data": np.where(enc_out > 0.5, enc_out, 0),
                                 "cmap": "bop blue",
                             },
                             "Decoder output": {
                                 "data": np.squeeze(dec_out),
                                 "cmap": "gist_earth",
                             },
                             "Input image": {
@@ -732,15 +746,16 @@
                 self.log(f"ETA: {eta:.1f} minutes")
                 self.log("-" * 20)
 
                 # Save the model
                 if epoch % 5 == 0:
                     torch.save(
                         model.state_dict(),
-                        self.config.results_path_folder + "/wnet_.pth",
+                        self.config.results_path_folder
+                        + "/wnet_checkpoint.pth",
                     )
 
             self.log("Training finished")
             if self.best_dice > -1:
                 best_dice_epoch = epoch
                 self.log(
                     f"Best dice metric : {self.best_dice} at epoch {best_dice_epoch}"
@@ -762,15 +777,15 @@
             torch.save(
                 model.state_dict(),
                 save_weights_path,
             )
 
             if WANDB_INSTALLED and self.wandb_config.save_model_artifact:
                 model_artifact = wandb.Artifact(
-                    "WNet",
+                    "WNet3D",
                     type="model",
                     description="CellSeg3D WNet",
                     metadata=self.config.__dict__,
                 )
                 model_artifact.add_file(save_weights_path)
                 wandb.log_artifact(model_artifact)
 
@@ -852,16 +867,15 @@
 
                 max_dice_channel = utils.seek_best_dice_coeff_channel(
                     y_pred=val_outputs, y_true=val_labels
                 )
                 self.dice_metric(
                     y_pred=val_outputs[
                         :,
-                        max_dice_channel : (max_dice_channel + 1),
-                        :,
+                        max_dice_channel:,  # : (max_dice_channel + 1),
                         :,
                         :,
                     ],
                     y=val_labels,
                 )
 
             # aggregate the final mean dice result
@@ -1109,21 +1123,31 @@
         # error_log = open(results_path +"/error_log.log" % multiprocessing.current_process().name, 'x')
         # faulthandler.enable(file=error_log, all_threads=True)
         #########################
         model_config = self.config.model_info
         weights_config = self.config.weights_info
         deterministic_config = self.config.deterministic_config
 
+        if self.config.device == "mps":
+            from os import environ
+
+            environ["PYTORCH_ENABLE_MPS_FALLBACK"] = "1"
+
         start_time = time.time()
 
         try:
             if WANDB_INSTALLED:
                 config_dict = self.config.__dict__
                 logger.debug(f"wandb config : {config_dict}")
                 try:
+                    if wandb.run is not None:
+                        logger.warning(
+                            "A previous wandb run is still active. It will be stopped before starting a new one."
+                        )
+                        wandb.finish()
                     wandb.init(
                         config=config_dict,
                         project="CellSeg3D",
                         name=f"{model_config.name}_supervised_training - {utils.get_date_time()}",
                         tags=[f"{model_config.name}", "supervised"],
                         mode=self.wandb_config.mode,
                     )
@@ -1406,21 +1430,21 @@
 
             best_metric = -1
             best_metric_epoch = -1
 
             # time = utils.get_date_time()
             logger.debug("Weights")
 
-            if weights_config.use_custom:
+            if weights_config.use_custom or weights_config.use_pretrained:
                 if weights_config.use_pretrained:
                     weights_file = model_class.weights_file
                     self.downloader.download_weights(model_name, weights_file)
-                    weights = PRETRAINED_WEIGHTS_DIR / Path(weights_file)
+                    weights = str(PRETRAINED_WEIGHTS_DIR / Path(weights_file))
                     weights_config.path = weights
-                else:
+                elif weights_config.use_custom:
                     weights = str(Path(weights_config.path))
 
                 try:
                     model.load_state_dict(
                         torch.load(
                             weights,
                             map_location=device,
@@ -1519,14 +1543,17 @@
                         optimizer = None
                         del optimizer
                         scheduler = None
                         del scheduler
                         if device.type == "cuda":
                             torch.cuda.empty_cache()
 
+                        if WANDB_INSTALLED:
+                            wandb.finish()
+
                     yield TrainingReport(
                         show_plot=False,
                         weights=model.state_dict(),
                         supervised=True,
                     )
 
                 if WANDB_INSTALLED:
```

### Comparing `napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/workers_utils.py` & `napari_cellseg3d-0.2.0/napari_cellseg3d/code_models/workers_utils.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.2/napari_cellseg3d/code_plugins/plugin_base.py` & `napari_cellseg3d-0.2.0/napari_cellseg3d/code_plugins/plugin_base.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.2/napari_cellseg3d/code_plugins/plugin_convert.py` & `napari_cellseg3d-0.2.0/napari_cellseg3d/code_plugins/plugin_convert.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.2/napari_cellseg3d/code_plugins/plugin_crf.py` & `napari_cellseg3d-0.2.0/napari_cellseg3d/code_plugins/plugin_crf.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.2/napari_cellseg3d/code_plugins/plugin_crop.py` & `napari_cellseg3d-0.2.0/napari_cellseg3d/code_plugins/plugin_crop.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.2/napari_cellseg3d/code_plugins/plugin_helper.py` & `napari_cellseg3d-0.2.0/napari_cellseg3d/code_plugins/plugin_helper.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,18 +17,18 @@
 class Helper(QWidget, metaclass=ui.QWidgetSingleton):
     """Tiny plugin showing link to documentation and about page."""
 
     def __init__(self, viewer: "napari.viewer.Viewer"):
         """Creates a widget with links to documentation and about page."""
         super().__init__()
 
-        self.help_url = "https://adaptivemotorcontrollab.github.io/CellSeg3d/"
+        self.help_url = "https://adaptivemotorcontrollab.github.io/CellSeg3D/"
 
         self.about_url = "https://wysscenter.ch/advances/3d-computer-vision-for-brain-analysis"
-        self.repo_url = "https://github.com/AdaptiveMotorControlLab/CellSeg3d"
+        self.repo_url = "https://github.com/AdaptiveMotorControlLab/CellSeg3D"
         self._viewer = viewer
 
         logo_path = str(
             pathlib.Path(__file__).parent.resolve() / "../res/logo_alpha.png"
         )
         print(logo_path)
         image = QPixmap(logo_path)
@@ -39,15 +39,15 @@
         self.logo_label.setIconSize(QSize(200, 200))
         self.logo_label.setStyleSheet(
             "QPushButton { background-color: transparent }"
         )
         self.logo_label.setToolTip("Open Github page")
 
         self.info_label = ui.make_label(
-            f"You are using napari-cellseg3d v.{'0.1.2'}\n\n"
+            f"You are using napari-cellseg3d v.{'0.2.0'}\n\n"
             f"Plugin for cell segmentation developed\n"
             f"by the Mathis Lab of Adaptive Motor Control\n\n"
             f"Code by :\nCyril Achard\nMaxime Vidal\nJessy Lauer\nMackenzie Mathis\n"
             f"\nReleased under the MIT license",
             self,
         )
```

### Comparing `napari_cellseg3d-0.1.2/napari_cellseg3d/code_plugins/plugin_metrics.py` & `napari_cellseg3d-0.2.0/napari_cellseg3d/code_plugins/plugin_metrics.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.2/napari_cellseg3d/code_plugins/plugin_model_inference.py` & `napari_cellseg3d-0.2.0/napari_cellseg3d/code_plugins/plugin_model_inference.py`

 * *Files 0% similar despite different names*

```diff
@@ -254,15 +254,15 @@
         )
         self.folder_choice.toggle()
         self.layer_choice.toggle()
 
         self._remove_unused()
 
     def _toggle_crf_choice(self):
-        if self.model_choice.currentText() == "WNet":
+        if self.model_choice.currentText() == "WNet3D":
             self.use_crf.setVisible(True)
         else:
             self.use_crf.setVisible(False)
 
     def _set_tooltips(self):
         ##################
         ##################
@@ -331,15 +331,15 @@
         ):
             return True
         return False
 
     def _restrict_window_size_for_model(self):
         """Sets the window size to a value that is compatible with the chosen model."""
         self.wnet_enabled = False
-        if self.model_choice.currentText() == "WNet":
+        if self.model_choice.currentText() == "WNet3D":
             self.wnet_enabled = True
             self.window_size_choice.setCurrentIndex(self._default_window_size)
             self.use_window_choice.setChecked(self.wnet_enabled)
         self.window_size_choice.setDisabled(
             self.wnet_enabled and not self.custom_weights_choice.isChecked()
         )
         self.use_window_choice.setDisabled(
```

### Comparing `napari_cellseg3d-0.1.2/napari_cellseg3d/code_plugins/plugin_model_training.py` & `napari_cellseg3d-0.2.0/napari_cellseg3d/code_plugins/plugin_model_training.py`

 * *Files 2% similar despite different names*

```diff
@@ -447,15 +447,15 @@
             if self.get_unsupervised_image_filepaths() == []:
                 logger.warning("Image paths are not correctly set")
                 return False
         return True
 
     def _toggle_unsupervised_mode(self, enabled=False):
         """Change all the UI elements needed for unsupervised learning mode."""
-        if self.model_choice.currentText() == "WNet" or enabled:
+        if self.model_choice.currentText() == "WNet3D" or enabled:
             unsupervised = True
             self.start_btn = self.start_button_unsupervised
             if self.image_filewidget.text_field.text() == "Images directory":
                 self.image_filewidget.text_field.setText("Validation images")
             if self.labels_filewidget.text_field.text() == "Labels directory":
                 self.labels_filewidget.text_field.setText("Validation labels")
             self.learning_rate_choice.lr_value_choice.setValue(2)
@@ -795,15 +795,15 @@
         ############
         ##################
         advanced_tab = ui.ContainerWidget(parent=self)
         self.wnet_widgets = WNetWidgets(parent=advanced_tab)
         ui.add_blank(advanced_tab, advanced_tab.layout)
         ##################
         model_params_group_w, model_params_group_l = ui.make_group(
-            "WNet parameters", r=20, b=5, t=11
+            "WNet3D parameters", r=20, b=5, t=11
         )
         ui.add_widgets(
             model_params_group_l,
             [
                 self.wnet_widgets.num_classes_choice.label,
                 self.wnet_widgets.num_classes_choice,
                 self.wnet_widgets.loss_choice.label,
@@ -1050,15 +1050,15 @@
 
         Returns:
             A worker config
         """
         logger.debug("Loading config...")
         model_config = config.ModelInfo(name=self.model_choice.currentText())
 
-        self.weights_config.path = self.weights_config.path
+        # self.weights_config.path = self.weights_config.path
         self.weights_config.use_custom = self.custom_weights_choice.isChecked()
 
         self.weights_config.use_pretrained = (
             self.use_transfer_choice.isChecked()
             and not self.custom_weights_choice.isChecked()
         )
         self.weights_config.use_custom = self.custom_weights_choice.isChecked()
@@ -1361,55 +1361,73 @@
                     f"latest_weights_aborted_training_{utils.get_time_filepath()}.pth",
                 ),
             )
             self.log.print_and_log("Saving complete")
             self.on_stop()
             self._stop_requested = False
 
-    def _make_csv(self):
-        size_column = range(1, self.worker_config.max_epochs + 1)
+    def _check_lens(self, size_column, loss_values):
+        if len(size_column) != len(loss_values):
+            logger.info(
+                f"Training was stopped, setting epochs for csv to {len(loss_values)}"
+            )
+            return range(1, len(loss_values) + 1)
+        return size_column
+
+    def _handle_loss_values(self, size_column, key):
+        loss_values = self.loss_1_values.get(key)
+        if loss_values is None:
+            return None
 
-        if len(self.loss_1_values) == 0 or self.loss_1_values is None:
+        if len(loss_values) == 0:
             logger.warning("No loss values to add to csv !")
-            return
+            return None
 
-        try:
-            self.loss_1_values["Loss"]
-            supervised = True
-        except KeyError:
-            try:
-                self.loss_1_values["SoftNCuts"]
-                supervised = False
-            except KeyError as e:
-                raise KeyError(
-                    "Error when making csv. Check loss dict keys ?"
-                ) from e
+        return self._check_lens(size_column, loss_values)
+
+    def _make_csv(self):  # TDOD(cyril) design could use a good rework
+        size_column = range(1, self.worker_config.max_epochs + 1)
+
+        supervised = True
+        size_column = self._handle_loss_values(size_column, "Loss")
+        if size_column is None:
+            size_column = self._handle_loss_values(size_column, "SoftNCuts")
+            if size_column is None:
+                raise KeyError("Error when making csv. Check loss dict keys ?")
+            supervised = False
 
         if supervised:
-            val = utils.fill_list_in_between(
+            val = utils.fill_list_in_between(  # fills the validation list based on validation interval
                 self.loss_2_values,
                 self.worker_config.validation_interval - 1,
                 "",
-            )[: len(size_column)]
+            )[
+                : len(size_column)
+            ]
 
             self.df = pd.DataFrame(
                 {
                     "epoch": size_column,
                     "loss": self.loss_1_values["Loss"],
                     "validation": val,
                 }
             )
             if len(val) != len(self.loss_1_values["Loss"]):
                 err = f"Validation and loss values don't have the same length ! Got {len(val)} and {len(self.loss_1_values['Loss'])}"
                 logger.error(err)
                 raise ValueError(err)
         else:
             ncuts_loss = self.loss_1_values["SoftNCuts"]
+
+            logger.debug(f"Epochs : {len(size_column)}")
+            logger.debug(f"Loss 1 values : {len(ncuts_loss)}")
+            logger.debug(f"Loss 2 values : {len(self.loss_2_values)}")
             try:
                 dice_metric = self.loss_1_values["Dice metric"]
+                logger.debug(f"Dice metric : {dice_metric}")
                 self.df = pd.DataFrame(
                     {
                         "Epoch": size_column,
                         "Ncuts loss": ncuts_loss,
                         "Dice metric": dice_metric,
                         "Reconstruction loss": self.loss_2_values,
                     }
@@ -1626,23 +1644,23 @@
         """Creates a collection of widgets for the WNet training GUI."""
         self.num_classes_choice = ui.DropdownMenu(
             entries=["2", "3", "4"],
             parent=parent,
             text_label="Number of classes",
         )
         self.intensity_sigma_choice = ui.DoubleIncrementCounter(
-            lower=1.0,
+            lower=0.01,
             upper=100.0,
             default=self.default_config.intensity_sigma,
             parent=parent,
             text_label="Intensity sigma",
         )
         self.intensity_sigma_choice.setMaximumWidth(20)
         self.spatial_sigma_choice = ui.DoubleIncrementCounter(
-            lower=1.0,
+            lower=0.01,
             upper=100.0,
             default=self.default_config.spatial_sigma,
             parent=parent,
             text_label="Spatial sigma",
         )
         self.spatial_sigma_choice.setMaximumWidth(20)
         self.radius_choice = ui.IntIncrementCounter(
@@ -1670,18 +1688,18 @@
             upper=1.0,
             default=0.5,
             parent=parent,
             text_label="Reconstruction weight",
         )
         self.reconstruction_weight_choice.setMaximumWidth(20)
         self.reconstruction_weight_divide_factor_choice = (
-            ui.IntIncrementCounter(
-                lower=1,
-                upper=10000,
-                default=100,
+            ui.DoubleIncrementCounter(
+                lower=0.01,
+                upper=10000.0,
+                default=1.0,
                 parent=parent,
                 text_label="Reconstruction weight divide factor",
             )
         )
         self.reconstruction_weight_divide_factor_choice.setMaximumWidth(20)
 
         self._set_tooltips()
```

### Comparing `napari_cellseg3d-0.1.2/napari_cellseg3d/code_plugins/plugin_review.py` & `napari_cellseg3d-0.2.0/napari_cellseg3d/code_plugins/plugin_review.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.2/napari_cellseg3d/code_plugins/plugin_review_dock.py` & `napari_cellseg3d-0.2.0/napari_cellseg3d/code_plugins/plugin_review_dock.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.2/napari_cellseg3d/code_plugins/plugin_utilities.py` & `napari_cellseg3d-0.2.0/napari_cellseg3d/code_plugins/plugin_utilities.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.2/napari_cellseg3d/config.py` & `napari_cellseg3d-0.2.0/napari_cellseg3d/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # TODO(cyril) add JSON load/save
 
 MODEL_LIST = {
     "SegResNet": SegResNet_,
     "VNet": VNet_,
     "TRAILMAP_MS": TRAILMAP_MS_,
     "SwinUNetR": SwinUNETR_,
-    "WNet": WNet_,
+    "WNet3D": WNet_,
     # "TRAILMAP": TRAILMAP,
     # "test" : DO NOT USE, reserved for testing
 }
 
 PRETRAINED_WEIGHTS_DIR = str(
     Path(__file__).parent.resolve() / Path("code_models/models/pretrained")
 )
@@ -395,15 +395,15 @@
     intensity_sigma: float = 1.0
     spatial_sigma: float = 4.0
     radius: int = 2
     # reconstruction loss params
     reconstruction_loss: str = "MSE"  # or "BCE"
     # summed losses weights
     n_cuts_weight: float = 0.5
-    rec_loss_weight: float = 0.5 / 100
+    rec_loss_weight: float = 0.5 / 1.0  # 0.5 / 100
     # normalization params
     # normalizing_function: callable = remap_image # FIXME: call directly in worker, not a param
     # data params
     train_data_dict: dict = None
     eval_volume_dict: str = None
     eval_batch_size: int = 1
```

### Comparing `napari_cellseg3d-0.1.2/napari_cellseg3d/dev_scripts/artefact_labeling.py` & `napari_cellseg3d-0.2.0/napari_cellseg3d/dev_scripts/artefact_labeling.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.2/napari_cellseg3d/dev_scripts/colab_training.py` & `napari_cellseg3d-0.2.0/napari_cellseg3d/dev_scripts/colab_training.py`

 * *Files 1% similar despite different names*

```diff
@@ -328,15 +328,15 @@
                 config_dict = self.config.__dict__
                 logger.debug(f"wandb config : {config_dict}")
                 wandb.init(
                     config=config_dict,
                     project="CellSeg3D (Colab)",
                     name=f"{self.config.model_info.name} training - {utils.get_date_time()}",
                     mode=self.wandb_config.mode,
-                    tags=["WNet", "Colab"],
+                    tags=["WNet3D", "Colab"],
                 )
 
             set_determinism(seed=self.config.deterministic_config.seed)
             torch.use_deterministic_algorithms(True, warn_only=True)
 
             device = self.config.device
 
@@ -375,15 +375,15 @@
 
             if WANDB_INSTALLED:
                 wandb.watch(model, log_freq=100)
 
             if self.config.weights_info.use_custom:
                 if self.config.weights_info.use_pretrained:
                     weights_file = "wnet.pth"
-                    self.downloader.download_weights("WNet", weights_file)
+                    self.downloader.download_weights("WNet3D", weights_file)
                     weights = PRETRAINED_WEIGHTS_DIR / Path(weights_file)
                     self.config.weights_info.path = weights
                 else:
                     weights = str(Path(self.config.weights_info.path))
 
                 try:
                     model.load_state_dict(
@@ -592,17 +592,17 @@
             torch.save(
                 model.state_dict(),
                 save_weights_path,
             )
 
             if WANDB_INSTALLED and self.wandb_config.save_model_artifact:
                 model_artifact = wandb.Artifact(
-                    "WNet",
+                    "WNet3D",
                     type="model",
-                    description="CellSeg3D WNet",
+                    description="CellSeg3D WNet3D",
                     metadata=self.config.__dict__,
                 )
                 model_artifact.add_file(save_weights_path)
                 wandb.log_artifact(model_artifact)
 
         except Exception as e:
             msg = f"Training failed with exception: {e}"
```

### Comparing `napari_cellseg3d-0.1.2/napari_cellseg3d/dev_scripts/correct_labels.py` & `napari_cellseg3d-0.2.0/napari_cellseg3d/dev_scripts/correct_labels.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.2/napari_cellseg3d/dev_scripts/crop_data.py` & `napari_cellseg3d-0.2.0/napari_cellseg3d/dev_scripts/crop_data.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.2/napari_cellseg3d/dev_scripts/evaluate_labels.py` & `napari_cellseg3d-0.2.0/napari_cellseg3d/dev_scripts/evaluate_labels.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.2/napari_cellseg3d/dev_scripts/remote_training.py` & `napari_cellseg3d-0.2.0/napari_cellseg3d/dev_scripts/remote_training.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.2/napari_cellseg3d/dev_scripts/sliding_window_voronoi.py` & `napari_cellseg3d-0.2.0/napari_cellseg3d/dev_scripts/sliding_window_voronoi.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.2/napari_cellseg3d/dev_scripts/thread_test.py` & `napari_cellseg3d-0.2.0/napari_cellseg3d/dev_scripts/thread_test.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.2/napari_cellseg3d/dev_scripts/whole_brain_utils.py` & `napari_cellseg3d-0.2.0/napari_cellseg3d/dev_scripts/whole_brain_utils.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.2/napari_cellseg3d/interface.py` & `napari_cellseg3d-0.2.0/napari_cellseg3d/interface.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.2/napari_cellseg3d/napari.yaml` & `napari_cellseg3d-0.2.0/napari_cellseg3d/napari.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -23,15 +23,15 @@
   - id: napari_cellseg3d.train
     title: Create Trainer widget
     python_name: napari_cellseg3d.plugins:Trainer
 
 
   widgets:
   - command: napari_cellseg3d.load
-    display_name: Review
+    display_name: Labeling
 
   - command: napari_cellseg3d.infer
     display_name: Inference
 
   - command: napari_cellseg3d.train
     display_name: Training
```

### Comparing `napari_cellseg3d-0.1.2/napari_cellseg3d/plugins.py` & `napari_cellseg3d-0.2.0/napari_cellseg3d/plugins.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.2/napari_cellseg3d/res/logo_alpha.png` & `napari_cellseg3d-0.2.0/napari_cellseg3d/res/logo_alpha.png`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.2/napari_cellseg3d/utils.py` & `napari_cellseg3d-0.2.0/napari_cellseg3d/utils.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.2/napari_cellseg3d.egg-info/PKG-INFO` & `napari_cellseg3d-0.2.0/napari_cellseg3d.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: napari_cellseg3d
-Version: 0.1.2
+Version: 0.2.0
 Summary: Plugin for cell segmentation in 3D
 Author-email: Cyril Achard <cyril.achard@epfl.ch>, Maxime Vidal <maxime.vidal@epfl.ch>, Mackenzie Mathis <mackenzie@post.harvard.edu>
 License: MIT
-Project-URL: Homepage, https://github.com/AdaptiveMotorControlLab/CellSeg3d
+Project-URL: Homepage, https://github.com/AdaptiveMotorControlLab/CellSeg3D
 Project-URL: Documentation, https://adaptivemotorcontrollab.github.io/cellseg3d-docs/res/welcome.html
-Project-URL: Issues, https://github.com/AdaptiveMotorControlLab/CellSeg3d/issues
+Project-URL: Issues, https://github.com/AdaptiveMotorControlLab/CellSeg3D/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Framework :: napari
 Classifier: Topic :: Software Development :: Testing
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -34,14 +34,20 @@
 Requires-Dist: torch>=1.11
 Requires-Dist: monai[einops,nibabel]>=0.9.0
 Requires-Dist: itk
 Requires-Dist: tqdm
 Requires-Dist: pyclesperanto-prototype
 Requires-Dist: tqdm
 Requires-Dist: matplotlib
+Provides-Extra: pyqt5
+Requires-Dist: pyqt5; extra == "pyqt5"
+Provides-Extra: pyside2
+Requires-Dist: pyside2; extra == "pyside2"
+Provides-Extra: pyside6
+Requires-Dist: pyside6; extra == "pyside6"
 Provides-Extra: onnx-cpu
 Requires-Dist: onnx; extra == "onnx-cpu"
 Requires-Dist: onnxruntime; extra == "onnx-cpu"
 Provides-Extra: onnx-gpu
 Requires-Dist: onnx; extra == "onnx-gpu"
 Requires-Dist: onnxruntime-gpu; extra == "onnx-gpu"
 Provides-Extra: wandb
@@ -61,112 +67,125 @@
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: coverage; extra == "test"
 Requires-Dist: tox; extra == "test"
 Requires-Dist: twine; extra == "test"
 Requires-Dist: onnx; extra == "test"
 Requires-Dist: onnxruntime; extra == "test"
 
-# napari-cellseg3D: a napari plug-in for direct 3D cell segmentation with deep learning
-
+# CellSeg3D: self-supervised (and supervised) 3D cell segmentation
 <img src="https://images.squarespace-cdn.com/content/v1/57f6d51c9f74566f55ecf271/838605d0-9723-4e43-83cd-6dbfe4adf36b/cellseg-logo.png?format=1500w" title="cellseg3d" alt="cellseg3d logo" width="350" align="right" vspace = "80"/>
 
 <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
-[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/AdaptiveMotorControlLab/CellSeg3d/raw/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/napari-cellseg3d.svg?color=green)](https://pypi.org/project/napari-cellseg3d)
+[![Downloads](https://static.pepy.tech/badge/napari-cellseg3d)](https://pepy.tech/project/napari-cellseg3d)
+[![Downloads](https://static.pepy.tech/badge/napari-cellseg3d/month)](https://pepy.tech/project/napari-cellseg3d)
+[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/AdaptiveMotorControlLab/CellSeg3D/raw/main/LICENSE)
 [![Python Version](https://img.shields.io/pypi/pyversions/napari-cellseg-annotator.svg?color=green)](https://python.org)
-[![codecov](https://codecov.io/gh/AdaptiveMotorControlLab/CellSeg3d/branch/main/graph/badge.svg?token=hzUcn3XN8F)](https://codecov.io/gh/AdaptiveMotorControlLab/CellSeg3d)
+[![codecov](https://codecov.io/gh/AdaptiveMotorControlLab/CellSeg3D/branch/main/graph/badge.svg?token=hzUcn3XN8F)](https://codecov.io/gh/AdaptiveMotorControlLab/CellSeg3D)
 [![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-cellseg3d)](https://www.napari-hub.org/plugins/napari-cellseg3d)
 
-A napari plugin for 3D cell segmentation: training, inference, and data review. In particular, this project was developed for analysis of mesoSPIM-acquired (cleared tissue + lightsheet) datasets.
+- A napari plugin for 3D cell segmentation: training, inference, and data review. In particular, this project was developed for analysis of mesoSPIM-acquired (cleared tissue + lightsheet) datasets.
 
-**Help us make the code better by reporting issues and adding your feature requests!**
+![demo](https://images.squarespace-cdn.com/content/v1/57f6d51c9f74566f55ecf271/0d16a71b-3ff2-477a-9d83-18d96cb1ce28/full_demo.gif?format=500w)
+
+## Installation
+
+ 💻 See the [Installation page] in the documentation for detailed instructions.
+
+## Documentation
+
+📚 A lot of documentation is available at https://AdaptiveMotorControlLab.github.io/CellSeg3D
+
+You can also generate docs by running ``make html`` in the docs/ folder.
+
+## Quick Start
 
-----------------------------------
+To use the plugin, please run:
+```
+napari
+```
+Then go into Plugins > napari-cellseg3d, and choose which tool to use.
+
+- **Review (label)**: This module allows you to review your labels, from predictions or manual labeling, and correct them if needed. It then saves the status of each file in a csv, for easier monitoring.
+- **Inference**: This module allows you to use pre-trained segmentation algorithms on volumes to automatically label cells and compute statistics.
+- **Train**:  This module allows you to train segmentation algorithms from labeled volumes.
+- **Utilities**: This module allows you to perform several actions like cropping your volumes and labels dynamically, by selecting a fixed size volume and moving it around the image; fragment images into smaller cubes for training; or converting labels from instance to segmentation and the opposite.
 
 ## News
 
-**New version : v0.1.2**
+**New version : v0.2.0**
 
-- Fixed manifest issue for PyPi
+- Changed project name to "napari_cellseg3d" to avoid setuptools deprecation
+- Small API changes for training/inference from a script
+- Some fixes to WandB integration ad csv saving after training
 
 Previous additions :
 
+- v0.1.2 :Fixed manifest issue for PyPi
 - Improved training interface
-- Unsupervised model : WNet
-  - Generate labels directly from raw data !
-  - Can be trained in napari directly or in Colab
+- Unsupervised model : WNet3D
+  - Generate labels directly from raw data!
+  - Can be trained in napari directly or in Google Colab
   - Pretrained weights for mesoSPIM whole-brain cell segmentation
 - WandB support (install wandb and login to use automatically when training)
 - Remade and improved documentation
   - Moved to Jupyter Book
   - Dedicated installation page, and working ARM64 install for macOS Silicon users
 - New utilities
 - Many small improvements and many bug fixes
 
-## Demo
-
-![demo](https://images.squarespace-cdn.com/content/v1/57f6d51c9f74566f55ecf271/0d16a71b-3ff2-477a-9d83-18d96cb1ce28/full_demo.gif?format=500w)
-
-## Installation
 
-See the [Installation page] in the documentation for detailed instructions.
 
-### M1 Mac users
+### Install note for ARM64 (Silicon) Mac users
 
 To avoid issues when installing on the ARM64 architecture, please follow these steps.
 
-1) Create a new conda env using the provided conda/napari_cellseg3d_m1.yml file :
+1) Create a new conda env using the provided conda/napari_CellSeg3D_ARM64.yml file :
 
         git clone https://github.com/AdaptiveMotorControlLab/CellSeg3d.git
         cd CellSeg3d
-        conda env create -f conda/napari_cellseg3d_m1.yml
-        conda activate napari_cellseg3d_m1
+        conda env create -f conda/CellSeg3D_ARM64.yml
+        conda activate napari_CellSeg3D_ARM64
 
-2) Install the plugin.
-   From repository root folder, run :
 
-        pip install -e .
-   OR directly via PyPi :
+2) Install a Qt backend (PySide or PyQt5)
+3) Launch napari, the plugin should be available in the plugins menu.
 
-        pip install napari-cellseg3d
 
-   OR directly via [napari-hub] (see Installation section above)
-
-## Documentation
-
-Available at https://AdaptiveMotorControlLab.github.io/CellSeg3d
-
-You can also generate docs by running ``make html`` in the docs/ folder.
-
-## Usage
-
-To use the plugin, please run:
-```
-napari
-```
-Then go into Plugins > napari-cellseg3d, and choose which tool to use.
-
-- **Review**: This module allows you to review your labels, from predictions or manual labeling, and correct them if needed. It then saves the status of each file in a csv, for easier monitoring.
-- **Inference**: This module allows you to use pre-trained segmentation algorithms on volumes to automatically label cells and compute statistics.
-- **Train**:  This module allows you to train segmentation algorithms from labeled volumes.
-- **Utilities**: This module allows you to perform several actions like cropping your volumes and labels dynamically, by selecting a fixed size volume and moving it around the image; computing prediction scores from ground truth and predicition labels; or converting labels from instance to segmentation and the opposite.
 
 ## Requirements
 
 **Python 3.8 or 3.9 required.**
 Requires **[napari]**, **[PyTorch]** and **[MONAI]**.
+Compatible with Windows, MacOS and Linux.
+Installation should not take more than 30 minutes, depending on your internet connection.
 
 For PyTorch, please see [the PyTorch website for installation instructions].
 
 A CUDA-capable GPU is not needed but very strongly recommended, especially for training.
 
 If you get errors from MONAI regarding missing readers, please see [MONAI's optional dependencies] page for instructions on getting the readers required by your images.
 
+## Quick demo
+
+After installation, you can run the plugin by running:
+
+        napari
+
+and launching the plugin from the Plugins menu.
+You may use the test volume in the `examples` folder to test the inference and review tools.
+This should run in far less than five minutes on a modern computer.
+
+You may also find a demo Colab notebook in the `notebooks` folder.
+
 ## Issues
 
+**Help us make the code better by reporting issues and adding your feature requests!**
+
+
 If you encounter any problems, please [file an issue] along with a detailed description.
 
 ## Testing
 
 Before testing, install all requirements using ``pip install napari-cellseg3d[test]``.
 
 ``pydensecrf`` is also required for testing.
@@ -193,31 +212,31 @@
 
 Distributed under the terms of the [MIT] license.
 
 "napari-cellseg3d" is free and open source software.
 
 [napari-hub]: https://www.napari-hub.org/plugins/napari-cellseg3d
 
-[file an issue]: https://github.com/AdaptiveMotorControlLab/CellSeg3d/issues
+[file an issue]: https://github.com/AdaptiveMotorControlLab/CellSeg3D/issues
 [napari]: https://github.com/napari/napari
 [Cookiecutter]: https://github.com/audreyr/cookiecutter
 [@napari]: https://github.com/napari
 [MIT]: http://opensource.org/licenses/MIT
 [cookiecutter-napari-plugin]: https://github.com/napari/cookiecutter-napari-plugin
 [tox]: https://tox.readthedocs.io/en/latest/
 [pip]: https://pypi.org/project/pip/
 [PyPI]: https://pypi.org/
-[Installation page]: https://adaptivemotorcontrollab.github.io/CellSeg3d/source/guides/installation_guide.html
+[Installation page]: https://adaptivemotorcontrollab.github.io/CellSeg3D/source/guides/installation_guide.html
 [the PyTorch website for installation instructions]: https://pytorch.org/get-started/locally/
 [PyTorch]: https://pytorch.org/get-started/locally/
 [MONAI's optional dependencies]: https://docs.monai.io/en/stable/installation.html#installing-the-recommended-dependencies
 [MONAI]: https://docs.monai.io/en/stable/installation.html#installing-the-recommended-dependencies
 
 ## Acknowledgements
 
-This plugin was developed by Cyril Achard, Maxime Vidal, Mackenzie Mathis.
-This work was funded, in part, from the Wyss Center to the [Mathis Laboratory of Adaptive Motor Control](https://www.mackenziemathislab.org/).
+This plugin was developed by originally Cyril Achard, Maxime Vidal, Mackenzie Mathis.
+This work was funded, in part, from the Wyss Center to the [Mathis Laboratory of Adaptive Intelligence](https://www.mackenziemathislab.org/).
 Please refer to the documentation for full acknowledgements.
 
 ## Plugin base
 
 This [napari] plugin was generated with [Cookiecutter] using [@napari]'s [cookiecutter-napari-plugin] template.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: napari_cellseg3d Version: 0.1.2 Summary: Plugin for
+Metadata-Version: 2.1 Name: napari_cellseg3d Version: 0.2.0 Summary: Plugin for
 cell segmentation in 3D Author-email: Cyril Achard
 epfl.ch>, Maxime Vidal
 epfl.ch>, Mackenzie Mathis
 post.harvard.edu> License: MIT Project-URL: Homepage, https://github.com/
-AdaptiveMotorControlLab/CellSeg3d Project-URL: Documentation, https://
+AdaptiveMotorControlLab/CellSeg3D Project-URL: Documentation, https://
 adaptivemotorcontrollab.github.io/cellseg3d-docs/res/welcome.html Project-URL:
-Issues, https://github.com/AdaptiveMotorControlLab/CellSeg3d/issues Classifier:
+Issues, https://github.com/AdaptiveMotorControlLab/CellSeg3D/issues Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Science/
 Research Classifier: Framework :: napari Classifier: Topic :: Software
 Development :: Testing Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Operating System :: OS
 Independent Classifier: License :: OSI Approved :: MIT License Classifier:
@@ -18,104 +18,117 @@
 Engineering :: Visualization Requires-Python: >=3.8 Description-Content-Type:
 text/markdown License-File: LICENSE Requires-Dist: numpy Requires-Dist: napari
 [all]>=0.4.14 Requires-Dist: QtPy Requires-Dist: scikit-image>=0.19.2 Requires-
 Dist: matplotlib>=3.4.1 Requires-Dist: tifffile>=2022.2.9 Requires-Dist:
 imagecodecs>=2023.3.16 Requires-Dist: torch>=1.11 Requires-Dist: monai
 [einops,nibabel]>=0.9.0 Requires-Dist: itk Requires-Dist: tqdm Requires-Dist:
 pyclesperanto-prototype Requires-Dist: tqdm Requires-Dist: matplotlib Provides-
-Extra: onnx-cpu Requires-Dist: onnx; extra == "onnx-cpu" Requires-Dist:
-onnxruntime; extra == "onnx-cpu" Provides-Extra: onnx-gpu Requires-Dist: onnx;
-extra == "onnx-gpu" Requires-Dist: onnxruntime-gpu; extra == "onnx-gpu"
-Provides-Extra: wandb Requires-Dist: wandb; extra == "wandb" Provides-Extra:
-dev Requires-Dist: isort; extra == "dev" Requires-Dist: black; extra == "dev"
-Requires-Dist: ruff; extra == "dev" Requires-Dist: pre-commit; extra == "dev"
-Requires-Dist: tuna; extra == "dev" Requires-Dist: twine; extra == "dev"
-Provides-Extra: docs Requires-Dist: jupyter-book; extra == "docs" Provides-
-Extra: test Requires-Dist: pytest; extra == "test" Requires-Dist: pytest_qt;
-extra == "test" Requires-Dist: pytest-cov; extra == "test" Requires-Dist:
-coverage; extra == "test" Requires-Dist: tox; extra == "test" Requires-Dist:
-twine; extra == "test" Requires-Dist: onnx; extra == "test" Requires-Dist:
-onnxruntime; extra == "test" # napari-cellseg3D: a napari plug-in for direct 3D
-cell segmentation with deep learning [cellseg3d logo]_[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_][!
-[License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://
-github.com/AdaptiveMotorControlLab/CellSeg3d/raw/main/LICENSE) [![PyPI](https:/
-/img.shields.io/pypi/v/napari-cellseg3d.svg?color=green)](https://pypi.org/
-project/napari-cellseg3d) [![Python Version](https://img.shields.io/pypi/
-pyversions/napari-cellseg-annotator.svg?color=green)](https://python.org) [!
-[codecov](https://codecov.io/gh/AdaptiveMotorControlLab/CellSeg3d/branch/main/
-graph/badge.svg?token=hzUcn3XN8F)](https://codecov.io/gh/
-AdaptiveMotorControlLab/CellSeg3d) [![napari hub](https://img.shields.io/
+Extra: pyqt5 Requires-Dist: pyqt5; extra == "pyqt5" Provides-Extra: pyside2
+Requires-Dist: pyside2; extra == "pyside2" Provides-Extra: pyside6 Requires-
+Dist: pyside6; extra == "pyside6" Provides-Extra: onnx-cpu Requires-Dist: onnx;
+extra == "onnx-cpu" Requires-Dist: onnxruntime; extra == "onnx-cpu" Provides-
+Extra: onnx-gpu Requires-Dist: onnx; extra == "onnx-gpu" Requires-Dist:
+onnxruntime-gpu; extra == "onnx-gpu" Provides-Extra: wandb Requires-Dist:
+wandb; extra == "wandb" Provides-Extra: dev Requires-Dist: isort; extra ==
+"dev" Requires-Dist: black; extra == "dev" Requires-Dist: ruff; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev" Requires-Dist: tuna; extra == "dev"
+Requires-Dist: twine; extra == "dev" Provides-Extra: docs Requires-Dist:
+jupyter-book; extra == "docs" Provides-Extra: test Requires-Dist: pytest; extra
+== "test" Requires-Dist: pytest_qt; extra == "test" Requires-Dist: pytest-cov;
+extra == "test" Requires-Dist: coverage; extra == "test" Requires-Dist: tox;
+extra == "test" Requires-Dist: twine; extra == "test" Requires-Dist: onnx;
+extra == "test" Requires-Dist: onnxruntime; extra == "test" # CellSeg3D: self-
+supervised (and supervised) 3D cell segmentation [cellseg3d logo]_[_C_o_d_e_ _s_t_y_l_e_:
+_b_l_a_c_k_][![PyPI](https://img.shields.io/pypi/v/napari-cellseg3d.svg?color=green)]
+(https://pypi.org/project/napari-cellseg3d) [![Downloads](https://
+static.pepy.tech/badge/napari-cellseg3d)](https://pepy.tech/project/napari-
+cellseg3d) [![Downloads](https://static.pepy.tech/badge/napari-cellseg3d/
+month)](https://pepy.tech/project/napari-cellseg3d) [![License: MIT](https://
+img.shields.io/badge/License-MIT-blue.svg)](https://github.com/
+AdaptiveMotorControlLab/CellSeg3D/raw/main/LICENSE) [![Python Version](https://
+img.shields.io/pypi/pyversions/napari-cellseg-annotator.svg?color=green)]
+(https://python.org) [![codecov](https://codecov.io/gh/AdaptiveMotorControlLab/
+CellSeg3D/branch/main/graph/badge.svg?token=hzUcn3XN8F)](https://codecov.io/gh/
+AdaptiveMotorControlLab/CellSeg3D) [![napari hub](https://img.shields.io/
 endpoint?url=https://api.napari-hub.org/shields/napari-cellseg3d)](https://
-www.napari-hub.org/plugins/napari-cellseg3d) A napari plugin for 3D cell
+www.napari-hub.org/plugins/napari-cellseg3d) - A napari plugin for 3D cell
 segmentation: training, inference, and data review. In particular, this project
 was developed for analysis of mesoSPIM-acquired (cleared tissue + lightsheet)
-datasets. **Help us make the code better by reporting issues and adding your
-feature requests!** ---------------------------------- ## News **New version :
-v0.1.2** - Fixed manifest issue for PyPi Previous additions : - Improved
-training interface - Unsupervised model : WNet - Generate labels directly from
-raw data ! - Can be trained in napari directly or in Colab - Pretrained weights
-for mesoSPIM whole-brain cell segmentation - WandB support (install wandb and
-login to use automatically when training) - Remade and improved documentation -
-Moved to Jupyter Book - Dedicated installation page, and working ARM64 install
-for macOS Silicon users - New utilities - Many small improvements and many bug
-fixes ## Demo ![demo](https://images.squarespace-cdn.com/content/v1/
+datasets. ![demo](https://images.squarespace-cdn.com/content/v1/
 57f6d51c9f74566f55ecf271/0d16a71b-3ff2-477a-9d83-18d96cb1ce28/
-full_demo.gif?format=500w) ## Installation See the [Installation page] in the
-documentation for detailed instructions. ### M1 Mac users To avoid issues when
-installing on the ARM64 architecture, please follow these steps. 1) Create a
-new conda env using the provided conda/napari_cellseg3d_m1.yml file : git clone
-https://github.com/AdaptiveMotorControlLab/CellSeg3d.git cd CellSeg3d conda env
-create -f conda/napari_cellseg3d_m1.yml conda activate napari_cellseg3d_m1 2)
-Install the plugin. From repository root folder, run : pip install -e . OR
-directly via PyPi : pip install napari-cellseg3d OR directly via [napari-hub]
-(see Installation section above) ## Documentation Available at https://
-AdaptiveMotorControlLab.github.io/CellSeg3d You can also generate docs by
-running ``make html`` in the docs/ folder. ## Usage To use the plugin, please
-run: ``` napari ``` Then go into Plugins > napari-cellseg3d, and choose which
-tool to use. - **Review**: This module allows you to review your labels, from
-predictions or manual labeling, and correct them if needed. It then saves the
-status of each file in a csv, for easier monitoring. - **Inference**: This
-module allows you to use pre-trained segmentation algorithms on volumes to
-automatically label cells and compute statistics. - **Train**: This module
-allows you to train segmentation algorithms from labeled volumes. -
-**Utilities**: This module allows you to perform several actions like cropping
-your volumes and labels dynamically, by selecting a fixed size volume and
-moving it around the image; computing prediction scores from ground truth and
-predicition labels; or converting labels from instance to segmentation and the
-opposite. ## Requirements **Python 3.8 or 3.9 required.** Requires **
-[napari]**, **[PyTorch]** and **[MONAI]**. For PyTorch, please see [the PyTorch
-website for installation instructions]. A CUDA-capable GPU is not needed but
-very strongly recommended, especially for training. If you get errors from
-MONAI regarding missing readers, please see [MONAI's optional dependencies]
-page for instructions on getting the readers required by your images. ## Issues
-If you encounter any problems, please [file an issue] along with a detailed
-description. ## Testing Before testing, install all requirements using ``pip
-install napari-cellseg3d[test]``. ``pydensecrf`` is also required for testing.
-To run tests locally: - Locally : run ``pytest`` in the plugin folder - Locally
-with coverage : In the plugin folder, run ``coverage run --
-source=napari_cellseg3d -m pytest`` then ``coverage xml`` to generate a .xml
-coverage file. - With tox : run ``tox`` in the plugin folder (will simulate
-tests with several python and OS configs, requires substantial storage space)
-## Contributing Contributions are very welcome. Please ensure the coverage at
-least stays the same before you submit a pull request. For local installation
-from Github cloning, please run: ``` pip install -e . ``` ## License
-Distributed under the terms of the [MIT] license. "napari-cellseg3d" is free
-and open source software. [napari-hub]: https://www.napari-hub.org/plugins/
-napari-cellseg3d [file an issue]: https://github.com/AdaptiveMotorControlLab/
-CellSeg3d/issues [napari]: https://github.com/napari/napari [Cookiecutter]:
-https://github.com/audreyr/cookiecutter [@napari]: https://github.com/napari
-[MIT]: http://opensource.org/licenses/MIT [cookiecutter-napari-plugin]: https:/
-/github.com/napari/cookiecutter-napari-plugin [tox]: https://
-tox.readthedocs.io/en/latest/ [pip]: https://pypi.org/project/pip/ [PyPI]:
-https://pypi.org/ [Installation page]: https://
-adaptivemotorcontrollab.github.io/CellSeg3d/source/guides/
+full_demo.gif?format=500w) ## Installation ð» See the [Installation page] in
+the documentation for detailed instructions. ## Documentation ð A lot of
+documentation is available at https://AdaptiveMotorControlLab.github.io/
+CellSeg3D You can also generate docs by running ``make html`` in the docs/
+folder. ## Quick Start To use the plugin, please run: ``` napari ``` Then go
+into Plugins > napari-cellseg3d, and choose which tool to use. - **Review
+(label)**: This module allows you to review your labels, from predictions or
+manual labeling, and correct them if needed. It then saves the status of each
+file in a csv, for easier monitoring. - **Inference**: This module allows you
+to use pre-trained segmentation algorithms on volumes to automatically label
+cells and compute statistics. - **Train**: This module allows you to train
+segmentation algorithms from labeled volumes. - **Utilities**: This module
+allows you to perform several actions like cropping your volumes and labels
+dynamically, by selecting a fixed size volume and moving it around the image;
+fragment images into smaller cubes for training; or converting labels from
+instance to segmentation and the opposite. ## News **New version : v0.2.0** -
+Changed project name to "napari_cellseg3d" to avoid setuptools deprecation -
+Small API changes for training/inference from a script - Some fixes to WandB
+integration ad csv saving after training Previous additions : - v0.1.2 :Fixed
+manifest issue for PyPi - Improved training interface - Unsupervised model :
+WNet3D - Generate labels directly from raw data! - Can be trained in napari
+directly or in Google Colab - Pretrained weights for mesoSPIM whole-brain cell
+segmentation - WandB support (install wandb and login to use automatically when
+training) - Remade and improved documentation - Moved to Jupyter Book -
+Dedicated installation page, and working ARM64 install for macOS Silicon users
+- New utilities - Many small improvements and many bug fixes ### Install note
+for ARM64 (Silicon) Mac users To avoid issues when installing on the ARM64
+architecture, please follow these steps. 1) Create a new conda env using the
+provided conda/napari_CellSeg3D_ARM64.yml file : git clone https://github.com/
+AdaptiveMotorControlLab/CellSeg3d.git cd CellSeg3d conda env create -f conda/
+CellSeg3D_ARM64.yml conda activate napari_CellSeg3D_ARM64 2) Install a Qt
+backend (PySide or PyQt5) 3) Launch napari, the plugin should be available in
+the plugins menu. ## Requirements **Python 3.8 or 3.9 required.** Requires **
+[napari]**, **[PyTorch]** and **[MONAI]**. Compatible with Windows, MacOS and
+Linux. Installation should not take more than 30 minutes, depending on your
+internet connection. For PyTorch, please see [the PyTorch website for
+installation instructions]. A CUDA-capable GPU is not needed but very strongly
+recommended, especially for training. If you get errors from MONAI regarding
+missing readers, please see [MONAI's optional dependencies] page for
+instructions on getting the readers required by your images. ## Quick demo
+After installation, you can run the plugin by running: napari and launching the
+plugin from the Plugins menu. You may use the test volume in the `examples`
+folder to test the inference and review tools. This should run in far less than
+five minutes on a modern computer. You may also find a demo Colab notebook in
+the `notebooks` folder. ## Issues **Help us make the code better by reporting
+issues and adding your feature requests!** If you encounter any problems,
+please [file an issue] along with a detailed description. ## Testing Before
+testing, install all requirements using ``pip install napari-cellseg3d[test]``.
+``pydensecrf`` is also required for testing. To run tests locally: - Locally :
+run ``pytest`` in the plugin folder - Locally with coverage : In the plugin
+folder, run ``coverage run --source=napari_cellseg3d -m pytest`` then
+``coverage xml`` to generate a .xml coverage file. - With tox : run ``tox`` in
+the plugin folder (will simulate tests with several python and OS configs,
+requires substantial storage space) ## Contributing Contributions are very
+welcome. Please ensure the coverage at least stays the same before you submit a
+pull request. For local installation from Github cloning, please run: ``` pip
+install -e . ``` ## License Distributed under the terms of the [MIT] license.
+"napari-cellseg3d" is free and open source software. [napari-hub]: https://
+www.napari-hub.org/plugins/napari-cellseg3d [file an issue]: https://
+github.com/AdaptiveMotorControlLab/CellSeg3D/issues [napari]: https://
+github.com/napari/napari [Cookiecutter]: https://github.com/audreyr/
+cookiecutter [@napari]: https://github.com/napari [MIT]: http://opensource.org/
+licenses/MIT [cookiecutter-napari-plugin]: https://github.com/napari/
+cookiecutter-napari-plugin [tox]: https://tox.readthedocs.io/en/latest/ [pip]:
+https://pypi.org/project/pip/ [PyPI]: https://pypi.org/ [Installation page]:
+https://adaptivemotorcontrollab.github.io/CellSeg3D/source/guides/
 installation_guide.html [the PyTorch website for installation instructions]:
 https://pytorch.org/get-started/locally/ [PyTorch]: https://pytorch.org/get-
 started/locally/ [MONAI's optional dependencies]: https://docs.monai.io/en/
 stable/installation.html#installing-the-recommended-dependencies [MONAI]:
 https://docs.monai.io/en/stable/installation.html#installing-the-recommended-
-dependencies ## Acknowledgements This plugin was developed by Cyril Achard,
-Maxime Vidal, Mackenzie Mathis. This work was funded, in part, from the Wyss
-Center to the [Mathis Laboratory of Adaptive Motor Control](https://
+dependencies ## Acknowledgements This plugin was developed by originally Cyril
+Achard, Maxime Vidal, Mackenzie Mathis. This work was funded, in part, from the
+Wyss Center to the [Mathis Laboratory of Adaptive Intelligence](https://
 www.mackenziemathislab.org/). Please refer to the documentation for full
 acknowledgements. ## Plugin base This [napari] plugin was generated with
 [Cookiecutter] using [@napari]'s [cookiecutter-napari-plugin] template.
```

### Comparing `napari_cellseg3d-0.1.2/napari_cellseg3d.egg-info/SOURCES.txt` & `napari_cellseg3d-0.2.0/napari_cellseg3d.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,15 @@
 ./napari_cellseg3d/code_plugins/plugin_utilities.py
 ./napari_cellseg3d/dev_scripts/__init__.py
 ./napari_cellseg3d/dev_scripts/artefact_labeling.py
 ./napari_cellseg3d/dev_scripts/colab_training.py
 ./napari_cellseg3d/dev_scripts/correct_labels.py
 ./napari_cellseg3d/dev_scripts/crop_data.py
 ./napari_cellseg3d/dev_scripts/evaluate_labels.py
+./napari_cellseg3d/dev_scripts/remote_inference.py
 ./napari_cellseg3d/dev_scripts/remote_training.py
 ./napari_cellseg3d/dev_scripts/sliding_window_voronoi.py
 ./napari_cellseg3d/dev_scripts/thread_test.py
 ./napari_cellseg3d/dev_scripts/whole_brain_utils.py
 ./napari_cellseg3d/res/__init__.py
 ./napari_cellseg3d/res/logo_alpha.png
 napari_cellseg3d.egg-info/PKG-INFO
```

### Comparing `napari_cellseg3d-0.1.2/pyproject.toml` & `napari_cellseg3d-0.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -45,17 +45,17 @@
     "pyclesperanto-prototype",
     "tqdm",
     "matplotlib",
 ]
 dynamic = ["version", "entry-points"]
 
 [project.urls]
-Homepage  = "https://github.com/AdaptiveMotorControlLab/CellSeg3d"
+Homepage  = "https://github.com/AdaptiveMotorControlLab/CellSeg3D"
 Documentation = "https://adaptivemotorcontrollab.github.io/cellseg3d-docs/res/welcome.html"
-Issues = "https://github.com/AdaptiveMotorControlLab/CellSeg3d/issues"
+Issues = "https://github.com/AdaptiveMotorControlLab/CellSeg3D/issues"
 
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 include-package-data = true
@@ -122,14 +122,23 @@
 profile = "black"
 line_length = 79
 
 [project.optional-dependencies]
 #crf = [
 #   "pydensecrf@git+https://github.com/lucasb-eyer/pydensecrf.git#egg=master",
 #]
+pyqt5 = [
+    "pyqt5",
+]
+pyside2 = [
+    "pyside2",
+]
+pyside6 = [
+    "pyside6",
+]
 onnx-cpu = [
     "onnx",
     "onnxruntime"
 ]
 onnx-gpu = [
     "onnx",
     "onnxruntime-gpu"
```

### Comparing `napari_cellseg3d-0.1.2/setup.cfg` & `napari_cellseg3d-0.2.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = napari_cellseg3d
-version = 0.1.2
+version = 0.2.0
 
 [options]
 packages = find:
 include_package_data = True
 python_requires = >=3.8
 package_dir = 
 	=.
@@ -29,20 +29,20 @@
 	matplotlib
 	vispy>=0.9.6
 
 [options.packages.find]
 where = .
 
 [options.package_data]
-napari-cellseg3d = 
+napari_cellseg3d = 
 	res/*.png
 	code_models/models/pretrained/*.json
 	napari.yaml
 
 [options.entry_points]
 napari.manifest = 
-	napari-cellseg3d = napari_cellseg3d:napari.yaml
+	napari_cellseg3d = napari_cellseg3d:napari.yaml
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

