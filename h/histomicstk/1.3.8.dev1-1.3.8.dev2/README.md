# Comparing `tmp/histomicstk-1.3.8.dev1.tar.gz` & `tmp/histomicstk-1.3.8.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "histomicstk-1.3.8.dev1.tar", last modified: Mon May 13 12:11:45 2024, max compression
+gzip compressed data, was "histomicstk-1.3.8.dev2.tar", last modified: Mon May 13 13:02:27 2024, max compression
```

## Comparing `histomicstk-1.3.8.dev1.tar` & `histomicstk-1.3.8.dev2.tar`

### file list

```diff
@@ -1,209 +1,209 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:11:45.370391 histomicstk-1.3.8.dev1/
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-13 12:11:34.000000 histomicstk-1.3.8.dev1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-13 12:11:34.000000 histomicstk-1.3.8.dev1/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9316 2024-05-13 12:11:34.000000 histomicstk-1.3.8.dev1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10173 2024-05-13 12:11:34.000000 histomicstk-1.3.8.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-13 12:11:34.000000 histomicstk-1.3.8.dev1/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     9800 2024-05-13 12:11:45.370391 histomicstk-1.3.8.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8046 2024-05-13 12:11:34.000000 histomicstk-1.3.8.dev1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:11:45.342391 histomicstk-1.3.8.dev1/histomicstk/
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:11:45.346391 histomicstk-1.3.8.dev1/histomicstk/annotations_and_masks/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/annotations_and_masks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26418 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/annotations_and_masks/annotation_and_mask_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12271 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/annotations_and_masks/annotation_database_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    37211 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/annotations_and_masks/annotations_to_masks_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)    28174 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/annotations_and_masks/annotations_to_object_mask_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)    24653 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/annotations_and_masks/masks_to_annotations_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)    27304 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/annotations_and_masks/polygon_merger.py
--rw-r--r--   0 runner    (1001) docker     (127)    10196 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/annotations_and_masks/polygon_merger_v2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:11:45.346391 histomicstk-1.3.8.dev1/histomicstk/annotations_and_masks/pyrtree/
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/annotations_and_masks/pyrtree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5376 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/annotations_and_masks/pyrtree/rect.py
--rw-r--r--   0 runner    (1001) docker     (127)    15078 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/annotations_and_masks/pyrtree/rtree.py
--rw-r--r--   0 runner    (1001) docker     (127)    14909 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/annotations_and_masks/review_gallery.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:11:45.346391 histomicstk-1.3.8.dev1/histomicstk/annotations_and_masks/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4234 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/annotations_and_masks/tests/test_annotation_and_mask_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4829 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/annotations_and_masks/tests/test_annotation_database_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    10375 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/annotations_and_masks/tests/test_annotations_to_masks_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     7622 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/annotations_and_masks/tests/test_annotations_to_object_mask_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     6544 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/annotations_and_masks/tests/test_masks_to_annotations_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4876 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/annotations_and_masks/tests/test_polygon_merger.py
--rw-r--r--   0 runner    (1001) docker     (127)     5582 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/annotations_and_masks/tests/test_review_gallery.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:11:45.346391 histomicstk-1.3.8.dev1/histomicstk/cli/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:11:45.350391 histomicstk-1.3.8.dev1/histomicstk/cli/BackgroundIntensity/
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/cli/BackgroundIntensity/BackgroundIntensity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/cli/BackgroundIntensity/BackgroundIntensity.xml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/cli/BackgroundIntensity/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:11:45.350391 histomicstk-1.3.8.dev1/histomicstk/cli/ColorDeconvolution/
--rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/cli/ColorDeconvolution/ColorDeconvolution.py
--rw-r--r--   0 runner    (1001) docker     (127)     4620 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/cli/ColorDeconvolution/ColorDeconvolution.xml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/cli/ColorDeconvolution/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:11:45.350391 histomicstk-1.3.8.dev1/histomicstk/cli/ComputeNucleiFeatures/
--rw-r--r--   0 runner    (1001) docker     (127)     8662 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/cli/ComputeNucleiFeatures/ComputeNucleiFeatures.py
--rw-r--r--   0 runner    (1001) docker     (127)    12746 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/cli/ComputeNucleiFeatures/ComputeNucleiFeatures.xml
--rw-r--r--   0 runner    (1001) docker     (127)     7848 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/cli/ComputeNucleiFeatures/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/cli/ComputeNucleiFeatures/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:11:45.350391 histomicstk-1.3.8.dev1/histomicstk/cli/NucleiClassification/
--rw-r--r--   0 runner    (1001) docker     (127)     9323 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/cli/NucleiClassification/NucleiClassification.py
--rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/cli/NucleiClassification/NucleiClassification.xml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/cli/NucleiClassification/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:11:45.350391 histomicstk-1.3.8.dev1/histomicstk/cli/NucleiDetection/
--rw-r--r--   0 runner    (1001) docker     (127)    12276 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/cli/NucleiDetection/NucleiDetection.py
--rw-r--r--   0 runner    (1001) docker     (127)    11008 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/cli/NucleiDetection/NucleiDetection.xml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/cli/NucleiDetection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:11:45.350391 histomicstk-1.3.8.dev1/histomicstk/cli/PositivePixelCount/
--rw-r--r--   0 runner    (1001) docker     (127)     7749 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/cli/PositivePixelCount/PositivePixelCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     6373 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/cli/PositivePixelCount/PositivePixelCount.xml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/cli/PositivePixelCount/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:11:45.350391 histomicstk-1.3.8.dev1/histomicstk/cli/SeparateStainsMacenkoPCA/
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/cli/SeparateStainsMacenkoPCA/SeparateStainsMacenkoPCA.py
--rw-r--r--   0 runner    (1001) docker     (127)     5011 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/cli/SeparateStainsMacenkoPCA/SeparateStainsMacenkoPCA.xml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/cli/SeparateStainsMacenkoPCA/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:11:45.350391 histomicstk-1.3.8.dev1/histomicstk/cli/SeparateStainsXuSnmf/
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/cli/SeparateStainsXuSnmf/SeparateStainsXuSnmf.py
--rw-r--r--   0 runner    (1001) docker     (127)     5765 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/cli/SeparateStainsXuSnmf/SeparateStainsXuSnmf.xml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/cli/SeparateStainsXuSnmf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:11:45.354391 histomicstk-1.3.8.dev1/histomicstk/cli/SuperpixelSegmentation/
--rw-r--r--   0 runner    (1001) docker     (127)    11856 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/cli/SuperpixelSegmentation/SuperpixelSegmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6100 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/cli/SuperpixelSegmentation/SuperpixelSegmentation.xml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/cli/SuperpixelSegmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/cli/dask_config.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)      423 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/cli/docker-entrypoint.sh
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/cli/slicer_cli_list.json
--rw-r--r--   0 runner    (1001) docker     (127)    16959 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:11:45.354391 histomicstk-1.3.8.dev1/histomicstk/features/
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/features/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/features/_compute_marginal_glcm_probs_cython.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     7331 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/features/compute_fsd_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     7927 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/features/compute_global_cell_graph_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/features/compute_gradient_features.py
--rw-r--r--   0 runner    (1001) docker     (127)    13389 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/features/compute_haralick_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     6070 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/features/compute_intensity_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     7883 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/features/compute_morphometry_features.py
--rw-r--r--   0 runner    (1001) docker     (127)    11575 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/features/compute_nuclei_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     8470 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/features/graycomatrixext.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:11:45.354391 histomicstk-1.3.8.dev1/histomicstk/filters/
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/filters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:11:45.354391 histomicstk-1.3.8.dev1/histomicstk/filters/edge/
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/filters/edge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/filters/edge/gaussian_grad.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:11:45.354391 histomicstk-1.3.8.dev1/histomicstk/filters/shape/
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/filters/shape/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/filters/shape/cdog.py
--rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/filters/shape/clog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/filters/shape/glog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/filters/shape/vesselness.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:11:45.354391 histomicstk-1.3.8.dev1/histomicstk/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/preprocessing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:11:45.358391 histomicstk-1.3.8.dev1/histomicstk/preprocessing/augmentation/
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/preprocessing/augmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/preprocessing/augmentation/color_augmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:11:45.358391 histomicstk-1.3.8.dev1/histomicstk/preprocessing/color_conversion/
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/preprocessing/color_conversion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/preprocessing/color_conversion/lab_mean_std.py
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/preprocessing/color_conversion/lab_to_rgb.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/preprocessing/color_conversion/od_to_rgb.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/preprocessing/color_conversion/rgb_to_hsi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/preprocessing/color_conversion/rgb_to_lab.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/preprocessing/color_conversion/rgb_to_od.py
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/preprocessing/color_conversion/rgb_to_sda.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/preprocessing/color_conversion/sda_to_rgb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:11:45.358391 histomicstk-1.3.8.dev1/histomicstk/preprocessing/color_deconvolution/
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/preprocessing/color_deconvolution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/preprocessing/color_deconvolution/_linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/preprocessing/color_deconvolution/color_convolution.py
--rw-r--r--   0 runner    (1001) docker     (127)    10216 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/preprocessing/color_deconvolution/color_deconvolution.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/preprocessing/color_deconvolution/complement_stain_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/preprocessing/color_deconvolution/find_stain_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/preprocessing/color_deconvolution/rgb_separate_stains_macenko_pca.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/preprocessing/color_deconvolution/rgb_separate_stains_xu_snmf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4487 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/preprocessing/color_deconvolution/separate_stains_macenko_pca.py
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/preprocessing/color_deconvolution/separate_stains_xu_snmf.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/preprocessing/color_deconvolution/stain_color_map.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:11:45.362391 histomicstk-1.3.8.dev1/histomicstk/preprocessing/color_normalization/
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/preprocessing/color_normalization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/preprocessing/color_normalization/background_intensity.py
--rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/preprocessing/color_normalization/deconvolution_based_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/preprocessing/color_normalization/reinhard.py
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/preprocessing/color_normalization/reinhard_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:11:45.362391 histomicstk-1.3.8.dev1/histomicstk/preprocessing/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5955 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/preprocessing/tests/test_normalization_and_augmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:11:45.362391 histomicstk-1.3.8.dev1/histomicstk/saliency/
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/saliency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23723 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/saliency/cellularity_detection_superpixels.py
--rw-r--r--   0 runner    (1001) docker     (127)    26865 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/saliency/cellularity_detection_thresholding.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:11:45.362391 histomicstk-1.3.8.dev1/histomicstk/saliency/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4873 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/saliency/tests/test_saliency.py
--rw-r--r--   0 runner    (1001) docker     (127)     8764 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/saliency/tissue_detection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:11:45.362391 histomicstk-1.3.8.dev1/histomicstk/segmentation/
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/segmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/segmentation/embed_boundaries.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:11:45.366391 histomicstk-1.3.8.dev1/histomicstk/segmentation/label/
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/segmentation/label/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/segmentation/label/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14960 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/segmentation/label/_trace_object_boundaries_cython.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/segmentation/label/area_open.py
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/segmentation/label/compact.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/segmentation/label/condense.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/segmentation/label/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/segmentation/label/delete_border.py
--rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/segmentation/label/delete_overlap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/segmentation/label/dilate_xor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/segmentation/label/perimeter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/segmentation/label/remove_overlap_nuclei.py
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/segmentation/label/shuffle.py
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/segmentation/label/split.py
--rw-r--r--   0 runner    (1001) docker     (127)     5940 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/segmentation/label/trace_object_boundaries.py
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/segmentation/label/width_open.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:11:45.366391 histomicstk-1.3.8.dev1/histomicstk/segmentation/level_set/
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/segmentation/level_set/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/segmentation/level_set/chan_vese.py
--rw-r--r--   0 runner    (1001) docker     (127)     5610 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/segmentation/level_set/reg_edge.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:11:45.366391 histomicstk-1.3.8.dev1/histomicstk/segmentation/nuclear/
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/segmentation/nuclear/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/segmentation/nuclear/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/segmentation/nuclear/_max_clustering_cython.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/segmentation/nuclear/detect_nuclei_kofahi.py
--rw-r--r--   0 runner    (1001) docker     (127)     4908 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/segmentation/nuclear/detect_tile_nuclei.py
--rw-r--r--   0 runner    (1001) docker     (127)     4860 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/segmentation/nuclear/gaussian_voting.py
--rw-r--r--   0 runner    (1001) docker     (127)     9032 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/segmentation/nuclear/gvf_tracking.py
--rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/segmentation/nuclear/max_clustering.py
--rw-r--r--   0 runner    (1001) docker     (127)    29320 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/segmentation/nuclear/min_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8309 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/segmentation/positive_pixel_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/segmentation/rag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/segmentation/rag_add_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/segmentation/rag_color.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:11:45.370391 histomicstk-1.3.8.dev1/histomicstk/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/utils/compute_tile_foreground_fraction.py
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/utils/convert_image_to_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/utils/convert_matrix_to_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/utils/del2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/utils/eigen.py
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/utils/exclude_nonfinite.py
--rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/utils/fit_poisson_mixture.py
--rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/utils/general_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    17842 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/utils/girder_convenience_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/utils/gradient_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/utils/hessian.py
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/utils/merge_colinear.py
--rw-r--r--   0 runner    (1001) docker     (127)     7858 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/utils/sample_pixels.py
--rw-r--r--   0 runner    (1001) docker     (127)     8433 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/utils/simple_mask.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:11:45.370391 histomicstk-1.3.8.dev1/histomicstk/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4122 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/utils/tests/test_girder_convenience_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:11:45.370391 histomicstk-1.3.8.dev1/histomicstk/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/workflows/specific_workflows.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:11:45.370391 histomicstk-1.3.8.dev1/histomicstk/workflows/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/workflows/tests/test_workflow_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     8435 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/histomicstk/workflows/workflow_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:11:45.370391 histomicstk-1.3.8.dev1/histomicstk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8380 2024-05-13 12:11:45.000000 histomicstk-1.3.8.dev1/histomicstk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 12:11:45.370391 histomicstk-1.3.8.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-05-13 12:11:35.000000 histomicstk-1.3.8.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:02:27.136257 histomicstk-1.3.8.dev2/
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-13 13:02:19.000000 histomicstk-1.3.8.dev2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-13 13:02:19.000000 histomicstk-1.3.8.dev2/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9316 2024-05-13 13:02:19.000000 histomicstk-1.3.8.dev2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10173 2024-05-13 13:02:19.000000 histomicstk-1.3.8.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-13 13:02:19.000000 histomicstk-1.3.8.dev2/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     9800 2024-05-13 13:02:27.136257 histomicstk-1.3.8.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8046 2024-05-13 13:02:19.000000 histomicstk-1.3.8.dev2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:02:27.108257 histomicstk-1.3.8.dev2/histomicstk/
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:02:27.112257 histomicstk-1.3.8.dev2/histomicstk/annotations_and_masks/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/annotations_and_masks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26418 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/annotations_and_masks/annotation_and_mask_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12271 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/annotations_and_masks/annotation_database_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37211 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/annotations_and_masks/annotations_to_masks_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28174 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/annotations_and_masks/annotations_to_object_mask_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24653 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/annotations_and_masks/masks_to_annotations_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27304 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/annotations_and_masks/polygon_merger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10196 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/annotations_and_masks/polygon_merger_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:02:27.112257 histomicstk-1.3.8.dev2/histomicstk/annotations_and_masks/pyrtree/
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/annotations_and_masks/pyrtree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5376 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/annotations_and_masks/pyrtree/rect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15078 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/annotations_and_masks/pyrtree/rtree.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14909 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/annotations_and_masks/review_gallery.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:02:27.112257 histomicstk-1.3.8.dev2/histomicstk/annotations_and_masks/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4234 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/annotations_and_masks/tests/test_annotation_and_mask_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4829 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/annotations_and_masks/tests/test_annotation_database_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10375 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/annotations_and_masks/tests/test_annotations_to_masks_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7622 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/annotations_and_masks/tests/test_annotations_to_object_mask_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6544 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/annotations_and_masks/tests/test_masks_to_annotations_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4876 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/annotations_and_masks/tests/test_polygon_merger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5582 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/annotations_and_masks/tests/test_review_gallery.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:02:27.112257 histomicstk-1.3.8.dev2/histomicstk/cli/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:02:27.112257 histomicstk-1.3.8.dev2/histomicstk/cli/BackgroundIntensity/
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/cli/BackgroundIntensity/BackgroundIntensity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/cli/BackgroundIntensity/BackgroundIntensity.xml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/cli/BackgroundIntensity/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:02:27.112257 histomicstk-1.3.8.dev2/histomicstk/cli/ColorDeconvolution/
+-rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/cli/ColorDeconvolution/ColorDeconvolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4620 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/cli/ColorDeconvolution/ColorDeconvolution.xml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/cli/ColorDeconvolution/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:02:27.116257 histomicstk-1.3.8.dev2/histomicstk/cli/ComputeNucleiFeatures/
+-rw-r--r--   0 runner    (1001) docker     (127)     8662 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/cli/ComputeNucleiFeatures/ComputeNucleiFeatures.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12746 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/cli/ComputeNucleiFeatures/ComputeNucleiFeatures.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     7848 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/cli/ComputeNucleiFeatures/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/cli/ComputeNucleiFeatures/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:02:27.116257 histomicstk-1.3.8.dev2/histomicstk/cli/NucleiClassification/
+-rw-r--r--   0 runner    (1001) docker     (127)     9323 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/cli/NucleiClassification/NucleiClassification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/cli/NucleiClassification/NucleiClassification.xml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/cli/NucleiClassification/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:02:27.116257 histomicstk-1.3.8.dev2/histomicstk/cli/NucleiDetection/
+-rw-r--r--   0 runner    (1001) docker     (127)    12276 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/cli/NucleiDetection/NucleiDetection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11008 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/cli/NucleiDetection/NucleiDetection.xml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/cli/NucleiDetection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:02:27.116257 histomicstk-1.3.8.dev2/histomicstk/cli/PositivePixelCount/
+-rw-r--r--   0 runner    (1001) docker     (127)     7749 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/cli/PositivePixelCount/PositivePixelCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6373 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/cli/PositivePixelCount/PositivePixelCount.xml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/cli/PositivePixelCount/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:02:27.116257 histomicstk-1.3.8.dev2/histomicstk/cli/SeparateStainsMacenkoPCA/
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/cli/SeparateStainsMacenkoPCA/SeparateStainsMacenkoPCA.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5011 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/cli/SeparateStainsMacenkoPCA/SeparateStainsMacenkoPCA.xml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/cli/SeparateStainsMacenkoPCA/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:02:27.116257 histomicstk-1.3.8.dev2/histomicstk/cli/SeparateStainsXuSnmf/
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/cli/SeparateStainsXuSnmf/SeparateStainsXuSnmf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5765 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/cli/SeparateStainsXuSnmf/SeparateStainsXuSnmf.xml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/cli/SeparateStainsXuSnmf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:02:27.116257 histomicstk-1.3.8.dev2/histomicstk/cli/SuperpixelSegmentation/
+-rw-r--r--   0 runner    (1001) docker     (127)    11856 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/cli/SuperpixelSegmentation/SuperpixelSegmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6100 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/cli/SuperpixelSegmentation/SuperpixelSegmentation.xml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/cli/SuperpixelSegmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/cli/dask_config.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      423 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/cli/docker-entrypoint.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/cli/slicer_cli_list.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16959 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:02:27.120257 histomicstk-1.3.8.dev2/histomicstk/features/
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/features/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/features/_compute_marginal_glcm_probs_cython.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     7366 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/features/compute_fsd_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7927 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/features/compute_global_cell_graph_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4172 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/features/compute_gradient_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13486 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/features/compute_haralick_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6070 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/features/compute_intensity_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7625 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/features/compute_morphometry_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11216 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/features/compute_nuclei_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8470 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/features/graycomatrixext.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:02:27.120257 histomicstk-1.3.8.dev2/histomicstk/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/filters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:02:27.120257 histomicstk-1.3.8.dev2/histomicstk/filters/edge/
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/filters/edge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/filters/edge/gaussian_grad.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:02:27.120257 histomicstk-1.3.8.dev2/histomicstk/filters/shape/
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/filters/shape/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/filters/shape/cdog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/filters/shape/clog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/filters/shape/glog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/filters/shape/vesselness.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:02:27.120257 histomicstk-1.3.8.dev2/histomicstk/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/preprocessing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:02:27.120257 histomicstk-1.3.8.dev2/histomicstk/preprocessing/augmentation/
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/preprocessing/augmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/preprocessing/augmentation/color_augmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:02:27.124257 histomicstk-1.3.8.dev2/histomicstk/preprocessing/color_conversion/
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/preprocessing/color_conversion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/preprocessing/color_conversion/lab_mean_std.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/preprocessing/color_conversion/lab_to_rgb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/preprocessing/color_conversion/od_to_rgb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/preprocessing/color_conversion/rgb_to_hsi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/preprocessing/color_conversion/rgb_to_lab.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/preprocessing/color_conversion/rgb_to_od.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/preprocessing/color_conversion/rgb_to_sda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/preprocessing/color_conversion/sda_to_rgb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:02:27.124257 histomicstk-1.3.8.dev2/histomicstk/preprocessing/color_deconvolution/
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/preprocessing/color_deconvolution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/preprocessing/color_deconvolution/_linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/preprocessing/color_deconvolution/color_convolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10216 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/preprocessing/color_deconvolution/color_deconvolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/preprocessing/color_deconvolution/complement_stain_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/preprocessing/color_deconvolution/find_stain_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/preprocessing/color_deconvolution/rgb_separate_stains_macenko_pca.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/preprocessing/color_deconvolution/rgb_separate_stains_xu_snmf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4487 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/preprocessing/color_deconvolution/separate_stains_macenko_pca.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/preprocessing/color_deconvolution/separate_stains_xu_snmf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/preprocessing/color_deconvolution/stain_color_map.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:02:27.124257 histomicstk-1.3.8.dev2/histomicstk/preprocessing/color_normalization/
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/preprocessing/color_normalization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/preprocessing/color_normalization/background_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/preprocessing/color_normalization/deconvolution_based_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/preprocessing/color_normalization/reinhard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/preprocessing/color_normalization/reinhard_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:02:27.124257 histomicstk-1.3.8.dev2/histomicstk/preprocessing/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5955 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/preprocessing/tests/test_normalization_and_augmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:02:27.124257 histomicstk-1.3.8.dev2/histomicstk/saliency/
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/saliency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23723 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/saliency/cellularity_detection_superpixels.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26865 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/saliency/cellularity_detection_thresholding.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:02:27.124257 histomicstk-1.3.8.dev2/histomicstk/saliency/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4873 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/saliency/tests/test_saliency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8764 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/saliency/tissue_detection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:02:27.128257 histomicstk-1.3.8.dev2/histomicstk/segmentation/
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/segmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/segmentation/embed_boundaries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:02:27.128257 histomicstk-1.3.8.dev2/histomicstk/segmentation/label/
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/segmentation/label/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/segmentation/label/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14960 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/segmentation/label/_trace_object_boundaries_cython.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/segmentation/label/area_open.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/segmentation/label/compact.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/segmentation/label/condense.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/segmentation/label/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/segmentation/label/delete_border.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/segmentation/label/delete_overlap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/segmentation/label/dilate_xor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/segmentation/label/perimeter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/segmentation/label/remove_overlap_nuclei.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/segmentation/label/shuffle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/segmentation/label/split.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5940 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/segmentation/label/trace_object_boundaries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/segmentation/label/width_open.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:02:27.128257 histomicstk-1.3.8.dev2/histomicstk/segmentation/level_set/
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/segmentation/level_set/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/segmentation/level_set/chan_vese.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5610 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/segmentation/level_set/reg_edge.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:02:27.132257 histomicstk-1.3.8.dev2/histomicstk/segmentation/nuclear/
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/segmentation/nuclear/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/segmentation/nuclear/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/segmentation/nuclear/_max_clustering_cython.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/segmentation/nuclear/detect_nuclei_kofahi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4908 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/segmentation/nuclear/detect_tile_nuclei.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4860 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/segmentation/nuclear/gaussian_voting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9032 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/segmentation/nuclear/gvf_tracking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/segmentation/nuclear/max_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29320 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/segmentation/nuclear/min_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8309 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/segmentation/positive_pixel_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/segmentation/rag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/segmentation/rag_add_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/segmentation/rag_color.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:02:27.132257 histomicstk-1.3.8.dev2/histomicstk/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/utils/compute_tile_foreground_fraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/utils/convert_image_to_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/utils/convert_matrix_to_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/utils/del2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/utils/eigen.py
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/utils/exclude_nonfinite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/utils/fit_poisson_mixture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/utils/general_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17842 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/utils/girder_convenience_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/utils/gradient_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/utils/hessian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/utils/merge_colinear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7858 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/utils/sample_pixels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8433 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/utils/simple_mask.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:02:27.132257 histomicstk-1.3.8.dev2/histomicstk/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4122 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/utils/tests/test_girder_convenience_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:02:27.136257 histomicstk-1.3.8.dev2/histomicstk/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/workflows/specific_workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:02:27.136257 histomicstk-1.3.8.dev2/histomicstk/workflows/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/workflows/tests/test_workflow_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8435 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/histomicstk/workflows/workflow_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:02:27.136257 histomicstk-1.3.8.dev2/histomicstk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8380 2024-05-13 13:02:27.000000 histomicstk-1.3.8.dev2/histomicstk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 13:02:27.136257 histomicstk-1.3.8.dev2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-05-13 13:02:20.000000 histomicstk-1.3.8.dev2/setup.py
```

### Comparing `histomicstk-1.3.8.dev1/CONTRIBUTING.rst` & `histomicstk-1.3.8.dev2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/LICENSE` & `histomicstk-1.3.8.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/NOTICE` & `histomicstk-1.3.8.dev2/NOTICE`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/PKG-INFO` & `histomicstk-1.3.8.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: histomicstk
-Version: 1.3.8.dev1
+Version: 1.3.8.dev2
 Summary: A Python toolkit for Histopathology Image Analysis
 Home-page: https://github.com/DigitalSlideArchive/HistomicsTK
 Author: Kitware, Inc.
 Author-email: developers@digitalslidearchive.net
 License: Apache Software License 2.0
 Keywords: histomicstk
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `histomicstk-1.3.8.dev1/README.rst` & `histomicstk-1.3.8.dev2/README.rst`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/__init__.py` & `histomicstk-1.3.8.dev2/histomicstk/__init__.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/annotations_and_masks/annotation_and_mask_utils.py` & `histomicstk-1.3.8.dev2/histomicstk/annotations_and_masks/annotation_and_mask_utils.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/annotations_and_masks/annotation_database_parser.py` & `histomicstk-1.3.8.dev2/histomicstk/annotations_and_masks/annotation_database_parser.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/annotations_and_masks/annotations_to_masks_handler.py` & `histomicstk-1.3.8.dev2/histomicstk/annotations_and_masks/annotations_to_masks_handler.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/annotations_and_masks/annotations_to_object_mask_handler.py` & `histomicstk-1.3.8.dev2/histomicstk/annotations_and_masks/annotations_to_object_mask_handler.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/annotations_and_masks/masks_to_annotations_handler.py` & `histomicstk-1.3.8.dev2/histomicstk/annotations_and_masks/masks_to_annotations_handler.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/annotations_and_masks/polygon_merger.py` & `histomicstk-1.3.8.dev2/histomicstk/annotations_and_masks/polygon_merger.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/annotations_and_masks/polygon_merger_v2.py` & `histomicstk-1.3.8.dev2/histomicstk/annotations_and_masks/polygon_merger_v2.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/annotations_and_masks/pyrtree/__init__.py` & `histomicstk-1.3.8.dev2/histomicstk/annotations_and_masks/pyrtree/__init__.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/annotations_and_masks/pyrtree/rect.py` & `histomicstk-1.3.8.dev2/histomicstk/annotations_and_masks/pyrtree/rect.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/annotations_and_masks/pyrtree/rtree.py` & `histomicstk-1.3.8.dev2/histomicstk/annotations_and_masks/pyrtree/rtree.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/annotations_and_masks/review_gallery.py` & `histomicstk-1.3.8.dev2/histomicstk/annotations_and_masks/review_gallery.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/annotations_and_masks/tests/test_annotation_and_mask_utils.py` & `histomicstk-1.3.8.dev2/histomicstk/annotations_and_masks/tests/test_annotation_and_mask_utils.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/annotations_and_masks/tests/test_annotation_database_parser.py` & `histomicstk-1.3.8.dev2/histomicstk/annotations_and_masks/tests/test_annotation_database_parser.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/annotations_and_masks/tests/test_annotations_to_masks_handler.py` & `histomicstk-1.3.8.dev2/histomicstk/annotations_and_masks/tests/test_annotations_to_masks_handler.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/annotations_and_masks/tests/test_annotations_to_object_mask_handler.py` & `histomicstk-1.3.8.dev2/histomicstk/annotations_and_masks/tests/test_annotations_to_object_mask_handler.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/annotations_and_masks/tests/test_masks_to_annotations_handler.py` & `histomicstk-1.3.8.dev2/histomicstk/annotations_and_masks/tests/test_masks_to_annotations_handler.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/annotations_and_masks/tests/test_polygon_merger.py` & `histomicstk-1.3.8.dev2/histomicstk/annotations_and_masks/tests/test_polygon_merger.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/annotations_and_masks/tests/test_review_gallery.py` & `histomicstk-1.3.8.dev2/histomicstk/annotations_and_masks/tests/test_review_gallery.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/cli/BackgroundIntensity/BackgroundIntensity.py` & `histomicstk-1.3.8.dev2/histomicstk/cli/BackgroundIntensity/BackgroundIntensity.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/cli/BackgroundIntensity/BackgroundIntensity.xml` & `histomicstk-1.3.8.dev2/histomicstk/cli/BackgroundIntensity/BackgroundIntensity.xml`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/cli/ColorDeconvolution/ColorDeconvolution.py` & `histomicstk-1.3.8.dev2/histomicstk/cli/ColorDeconvolution/ColorDeconvolution.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/cli/ColorDeconvolution/ColorDeconvolution.xml` & `histomicstk-1.3.8.dev2/histomicstk/cli/ColorDeconvolution/ColorDeconvolution.xml`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/cli/ComputeNucleiFeatures/ComputeNucleiFeatures.py` & `histomicstk-1.3.8.dev2/histomicstk/cli/ComputeNucleiFeatures/ComputeNucleiFeatures.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/cli/ComputeNucleiFeatures/ComputeNucleiFeatures.xml` & `histomicstk-1.3.8.dev2/histomicstk/cli/ComputeNucleiFeatures/ComputeNucleiFeatures.xml`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/cli/ComputeNucleiFeatures/README.md` & `histomicstk-1.3.8.dev2/histomicstk/cli/ComputeNucleiFeatures/README.md`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/cli/NucleiClassification/NucleiClassification.py` & `histomicstk-1.3.8.dev2/histomicstk/cli/NucleiClassification/NucleiClassification.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/cli/NucleiClassification/NucleiClassification.xml` & `histomicstk-1.3.8.dev2/histomicstk/cli/NucleiClassification/NucleiClassification.xml`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/cli/NucleiDetection/NucleiDetection.py` & `histomicstk-1.3.8.dev2/histomicstk/cli/NucleiDetection/NucleiDetection.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/cli/NucleiDetection/NucleiDetection.xml` & `histomicstk-1.3.8.dev2/histomicstk/cli/NucleiDetection/NucleiDetection.xml`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/cli/PositivePixelCount/PositivePixelCount.py` & `histomicstk-1.3.8.dev2/histomicstk/cli/PositivePixelCount/PositivePixelCount.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/cli/PositivePixelCount/PositivePixelCount.xml` & `histomicstk-1.3.8.dev2/histomicstk/cli/PositivePixelCount/PositivePixelCount.xml`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/cli/SeparateStainsMacenkoPCA/SeparateStainsMacenkoPCA.py` & `histomicstk-1.3.8.dev2/histomicstk/cli/SeparateStainsMacenkoPCA/SeparateStainsMacenkoPCA.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/cli/SeparateStainsMacenkoPCA/SeparateStainsMacenkoPCA.xml` & `histomicstk-1.3.8.dev2/histomicstk/cli/SeparateStainsMacenkoPCA/SeparateStainsMacenkoPCA.xml`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/cli/SeparateStainsXuSnmf/SeparateStainsXuSnmf.py` & `histomicstk-1.3.8.dev2/histomicstk/cli/SeparateStainsXuSnmf/SeparateStainsXuSnmf.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/cli/SeparateStainsXuSnmf/SeparateStainsXuSnmf.xml` & `histomicstk-1.3.8.dev2/histomicstk/cli/SeparateStainsXuSnmf/SeparateStainsXuSnmf.xml`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/cli/SuperpixelSegmentation/SuperpixelSegmentation.py` & `histomicstk-1.3.8.dev2/histomicstk/cli/SuperpixelSegmentation/SuperpixelSegmentation.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/cli/SuperpixelSegmentation/SuperpixelSegmentation.xml` & `histomicstk-1.3.8.dev2/histomicstk/cli/SuperpixelSegmentation/SuperpixelSegmentation.xml`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/cli/slicer_cli_list.json` & `histomicstk-1.3.8.dev2/histomicstk/cli/slicer_cli_list.json`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/cli/utils.py` & `histomicstk-1.3.8.dev2/histomicstk/cli/utils.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/features/__init__.py` & `histomicstk-1.3.8.dev2/histomicstk/features/__init__.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/features/_compute_marginal_glcm_probs_cython.pyx` & `histomicstk-1.3.8.dev2/histomicstk/features/_compute_marginal_glcm_probs_cython.pyx`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/features/compute_fsd_features.py` & `histomicstk-1.3.8.dev2/histomicstk/features/compute_fsd_features.py`

 * *Files 7% similar despite different names*

```diff
@@ -52,42 +52,44 @@
     # get the number of objects in Label
     if rprops is None:
         rprops = regionprops(im_label)
 
     # create pandas data frame containing the features for each object
     numFeatures = len(feature_list)
     numLabels = len(rprops)
-    fdata = pd.DataFrame(np.zeros((numLabels, numFeatures)),
-                         columns=feature_list)
 
-    # fourier descriptors, spaced evenly over the interval 1:K/2
+    # pre-compute Interval outside the loop
     Interval = np.round(
-        np.power(
-            2, np.linspace(0, np.log2(K) - 1, Fs + 1, endpoint=True),
-        ),
+        np.power(2, np.linspace(0, np.log2(K) - 1, Fs + 1, endpoint=True)),
     ).astype(np.uint8)
 
+    # initialize an empty list to collect data
+    data_list = []
+
     for i in range(numLabels):
         # get bounds of dilated nucleus
-        min_row, max_row, min_col, max_col = \
-            _GetBounds(rprops[i].bbox, Delta, sizex, sizey)
+        min_row, max_row, min_col, max_col = _GetBounds(
+            rprops[i].bbox, Delta, sizex, sizey,
+        )
+
         # grab label mask
-        lmask = (
-            im_label[min_row:max_row, min_col:max_col] == rprops[i].label
-        ).astype(bool)
+        lmask = (im_label[min_row:max_row, min_col:max_col] == rprops[i].label).astype(bool)
         # find boundaries
         Bounds = np.argwhere(
             find_boundaries(lmask, mode='inner').astype(np.uint8) == 1,
         )
         # check length of boundaries
         if len(Bounds) < 2:
-            fdata.iloc[i, :] = 0
+            data_list.append(np.zeros(numFeatures))
         else:
-            # compute fourier descriptors
-            fdata.iloc[i, :] = _FSDs(Bounds[:, 0], Bounds[:, 1], K, Interval)
+            # compute fourier descriptors and collect data
+            data_list.append(_FSDs(Bounds[:, 0], Bounds[:, 1], K, Interval))
+
+    # create DataFrame after the loop
+    fdata = pd.DataFrame(data_list, columns=feature_list)
 
     return fdata
 
 
 def _InterpolateArcLength(X, Y, K):
     """
     Resamples boundary points [X, Y] at L total equal arc-length locations.
```

### Comparing `histomicstk-1.3.8.dev1/histomicstk/features/compute_global_cell_graph_features.py` & `histomicstk-1.3.8.dev2/histomicstk/features/compute_global_cell_graph_features.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/features/compute_gradient_features.py` & `histomicstk-1.3.8.dev2/histomicstk/features/compute_gradient_features.py`

 * *Files 21% similar despite different names*

```diff
@@ -74,61 +74,64 @@
         'Gradient.Mag.Kurtosis',
         'Gradient.Mag.HistEntropy',
         'Gradient.Mag.HistEnergy',
         'Gradient.Canny.Sum',
         'Gradient.Canny.Mean',
     ]
 
-    # compute object properties if not provided
+    # Compute object properties if not provided
     if rprops is None:
         rprops = regionprops(im_label)
 
-    # create pandas data frame containing the features for each object
-    numFeatures = len(feature_list)
     numLabels = len(rprops)
-    fdata = pd.DataFrame(np.zeros((numLabels, numFeatures)),
-                         columns=feature_list)
 
     Gx, Gy = np.gradient(im_intensity)
     diffG = np.sqrt(Gx**2 + Gy**2)
     cannyG = canny(im_intensity)
 
+    # Prepare data collection
+    data = []
+
     for i in range(numLabels):
         if rprops[i] is None:
             continue
 
         # get gradients of object pixels
-        pixelGradients = np.sort(
-            diffG[rprops[i].coords[:, 0], rprops[i].coords[:, 1]],
-        )
-
-        # compute mean
-        fdata.at[i, 'Gradient.Mag.Mean'] = np.mean(pixelGradients)
-
-        # compute standard deviation
-        fdata.at[i, 'Gradient.Mag.Std'] = np.std(pixelGradients)
-
-        # compute skewness
-        fdata.at[i, 'Gradient.Mag.Skewness'] = scipy.stats.skew(pixelGradients)
+        pixelGradients = np.sort(diffG[rprops[i].coords[:, 0], rprops[i].coords[:, 1]])
 
-        # compute kurtosis
-        fdata.at[i, 'Gradient.Mag.Kurtosis'] = \
-            scipy.stats.kurtosis(pixelGradients)
-
-        # compute intensity histogram
+        # Compute intensity histogram
         hist, bins = np.histogram(pixelGradients, bins=num_hist_bins)
         prob = hist / np.sum(hist, dtype=np.float32)
 
-        # compute entropy
-        fdata.at[i, 'Gradient.Mag.HistEntropy'] = scipy.stats.entropy(prob)
-
-        # compute energy
-        fdata.at[i, 'Gradient.Mag.HistEnergy'] = np.sum(prob**2)
-
+        # Canny edges for the object
         bw_canny = cannyG[rprops[i].coords[:, 0], rprops[i].coords[:, 1]]
         canny_sum = np.sum(bw_canny).astype('float')
 
-        fdata.at[i, 'Gradient.Canny.Sum'] = canny_sum
+        # Aggregate features
+        features = [
+            np.mean(pixelGradients),  # Mean
+            np.std(pixelGradients),  # Std
+            scipy.stats.skew(pixelGradients),  # Skewness
+            scipy.stats.kurtosis(pixelGradients),  # Kurtosis
+            scipy.stats.entropy(prob),  # HistEntropy
+            np.sum(prob**2),  # HistEnergy
+            canny_sum,  # Canny.Sum
+            canny_sum / len(pixelGradients),  # Canny.Mean
+        ]
+
+        data.append(features)
+
+    # Create DataFrame
+    feature_list = [
+        'Gradient.Mag.Mean',
+        'Gradient.Mag.Std',
+        'Gradient.Mag.Skewness',
+        'Gradient.Mag.Kurtosis',
+        'Gradient.Mag.HistEntropy',
+        'Gradient.Mag.HistEnergy',
+        'Gradient.Canny.Sum',
+        'Gradient.Canny.Mean',
+    ]
 
-        fdata.at[i, 'Gradient.Canny.Mean'] = canny_sum / len(pixelGradients)
+    fdata = pd.DataFrame(data, columns=feature_list)
 
     return fdata
```

### Comparing `histomicstk-1.3.8.dev1/histomicstk/features/compute_haralick_features.py` & `histomicstk-1.3.8.dev2/histomicstk/features/compute_haralick_features.py`

 * *Files 13% similar despite different names*

```diff
@@ -238,145 +238,159 @@
 
     # num_levels
     if num_levels is None:
         num_levels = _default_num_levels(im_intensity)
 
     # check for consistent shapes between 'I' and 'Label'
     if im_intensity.shape != im_label.shape:
-        msg = "Inputs 'I' and 'Label' must have same shape"
-        raise ValueError(msg)
+        err_str = 'Inputs I and Label must have same shape'
+        raise ValueError(err_str)
 
     num_dims = len(im_intensity.shape)
 
     # offsets
     if offsets is None:
-
         # set default offset value
         offsets = _default_offsets(im_intensity)
 
     else:
-
         # check sanity
         if offsets.shape[1] != num_dims:
-            msg = 'Dimension mismatch between input image and offsets'
-            raise ValueError(
-                msg,
-            )
+            err_str = 'Dimension mismatch between input image and offsets'
+            raise ValueError(err_str)
 
     num_offsets = offsets.shape[0]
 
     # compute object properties if not provided
     if rprops is None:
         rprops = regionprops(im_label)
 
     # create pandas data frame containing the features for each object
     numLabels = len(rprops)
-    fdata = pd.DataFrame(np.zeros((numLabels, len(agg_feature_list))),
-                         columns=agg_feature_list)
+    fdata = pd.DataFrame(
+        np.zeros((numLabels, len(agg_feature_list))), columns=agg_feature_list,
+    )
 
     n_Minus = np.arange(num_levels)
     n_Plus = np.arange(2 * num_levels - 1)
 
     x, y = np.mgrid[0:num_levels, 0:num_levels]
     xy = x * y
-    xy_IDM = 1. / (1 + np.square(x - y))
+    xy_IDM = 1.0 / (1 + np.square(x - y))
 
     e = 0.00001  # small positive constant to avoid log 0
-    eps = np.finfo(float).eps  # small constant to avoid div / 0
+
+    num_features = len(feature_list)
+
+    # Initialize the array for aggregated features
+    aggregated_features = np.zeros(
+        (numLabels, 2 * num_features),
+    )  # Alternating mean and range
 
     for i in range(numLabels):
         if rprops[i] is None:
             continue
 
         # get bounds of an intensity image
         minr, minc, maxr, maxc = rprops[i].bbox
 
         # grab nucleus mask
-        subImage = im_intensity[minr:maxr + 1, minc:maxc + 1]
+        subImage = im_intensity[minr: maxr + 1, minc: maxc + 1].astype(np.uint8)
 
         # gets GLCM or gray-tone spatial dependence matrix
-        arrayGLCM = graycomatrixext(subImage, offsets=offsets,
-                                    num_levels=num_levels,
-                                    gray_limits=gray_limits,
-                                    symmetric=True, normed=True)
-
-        # Compute haralick features for each offset
-        ldata = pd.DataFrame(np.zeros((num_offsets, len(feature_list))),
-                             columns=feature_list)
+        arrayGLCM = graycomatrixext(
+            subImage,
+            offsets=offsets,
+            num_levels=num_levels,
+            gray_limits=gray_limits,
+            symmetric=True,
+            normed=True,
+        )
 
-        for r in range(num_offsets):
+        features_per_offset = np.zeros((num_offsets, num_features))
 
+        for r in range(num_offsets):
             nGLCM = arrayGLCM[:, :, r]
 
             # get marginal-probabilities
-            px, py, pxPlusy, pxMinusy = _compute_marginal_glcm_probs_cython(
-                nGLCM)
+            px, py, pxPlusy, pxMinusy = _compute_marginal_glcm_probs_cython(nGLCM)
 
             # computes angular second moment
-            ldata.at[r, 'Haralick.ASM'] = np.sum(np.square(nGLCM))
+            ASM = np.sum(np.square(nGLCM))
 
             # computes contrast
-            ldata.at[r, 'Haralick.Contrast'] = \
-                np.dot(np.square(n_Minus), pxMinusy)
+            Contrast = np.dot(np.square(n_Minus), pxMinusy)
 
             # computes correlation
             # gets weighted mean and standard deviation of px and py
             meanx = np.dot(n_Minus, px)
             variance = np.dot(px, np.square(n_Minus)) - np.square(meanx)
             nGLCMr = np.ravel(nGLCM)
-
-            har_corr = (np.dot(np.ravel(xy), nGLCMr) - np.square(meanx)) /\
-                max(eps, variance)
-            ldata.at[r, 'Haralick.Correlation'] = np.clip(har_corr,
-                                                          a_min=-1, a_max=1)
+            Correlation = (np.dot(np.ravel(xy), nGLCMr) - np.square(meanx)) / variance
 
             # computes sum of squares : variance
-            ldata.at[r, 'Haralick.SumOfSquares'] = variance
+            SumOfSquares = variance
 
             # computes inverse difference moment
-            ldata.at[r, 'Haralick.IDM'] = \
-                np.dot(np.ravel(xy_IDM), nGLCMr)
+            IDM = np.dot(np.ravel(xy_IDM), nGLCMr)
 
             # computes sum average
-            ldata.at[r, 'Haralick.SumAverage'] = \
-                np.dot(n_Plus, pxPlusy)
+            SumAverage = np.dot(n_Plus, pxPlusy)
 
             # computes sum variance
             # [1] uses sum entropy, but we use sum average
-            ldata.at[r, 'Haralick.SumVariance'] = \
-                np.dot(np.square(n_Plus), pxPlusy) - \
-                np.square(ldata.at[r, 'Haralick.SumAverage'])
+            SumVariance = np.dot(np.square(n_Plus), pxPlusy) - np.square(SumAverage)
 
             # computes sum entropy
-            ldata.at[r, 'Haralick.SumEntropy'] = \
-                -np.dot(pxPlusy, np.log2(pxPlusy + e))
+            SumEntropy = -np.dot(pxPlusy, np.log2(pxPlusy + e))
 
             # computes entropy
-            ldata.at[r, 'Haralick.Entropy'] = \
-                -np.dot(nGLCMr, np.log2(nGLCMr + e))
+            Entropy = -np.dot(nGLCMr, np.log2(nGLCMr + e))
 
             # computes variance px-y
-            ldata.at[r, 'Haralick.DifferenceVariance'] = np.var(pxMinusy)
+            DifferenceVariance = np.var(pxMinusy)
 
             # computes difference entropy px-y
-            ldata.at[r, 'Haralick.DifferenceEntropy'] = \
-                -np.dot(pxMinusy, np.log2(pxMinusy + e))
+            DifferenceEntropy = -np.dot(pxMinusy, np.log2(pxMinusy + e))
 
             # computes information measures of correlation
             # gets entropies of px and py
             HX = -np.dot(px, np.log2(px + e))
             HY = -np.dot(py, np.log2(py + e))
-            HXY = ldata.at[r, 'Haralick.Entropy']
+            HXY = Entropy
             pxy_ij = np.outer(px, py)
             pxy_ijr = np.ravel(pxy_ij)
             HXY1 = -np.dot(nGLCMr, np.log2(pxy_ijr + e))
             HXY2 = -np.dot(pxy_ijr, np.log2(pxy_ijr + e))
-            ldata.at[r, 'Haralick.IMC1'] = ((HXY - HXY1) / max(HX, HY)) if max(HX, HY) else 0
+            IMC1 = (HXY - HXY1) / max(HX, HY)
 
             # computes information measures of correlation
-            ldata.at[r, 'Haralick.IMC2'] = \
-                np.sqrt(max(0, 1 - np.exp(-2.0 * (HXY2 - HXY))))
+            IMC2 = np.sqrt(1 - np.exp(-2.0 * (HXY2 - HXY)))
+
+            features_per_offset[r] = [
+                ASM,
+                Contrast,
+                Correlation,
+                SumOfSquares,
+                IDM,
+                SumAverage,
+                SumVariance,
+                SumEntropy,
+                Entropy,
+                DifferenceVariance,
+                DifferenceEntropy,
+                IMC1,
+                IMC2,
+            ]
+
+            # Calculate means and ranges across all features in a vectorized manner
+            means = np.mean(features_per_offset, axis=0)
+            ranges = np.ptp(features_per_offset, axis=0)
+
+            # Assign means and ranges to the aggregated_features array in alternating columns
+            aggregated_features[i, ::2] = means
+            aggregated_features[i, 1::2] = ranges
 
-        fdata.values[i, ::2] = np.mean(ldata.values, axis=0)
-        fdata.values[i, 1::2] = np.ptp(ldata.values, axis=0)
+    # Preparing DataFrame columns with alternating mean and range suffixes
+    fdata = pd.DataFrame(aggregated_features, columns=agg_feature_list)
 
     return fdata
```

### Comparing `histomicstk-1.3.8.dev1/histomicstk/features/compute_intensity_features.py` & `histomicstk-1.3.8.dev2/histomicstk/features/compute_intensity_features.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/features/compute_morphometry_features.py` & `histomicstk-1.3.8.dev2/histomicstk/features/compute_morphometry_features.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import warnings
-from collections import OrderedDict
 
 import numpy as np
 
 
 def compute_morphometry_features(im_label, rprops=None):
     """
     Calculate morphometry features for each object
@@ -98,70 +97,76 @@
     from skimage.measure import regionprops
 
     # compute object properties if not provided
     if rprops is None:
         rprops = regionprops(im_label)
     intensity_wtd = rprops[0]._intensity_image is not None
 
-    # List of feature names
-    featname_map = OrderedDict({
-        'Orientation.Orientation': 'orientation',
-        'Size.Area': 'area',
-        'Size.ConvexHullArea': 'convex_area',
-        'Size.MajorAxisLength': 'major_axis_length',
-        'Size.MinorAxisLength': 'minor_axis_length',
-        'Size.Perimeter': 'perimeter',
-        'Shape.Circularity': None,
-        'Shape.Eccentricity': 'eccentricity',
-        'Shape.EquivalentDiameter': 'equivalent_diameter',
-        'Shape.Extent': 'extent',
-        'Shape.FractalDimension': None,
-        'Shape.MinorMajorAxisRatio': None,
-        'Shape.Solidity': 'solidity',
-    })
-    hu_cols = ['Shape.HuMoments%d' % k for k in range(1, 8)]
-    featname_map.update({col: None for col in hu_cols})
+    # Define the feature list as tuples of (feature name, attribute or function)
+    feature_list = [
+        ('Orientation.Orientation', 'orientation'),
+        ('Size.Area', 'area'),
+        ('Size.ConvexHullArea', 'convex_area'),
+        ('Size.MajorAxisLength', 'major_axis_length'),
+        ('Size.MinorAxisLength', 'minor_axis_length'),
+        ('Size.Perimeter', 'perimeter'),
+        (
+            'Shape.Circularity',
+            lambda rp: 4
+            * np.pi
+            * rp.area
+            / (rp.perimeter**2 if rp.perimeter > 0 else 1),
+        ),
+        ('Shape.Eccentricity', 'eccentricity'),
+        ('Shape.EquivalentDiameter', 'equivalent_diameter'),
+        ('Shape.Extent', 'extent'),
+        ('Shape.FractalDimension', lambda rp: _fractal_dimension(rp.image)),
+        (
+            'Shape.MinorMajorAxisRatio',
+            lambda rp: rp.minor_axis_length / rp.major_axis_length
+            if rp.major_axis_length > 0
+            else 1,
+        ),
+        ('Shape.Solidity', 'solidity'),
+    ]
+
+    # Add Hu moments features
+    hu_moments = [
+        ('Shape.HuMoments' + str(k), lambda rp, k=k: rp.moments_hu[k - 1])
+        for k in range(1, 8)
+    ]
+    feature_list.extend(hu_moments)
     if intensity_wtd:
-        wtd_hu_cols = [col.replace('.Hu', '.WeightedHu') for col in hu_cols]
-        featname_map.update({col: None for col in wtd_hu_cols})
-    feature_list = featname_map.keys()
-    mapped_feats = [k for k, v in featname_map.items() if v is not None]
-
-    # create pandas data frame containing the features for each object
-    numFeatures = len(feature_list)
-    numLabels = len(rprops)
-    fdata = pd.DataFrame(np.zeros((numLabels, numFeatures)),
-                         columns=feature_list)
-
-    for i, nprop in enumerate(rprops):
-
-        # assign some features from sklearn as-is
-        for name in mapped_feats:
-            fdata.at[i, name] = nprop[featname_map[name]]
-
-        # compute Circularity
-        numerator = 4 * np.pi * nprop.area
-        denominator = nprop.perimeter ** 2
-        if denominator > 0:
-            fdata.at[i, 'Shape.Circularity'] = numerator / denominator
-
-        # compute fractal dimension (boundary complexity)
-        fdata.at[i, 'Shape.FractalDimension'] = _fractal_dimension(nprop.image)
-
-        # compute Minor to Major axis ratio
-        if nprop.major_axis_length > 0:
-            fdata.at[i, 'Shape.MinorMajorAxisRatio'] = \
-                nprop.minor_axis_length / nprop.major_axis_length
-        else:
-            fdata.at[i, 'Shape.MinorMajorAxisRatio'] = 1
-
-        # Hu moments, raw and possibly also intensity-weighted
-        fdata.loc[i, hu_cols] = nprop.moments_hu
-        if intensity_wtd:
-            fdata.loc[i, wtd_hu_cols] = nprop.weighted_moments_hu
+        wtd_hu_moments = [
+            (
+                'Shape.WeightedHuMoments' + str(k),
+                lambda rp, k=k: rp.weighted_moments_hu[k - 1],
+            )
+            for k in range(1, 8)
+        ]
+        feature_list.extend(wtd_hu_moments)
+
+    data = []
+
+    for prop in rprops:
+        row = []
+        for name, attr in feature_list:
+            if callable(attr):
+                value = attr(prop)
+            else:
+                value = getattr(prop, attr, np.nan)
+
+            # Check if the feature is Area or ConvexHullArea and ensure it is a float
+            if name in ('Size.Area', 'Size.ConvexHullArea'):
+                value = float(value)  # Cast to float here
+
+            row.append(value)
+        data.append(row)
+
+    fdata = pd.DataFrame(data, columns=[name for name, _ in feature_list])
 
     return fdata
 
 
 def _fractal_dimension(Z):
     """
     Calculate the fractal dimension of an object (boundary complexity).
```

### Comparing `histomicstk-1.3.8.dev1/histomicstk/features/compute_nuclei_features.py` & `histomicstk-1.3.8.dev2/histomicstk/features/compute_nuclei_features.py`

 * *Files 14% similar despite different names*

```diff
@@ -167,125 +167,121 @@
     #  improving efficiency in the future somehow (cython? reuse? etc)
 
     feature_list = []
 
     # get the objects in im_label
     nuclei_props = regionprops(im_label, intensity_image=im_nuclei)
 
-    # extract object locations and identifiers
-    idata = pd.DataFrame()
-    for i, nprop in enumerate(nuclei_props):
-        idata.at[i, 'Label'] = nprop.label
-        idata.at[i, 'Identifier.Xmin'] = nprop.bbox[1]
-        idata.at[i, 'Identifier.Ymin'] = nprop.bbox[0]
-        idata.at[i, 'Identifier.Xmax'] = nprop.bbox[3]
-        idata.at[i, 'Identifier.Ymax'] = nprop.bbox[2]
-        idata.at[i, 'Identifier.CentroidX'] = nprop.centroid[1]
-        idata.at[i, 'Identifier.CentroidY'] = nprop.centroid[0]
-        if im_nuclei is not None:
-            # intensity-weighted centroid
-            wcy, wcx = nprop.weighted_centroid
-            idata.at[i, 'Identifier.WeightedCentroidX'] = wcx
-            idata.at[i, 'Identifier.WeightedCentroidY'] = wcy
+    im_nuclei_bool = im_nuclei is not None
+
+    data = []
+
+    def process_nucleus(nprop, im_nuclei_bool):
+        for nprop in nuclei_props:
+            row = {
+                'Label': nprop.label,
+                'Identifier.Xmin': nprop.bbox[1],
+                'Identifier.Ymin': nprop.bbox[0],
+                'Identifier.Xmax': nprop.bbox[3],
+                'Identifier.Ymax': nprop.bbox[2],
+                'Identifier.Centroid': nprop.centroid[1],
+                'Identifier.CentroidY': nprop.centroid[0],
+            }
+            if im_nuclei_bool:
+                wcy, wcx = nprop.weighted_centroid
+                row['Identifier.WeightedCentroidX'] = wcx
+                row['Identifier.WeightedCentroidY'] = wcy
+            data.append(row)
+        return pd.DataFrame(data)
+
+    # create the DataFrame in one step
+    idata = process_nucleus(nuclei_props, im_nuclei_bool)
     feature_list.append(idata)
 
+    def conditional(flag, func, args, kwargs, prefix=None):
+        if flag:
+            output = func(*args, **kwargs)
+            if prefix:
+                output.columns = [prefix + col for col in output.columns]
+            return output
+        else:
+            return pd.DataFrame()  # return an empty DataFrame if condition is not met
+
     # compute cytoplasm mask
     if im_cytoplasm is not None:
 
         cyto_mask = htk_label.dilate_xor(im_label, neigh_width=cyto_width)
 
         cyto_props = regionprops(cyto_mask, intensity_image=im_cytoplasm)
 
         # ensure that cytoplasm props order corresponds to the nuclei
         lablocs = {v['label']: i for i, v in enumerate(cyto_props)}
         cyto_props = [cyto_props[lablocs[v['label']]] if v['label'] in lablocs else None
                       for v in nuclei_props]
 
     # compute morphometry features
-    if morphometry_features_flag:
-
-        fmorph = compute_morphometry_features(im_label, rprops=nuclei_props)
-
-        feature_list.append(fmorph)
+    feature_list.append(conditional(
+        morphometry_features_flag,
+        compute_morphometry_features,
+        [im_label], {'rprops': nuclei_props},
+    ))
 
     # compute FSD features
-    if fsd_features_flag:
-
-        ffsd = compute_fsd_features(im_label, fsd_bnd_pts, fsd_freq_bins,
-                                    cyto_width, rprops=nuclei_props)
-
-        feature_list.append(ffsd)
+    feature_list.append(conditional(
+        fsd_features_flag,
+        compute_fsd_features,
+        [im_label, fsd_bnd_pts, fsd_freq_bins, cyto_width], {'rprops': nuclei_props},
+    ))
 
     # compute nuclei intensity features
-    if intensity_features_flag:
-
-        fint_nuclei = compute_intensity_features(im_label, im_nuclei,
-                                                 rprops=nuclei_props)
-        fint_nuclei.columns = ['Nucleus.' + col
-                               for col in fint_nuclei.columns]
-
-        feature_list.append(fint_nuclei)
+    feature_list.append(conditional(
+        intensity_features_flag,
+        compute_intensity_features,
+        [im_label, im_nuclei], {'rprops': nuclei_props}, prefix='Nucleus.',
+    ))
 
     # compute cytoplasm intensity features
-    if intensity_features_flag and im_cytoplasm is not None:
-
-        fint_cytoplasm = compute_intensity_features(cyto_mask, im_cytoplasm,
-                                                    rprops=cyto_props)
-        fint_cytoplasm.columns = ['Cytoplasm.' + col
-                                  for col in fint_cytoplasm.columns]
-
-        feature_list.append(fint_cytoplasm)
+    if im_cytoplasm is not None:
+        feature_list.append(conditional(
+            intensity_features_flag,
+            compute_intensity_features,
+            [cyto_mask, im_cytoplasm], {'rprops': cyto_props}, prefix='Cytoplasm.',
+        ))
 
     # compute nuclei gradient features
-    if gradient_features_flag:
-
-        fgrad_nuclei = compute_gradient_features(im_label, im_nuclei,
-                                                 rprops=nuclei_props)
-        fgrad_nuclei.columns = ['Nucleus.' + col
-                                for col in fgrad_nuclei.columns]
-
-        feature_list.append(fgrad_nuclei)
+    feature_list.append(conditional(
+        gradient_features_flag,
+        compute_gradient_features,
+        [im_label, im_nuclei], {'rprops': nuclei_props}, prefix='Nucleus.',
+    ))
 
     # compute cytoplasm gradient features
-    if gradient_features_flag and im_cytoplasm is not None:
-
-        fgrad_cytoplasm = compute_gradient_features(cyto_mask, im_cytoplasm,
-                                                    rprops=cyto_props)
-        fgrad_cytoplasm.columns = ['Cytoplasm.' + col
-                                   for col in fgrad_cytoplasm.columns]
-
-        feature_list.append(fgrad_cytoplasm)
+    if im_cytoplasm is not None:
+        feature_list.append(conditional(
+            gradient_features_flag,
+            compute_gradient_features,
+            [cyto_mask, im_cytoplasm], {'rprops': cyto_props}, prefix='Cytoplasm.',
+        ))
 
     # compute nuclei haralick features
-    if haralick_features_flag:
-
-        fharalick_nuclei = compute_haralick_features(
-            im_label, im_nuclei,
-            num_levels=num_glcm_levels,
-            rprops=nuclei_props,
-        )
-
-        fharalick_nuclei.columns = ['Nucleus.' + col
-                                    for col in fharalick_nuclei.columns]
-
-        feature_list.append(fharalick_nuclei)
+    feature_list.append(conditional(
+        haralick_features_flag,
+        compute_haralick_features,
+        [im_label, im_nuclei], {'num_levels': num_glcm_levels, 'rprops': nuclei_props},
+        prefix='Nucleus.',
+    ))
 
     # compute cytoplasm haralick features
-    if haralick_features_flag and im_cytoplasm is not None:
-
-        fharalick_cytoplasm = compute_haralick_features(
-            cyto_mask, im_cytoplasm,
-            num_levels=num_glcm_levels,
-            rprops=cyto_props,
-        )
-
-        fharalick_cytoplasm.columns = ['Cytoplasm.' + col
-                                       for col in fharalick_cytoplasm.columns]
-
-        feature_list.append(fharalick_cytoplasm)
+    if im_cytoplasm is not None:
+        feature_list.append(conditional(
+            haralick_features_flag,
+            compute_haralick_features,
+            [cyto_mask, im_cytoplasm], {'num_levels': num_glcm_levels, 'rprops': cyto_props},
+            prefix='Cytoplasm.',
+        ))
 
     # Merge all features
     fdata = pd.concat(feature_list, axis=1)
 
     if return_nuclei_annotation:
         # Create nuclei segmentation with the generated regionprops
         nuclei_annot_list, selected_rows = cli_utils.create_tile_nuclei_annotations(
```

### Comparing `histomicstk-1.3.8.dev1/histomicstk/features/graycomatrixext.py` & `histomicstk-1.3.8.dev2/histomicstk/features/graycomatrixext.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/filters/edge/gaussian_grad.py` & `histomicstk-1.3.8.dev2/histomicstk/filters/edge/gaussian_grad.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/filters/shape/cdog.py` & `histomicstk-1.3.8.dev2/histomicstk/filters/shape/cdog.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/filters/shape/clog.py` & `histomicstk-1.3.8.dev2/histomicstk/filters/shape/clog.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/filters/shape/glog.py` & `histomicstk-1.3.8.dev2/histomicstk/filters/shape/glog.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/filters/shape/vesselness.py` & `histomicstk-1.3.8.dev2/histomicstk/filters/shape/vesselness.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/preprocessing/augmentation/__init__.py` & `histomicstk-1.3.8.dev2/histomicstk/preprocessing/augmentation/__init__.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/preprocessing/augmentation/color_augmentation.py` & `histomicstk-1.3.8.dev2/histomicstk/preprocessing/augmentation/color_augmentation.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/preprocessing/color_conversion/__init__.py` & `histomicstk-1.3.8.dev2/histomicstk/preprocessing/color_conversion/__init__.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/preprocessing/color_conversion/lab_mean_std.py` & `histomicstk-1.3.8.dev2/histomicstk/preprocessing/color_conversion/lab_mean_std.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/preprocessing/color_conversion/lab_to_rgb.py` & `histomicstk-1.3.8.dev2/histomicstk/preprocessing/color_conversion/lab_to_rgb.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/preprocessing/color_conversion/od_to_rgb.py` & `histomicstk-1.3.8.dev2/histomicstk/preprocessing/color_conversion/od_to_rgb.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/preprocessing/color_conversion/rgb_to_hsi.py` & `histomicstk-1.3.8.dev2/histomicstk/preprocessing/color_conversion/rgb_to_hsi.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/preprocessing/color_conversion/rgb_to_lab.py` & `histomicstk-1.3.8.dev2/histomicstk/preprocessing/color_conversion/rgb_to_lab.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/preprocessing/color_conversion/rgb_to_od.py` & `histomicstk-1.3.8.dev2/histomicstk/preprocessing/color_conversion/rgb_to_od.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/preprocessing/color_conversion/rgb_to_sda.py` & `histomicstk-1.3.8.dev2/histomicstk/preprocessing/color_conversion/rgb_to_sda.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/preprocessing/color_conversion/sda_to_rgb.py` & `histomicstk-1.3.8.dev2/histomicstk/preprocessing/color_conversion/sda_to_rgb.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/preprocessing/color_deconvolution/__init__.py` & `histomicstk-1.3.8.dev2/histomicstk/preprocessing/color_deconvolution/__init__.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/preprocessing/color_deconvolution/color_convolution.py` & `histomicstk-1.3.8.dev2/histomicstk/preprocessing/color_deconvolution/color_convolution.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/preprocessing/color_deconvolution/color_deconvolution.py` & `histomicstk-1.3.8.dev2/histomicstk/preprocessing/color_deconvolution/color_deconvolution.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/preprocessing/color_deconvolution/complement_stain_matrix.py` & `histomicstk-1.3.8.dev2/histomicstk/preprocessing/color_deconvolution/complement_stain_matrix.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/preprocessing/color_deconvolution/find_stain_index.py` & `histomicstk-1.3.8.dev2/histomicstk/preprocessing/color_deconvolution/find_stain_index.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/preprocessing/color_deconvolution/rgb_separate_stains_macenko_pca.py` & `histomicstk-1.3.8.dev2/histomicstk/preprocessing/color_deconvolution/rgb_separate_stains_macenko_pca.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/preprocessing/color_deconvolution/rgb_separate_stains_xu_snmf.py` & `histomicstk-1.3.8.dev2/histomicstk/preprocessing/color_deconvolution/rgb_separate_stains_xu_snmf.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/preprocessing/color_deconvolution/separate_stains_macenko_pca.py` & `histomicstk-1.3.8.dev2/histomicstk/preprocessing/color_deconvolution/separate_stains_macenko_pca.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/preprocessing/color_deconvolution/separate_stains_xu_snmf.py` & `histomicstk-1.3.8.dev2/histomicstk/preprocessing/color_deconvolution/separate_stains_xu_snmf.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/preprocessing/color_normalization/__init__.py` & `histomicstk-1.3.8.dev2/histomicstk/preprocessing/color_normalization/__init__.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/preprocessing/color_normalization/background_intensity.py` & `histomicstk-1.3.8.dev2/histomicstk/preprocessing/color_normalization/background_intensity.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/preprocessing/color_normalization/deconvolution_based_normalization.py` & `histomicstk-1.3.8.dev2/histomicstk/preprocessing/color_normalization/deconvolution_based_normalization.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/preprocessing/color_normalization/reinhard.py` & `histomicstk-1.3.8.dev2/histomicstk/preprocessing/color_normalization/reinhard.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/preprocessing/color_normalization/reinhard_stats.py` & `histomicstk-1.3.8.dev2/histomicstk/preprocessing/color_normalization/reinhard_stats.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/preprocessing/tests/test_normalization_and_augmentation.py` & `histomicstk-1.3.8.dev2/histomicstk/preprocessing/tests/test_normalization_and_augmentation.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/saliency/cellularity_detection_superpixels.py` & `histomicstk-1.3.8.dev2/histomicstk/saliency/cellularity_detection_superpixels.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/saliency/cellularity_detection_thresholding.py` & `histomicstk-1.3.8.dev2/histomicstk/saliency/cellularity_detection_thresholding.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/saliency/tests/test_saliency.py` & `histomicstk-1.3.8.dev2/histomicstk/saliency/tests/test_saliency.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/saliency/tissue_detection.py` & `histomicstk-1.3.8.dev2/histomicstk/saliency/tissue_detection.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/segmentation/__init__.py` & `histomicstk-1.3.8.dev2/histomicstk/segmentation/__init__.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/segmentation/embed_boundaries.py` & `histomicstk-1.3.8.dev2/histomicstk/segmentation/embed_boundaries.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/segmentation/label/__init__.py` & `histomicstk-1.3.8.dev2/histomicstk/segmentation/label/__init__.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/segmentation/label/_trace_object_boundaries_cython.pyx` & `histomicstk-1.3.8.dev2/histomicstk/segmentation/label/_trace_object_boundaries_cython.pyx`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/segmentation/label/area_open.py` & `histomicstk-1.3.8.dev2/histomicstk/segmentation/label/area_open.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/segmentation/label/compact.py` & `histomicstk-1.3.8.dev2/histomicstk/segmentation/label/compact.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/segmentation/label/condense.py` & `histomicstk-1.3.8.dev2/histomicstk/segmentation/label/condense.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/segmentation/label/delete.py` & `histomicstk-1.3.8.dev2/histomicstk/segmentation/label/delete.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/segmentation/label/delete_border.py` & `histomicstk-1.3.8.dev2/histomicstk/segmentation/label/delete_border.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/segmentation/label/delete_overlap.py` & `histomicstk-1.3.8.dev2/histomicstk/segmentation/label/delete_overlap.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/segmentation/label/dilate_xor.py` & `histomicstk-1.3.8.dev2/histomicstk/segmentation/label/dilate_xor.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/segmentation/label/perimeter.py` & `histomicstk-1.3.8.dev2/histomicstk/segmentation/label/perimeter.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/segmentation/label/remove_overlap_nuclei.py` & `histomicstk-1.3.8.dev2/histomicstk/segmentation/label/remove_overlap_nuclei.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/segmentation/label/shuffle.py` & `histomicstk-1.3.8.dev2/histomicstk/segmentation/label/shuffle.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/segmentation/label/split.py` & `histomicstk-1.3.8.dev2/histomicstk/segmentation/label/split.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/segmentation/label/trace_object_boundaries.py` & `histomicstk-1.3.8.dev2/histomicstk/segmentation/label/trace_object_boundaries.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/segmentation/label/width_open.py` & `histomicstk-1.3.8.dev2/histomicstk/segmentation/label/width_open.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/segmentation/level_set/chan_vese.py` & `histomicstk-1.3.8.dev2/histomicstk/segmentation/level_set/chan_vese.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/segmentation/level_set/reg_edge.py` & `histomicstk-1.3.8.dev2/histomicstk/segmentation/level_set/reg_edge.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/segmentation/nuclear/__init__.py` & `histomicstk-1.3.8.dev2/histomicstk/segmentation/nuclear/__init__.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/segmentation/nuclear/_max_clustering_cython.pyx` & `histomicstk-1.3.8.dev2/histomicstk/segmentation/nuclear/_max_clustering_cython.pyx`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/segmentation/nuclear/detect_nuclei_kofahi.py` & `histomicstk-1.3.8.dev2/histomicstk/segmentation/nuclear/detect_nuclei_kofahi.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/segmentation/nuclear/detect_tile_nuclei.py` & `histomicstk-1.3.8.dev2/histomicstk/segmentation/nuclear/detect_tile_nuclei.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/segmentation/nuclear/gaussian_voting.py` & `histomicstk-1.3.8.dev2/histomicstk/segmentation/nuclear/gaussian_voting.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/segmentation/nuclear/gvf_tracking.py` & `histomicstk-1.3.8.dev2/histomicstk/segmentation/nuclear/gvf_tracking.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/segmentation/nuclear/max_clustering.py` & `histomicstk-1.3.8.dev2/histomicstk/segmentation/nuclear/max_clustering.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/segmentation/nuclear/min_model.py` & `histomicstk-1.3.8.dev2/histomicstk/segmentation/nuclear/min_model.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/segmentation/positive_pixel_count.py` & `histomicstk-1.3.8.dev2/histomicstk/segmentation/positive_pixel_count.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/segmentation/rag.py` & `histomicstk-1.3.8.dev2/histomicstk/segmentation/rag.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/segmentation/rag_add_layer.py` & `histomicstk-1.3.8.dev2/histomicstk/segmentation/rag_add_layer.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/segmentation/rag_color.py` & `histomicstk-1.3.8.dev2/histomicstk/segmentation/rag_color.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/utils/__init__.py` & `histomicstk-1.3.8.dev2/histomicstk/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/utils/compute_tile_foreground_fraction.py` & `histomicstk-1.3.8.dev2/histomicstk/utils/compute_tile_foreground_fraction.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/utils/del2.py` & `histomicstk-1.3.8.dev2/histomicstk/utils/del2.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/utils/eigen.py` & `histomicstk-1.3.8.dev2/histomicstk/utils/eigen.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/utils/fit_poisson_mixture.py` & `histomicstk-1.3.8.dev2/histomicstk/utils/fit_poisson_mixture.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/utils/general_utils.py` & `histomicstk-1.3.8.dev2/histomicstk/utils/general_utils.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/utils/girder_convenience_utils.py` & `histomicstk-1.3.8.dev2/histomicstk/utils/girder_convenience_utils.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/utils/gradient_diffusion.py` & `histomicstk-1.3.8.dev2/histomicstk/utils/gradient_diffusion.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/utils/hessian.py` & `histomicstk-1.3.8.dev2/histomicstk/utils/hessian.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/utils/merge_colinear.py` & `histomicstk-1.3.8.dev2/histomicstk/utils/merge_colinear.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/utils/sample_pixels.py` & `histomicstk-1.3.8.dev2/histomicstk/utils/sample_pixels.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/utils/simple_mask.py` & `histomicstk-1.3.8.dev2/histomicstk/utils/simple_mask.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/utils/tests/test_girder_convenience_utils.py` & `histomicstk-1.3.8.dev2/histomicstk/utils/tests/test_girder_convenience_utils.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/workflows/specific_workflows.py` & `histomicstk-1.3.8.dev2/histomicstk/workflows/specific_workflows.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/workflows/tests/test_workflow_runner.py` & `histomicstk-1.3.8.dev2/histomicstk/workflows/tests/test_workflow_runner.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk/workflows/workflow_runner.py` & `histomicstk-1.3.8.dev2/histomicstk/workflows/workflow_runner.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/histomicstk.egg-info/SOURCES.txt` & `histomicstk-1.3.8.dev2/histomicstk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.8.dev1/setup.py` & `histomicstk-1.3.8.dev2/setup.py`

 * *Files identical despite different names*

