# Comparing `tmp/nerfstudio-1.0.3.tar.gz` & `tmp/nerfstudio-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nerfstudio-1.0.3.tar", last modified: Wed Apr  3 01:25:34 2024, max compression
+gzip compressed data, was "nerfstudio-1.1.0.tar", last modified: Mon May 13 19:06:44 2024, max compression
```

## Comparing `nerfstudio-1.0.3.tar` & `nerfstudio-1.1.0.tar`

### file list

```diff
@@ -1,258 +1,258 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.643997 nerfstudio-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    23709 2024-04-03 01:25:34.643997 nerfstudio-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20055 2024-04-03 01:25:32.000000 nerfstudio-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.599997 nerfstudio-1.0.3/nerfstudio/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.603997 nerfstudio-1.0.3/nerfstudio/cameras/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/cameras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8116 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/cameras/camera_optimizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6558 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/cameras/camera_paths.py
--rw-r--r--   0 runner    (1001) docker     (127)    33058 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/cameras/camera_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    50983 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/cameras/cameras.py
--rw-r--r--   0 runner    (1001) docker     (127)     4790 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/cameras/lie_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    11014 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/cameras/rays.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.603997 nerfstudio-1.0.3/nerfstudio/configs/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6001 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/configs/base_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/configs/config_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/configs/dataparser_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5781 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/configs/experiment_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    10012 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/configs/external_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)    27707 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/configs/method_configs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.603997 nerfstudio-1.0.3/nerfstudio/data/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.607997 nerfstudio-1.0.3/nerfstudio/data/datamanagers/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/data/datamanagers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25171 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/data/datamanagers/base_datamanager.py
--rw-r--r--   0 runner    (1001) docker     (127)    22509 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/data/datamanagers/full_images_datamanager.py
--rw-r--r--   0 runner    (1001) docker     (127)    15085 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/data/datamanagers/parallel_datamanager.py
--rw-r--r--   0 runner    (1001) docker     (127)    11917 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/data/datamanagers/random_cameras_datamanager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.607997 nerfstudio-1.0.3/nerfstudio/data/dataparsers/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/data/dataparsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9186 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/data/dataparsers/arkitscenes_dataparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     7549 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/data/dataparsers/base_dataparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/data/dataparsers/blender_dataparser.py
--rw-r--r--   0 runner    (1001) docker     (127)    26907 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/data/dataparsers/colmap_dataparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/data/dataparsers/dnerf_dataparser.py
--rw-r--r--   0 runner    (1001) docker     (127)    13725 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/data/dataparsers/dycheck_dataparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     9155 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/data/dataparsers/instant_ngp_dataparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     4270 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/data/dataparsers/minimal_dataparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     8502 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/data/dataparsers/nerfosr_dataparser.py
--rw-r--r--   0 runner    (1001) docker     (127)    21922 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/data/dataparsers/nerfstudio_dataparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     8759 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/data/dataparsers/nuscenes_dataparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     6957 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/data/dataparsers/phototourism_dataparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     6832 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/data/dataparsers/scannet_dataparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     8128 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/data/dataparsers/scannetpp_dataparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     5943 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/data/dataparsers/sdfstudio_dataparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     5963 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/data/dataparsers/sitcoms3d_dataparser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.611997 nerfstudio-1.0.3/nerfstudio/data/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/data/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6822 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/data/datasets/base_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     6002 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/data/datasets/depth_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3877 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/data/datasets/sdf_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/data/datasets/semantic_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    23230 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/data/pixel_samplers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4310 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/data/scene_box.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.611997 nerfstudio-1.0.3/nerfstudio/data/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/data/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20474 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/data/utils/colmap_parsing_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/data/utils/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9324 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/data/utils/dataloaders.py
--rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/data/utils/dataparsers_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9818 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/data/utils/nerfstudio_collate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/data/utils/pixel_sampling_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.611997 nerfstudio-1.0.3/nerfstudio/engine/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/engine/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)     8416 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/engine/optimizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6170 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/engine/schedulers.py
--rw-r--r--   0 runner    (1001) docker     (127)    24265 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/engine/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.611997 nerfstudio-1.0.3/nerfstudio/exporter/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/exporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14319 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/exporter/exporter_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10659 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/exporter/marching_cubes.py
--rw-r--r--   0 runner    (1001) docker     (127)    21099 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/exporter/texture_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14230 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/exporter/tsdf_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.615997 nerfstudio-1.0.3/nerfstudio/field_components/
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/field_components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/field_components/activations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/field_components/base_field_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/field_components/embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)    32841 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/field_components/encodings.py
--rw-r--r--   0 runner    (1001) docker     (127)     6973 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/field_components/field_heads.py
--rw-r--r--   0 runner    (1001) docker     (127)    11936 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/field_components/mlp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/field_components/spatial_distortions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/field_components/temporal_distortions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.615997 nerfstudio-1.0.3/nerfstudio/fields/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/fields/base_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     4761 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/fields/density_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     5888 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/fields/generfacto_field.py
--rw-r--r--   0 runner    (1001) docker     (127)    13375 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/fields/nerfacto_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     7046 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/fields/nerfw_field.py
--rw-r--r--   0 runner    (1001) docker     (127)    18116 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/fields/sdf_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     4291 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/fields/semantic_nerf_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/fields/tensorf_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     4789 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/fields/vanilla_nerf_field.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.615997 nerfstudio-1.0.3/nerfstudio/generative/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/generative/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9054 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/generative/deepfloyd.py
--rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/generative/positional_text_embeddings.py
--rw-r--r--   0 runner    (1001) docker     (127)    11987 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/generative/stable_diffusion.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.619997 nerfstudio-1.0.3/nerfstudio/model_components/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/model_components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22329 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/model_components/losses.py
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/model_components/ray_generators.py
--rw-r--r--   0 runner    (1001) docker     (127)    29334 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/model_components/ray_samplers.py
--rw-r--r--   0 runner    (1001) docker     (127)    16812 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/model_components/renderers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7079 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/model_components/scene_colliders.py
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/model_components/shaders.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.619997 nerfstudio-1.0.3/nerfstudio/models/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10388 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/models/base_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    17095 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/models/base_surface_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/models/depth_nerfacto.py
--rw-r--r--   0 runner    (1001) docker     (127)    22094 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/models/generfacto.py
--rw-r--r--   0 runner    (1001) docker     (127)    10542 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/models/instant_ngp.py
--rw-r--r--   0 runner    (1001) docker     (127)     9228 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/models/mipnerf.py
--rw-r--r--   0 runner    (1001) docker     (127)    19375 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/models/nerfacto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4144 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/models/neus.py
--rw-r--r--   0 runner    (1001) docker     (127)     9481 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/models/neus_facto.py
--rw-r--r--   0 runner    (1001) docker     (127)    13779 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/models/semantic_nerfw.py
--rw-r--r--   0 runner    (1001) docker     (127)    39464 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/models/splatfacto.py
--rw-r--r--   0 runner    (1001) docker     (127)    15809 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/models/tensorf.py
--rw-r--r--   0 runner    (1001) docker     (127)    11325 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/models/vanilla_nerf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.619997 nerfstudio-1.0.3/nerfstudio/pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18055 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/pipelines/base_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/pipelines/dynamic_batch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.623997 nerfstudio-1.0.3/nerfstudio/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/plugins/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/plugins/registry_dataparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/plugins/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.623997 nerfstudio-1.0.3/nerfstudio/process_data/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/process_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/process_data/base_converter_to_nerfstudio_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    10235 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/process_data/colmap_converter_to_nerfstudio_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    27598 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/process_data/colmap_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12843 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/process_data/equirect_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/process_data/hloc_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5799 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/process_data/images_to_nerfstudio_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     7871 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/process_data/metashape_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6969 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/process_data/odm_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8989 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/process_data/polycam_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    25630 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/process_data/process_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4841 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/process_data/realitycapture_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/process_data/record3d_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6097 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/process_data/video_to_nerfstudio_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.623997 nerfstudio-1.0.3/nerfstudio/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/scripts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.623997 nerfstudio-1.0.3/nerfstudio/scripts/blender/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/scripts/blender/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17246 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/scripts/blender/nerfstudio_blender.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.627997 nerfstudio-1.0.3/nerfstudio/scripts/completions/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/scripts/completions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15529 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/scripts/completions/install.py
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/scripts/completions/setup.bash
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/scripts/completions/setup.zsh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.627997 nerfstudio-1.0.3/nerfstudio/scripts/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)     6544 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/scripts/datasets/process_nuscenes_masks.py
--rw-r--r--   0 runner    (1001) docker     (127)     9284 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/scripts/datasets/process_project_aria.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.627997 nerfstudio-1.0.3/nerfstudio/scripts/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/scripts/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/scripts/docs/add_nb_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/scripts/docs/build_docs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.627997 nerfstudio-1.0.3/nerfstudio/scripts/downloads/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/scripts/downloads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24960 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/scripts/downloads/download_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    18554 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/scripts/downloads/eyeful_tower.py
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/scripts/downloads/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/scripts/eval.py
--rw-r--r--   0 runner    (1001) docker     (127)    26818 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/scripts/exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.627997 nerfstudio-1.0.3/nerfstudio/scripts/github/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/scripts/github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4401 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/scripts/github/run_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)    21495 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/scripts/process_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    41704 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/scripts/render.py
--rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/scripts/texture.py
--rw-r--r--   0 runner    (1001) docker     (127)     9807 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/scripts/train.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.627997 nerfstudio-1.0.3/nerfstudio/scripts/viewer/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/scripts/viewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/scripts/viewer/run_viewer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/scripts/viewer/sync_viser_message_defs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.631997 nerfstudio-1.0.3/nerfstudio/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/utils/colormaps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/utils/comms.py
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     4618 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/utils/eval_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/utils/external.py
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/utils/install_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (127)    18643 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/utils/math.py
--rw-r--r--   0 runner    (1001) docker     (127)     7365 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)    16909 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/utils/plotly_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/utils/poses.py
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/utils/printing.py
--rw-r--r--   0 runner    (1001) docker     (127)     7950 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/utils/profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/utils/rich_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/utils/scripts.py
--rw-r--r--   0 runner    (1001) docker     (127)    13665 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/utils/tensor_dataclass.py
--rw-r--r--   0 runner    (1001) docker     (127)    18988 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/utils/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.631997 nerfstudio-1.0.3/nerfstudio/viewer/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/viewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16956 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/viewer/control_panel.py
--rw-r--r--   0 runner    (1001) docker     (127)     8536 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/viewer/export_panel.py
--rw-r--r--   0 runner    (1001) docker     (127)    46800 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/viewer/render_panel.py
--rw-r--r--   0 runner    (1001) docker     (127)    16129 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/viewer/render_state_machine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.631997 nerfstudio-1.0.3/nerfstudio/viewer/server/
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/viewer/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/viewer/server/viewer_elements.py
--rw-r--r--   0 runner    (1001) docker     (127)     5320 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/viewer/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    24095 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/viewer/viewer.py
--rw-r--r--   0 runner    (1001) docker     (127)    24037 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/viewer/viewer_elements.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.631997 nerfstudio-1.0.3/nerfstudio/viewer_legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/viewer_legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.635997 nerfstudio-1.0.3/nerfstudio/viewer_legacy/app/
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/viewer_legacy/app/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.635997 nerfstudio-1.0.3/nerfstudio/viewer_legacy/app/public/
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/viewer_legacy/app/public/manifest.json
--rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/viewer_legacy/app/run_deploy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.599997 nerfstudio-1.0.3/nerfstudio/viewer_legacy/app/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.635997 nerfstudio-1.0.3/nerfstudio/viewer_legacy/app/src/themes/
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/viewer_legacy/app/src/themes/leva_theme.json
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/viewer_legacy/app/tsconfig.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.635997 nerfstudio-1.0.3/nerfstudio/viewer_legacy/server/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/viewer_legacy/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14722 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/viewer_legacy/server/control_panel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/viewer_legacy/server/gui_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/viewer_legacy/server/path.py
--rw-r--r--   0 runner    (1001) docker     (127)    13176 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/viewer_legacy/server/render_state_machine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.635997 nerfstudio-1.0.3/nerfstudio/viewer_legacy/server/state/
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/viewer_legacy/server/state/node.py
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/viewer_legacy/server/state/state_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     3919 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/viewer_legacy/server/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    18868 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/viewer_legacy/server/viewer_elements.py
--rw-r--r--   0 runner    (1001) docker     (127)    19998 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/viewer_legacy/server/viewer_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/viewer_legacy/server/viewer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.635997 nerfstudio-1.0.3/nerfstudio/viewer_legacy/viser/
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/viewer_legacy/viser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6371 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/viewer_legacy/viser/gui.py
--rw-r--r--   0 runner    (1001) docker     (127)    21923 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/viewer_legacy/viser/message_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7352 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/viewer_legacy/viser/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/nerfstudio/viewer_legacy/viser/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.635997 nerfstudio-1.0.3/nerfstudio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    23709 2024-04-03 01:25:34.000000 nerfstudio-1.0.3/nerfstudio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8340 2024-04-03 01:25:34.000000 nerfstudio-1.0.3/nerfstudio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 01:25:34.000000 nerfstudio-1.0.3/nerfstudio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-03 01:25:34.000000 nerfstudio-1.0.3/nerfstudio.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-03 01:25:34.000000 nerfstudio-1.0.3/nerfstudio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-03 01:25:34.000000 nerfstudio-1.0.3/nerfstudio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5837 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 01:25:34.643997 nerfstudio-1.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:25:34.635997 nerfstudio-1.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-04-03 01:25:24.000000 nerfstudio-1.0.3/tests/test_train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:06:44.062272 nerfstudio-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    23710 2024-05-13 19:06:44.062272 nerfstudio-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20055 2024-05-13 19:06:41.000000 nerfstudio-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:06:44.022271 nerfstudio-1.1.0/nerfstudio/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:06:44.022271 nerfstudio-1.1.0/nerfstudio/cameras/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/cameras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8478 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/cameras/camera_optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6558 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/cameras/camera_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33058 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/cameras/camera_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51731 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/cameras/cameras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4790 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/cameras/lie_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11014 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/cameras/rays.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:06:44.026271 nerfstudio-1.1.0/nerfstudio/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6001 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/configs/base_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/configs/config_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/configs/dataparser_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5781 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/configs/experiment_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11225 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/configs/external_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27879 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/configs/method_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:06:44.026271 nerfstudio-1.1.0/nerfstudio/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:06:44.026271 nerfstudio-1.1.0/nerfstudio/data/datamanagers/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/data/datamanagers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25171 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/data/datamanagers/base_datamanager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22350 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/data/datamanagers/full_images_datamanager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15085 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/data/datamanagers/parallel_datamanager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11917 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/data/datamanagers/random_cameras_datamanager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:06:44.030271 nerfstudio-1.1.0/nerfstudio/data/dataparsers/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/data/dataparsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9186 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/data/dataparsers/arkitscenes_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7549 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/data/dataparsers/base_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/data/dataparsers/blender_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28398 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/data/dataparsers/colmap_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/data/dataparsers/dnerf_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13725 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/data/dataparsers/dycheck_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9155 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/data/dataparsers/instant_ngp_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4270 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/data/dataparsers/minimal_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8502 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/data/dataparsers/nerfosr_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21922 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/data/dataparsers/nerfstudio_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8759 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/data/dataparsers/nuscenes_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6957 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/data/dataparsers/phototourism_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6832 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/data/dataparsers/scannet_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8128 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/data/dataparsers/scannetpp_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5943 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/data/dataparsers/sdfstudio_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5963 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/data/dataparsers/sitcoms3d_dataparser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:06:44.030271 nerfstudio-1.1.0/nerfstudio/data/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/data/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6822 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/data/datasets/base_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6002 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/data/datasets/depth_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3877 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/data/datasets/sdf_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/data/datasets/semantic_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23189 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/data/pixel_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4310 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/data/scene_box.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:06:44.030271 nerfstudio-1.1.0/nerfstudio/data/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/data/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20474 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/data/utils/colmap_parsing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/data/utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9324 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/data/utils/dataloaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/data/utils/dataparsers_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10340 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/data/utils/nerfstudio_collate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3707 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/data/utils/pixel_sampling_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:06:44.030271 nerfstudio-1.1.0/nerfstudio/engine/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/engine/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8416 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/engine/optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6170 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/engine/schedulers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25474 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/engine/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:06:44.034272 nerfstudio-1.1.0/nerfstudio/exporter/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/exporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13245 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/exporter/exporter_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10659 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/exporter/marching_cubes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21099 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/exporter/texture_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14230 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/exporter/tsdf_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:06:44.034272 nerfstudio-1.1.0/nerfstudio/field_components/
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/field_components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/field_components/activations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/field_components/base_field_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/field_components/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32841 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/field_components/encodings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6973 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/field_components/field_heads.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11936 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/field_components/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/field_components/spatial_distortions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/field_components/temporal_distortions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:06:44.034272 nerfstudio-1.1.0/nerfstudio/fields/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/fields/base_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4761 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/fields/density_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5888 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/fields/generfacto_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13375 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/fields/nerfacto_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7046 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/fields/nerfw_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18116 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/fields/sdf_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4291 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/fields/semantic_nerf_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/fields/tensorf_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4789 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/fields/vanilla_nerf_field.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:06:44.034272 nerfstudio-1.1.0/nerfstudio/generative/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/generative/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9054 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/generative/deepfloyd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/generative/positional_text_embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11987 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/generative/stable_diffusion.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:06:44.038272 nerfstudio-1.1.0/nerfstudio/model_components/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/model_components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22329 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/model_components/losses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/model_components/ray_generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29334 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/model_components/ray_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16812 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/model_components/renderers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7079 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/model_components/scene_colliders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/model_components/shaders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:06:44.038272 nerfstudio-1.1.0/nerfstudio/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10388 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/models/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17095 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/models/base_surface_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/models/depth_nerfacto.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22094 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/models/generfacto.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10542 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/models/instant_ngp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9228 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/models/mipnerf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19375 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/models/nerfacto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4144 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/models/neus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9481 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/models/neus_facto.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13779 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/models/semantic_nerfw.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39985 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/models/splatfacto.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15809 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/models/tensorf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11325 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/models/vanilla_nerf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:06:44.038272 nerfstudio-1.1.0/nerfstudio/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18390 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/pipelines/base_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/pipelines/dynamic_batch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:06:44.042271 nerfstudio-1.1.0/nerfstudio/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/plugins/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/plugins/registry_dataparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/plugins/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:06:44.042271 nerfstudio-1.1.0/nerfstudio/process_data/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/process_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/process_data/base_converter_to_nerfstudio_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10793 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/process_data/colmap_converter_to_nerfstudio_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28081 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/process_data/colmap_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12843 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/process_data/equirect_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/process_data/hloc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5799 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/process_data/images_to_nerfstudio_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9074 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/process_data/metashape_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6971 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/process_data/odm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10789 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/process_data/polycam_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25630 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/process_data/process_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5200 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/process_data/realitycapture_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/process_data/record3d_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6097 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/process_data/video_to_nerfstudio_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:06:44.042271 nerfstudio-1.1.0/nerfstudio/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/scripts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:06:44.046272 nerfstudio-1.1.0/nerfstudio/scripts/blender/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/scripts/blender/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17246 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/scripts/blender/nerfstudio_blender.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:06:44.046272 nerfstudio-1.1.0/nerfstudio/scripts/completions/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/scripts/completions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15529 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/scripts/completions/install.py
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/scripts/completions/setup.bash
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/scripts/completions/setup.zsh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:06:44.046272 nerfstudio-1.1.0/nerfstudio/scripts/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)     6544 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/scripts/datasets/process_nuscenes_masks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9284 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/scripts/datasets/process_project_aria.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:06:44.046272 nerfstudio-1.1.0/nerfstudio/scripts/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/scripts/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/scripts/docs/add_nb_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/scripts/docs/build_docs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:06:44.046272 nerfstudio-1.1.0/nerfstudio/scripts/downloads/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/scripts/downloads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24960 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/scripts/downloads/download_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18592 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/scripts/downloads/eyeful_tower.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/scripts/downloads/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/scripts/eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27773 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/scripts/exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:06:44.046272 nerfstudio-1.1.0/nerfstudio/scripts/github/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/scripts/github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4432 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/scripts/github/run_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22637 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/scripts/process_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41704 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/scripts/render.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/scripts/texture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9807 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/scripts/train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:06:44.046272 nerfstudio-1.1.0/nerfstudio/scripts/viewer/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/scripts/viewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/scripts/viewer/run_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/scripts/viewer/sync_viser_message_defs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:06:44.050272 nerfstudio-1.1.0/nerfstudio/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7689 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/utils/colormaps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/utils/comms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4618 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/utils/eval_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/utils/external.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/utils/install_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18643 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/utils/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7365 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16909 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/utils/plotly_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/utils/poses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/utils/printing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7950 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/utils/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/utils/rich_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/utils/scripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13665 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/utils/tensor_dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18988 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/utils/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:06:44.050272 nerfstudio-1.1.0/nerfstudio/viewer/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/viewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16956 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/viewer/control_panel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8603 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/viewer/export_panel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46800 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/viewer/render_panel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16238 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/viewer/render_state_machine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:06:44.050272 nerfstudio-1.1.0/nerfstudio/viewer/server/
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/viewer/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/viewer/server/viewer_elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5519 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/viewer/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24634 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/viewer/viewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24700 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/viewer/viewer_elements.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:06:44.054272 nerfstudio-1.1.0/nerfstudio/viewer_legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/viewer_legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:06:44.054272 nerfstudio-1.1.0/nerfstudio/viewer_legacy/app/
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/viewer_legacy/app/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:06:44.054272 nerfstudio-1.1.0/nerfstudio/viewer_legacy/app/public/
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/viewer_legacy/app/public/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/viewer_legacy/app/run_deploy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:06:44.018271 nerfstudio-1.1.0/nerfstudio/viewer_legacy/app/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:06:44.054272 nerfstudio-1.1.0/nerfstudio/viewer_legacy/app/src/themes/
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/viewer_legacy/app/src/themes/leva_theme.json
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/viewer_legacy/app/tsconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:06:44.054272 nerfstudio-1.1.0/nerfstudio/viewer_legacy/server/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/viewer_legacy/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14722 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/viewer_legacy/server/control_panel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/viewer_legacy/server/gui_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/viewer_legacy/server/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13176 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/viewer_legacy/server/render_state_machine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:06:44.054272 nerfstudio-1.1.0/nerfstudio/viewer_legacy/server/state/
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/viewer_legacy/server/state/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/viewer_legacy/server/state/state_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3919 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/viewer_legacy/server/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18868 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/viewer_legacy/server/viewer_elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19998 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/viewer_legacy/server/viewer_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/viewer_legacy/server/viewer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:06:44.054272 nerfstudio-1.1.0/nerfstudio/viewer_legacy/viser/
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/viewer_legacy/viser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6371 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/viewer_legacy/viser/gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21923 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/viewer_legacy/viser/message_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7352 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/viewer_legacy/viser/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/nerfstudio/viewer_legacy/viser/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:06:44.054272 nerfstudio-1.1.0/nerfstudio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    23710 2024-05-13 19:06:43.000000 nerfstudio-1.1.0/nerfstudio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8340 2024-05-13 19:06:44.000000 nerfstudio-1.1.0/nerfstudio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 19:06:43.000000 nerfstudio-1.1.0/nerfstudio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-13 19:06:43.000000 nerfstudio-1.1.0/nerfstudio.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-13 19:06:43.000000 nerfstudio-1.1.0/nerfstudio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-13 19:06:43.000000 nerfstudio-1.1.0/nerfstudio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5838 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 19:06:44.062272 nerfstudio-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:06:44.054272 nerfstudio-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-05-13 19:06:34.000000 nerfstudio-1.1.0/tests/test_train.py
```

### Comparing `nerfstudio-1.0.3/LICENSE` & `nerfstudio-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/PKG-INFO` & `nerfstudio-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nerfstudio
-Version: 1.0.3
+Version: 1.1.0
 Summary: All-in-one repository for state-of-the-art NeRFs
 License: Apache 2.0
 Project-URL: Documentation, https://docs.nerf.studio
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
@@ -44,21 +44,21 @@
 Requires-Dist: scikit-image>=0.19.3
 Requires-Dist: splines==0.3.0
 Requires-Dist: tensorboard>=2.13.0
 Requires-Dist: torch>=1.13.1
 Requires-Dist: torchvision>=0.14.1
 Requires-Dist: torchmetrics[image]>=1.0.1
 Requires-Dist: typing_extensions>=4.4.0
-Requires-Dist: viser==0.1.26
+Requires-Dist: viser==0.1.27
 Requires-Dist: nuscenes-devkit>=1.1.1
 Requires-Dist: wandb>=0.13.3
 Requires-Dist: xatlas
 Requires-Dist: trimesh>=3.20.2
 Requires-Dist: timm==0.6.7
-Requires-Dist: gsplat>=0.1.9
+Requires-Dist: gsplat>=0.1.11
 Requires-Dist: pytorch-msssim
 Requires-Dist: pathos
 Requires-Dist: packaging
 Provides-Extra: gen
 Requires-Dist: diffusers==0.16.1; extra == "gen"
 Requires-Dist: transformers==4.29.2; extra == "gen"
 Requires-Dist: accelerate==0.19.0; extra == "gen"
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nerfstudio Version: 1.0.3 Summary: All-in-one
+Metadata-Version: 2.1 Name: nerfstudio Version: 1.1.0 Summary: All-in-one
 repository for state-of-the-art NeRFs License: Apache 2.0 Project-URL:
 Documentation, https://docs.nerf.studio Classifier: Development Status :: 3 -
 Alpha Classifier: Programming Language :: Python Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 appdirs>=1.4 Requires-Dist: av>=9.2.0 Requires-Dist: awscli>=1.31.10 Requires-
 Dist: comet_ml>=3.33.8 Requires-Dist: cryptography>=38 Requires-Dist:
 tyro>=0.6.6 Requires-Dist: gdown>=4.6.0 Requires-Dist: ninja>=1.10 Requires-
@@ -18,17 +18,17 @@
 "aarch64" Requires-Dist: pyngrok>=5.1.0 Requires-Dist: python-socketio>=5.7.1
 Requires-Dist: pyquaternion>=0.9.9 Requires-Dist: rawpy>=0.18.1;
 platform_machine != "arm64" Requires-Dist: newrawpy>=1.0.0b0; platform_machine
 == "arm64" Requires-Dist: requests Requires-Dist: rich>=12.5.1 Requires-Dist:
 scikit-image>=0.19.3 Requires-Dist: splines==0.3.0 Requires-Dist:
 tensorboard>=2.13.0 Requires-Dist: torch>=1.13.1 Requires-Dist:
 torchvision>=0.14.1 Requires-Dist: torchmetrics[image]>=1.0.1 Requires-Dist:
-typing_extensions>=4.4.0 Requires-Dist: viser==0.1.26 Requires-Dist: nuscenes-
+typing_extensions>=4.4.0 Requires-Dist: viser==0.1.27 Requires-Dist: nuscenes-
 devkit>=1.1.1 Requires-Dist: wandb>=0.13.3 Requires-Dist: xatlas Requires-Dist:
-trimesh>=3.20.2 Requires-Dist: timm==0.6.7 Requires-Dist: gsplat>=0.1.9
+trimesh>=3.20.2 Requires-Dist: timm==0.6.7 Requires-Dist: gsplat>=0.1.11
 Requires-Dist: pytorch-msssim Requires-Dist: pathos Requires-Dist: packaging
 Provides-Extra: gen Requires-Dist: diffusers==0.16.1; extra == "gen" Requires-
 Dist: transformers==4.29.2; extra == "gen" Requires-Dist: accelerate==0.19.0;
 extra == "gen" Requires-Dist: bitsandbytes==0.39.0; extra == "gen" Requires-
 Dist: sentencepiece==0.1.99; extra == "gen" Provides-Extra: dev Requires-Dist:
 pre-commit==3.3.2; extra == "dev" Requires-Dist: pytest==7.1.2; extra == "dev"
 Requires-Dist: pytest-xdist==2.5.0; extra == "dev" Requires-Dist:
```

### Comparing `nerfstudio-1.0.3/README.md` & `nerfstudio-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/__init__.py` & `nerfstudio-1.1.0/nerfstudio/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/cameras/__init__.py` & `nerfstudio-1.1.0/nerfstudio/cameras/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/cameras/camera_optimizers.py` & `nerfstudio-1.1.0/nerfstudio/cameras/camera_optimizers.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 from __future__ import annotations
 
 import functools
 from dataclasses import dataclass, field
 from typing import Literal, Optional, Type, Union
 
+import numpy
 import torch
 import tyro
 from jaxtyping import Float, Int
 from torch import Tensor, nn
 from typing_extensions import assert_never
 
 from nerfstudio.cameras.cameras import Cameras
@@ -147,23 +148,28 @@
     def apply_to_raybundle(self, raybundle: RayBundle) -> None:
         """Apply the pose correction to the raybundle"""
         if self.config.mode != "off":
             correction_matrices = self(raybundle.camera_indices.squeeze())  # type: ignore
             raybundle.origins = raybundle.origins + correction_matrices[:, :3, 3]
             raybundle.directions = torch.bmm(correction_matrices[:, :3, :3], raybundle.directions[..., None]).squeeze()
 
-    def apply_to_camera(self, camera: Cameras) -> None:
-        """Apply the pose correction to the raybundle"""
-        if self.config.mode != "off":
-            assert camera.metadata is not None, "Must provide id of camera in its metadata"
-            assert "cam_idx" in camera.metadata, "Must provide id of camera in its metadata"
-            camera_idx = camera.metadata["cam_idx"]
-            adj = self(torch.tensor([camera_idx], dtype=torch.long, device=camera.device))  # type: ignore
-            adj = torch.cat([adj, torch.Tensor([0, 0, 0, 1])[None, None].to(adj)], dim=1)
-            camera.camera_to_worlds = torch.bmm(camera.camera_to_worlds, adj)
+    def apply_to_camera(self, camera: Cameras) -> torch.Tensor:
+        """Apply the pose correction to the world-to-camera matrix in a Camera object"""
+        if self.config.mode == "off":
+            return camera.camera_to_worlds
+
+        assert camera.metadata is not None, "Must provide id of camera in its metadata"
+        if "cam_idx" not in camera.metadata:
+            # Evalutaion cams?
+            return camera.camera_to_worlds
+
+        camera_idx = camera.metadata["cam_idx"]
+        adj = self(torch.tensor([camera_idx], dtype=torch.long, device=camera.device))  # type: ignore
+        adj = torch.cat([adj, torch.Tensor([0, 0, 0, 1])[None, None].to(adj)], dim=1)
+        return torch.bmm(camera.camera_to_worlds, adj)
 
     def get_loss_dict(self, loss_dict: dict) -> None:
         """Add regularization"""
         if self.config.mode != "off":
             loss_dict["camera_opt_regularizer"] = (
                 self.pose_adjustment[:, :3].norm(dim=-1).mean() * self.config.trans_l2_penalty
                 + self.pose_adjustment[:, 3:].norm(dim=-1).mean() * self.config.rot_l2_penalty
@@ -172,16 +178,20 @@
     def get_correction_matrices(self):
         """Get optimized pose correction matrices"""
         return self(torch.arange(0, self.num_cameras).long())
 
     def get_metrics_dict(self, metrics_dict: dict) -> None:
         """Get camera optimizer metrics"""
         if self.config.mode != "off":
-            metrics_dict["camera_opt_translation"] = self.pose_adjustment[:, :3].norm()
-            metrics_dict["camera_opt_rotation"] = self.pose_adjustment[:, 3:].norm()
+            trans = self.pose_adjustment[:, :3].detach().norm(dim=-1)
+            rot = self.pose_adjustment[:, 3:].detach().norm(dim=-1)
+            metrics_dict["camera_opt_translation_max"] = trans.max()
+            metrics_dict["camera_opt_translation_mean"] = trans.mean()
+            metrics_dict["camera_opt_rotation_mean"] = numpy.rad2deg(rot.mean().cpu())
+            metrics_dict["camera_opt_rotation_max"] = numpy.rad2deg(rot.max().cpu())
 
     def get_param_groups(self, param_groups: dict) -> None:
         """Get camera optimizer parameters"""
         camera_opt_params = list(self.parameters())
         if self.config.mode != "off":
             assert len(camera_opt_params) > 0
             param_groups["camera_opt"] = camera_opt_params
```

### Comparing `nerfstudio-1.0.3/nerfstudio/cameras/camera_paths.py` & `nerfstudio-1.1.0/nerfstudio/cameras/camera_paths.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/cameras/camera_utils.py` & `nerfstudio-1.1.0/nerfstudio/cameras/camera_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/cameras/cameras.py` & `nerfstudio-1.1.0/nerfstudio/cameras/cameras.py`

 * *Files 2% similar despite different names*

```diff
@@ -980,20 +980,23 @@
         K[..., 1, 1] = self.fy.squeeze(-1)
         K[..., 0, 2] = self.cx.squeeze(-1)
         K[..., 1, 2] = self.cy.squeeze(-1)
         K[..., 2, 2] = 1.0
         return K
 
     def rescale_output_resolution(
-        self, scaling_factor: Union[Shaped[Tensor, "*num_cameras"], Shaped[Tensor, "*num_cameras 1"], float, int]
+        self,
+        scaling_factor: Union[Shaped[Tensor, "*num_cameras"], Shaped[Tensor, "*num_cameras 1"], float, int],
+        scale_rounding_mode: str = "floor",
     ) -> None:
         """Rescale the output resolution of the cameras.
 
         Args:
             scaling_factor: Scaling factor to apply to the output resolution.
+            scale_rounding_mode: round down or round up when calculating the scaled image height and width
         """
         if isinstance(scaling_factor, (float, int)):
             scaling_factor = torch.tensor([scaling_factor]).to(self.device).broadcast_to((self.cx.shape))
         elif isinstance(scaling_factor, torch.Tensor) and scaling_factor.shape == self.shape:
             scaling_factor = scaling_factor.unsqueeze(-1)
         elif isinstance(scaling_factor, torch.Tensor) and scaling_factor.shape == (*self.shape, 1):
             pass
@@ -1002,9 +1005,18 @@
                 f"Scaling factor must be a float, int, or a tensor of shape {self.shape} or {(*self.shape, 1)}."
             )
 
         self.fx = self.fx * scaling_factor
         self.fy = self.fy * scaling_factor
         self.cx = self.cx * scaling_factor
         self.cy = self.cy * scaling_factor
-        self.height = (self.height * scaling_factor).to(torch.int64)
-        self.width = (self.width * scaling_factor).to(torch.int64)
+        if scale_rounding_mode == "floor":
+            self.height = (self.height * scaling_factor).to(torch.int64)
+            self.width = (self.width * scaling_factor).to(torch.int64)
+        elif scale_rounding_mode == "round":
+            self.height = torch.floor(0.5 + (self.height * scaling_factor)).to(torch.int64)
+            self.width = torch.floor(0.5 + (self.width * scaling_factor)).to(torch.int64)
+        elif scale_rounding_mode == "ceil":
+            self.height = torch.ceil(self.height * scaling_factor).to(torch.int64)
+            self.width = torch.ceil(self.width * scaling_factor).to(torch.int64)
+        else:
+            raise ValueError("Scale rounding mode must be 'floor', 'round' or 'ceil'.")
```

### Comparing `nerfstudio-1.0.3/nerfstudio/cameras/lie_groups.py` & `nerfstudio-1.1.0/nerfstudio/cameras/lie_groups.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/cameras/rays.py` & `nerfstudio-1.1.0/nerfstudio/cameras/rays.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/configs/__init__.py` & `nerfstudio-1.1.0/nerfstudio/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/configs/base_config.py` & `nerfstudio-1.1.0/nerfstudio/configs/base_config.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/configs/config_utils.py` & `nerfstudio-1.1.0/nerfstudio/configs/config_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/configs/dataparser_configs.py` & `nerfstudio-1.1.0/nerfstudio/configs/dataparser_configs.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/configs/experiment_config.py` & `nerfstudio-1.1.0/nerfstudio/configs/experiment_config.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/configs/external_methods.py` & `nerfstudio-1.1.0/nerfstudio/configs/external_methods.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 """This file contains the configuration for external methods which are not included in this repository."""
+
 import inspect
 import subprocess
 import sys
 from dataclasses import dataclass
 from typing import Dict, List, Optional, Tuple
 
 import tyro
@@ -136,14 +137,27 @@
                 "Real-time rendering model from Volinga. Directly exportable to NVOL format at https://volinga.ai/",
             ),
         ],
         pip_package="git+https://github.com/Volinga/volinga-model",
     )
 )
 
+# BioNeRF
+external_methods.append(
+    ExternalMethod(
+        """[bold yellow]BioNeRF[/bold yellow]
+For more information visit: https://docs.nerf.studio/nerfology/methods/bionerf.html
+
+To enable BioNeRF, you must install it first by running:
+  [grey]pip install git+https://github.com/Leandropassosjr/ns_bionerf[/grey]""",
+        configurations=[("BioNeRF", "BioNeRF. Nerfstudio implementation")],
+        pip_package="git+https://github.com/Leandropassosjr/ns_bionerf",
+    )
+)
+
 # Instruct-GS2GS
 external_methods.append(
     ExternalMethod(
         """[bold yellow]Instruct-GS2GS[/bold yellow]
 For more information visit: https://docs.nerf.studio/nerfology/methods/igs2gs.html
 
 To enable Instruct-GS2GS, you must install it first by running:
@@ -204,14 +218,30 @@
         configurations=[
             ("zipnerf", "A pytorch implementation of 'Zip-NeRF: Anti-Aliased Grid-Based Neural Radiance Fields'")
         ],
         pip_package="pip install git+https://github.com/SuLvXiangXin/zipnerf-pytorch",
     )
 )
 
+# SIGNeRF
+external_methods.append(
+    ExternalMethod(
+        """[bold yellow]SIGNeRF[/bold yellow]
+For more information visit: https://docs.nerf.studio/nerfology/methods/signerf.html
+
+To enable SIGNeRF, you must install it first by running:
+  [grey]pip install git+https://github.com/cgtuebingen/SIGNeRF[/grey] and install Stable Diffusion Web UI see [grey]https://github.com/cgtuebingen/SIGNeRF?tab=readme-ov-file#installation[/grey]""",
+        configurations=[
+            ("signerf", "SIGNeRF method (high quality) used in paper"),
+            ("signerf_nerfacto", "SIGNeRF method combined with Nerfacto (faster training less quality)"),
+        ],
+        pip_package="git+https://github.com/cgtuebingen/SIGNeRF",
+    )
+)
+
 
 @dataclass
 class ExternalMethodDummyTrainerConfig:
     """Dummy trainer config for external methods (a) which do not have an
     implementation in this repository, and (b) are not yet installed. When this
     config is instantiated, we give the user the option to install the method.
     """
```

### Comparing `nerfstudio-1.0.3/nerfstudio/configs/method_configs.py` & `nerfstudio-1.1.0/nerfstudio/configs/method_configs.py`

 * *Files 2% similar despite different names*

```diff
@@ -628,16 +628,18 @@
         },
         "scales": {
             "optimizer": AdamOptimizerConfig(lr=0.005, eps=1e-15),
             "scheduler": None,
         },
         "quats": {"optimizer": AdamOptimizerConfig(lr=0.001, eps=1e-15), "scheduler": None},
         "camera_opt": {
-            "optimizer": AdamOptimizerConfig(lr=1e-3, eps=1e-15),
-            "scheduler": ExponentialDecaySchedulerConfig(lr_final=5e-5, max_steps=30000),
+            "optimizer": AdamOptimizerConfig(lr=1e-4, eps=1e-15),
+            "scheduler": ExponentialDecaySchedulerConfig(
+                lr_final=5e-7, max_steps=30000, warmup_steps=1000, lr_pre_warmup=0
+            ),
         },
     },
     viewer=ViewerConfig(num_rays_per_chunk=1 << 15),
     vis="viewer",
 )
 
 method_configs["splatfacto-big"] = TrainerConfig(
@@ -652,14 +654,15 @@
         datamanager=FullImageDatamanagerConfig(
             dataparser=NerfstudioDataParserConfig(load_3D_points=True),
             cache_images_type="uint8",
         ),
         model=SplatfactoModelConfig(
             cull_alpha_thresh=0.005,
             continue_cull_post_densification=False,
+            densify_grad_thresh=0.0006,
         ),
     ),
     optimizers={
         "means": {
             "optimizer": AdamOptimizerConfig(lr=1.6e-4, eps=1e-15),
             "scheduler": ExponentialDecaySchedulerConfig(
                 lr_final=1.6e-6,
@@ -680,16 +683,18 @@
         },
         "scales": {
             "optimizer": AdamOptimizerConfig(lr=0.005, eps=1e-15),
             "scheduler": None,
         },
         "quats": {"optimizer": AdamOptimizerConfig(lr=0.001, eps=1e-15), "scheduler": None},
         "camera_opt": {
-            "optimizer": AdamOptimizerConfig(lr=1e-3, eps=1e-15),
-            "scheduler": ExponentialDecaySchedulerConfig(lr_final=5e-5, max_steps=30000),
+            "optimizer": AdamOptimizerConfig(lr=1e-4, eps=1e-15),
+            "scheduler": ExponentialDecaySchedulerConfig(
+                lr_final=5e-7, max_steps=30000, warmup_steps=1000, lr_pre_warmup=0
+            ),
         },
     },
     viewer=ViewerConfig(num_rays_per_chunk=1 << 15),
     vis="viewer",
 )
```

### Comparing `nerfstudio-1.0.3/nerfstudio/data/__init__.py` & `nerfstudio-1.1.0/nerfstudio/data/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/data/datamanagers/__init__.py` & `nerfstudio-1.1.0/nerfstudio/data/datamanagers/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/data/datamanagers/base_datamanager.py` & `nerfstudio-1.1.0/nerfstudio/data/datamanagers/base_datamanager.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/data/datamanagers/full_images_datamanager.py` & `nerfstudio-1.1.0/nerfstudio/data/datamanagers/full_images_datamanager.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 from typing import Dict, ForwardRef, Generic, List, Literal, Optional, Tuple, Type, Union, cast, get_args, get_origin
 
 import cv2
 import numpy as np
 import torch
 from rich.progress import track
 from torch.nn import Parameter
+from typing_extensions import assert_never
 
 from nerfstudio.cameras.camera_utils import fisheye624_project, fisheye624_unproject_helper
 from nerfstudio.cameras.cameras import Cameras, CameraType
 from nerfstudio.configs.dataparser_configs import AnnotatedDataParserUnion
 from nerfstudio.data.datamanagers.base_datamanager import DataManager, DataManagerConfig, TDataset
 from nerfstudio.data.dataparsers.base_dataparser import DataparserOutputs
 from nerfstudio.data.dataparsers.nerfstudio_dataparser import NerfstudioDataParserConfig
@@ -111,126 +112,107 @@
         self.eval_dataset = self.create_eval_dataset()
         if len(self.train_dataset) > 500 and self.config.cache_images == "gpu":
             CONSOLE.print(
                 "Train dataset has over 500 images, overriding cache_images to cpu",
                 style="bold yellow",
             )
             self.config.cache_images = "cpu"
-        self.cached_train, self.cached_eval = self.cache_images(self.config.cache_images)
         self.exclude_batch_keys_from_device = self.train_dataset.exclude_batch_keys_from_device
         if self.config.masks_on_gpu is True:
             self.exclude_batch_keys_from_device.remove("mask")
         if self.config.images_on_gpu is True:
             self.exclude_batch_keys_from_device.remove("image")
 
         # Some logic to make sure we sample every camera in equal amounts
         self.train_unseen_cameras = [i for i in range(len(self.train_dataset))]
         self.eval_unseen_cameras = [i for i in range(len(self.eval_dataset))]
         assert len(self.train_unseen_cameras) > 0, "No data found in dataset"
 
         super().__init__()
 
-    def cache_images(self, cache_images_option):
-        cached_train = []
-        cached_eval = []
-
-        def process_train_data(idx):
-            # cv2.undistort the images / cameras
-            data = self.train_dataset.get_data(idx, image_type=self.config.cache_images_type)
-            camera = self.train_dataset.cameras[idx].reshape(())
-            K = camera.get_intrinsics_matrices().numpy()
-            if camera.distortion_params is None:
-                return data
-            distortion_params = camera.distortion_params.numpy()
-            image = data["image"].numpy()
-
-            K, image, mask = _undistort_image(camera, distortion_params, data, image, K)
-            data["image"] = torch.from_numpy(image)
-            if mask is not None:
-                data["mask"] = mask
+    @cached_property
+    def cached_train(self) -> List[Dict[str, torch.Tensor]]:
+        """Get the training images. Will load and undistort the images the
+        first time this (cached) property is accessed."""
+        return self._load_images("train", cache_images_device=self.config.cache_images)
 
-            self.train_dataset.cameras.fx[idx] = float(K[0, 0])
-            self.train_dataset.cameras.fy[idx] = float(K[1, 1])
-            self.train_dataset.cameras.cx[idx] = float(K[0, 2])
-            self.train_dataset.cameras.cy[idx] = float(K[1, 2])
-            self.train_dataset.cameras.width[idx] = image.shape[1]
-            self.train_dataset.cameras.height[idx] = image.shape[0]
-            return data
+    @cached_property
+    def cached_eval(self) -> List[Dict[str, torch.Tensor]]:
+        """Get the eval images. Will load and undistort the images the
+        first time this (cached) property is accessed."""
+        return self._load_images("eval", cache_images_device=self.config.cache_images)
+
+    def _load_images(
+        self, split: Literal["train", "eval"], cache_images_device: Literal["cpu", "gpu"]
+    ) -> List[Dict[str, torch.Tensor]]:
+        undistorted_images: List[Dict[str, torch.Tensor]] = []
+
+        # Which dataset?
+        if split == "train":
+            dataset = self.train_dataset
+        elif split == "eval":
+            dataset = self.eval_dataset
+        else:
+            assert_never(split)
 
-        def process_eval_data(idx):
-            # cv2.undistort the images / cameras
-            data = self.eval_dataset.get_data(idx, image_type=self.config.cache_images_type)
-            camera = self.eval_dataset.cameras[idx].reshape(())
-            K = camera.get_intrinsics_matrices().numpy()
+        def undistort_idx(idx: int) -> Dict[str, torch.Tensor]:
+            data = dataset.get_data(idx, image_type=self.config.cache_images_type)
+            camera = dataset.cameras[idx].reshape(())
+            assert data["image"].shape[1] == camera.width.item() and data["image"].shape[0] == camera.height.item(), (
+                f'The size of image ({data["image"].shape[1]}, {data["image"].shape[0]}) loaded '
+                f'does not match the camera parameters ({camera.width.item(), camera.height.item()})'
+            )
             if camera.distortion_params is None:
                 return data
+            K = camera.get_intrinsics_matrices().numpy()
             distortion_params = camera.distortion_params.numpy()
             image = data["image"].numpy()
 
             K, image, mask = _undistort_image(camera, distortion_params, data, image, K)
             data["image"] = torch.from_numpy(image)
             if mask is not None:
                 data["mask"] = mask
 
-            self.eval_dataset.cameras.fx[idx] = float(K[0, 0])
-            self.eval_dataset.cameras.fy[idx] = float(K[1, 1])
-            self.eval_dataset.cameras.cx[idx] = float(K[0, 2])
-            self.eval_dataset.cameras.cy[idx] = float(K[1, 2])
-            self.eval_dataset.cameras.width[idx] = image.shape[1]
-            self.eval_dataset.cameras.height[idx] = image.shape[0]
+            dataset.cameras.fx[idx] = float(K[0, 0])
+            dataset.cameras.fy[idx] = float(K[1, 1])
+            dataset.cameras.cx[idx] = float(K[0, 2])
+            dataset.cameras.cy[idx] = float(K[1, 2])
+            dataset.cameras.width[idx] = image.shape[1]
+            dataset.cameras.height[idx] = image.shape[0]
             return data
 
-        CONSOLE.log("Caching / undistorting train images")
+        CONSOLE.log(f"Caching / undistorting {split} images")
         with ThreadPoolExecutor(max_workers=2) as executor:
-            cached_train = list(
+            undistorted_images = list(
                 track(
                     executor.map(
-                        process_train_data,
-                        range(len(self.train_dataset)),
+                        undistort_idx,
+                        range(len(dataset)),
                     ),
-                    description="Caching / undistorting train images",
+                    description=f"Caching / undistorting {split} images",
                     transient=True,
-                    total=len(self.train_dataset),
+                    total=len(dataset),
                 )
             )
 
-        CONSOLE.log("Caching / undistorting eval images")
-        with ThreadPoolExecutor(max_workers=2) as executor:
-            cached_eval = list(
-                track(
-                    executor.map(
-                        process_eval_data,
-                        range(len(self.eval_dataset)),
-                    ),
-                    description="Caching / undistorting eval images",
-                    transient=True,
-                    total=len(self.eval_dataset),
-                )
-            )
-
-        if cache_images_option == "gpu":
-            for cache in cached_train:
+        # Move to device.
+        if cache_images_device == "gpu":
+            for cache in undistorted_images:
                 cache["image"] = cache["image"].to(self.device)
                 if "mask" in cache:
                     cache["mask"] = cache["mask"].to(self.device)
-            for cache in cached_eval:
-                cache["image"] = cache["image"].to(self.device)
-                if "mask" in cache:
-                    cache["mask"] = cache["mask"].to(self.device)
-        else:
-            for cache in cached_train:
-                cache["image"] = cache["image"].pin_memory()
-                if "mask" in cache:
-                    cache["mask"] = cache["mask"].pin_memory()
-            for cache in cached_eval:
+        elif cache_images_device == "cpu":
+            for cache in undistorted_images:
                 cache["image"] = cache["image"].pin_memory()
                 if "mask" in cache:
                     cache["mask"] = cache["mask"].pin_memory()
+        else:
+            assert_never(cache_images_device)
 
-        return cached_train, cached_eval
+        return undistorted_images
 
     def create_train_dataset(self) -> TDataset:
         """Sets up the data loaders for training"""
         return self.dataset_type(
             dataparser_outputs=self.train_dataparser_outputs,
             scale_factor=self.config.camera_res_scale_factor,
         )
@@ -353,26 +335,34 @@
 
 
 def _undistort_image(
     camera: Cameras, distortion_params: np.ndarray, data: dict, image: np.ndarray, K: np.ndarray
 ) -> Tuple[np.ndarray, np.ndarray, Optional[torch.Tensor]]:
     mask = None
     if camera.camera_type.item() == CameraType.PERSPECTIVE.value:
+        assert distortion_params[3] == 0, (
+            "We doesn't support the 4th Brown parameter for image undistortion, "
+            "Only k1, k2, k3, p1, p2 can be non-zero."
+        )
         distortion_params = np.array(
             [
                 distortion_params[0],
                 distortion_params[1],
                 distortion_params[4],
                 distortion_params[5],
                 distortion_params[2],
                 distortion_params[3],
                 0,
                 0,
             ]
         )
+        # because OpenCV expects the pixel coord to be top-left, we need to shift the principal point by 0.5
+        # see https://github.com/nerfstudio-project/nerfstudio/issues/3048
+        K[0, 2] = K[0, 2] - 0.5
+        K[1, 2] = K[1, 2] - 0.5
         if np.any(distortion_params):
             newK, roi = cv2.getOptimalNewCameraMatrix(K, distortion_params, (image.shape[1], image.shape[0]), 0)
             image = cv2.undistort(image, K, distortion_params, None, newK)  # type: ignore
         else:
             newK = K
             roi = 0, 0, image.shape[1], image.shape[0]
         # crop the image and update the intrinsics accordingly
@@ -385,17 +375,21 @@
             mask = mask.astype(np.uint8) * 255
             if np.any(distortion_params):
                 mask = cv2.undistort(mask, K, distortion_params, None, newK)  # type: ignore
             mask = mask[y : y + h, x : x + w]
             mask = torch.from_numpy(mask).bool()
             if len(mask.shape) == 2:
                 mask = mask[:, :, None]
+        newK[0, 2] = newK[0, 2] + 0.5
+        newK[1, 2] = newK[1, 2] + 0.5
         K = newK
 
     elif camera.camera_type.item() == CameraType.FISHEYE.value:
+        K[0, 2] = K[0, 2] - 0.5
+        K[1, 2] = K[1, 2] - 0.5
         distortion_params = np.array(
             [distortion_params[0], distortion_params[1], distortion_params[2], distortion_params[3]]
         )
         newK = cv2.fisheye.estimateNewCameraMatrixForUndistortRectify(
             K, distortion_params, (image.shape[1], image.shape[0]), np.eye(3), balance=0
         )
         map1, map2 = cv2.fisheye.initUndistortRectifyMap(
@@ -406,14 +400,16 @@
         if "mask" in data:
             mask = data["mask"].numpy()
             mask = mask.astype(np.uint8) * 255
             mask = cv2.fisheye.undistortImage(mask, K, distortion_params, None, newK)
             mask = torch.from_numpy(mask).bool()
             if len(mask.shape) == 2:
                 mask = mask[:, :, None]
+        newK[0, 2] = newK[0, 2] + 0.5
+        newK[1, 2] = newK[1, 2] + 0.5
         K = newK
     elif camera.camera_type.item() == CameraType.FISHEYE624.value:
         fisheye624_params = torch.cat(
             [camera.fx, camera.fy, camera.cx, camera.cy, torch.from_numpy(distortion_params)], dim=0
         )
         assert fisheye624_params.shape == (16,)
         assert (
```

### Comparing `nerfstudio-1.0.3/nerfstudio/data/datamanagers/parallel_datamanager.py` & `nerfstudio-1.1.0/nerfstudio/data/datamanagers/parallel_datamanager.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -89,18 +89,18 @@
         self.out_queue = out_queue
         self.config = config
         self.dataparser_outputs = dataparser_outputs
         self.dataset = dataset
         self.exclude_batch_keys_from_device = self.dataset.exclude_batch_keys_from_device
         self.pixel_sampler = pixel_sampler
         self.ray_generator = RayGenerator(self.dataset.cameras)
-        self.cache_images()
 
     def run(self):
         """Append out queue in parallel with ray bundles and batches."""
+        self.cache_images()
         while True:
             batch = self.pixel_sampler.sample(self.img_data)
             ray_indices = batch["indices"]
             ray_bundle: RayBundle = self.ray_generator(ray_indices)
             # check that GPUs are available
             if torch.cuda.is_available():
                 ray_bundle = ray_bundle.pin_memory()
```

### Comparing `nerfstudio-1.0.3/nerfstudio/data/datamanagers/random_cameras_datamanager.py` & `nerfstudio-1.1.0/nerfstudio/data/datamanagers/random_cameras_datamanager.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/data/dataparsers/__init__.py` & `nerfstudio-1.1.0/nerfstudio/data/dataparsers/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/data/dataparsers/arkitscenes_dataparser.py` & `nerfstudio-1.1.0/nerfstudio/data/dataparsers/arkitscenes_dataparser.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/data/dataparsers/base_dataparser.py` & `nerfstudio-1.1.0/nerfstudio/data/dataparsers/base_dataparser.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/data/dataparsers/blender_dataparser.py` & `nerfstudio-1.1.0/nerfstudio/data/dataparsers/dnerf_dataparser.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,56 +27,59 @@
 from nerfstudio.data.dataparsers.base_dataparser import DataParser, DataParserConfig, DataparserOutputs
 from nerfstudio.data.scene_box import SceneBox
 from nerfstudio.utils.colors import get_color
 from nerfstudio.utils.io import load_from_json
 
 
 @dataclass
-class BlenderDataParserConfig(DataParserConfig):
-    """Blender dataset parser config"""
+class DNeRFDataParserConfig(DataParserConfig):
+    """D-NeRF dataset parser config"""
 
-    _target: Type = field(default_factory=lambda: Blender)
+    _target: Type = field(default_factory=lambda: DNeRF)
     """target class to instantiate"""
-    data: Path = Path("data/blender/lego")
+    data: Path = Path("data/dnerf/lego")
     """Directory specifying location of data."""
     scale_factor: float = 1.0
     """How much to scale the camera origins by."""
     alpha_color: str = "white"
     """alpha color of background"""
 
 
 @dataclass
-class Blender(DataParser):
-    """Blender Dataset
-    Some of this code comes from https://github.com/yenchenlin/nerf-pytorch/blob/master/load_blender.py#L37.
-    """
+class DNeRF(DataParser):
+    """DNeRF Dataset"""
 
-    config: BlenderDataParserConfig
+    config: DNeRFDataParserConfig
+    includes_time: bool = True
 
-    def __init__(self, config: BlenderDataParserConfig):
+    def __init__(self, config: DNeRFDataParserConfig):
         super().__init__(config=config)
         self.data: Path = config.data
         self.scale_factor: float = config.scale_factor
         self.alpha_color = config.alpha_color
+
+    def _generate_dataparser_outputs(self, split="train"):
         if self.alpha_color is not None:
-            self.alpha_color_tensor = get_color(self.alpha_color)
+            alpha_color_tensor = get_color(self.alpha_color)
         else:
-            self.alpha_color_tensor = None
+            alpha_color_tensor = None
 
-    def _generate_dataparser_outputs(self, split="train"):
         meta = load_from_json(self.data / f"transforms_{split}.json")
         image_filenames = []
         poses = []
+        times = []
         for frame in meta["frames"]:
             fname = self.data / Path(frame["file_path"].replace("./", "") + ".png")
             image_filenames.append(fname)
             poses.append(np.array(frame["transform_matrix"]))
+            times.append(frame["time"])
         poses = np.array(poses).astype(np.float32)
+        times = torch.tensor(times, dtype=torch.float32)
 
-        img_0 = imageio.v2.imread(image_filenames[0])
+        img_0 = imageio.imread(image_filenames[0])
         image_height, image_width = img_0.shape[:2]
         camera_angle_x = float(meta["camera_angle_x"])
         focal_length = 0.5 * image_width / np.tan(0.5 * camera_angle_x)
 
         cx = image_width / 2.0
         cy = image_height / 2.0
         camera_to_world = torch.from_numpy(poses[:, :3])  # camera to world transform
@@ -88,18 +91,19 @@
         cameras = Cameras(
             camera_to_worlds=camera_to_world,
             fx=focal_length,
             fy=focal_length,
             cx=cx,
             cy=cy,
             camera_type=CameraType.PERSPECTIVE,
+            times=times,
         )
 
         dataparser_outputs = DataparserOutputs(
             image_filenames=image_filenames,
             cameras=cameras,
-            alpha_color=self.alpha_color_tensor,
+            alpha_color=alpha_color_tensor,
             scene_box=scene_box,
             dataparser_scale=self.scale_factor,
         )
 
         return dataparser_outputs
```

### Comparing `nerfstudio-1.0.3/nerfstudio/data/dataparsers/colmap_dataparser.py` & `nerfstudio-1.1.0/nerfstudio/data/dataparsers/colmap_dataparser.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """ Data parser for nerfstudio datasets. """
 
 from __future__ import annotations
 
+import math
 import sys
 from dataclasses import dataclass, field
 from functools import partial
 from pathlib import Path
 from typing import List, Literal, Optional, Type
 
 import numpy as np
@@ -52,14 +53,16 @@
     """target class to instantiate"""
     data: Path = Path()
     """Directory or explicit json file path specifying location of data."""
     scale_factor: float = 1.0
     """How much to scale the camera origins by."""
     downscale_factor: Optional[int] = None
     """How much to downscale images. If not set, images are chosen such that the max dimension is <1600px."""
+    downscale_rounding_mode: Literal["floor", "round", "ceil"] = "floor"
+    """How to round downscale image height and Image width."""
     scene_scale: float = 1.0
     """How much to scale the region of interest by."""
     orientation_method: Literal["pca", "up", "vertical", "none"] = "up"
     """The method to use for orientation."""
     center_method: Literal["poses", "focus", "none"] = "poses"
     """The method to use to center the poses."""
     auto_scale_poses: bool = True
@@ -351,15 +354,17 @@
             distortion_params=distortion_params,
             height=height,
             width=width,
             camera_to_worlds=poses[:, :3, :4],
             camera_type=camera_type,
         )
 
-        cameras.rescale_output_resolution(scaling_factor=1.0 / downscale_factor)
+        cameras.rescale_output_resolution(
+            scaling_factor=1.0 / downscale_factor, scale_rounding_mode=self.config.downscale_rounding_mode
+        )
 
         if "applied_transform" in meta:
             applied_transform = torch.tensor(meta["applied_transform"], dtype=transform_matrix.dtype)
             transform_matrix = transform_matrix @ torch.cat(
                 [applied_transform, torch.tensor([[0, 0, 0, 1]], dtype=transform_matrix.dtype)], 0
             )
         if "applied_scale" in meta:
@@ -448,26 +453,47 @@
                     torch.cat((nxy, torch.full((max_num_points - len(nxy), nxy.shape[-1]), 0, dtype=torch.float32)))
                     / downscale_factor
                 )
             out["points3D_image_ids"] = torch.stack(points3D_image_ids, dim=0)
             out["points3D_points2D_xy"] = torch.stack(points3D_image_xy, dim=0)
         return out
 
-    def _downscale_images(self, paths, get_fname, downscale_factor: int, nearest_neighbor: bool = False):
+    def _downscale_images(
+        self,
+        paths,
+        get_fname,
+        downscale_factor: int,
+        downscale_rounding_mode: str = "floor",
+        nearest_neighbor: bool = False,
+    ):
+        def calculate_scaled_size(original_width, original_height, downscale_factor, mode="floor"):
+            if mode == "floor":
+                return math.floor(original_width / downscale_factor), math.floor(original_height / downscale_factor)
+            elif mode == "round":
+                return round(original_width / downscale_factor), round(original_height / downscale_factor)
+            elif mode == "ceil":
+                return math.ceil(original_width / downscale_factor), math.ceil(original_height / downscale_factor)
+            else:
+                raise ValueError("Invalid mode. Choose from 'floor', 'round', or 'ceil'.")
+
         with status(msg="[bold yellow]Downscaling images...", spinner="growVertical"):
             assert downscale_factor > 1
             assert isinstance(downscale_factor, int)
+            filepath = next(iter(paths))
+            img = Image.open(filepath)
+            w, h = img.size
+            w_scaled, h_scaled = calculate_scaled_size(w, h, downscale_factor, downscale_rounding_mode)
             # Using %05d ffmpeg commands appears to be unreliable (skips images).
             for path in paths:
                 nn_flag = "" if not nearest_neighbor else ":flags=neighbor"
                 path_out = get_fname(path)
                 path_out.parent.mkdir(parents=True, exist_ok=True)
                 ffmpeg_cmd = [
                     f'ffmpeg -y -noautorotate -i "{path}" ',
-                    f"-q:v 2 -vf scale=iw/{downscale_factor}:ih/{downscale_factor}{nn_flag} ",
+                    f"-q:v 2 -vf scale={w_scaled}:{h_scaled}{nn_flag} ",
                     f'"{path_out}"',
                 ]
                 ffmpeg_cmd = " ".join(ffmpeg_cmd)
                 run_command(ffmpeg_cmd)
 
         CONSOLE.log("[bold green]:tada: Done downscaling images.")
 
@@ -484,15 +510,15 @@
             base_part = parent.parent / (str(parent.name) + f"_{self._downscale_factor}")
             return base_part / rel_part
 
         filepath = next(iter(image_filenames))
         if self._downscale_factor is None:
             if self.config.downscale_factor is None:
                 test_img = Image.open(filepath)
-                h, w = test_img.size
+                w, h = test_img.size
                 max_res = max(h, w)
                 df = 0
                 while True:
                     if (max_res / 2 ** (df)) <= MAX_AUTO_RESOLUTION:
                         break
                     df += 1
 
@@ -504,36 +530,43 @@
                 get_fname(self.config.data / self.config.images_path, fp).parent.exists() for fp in image_filenames
             ):
                 # Downscaled images not found
                 # Ask if user wants to downscale the images automatically here
                 CONSOLE.print(
                     f"[bold red]Downscaled images do not exist for factor of {self._downscale_factor}.[/bold red]"
                 )
-                if Confirm.ask("\nWould you like to downscale the images now?", default=False, console=CONSOLE):
+                if Confirm.ask(
+                    f"\nWould you like to downscale the images using '{self.config.downscale_rounding_mode}' rounding mode now?",
+                    default=False,
+                    console=CONSOLE,
+                ):
                     # Install the method
                     self._downscale_images(
                         image_filenames,
                         partial(get_fname, self.config.data / self.config.images_path),
                         self._downscale_factor,
+                        self.config.downscale_rounding_mode,
                         nearest_neighbor=False,
                     )
                     if len(mask_filenames) > 0:
                         assert self.config.masks_path is not None
                         self._downscale_images(
                             mask_filenames,
                             partial(get_fname, self.config.data / self.config.masks_path),
                             self._downscale_factor,
+                            self.config.downscale_rounding_mode,
                             nearest_neighbor=True,
                         )
                     if len(depth_filenames) > 0:
                         assert self.config.depths_path is not None
                         self._downscale_images(
                             depth_filenames,
                             partial(get_fname, self.config.data / self.config.depths_path),
                             self._downscale_factor,
+                            self.config.downscale_rounding_mode,
                             nearest_neighbor=True,
                         )
                 else:
                     sys.exit(1)
 
         # Return transformed filenames
         if self._downscale_factor > 1:
```

### Comparing `nerfstudio-1.0.3/nerfstudio/data/dataparsers/dycheck_dataparser.py` & `nerfstudio-1.1.0/nerfstudio/data/dataparsers/dycheck_dataparser.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/data/dataparsers/instant_ngp_dataparser.py` & `nerfstudio-1.1.0/nerfstudio/data/dataparsers/instant_ngp_dataparser.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/data/dataparsers/minimal_dataparser.py` & `nerfstudio-1.1.0/nerfstudio/data/dataparsers/minimal_dataparser.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/data/dataparsers/nerfosr_dataparser.py` & `nerfstudio-1.1.0/nerfstudio/data/dataparsers/nerfosr_dataparser.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/data/dataparsers/nerfstudio_dataparser.py` & `nerfstudio-1.1.0/nerfstudio/data/dataparsers/nerfstudio_dataparser.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/data/dataparsers/nuscenes_dataparser.py` & `nerfstudio-1.1.0/nerfstudio/data/dataparsers/nuscenes_dataparser.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/data/dataparsers/phototourism_dataparser.py` & `nerfstudio-1.1.0/nerfstudio/data/dataparsers/phototourism_dataparser.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/data/dataparsers/scannet_dataparser.py` & `nerfstudio-1.1.0/nerfstudio/data/dataparsers/scannet_dataparser.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/data/dataparsers/scannetpp_dataparser.py` & `nerfstudio-1.1.0/nerfstudio/data/dataparsers/scannetpp_dataparser.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/data/dataparsers/sdfstudio_dataparser.py` & `nerfstudio-1.1.0/nerfstudio/data/dataparsers/sdfstudio_dataparser.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/data/dataparsers/sitcoms3d_dataparser.py` & `nerfstudio-1.1.0/nerfstudio/data/dataparsers/sitcoms3d_dataparser.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/data/datasets/__init__.py` & `nerfstudio-1.1.0/nerfstudio/data/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/data/datasets/base_dataset.py` & `nerfstudio-1.1.0/nerfstudio/data/datasets/base_dataset.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/data/datasets/depth_dataset.py` & `nerfstudio-1.1.0/nerfstudio/data/datasets/depth_dataset.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/data/datasets/sdf_dataset.py` & `nerfstudio-1.1.0/nerfstudio/data/datasets/sdf_dataset.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/data/datasets/semantic_dataset.py` & `nerfstudio-1.1.0/nerfstudio/data/datasets/semantic_dataset.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/data/pixel_samplers.py` & `nerfstudio-1.1.0/nerfstudio/data/pixel_samplers.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from typing import Dict, Optional, Type, Union
 
 import torch
 from jaxtyping import Int
 from torch import Tensor
 
 from nerfstudio.configs.base_config import InstantiateConfig
-from nerfstudio.data.utils.pixel_sampling_utils import erode_mask
+from nerfstudio.data.utils.pixel_sampling_utils import divide_rays_per_image, erode_mask
 
 
 @dataclass
 class PixelSamplerConfig(InstantiateConfig):
     """Configuration for pixel sampler instantiation."""
 
     _target: Type = field(default_factory=lambda: PixelSampler)
@@ -298,45 +298,37 @@
         num_images = len(batch["image"])
 
         # only sample within the mask, if the mask is in the batch
         all_indices = []
         all_images = []
         all_depth_images = []
 
-        num_rays_in_batch = num_rays_per_batch // num_images
-        if num_rays_in_batch % 2 != 0:
-            num_rays_in_batch += 1
+        assert num_rays_per_batch % 2 == 0, "num_rays_per_batch must be divisible by 2"
+        num_rays_per_image = divide_rays_per_image(num_rays_per_batch, num_images)
 
         if "mask" in batch:
-            for i in range(num_images):
+            for i, num_rays in enumerate(num_rays_per_image):
                 image_height, image_width, _ = batch["image"][i].shape
 
-                if i == num_images - 1:
-                    num_rays_in_batch = num_rays_per_batch - (num_images - 1) * num_rays_in_batch
-
                 indices = self.sample_method(
-                    num_rays_in_batch, 1, image_height, image_width, mask=batch["mask"][i].unsqueeze(0), device=device
+                    num_rays, 1, image_height, image_width, mask=batch["mask"][i].unsqueeze(0), device=device
                 )
                 indices[:, 0] = i
                 all_indices.append(indices)
                 all_images.append(batch["image"][i][indices[:, 1], indices[:, 2]])
                 if "depth_image" in batch:
                     all_depth_images.append(batch["depth_image"][i][indices[:, 1], indices[:, 2]])
 
         else:
-            for i in range(num_images):
+            for i, num_rays in enumerate(num_rays_per_image):
                 image_height, image_width, _ = batch["image"][i].shape
-                if i == num_images - 1:
-                    num_rays_in_batch = num_rays_per_batch - (num_images - 1) * num_rays_in_batch
                 if self.config.is_equirectangular:
-                    indices = self.sample_method_equirectangular(
-                        num_rays_in_batch, 1, image_height, image_width, device=device
-                    )
+                    indices = self.sample_method_equirectangular(num_rays, 1, image_height, image_width, device=device)
                 else:
-                    indices = self.sample_method(num_rays_in_batch, 1, image_height, image_width, device=device)
+                    indices = self.sample_method(num_rays, 1, image_height, image_width, device=device)
                 indices[:, 0] = i
                 all_indices.append(indices)
                 all_images.append(batch["image"][i][indices[:, 1], indices[:, 2]])
                 if "depth_image" in batch:
                     all_depth_images.append(batch["depth_image"][i][indices[:, 1], indices[:, 2]])
 
         indices = torch.cat(all_indices, dim=0)
@@ -400,14 +392,18 @@
 
     Args:
         config: the PatchPixelSamplerConfig used to instantiate class
     """
 
     config: PatchPixelSamplerConfig
 
+    def __init__(self, config: PatchPixelSamplerConfig, **kwargs) -> None:
+        super().__init__(config, **kwargs)
+        self.config.patch_size = self.kwargs.get("patch_size", self.config.patch_size)
+
     def set_num_rays_per_batch(self, num_rays_per_batch: int):
         """Set the number of rays to sample per batch. Overridden to deal with patch-based sampling.
 
         Args:
             num_rays_per_batch: number of rays to sample per batch
         """
         self.num_rays_per_batch = (num_rays_per_batch // (self.config.patch_size**2)) * (self.config.patch_size**2)
```

### Comparing `nerfstudio-1.0.3/nerfstudio/data/scene_box.py` & `nerfstudio-1.1.0/nerfstudio/data/scene_box.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/data/utils/__init__.py` & `nerfstudio-1.1.0/nerfstudio/data/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/data/utils/colmap_parsing_utils.py` & `nerfstudio-1.1.0/nerfstudio/data/utils/colmap_parsing_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/data/utils/data_utils.py` & `nerfstudio-1.1.0/nerfstudio/data/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/data/utils/dataloaders.py` & `nerfstudio-1.1.0/nerfstudio/data/utils/dataloaders.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/data/utils/dataparsers_utils.py` & `nerfstudio-1.1.0/nerfstudio/data/utils/dataparsers_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/data/utils/nerfstudio_collate.py` & `nerfstudio-1.1.0/nerfstudio/data/utils/nerfstudio_collate.py`

 * *Files 4% similar despite different names*

```diff
@@ -151,50 +151,64 @@
         # If a camera, just concatenate along the batch dimension. In the future, this may change to stacking
         assert all((isinstance(cam, Cameras) for cam in batch))
         assert all((cam.distortion_params is None for cam in batch)) or all(
             (cam.distortion_params is not None for cam in batch)
         ), "All cameras must have distortion parameters or none of them should have distortion parameters.\
             Generalized batching will be supported in the future."
 
+        if batch[0].metadata is not None:
+            metadata_keys = batch[0].metadata.keys()
+            assert all(
+                (cam.metadata.keys() == metadata_keys for cam in batch)
+            ), "All cameras must have the same metadata keys."
+        else:
+            assert all((cam.metadata is None for cam in batch)), "All cameras must have the same metadata keys."
+
+        if batch[0].times is not None:
+            assert all((cam.times is not None for cam in batch)), "All cameras must have times present or absent."
+        else:
+            assert all((cam.times is None for cam in batch)), "All cameras must have times present or absent."
+
         # If no batch dimension exists, then we need to stack everything and create a batch dimension on 0th dim
         if elem.shape == ():
             op = torch.stack
         # If batch dimension exists, then we need to concatenate along the 0th dimension
         else:
             op = torch.cat
 
         # Create metadata dictionary
-        metadata_keys = batch[0].metadata.keys()
-        assert all(
-            (cam.metadata.keys() == metadata_keys for cam in batch)
-        ), "All cameras must have the same metadata keys."
-        metadata = {key: op([cam.metadata[key] for cam in batch], dim=0) for key in metadata_keys}
+        if batch[0].metadata is not None:
+            metadata = {key: op([cam.metadata[key] for cam in batch], dim=0) for key in batch[0].metadata.keys()}
+        else:
+            metadata = None
+
+        if batch[0].distortion_params is not None:
+            distortion_params = op(
+                [cameras.distortion_params for cameras in batch],
+                dim=0,
+            )
+        else:
+            distortion_params = None
+
+        if batch[0].times is not None:
+            times = torch.stack([cameras.times for cameras in batch], dim=0)
+        else:
+            times = None
 
         return Cameras(
             op([cameras.camera_to_worlds for cameras in batch], dim=0),
             op([cameras.fx for cameras in batch], dim=0),
             op([cameras.fy for cameras in batch], dim=0),
             op([cameras.cx for cameras in batch], dim=0),
             op([cameras.cy for cameras in batch], dim=0),
             height=op([cameras.height for cameras in batch], dim=0),
             width=op([cameras.width for cameras in batch], dim=0),
-            distortion_params=op(
-                [
-                    cameras.distortion_params
-                    if cameras.distortion_params is not None
-                    else torch.zeros_like(cameras.distortion_params)
-                    for cameras in batch
-                ],
-                dim=0,
-            ),
+            distortion_params=distortion_params,
             camera_type=op([cameras.camera_type for cameras in batch], dim=0),
-            times=torch.stack(
-                [cameras.times if cameras.times is not None else -torch.ones_like(cameras.times) for cameras in batch],
-                dim=0,
-            ),
+            times=times,
             metadata=metadata,
         )
 
     for type_key in extra_mappings:
         if isinstance(elem, type_key):
             return extra_mappings[type_key](batch)
```

### Comparing `nerfstudio-1.0.3/nerfstudio/engine/__init__.py` & `nerfstudio-1.1.0/nerfstudio/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/engine/callbacks.py` & `nerfstudio-1.1.0/nerfstudio/engine/callbacks.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/engine/optimizers.py` & `nerfstudio-1.1.0/nerfstudio/engine/optimizers.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/engine/schedulers.py` & `nerfstudio-1.1.0/nerfstudio/engine/schedulers.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/engine/trainer.py` & `nerfstudio-1.1.0/nerfstudio/engine/trainer.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 from collections import defaultdict
 from dataclasses import dataclass, field
 from pathlib import Path
 from threading import Lock
 from typing import DefaultDict, Dict, List, Literal, Optional, Tuple, Type, cast
 
 import torch
+import viser
 from rich import box, style
 from rich.panel import Panel
 from rich.table import Table
 from torch.cuda.amp.grad_scaler import GradScaler
 
 from nerfstudio.configs.experiment_config import ExperimentConfig
 from nerfstudio.engine.callbacks import TrainingCallback, TrainingCallbackAttributes, TrainingCallbackLocation
@@ -133,14 +134,17 @@
         self.base_dir: Path = config.get_base_dir()
         # directory to save checkpoints
         self.checkpoint_dir: Path = config.get_checkpoint_dir()
         CONSOLE.log(f"Saving checkpoints to: {self.checkpoint_dir}")
 
         self.viewer_state = None
 
+        # used to keep track of the current step
+        self.step = 0
+
     def setup(self, test_mode: Literal["test", "val", "inference"] = "val") -> None:
         """Setup the Trainer by calling other setup functions.
 
         Args:
             test_mode:
                 'val': loads train/val datasets into memory
                 'test': loads train/test datasets into memory
@@ -229,16 +233,23 @@
             self.base_dir / "dataparser_transforms.json"
         )
 
         self._init_viewer_state()
         with TimeWriter(writer, EventName.TOTAL_TRAIN_TIME):
             num_iterations = self.config.max_num_iterations
             step = 0
+            self.stop_training = False
             for step in range(self._start_step, self._start_step + num_iterations):
+                self.step = step
+                if self.stop_training:
+                    break
                 while self.training_state == "paused":
+                    if self.stop_training:
+                        self._after_train()
+                        return
                     time.sleep(0.01)
                 with self.train_lock:
                     with TimeWriter(writer, EventName.ITER_TRAIN_TIME, step=step) as train_t:
                         self.pipeline.train()
 
                         # training callbacks before the training iteration
                         for callback in self.callbacks:
@@ -287,33 +298,47 @@
                     self.eval_iteration(step)
 
                 if step_check(step, self.config.steps_per_save):
                     self.save_checkpoint(step)
 
                 writer.write_out_storage()
 
-        # save checkpoint at the end of training
-        self.save_checkpoint(step)
+        # save checkpoint at the end of training, and write out any remaining events
+        self._after_train()
 
+    def shutdown(self) -> None:
+        """Stop the trainer and stop all associated threads/processes (such as the viewer)."""
+        self.stop_training = True  # tell the training loop to stop
+        if self.viewer_state is not None:
+            # stop the viewer
+            # this condition excludes the case where `viser_server` is either `None` or an
+            # instance of `viewer_legacy`'s `ViserServer` instead of the upstream one.
+            if isinstance(self.viewer_state.viser_server, viser.ViserServer):
+                self.viewer_state.viser_server.stop()
+
+    def _after_train(self) -> None:
+        """Function to run after training is complete"""
+        self.training_state = "completed"  # used to update the webui state
+        # save checkpoint at the end of training
+        self.save_checkpoint(self.step)
         # write out any remaining events (e.g., total train time)
         writer.write_out_storage()
-
         table = Table(
             title=None,
             show_header=False,
             box=box.MINIMAL,
             title_style=style.Style(bold=True),
         )
         table.add_row("Config File", str(self.config.get_base_dir() / "config.yml"))
         table.add_row("Checkpoint Directory", str(self.checkpoint_dir))
         CONSOLE.print(Panel(table, title="[bold][green]:tada: Training Finished :tada:[/bold]", expand=False))
 
         # after train end callbacks
         for callback in self.callbacks:
-            callback.run_callback_at_location(step=step, location=TrainingCallbackLocation.AFTER_TRAIN)
+            callback.run_callback_at_location(step=self.step, location=TrainingCallbackLocation.AFTER_TRAIN)
 
         if not self.config.viewer.quit_on_train_completion:
             self._train_complete_viewer()
 
     @check_main_thread
     def _check_viewer_warnings(self) -> None:
         """Helper to print out any warnings regarding the way the viewer/loggers are enabled"""
```

### Comparing `nerfstudio-1.0.3/nerfstudio/exporter/__init__.py` & `nerfstudio-1.1.0/nerfstudio/exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/exporter/exporter_utils.py` & `nerfstudio-1.1.0/nerfstudio/exporter/exporter_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -85,34 +85,28 @@
     num_points: int = 1000000,
     remove_outliers: bool = True,
     estimate_normals: bool = False,
     reorient_normals: bool = False,
     rgb_output_name: str = "rgb",
     depth_output_name: str = "depth",
     normal_output_name: Optional[str] = None,
-    use_bounding_box: bool = True,
-    bounding_box_min: Optional[Tuple[float, float, float]] = None,
-    bounding_box_max: Optional[Tuple[float, float, float]] = None,
     crop_obb: Optional[OrientedBox] = None,
     std_ratio: float = 10.0,
 ) -> o3d.geometry.PointCloud:
     """Generate a point cloud from a nerf.
 
     Args:
         pipeline: Pipeline to evaluate with.
         num_points: Number of points to generate. May result in less if outlier removal is used.
         remove_outliers: Whether to remove outliers.
         reorient_normals: Whether to re-orient the normals based on the view direction.
         estimate_normals: Whether to estimate normals.
         rgb_output_name: Name of the RGB output.
         depth_output_name: Name of the depth output.
         normal_output_name: Name of the normal output.
-        use_bounding_box: Whether to use a bounding box to sample points.
-        bounding_box_min: Minimum of the bounding box.
-        bounding_box_max: Maximum of the bounding box.
         std_ratio: Threshold based on STD of the average distances across the point cloud to remove outliers.
 
     Returns:
         Point cloud.
     """
 
     progress = Progress(
@@ -122,16 +116,14 @@
         TimeRemainingColumn(elapsed_when_finished=True, compact=True),
         console=CONSOLE,
     )
     points = []
     rgbs = []
     normals = []
     view_directions = []
-    if use_bounding_box and (crop_obb is not None and bounding_box_max is not None):
-        CONSOLE.print("Provided aabb and crop_obb at the same time, using only the obb", style="bold yellow")
     with progress as progress_bar:
         task = progress_bar.add_task("Generating Point Cloud", total=num_points)
         while not progress_bar.finished:
             normal = None
 
             with torch.no_grad():
                 ray_bundle, _ = pipeline.datamanager.next_train(0)
@@ -167,29 +159,21 @@
             mask = rgba[..., -1] > 0.5
             point = point[mask]
             view_direction = view_direction[mask]
             rgb = rgba[mask][..., :3]
             if normal is not None:
                 normal = normal[mask]
 
-            if use_bounding_box:
-                if crop_obb is None:
-                    comp_l = torch.tensor(bounding_box_min, device=point.device)
-                    comp_m = torch.tensor(bounding_box_max, device=point.device)
-                    assert torch.all(
-                        comp_l < comp_m
-                    ), f"Bounding box min {bounding_box_min} must be smaller than max {bounding_box_max}"
-                    mask = torch.all(torch.concat([point > comp_l, point < comp_m], dim=-1), dim=-1)
-                else:
-                    mask = crop_obb.within(point)
-                point = point[mask]
-                rgb = rgb[mask]
-                view_direction = view_direction[mask]
-                if normal is not None:
-                    normal = normal[mask]
+            if crop_obb is not None:
+                mask = crop_obb.within(point)
+            point = point[mask]
+            rgb = rgb[mask]
+            view_direction = view_direction[mask]
+            if normal is not None:
+                normal = normal[mask]
 
             points.append(point)
             rgbs.append(rgb)
             view_directions.append(view_direction)
             if normal is not None:
                 normals.append(normal)
             progress.advance(task, point.shape[0])
```

### Comparing `nerfstudio-1.0.3/nerfstudio/exporter/marching_cubes.py` & `nerfstudio-1.1.0/nerfstudio/exporter/marching_cubes.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/exporter/texture_utils.py` & `nerfstudio-1.1.0/nerfstudio/exporter/texture_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/exporter/tsdf_utils.py` & `nerfstudio-1.1.0/nerfstudio/exporter/tsdf_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/field_components/__init__.py` & `nerfstudio-1.1.0/nerfstudio/field_components/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/field_components/activations.py` & `nerfstudio-1.1.0/nerfstudio/field_components/activations.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/field_components/base_field_component.py` & `nerfstudio-1.1.0/nerfstudio/field_components/base_field_component.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/field_components/embedding.py` & `nerfstudio-1.1.0/nerfstudio/field_components/embedding.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/field_components/encodings.py` & `nerfstudio-1.1.0/nerfstudio/field_components/encodings.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/field_components/field_heads.py` & `nerfstudio-1.1.0/nerfstudio/field_components/field_heads.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/field_components/mlp.py` & `nerfstudio-1.1.0/nerfstudio/field_components/mlp.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/field_components/spatial_distortions.py` & `nerfstudio-1.1.0/nerfstudio/field_components/spatial_distortions.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/field_components/temporal_distortions.py` & `nerfstudio-1.1.0/nerfstudio/field_components/temporal_distortions.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/fields/__init__.py` & `nerfstudio-1.1.0/nerfstudio/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/fields/base_field.py` & `nerfstudio-1.1.0/nerfstudio/fields/base_field.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/fields/density_fields.py` & `nerfstudio-1.1.0/nerfstudio/fields/density_fields.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/fields/generfacto_field.py` & `nerfstudio-1.1.0/nerfstudio/fields/generfacto_field.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/fields/nerfacto_field.py` & `nerfstudio-1.1.0/nerfstudio/fields/nerfacto_field.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/fields/nerfw_field.py` & `nerfstudio-1.1.0/nerfstudio/fields/nerfw_field.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/fields/sdf_field.py` & `nerfstudio-1.1.0/nerfstudio/fields/sdf_field.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/fields/semantic_nerf_field.py` & `nerfstudio-1.1.0/nerfstudio/fields/semantic_nerf_field.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/fields/tensorf_field.py` & `nerfstudio-1.1.0/nerfstudio/fields/tensorf_field.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/fields/vanilla_nerf_field.py` & `nerfstudio-1.1.0/nerfstudio/fields/vanilla_nerf_field.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/generative/__init__.py` & `nerfstudio-1.1.0/nerfstudio/generative/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/generative/deepfloyd.py` & `nerfstudio-1.1.0/nerfstudio/generative/deepfloyd.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/generative/positional_text_embeddings.py` & `nerfstudio-1.1.0/nerfstudio/generative/positional_text_embeddings.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/generative/stable_diffusion.py` & `nerfstudio-1.1.0/nerfstudio/generative/stable_diffusion.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/model_components/__init__.py` & `nerfstudio-1.1.0/nerfstudio/model_components/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/model_components/losses.py` & `nerfstudio-1.1.0/nerfstudio/model_components/losses.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/model_components/ray_generators.py` & `nerfstudio-1.1.0/nerfstudio/model_components/ray_generators.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/model_components/ray_samplers.py` & `nerfstudio-1.1.0/nerfstudio/model_components/ray_samplers.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/model_components/renderers.py` & `nerfstudio-1.1.0/nerfstudio/model_components/renderers.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/model_components/scene_colliders.py` & `nerfstudio-1.1.0/nerfstudio/model_components/scene_colliders.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/model_components/shaders.py` & `nerfstudio-1.1.0/nerfstudio/model_components/shaders.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/models/__init__.py` & `nerfstudio-1.1.0/nerfstudio/models/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/models/base_model.py` & `nerfstudio-1.1.0/nerfstudio/models/base_model.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/models/base_surface_model.py` & `nerfstudio-1.1.0/nerfstudio/models/base_surface_model.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/models/depth_nerfacto.py` & `nerfstudio-1.1.0/nerfstudio/models/depth_nerfacto.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/models/generfacto.py` & `nerfstudio-1.1.0/nerfstudio/models/generfacto.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/models/instant_ngp.py` & `nerfstudio-1.1.0/nerfstudio/models/instant_ngp.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/models/mipnerf.py` & `nerfstudio-1.1.0/nerfstudio/models/mipnerf.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/models/nerfacto.py` & `nerfstudio-1.1.0/nerfstudio/models/nerfacto.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/models/neus.py` & `nerfstudio-1.1.0/nerfstudio/models/neus.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/models/neus_facto.py` & `nerfstudio-1.1.0/nerfstudio/models/neus_facto.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/models/semantic_nerfw.py` & `nerfstudio-1.1.0/nerfstudio/models/semantic_nerfw.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/models/splatfacto.py` & `nerfstudio-1.1.0/nerfstudio/models/splatfacto.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 from gsplat.project_gaussians import project_gaussians
 from gsplat.rasterize import rasterize_gaussians
 from gsplat.sh import num_sh_bases, spherical_harmonics
 from pytorch_msssim import SSIM
 from torch.nn import Parameter
 from typing_extensions import Literal
 
+from nerfstudio.cameras.camera_optimizers import CameraOptimizer, CameraOptimizerConfig
 from nerfstudio.cameras.cameras import Cameras
 from nerfstudio.data.scene_box import OrientedBox
 from nerfstudio.engine.callbacks import TrainingCallback, TrainingCallbackAttributes, TrainingCallbackLocation
 from nerfstudio.engine.optimizers import Optimizers
 
 # need following import for background color override
 from nerfstudio.model_components import renderers
@@ -75,14 +76,29 @@
     """
     Converts from the 0th spherical harmonic coefficient to RGB values [0,1]
     """
     C0 = 0.28209479177387814
     return sh * C0 + 0.5
 
 
+def resize_image(image: torch.Tensor, d: int):
+    """
+    Downscale images using the same 'area' method in opencv
+
+    :param image shape [H, W, C]
+    :param d downscale factor (must be 2, 4, 8, etc.)
+
+    return downscaled image in shape [H//d, W//d, C]
+    """
+    import torch.nn.functional as tf
+
+    weight = (1.0 / (d * d)) * torch.ones((1, 1, d, d), dtype=torch.float32, device=image.device)
+    return tf.conv2d(image.permute(2, 0, 1)[:, None, ...], weight, stride=d).squeeze(1).permute(1, 2, 0)
+
+
 @dataclass
 class SplatfactoModelConfig(ModelConfig):
     """Splatfacto Model Config, nerfstudio's implementation of Gaussian Splatting"""
 
     _target: Type = field(default_factory=lambda: SplatfactoModel)
     warmup_length: int = 500
     """period of steps where refinement is turned off"""
@@ -98,15 +114,15 @@
     """threshold of opacity for culling gaussians. One can set it to a lower value (e.g. 0.005) for higher quality."""
     cull_scale_thresh: float = 0.5
     """threshold of scale for culling huge gaussians"""
     continue_cull_post_densification: bool = True
     """If True, continue to cull gaussians post refinement"""
     reset_alpha_every: int = 30
     """Every this many refinement steps, reset the alpha"""
-    densify_grad_thresh: float = 0.0002
+    densify_grad_thresh: float = 0.0008
     """threshold of positional gradient norm for densifying gaussians"""
     densify_size_thresh: float = 0.01
     """below this size, gaussians are *duplicated*, otherwise split"""
     n_split_samples: int = 2
     """number of samples to split gaussians into"""
     sh_degree_interval: int = 1000
     """every n intervals turn on another sh degree"""
@@ -142,14 +158,16 @@
     approach is however not suitable to render tiny gaussians at higher or lower resolution than the captured, which
     results "aliasing-like" artifacts. The antialiased mode overcomes this limitation by calculating compensation factors
     and apply them to the opacities of gaussians to preserve the total integrated density of splats.
 
     However, PLY exported with antialiased rasterize mode is not compatible with classic mode. Thus many web viewers that
     were implemented for classic mode can not render antialiased mode PLY properly without modifications.
     """
+    camera_optimizer: CameraOptimizerConfig = field(default_factory=lambda: CameraOptimizerConfig(mode="off"))
+    """Config of the camera optimizer to use"""
 
 
 class SplatfactoModel(Model):
     """Nerfstudio's implementation of Gaussian Splatting
 
     Args:
         config: Splatfacto configuration to instantiate model
@@ -209,14 +227,18 @@
                 "quats": quats,
                 "features_dc": features_dc,
                 "features_rest": features_rest,
                 "opacities": opacities,
             }
         )
 
+        self.camera_optimizer: CameraOptimizer = self.config.camera_optimizer.setup(
+            num_cameras=self.num_train_data, device="cpu"
+        )
+
         # metrics
         from torchmetrics.image import PeakSignalNoiseRatio
         from torchmetrics.image.lpip import LearnedPerceptualImagePatchSimilarity
 
         self.psnr = PeakSignalNoiseRatio(data_range=1.0)
         self.ssim = SSIM(data_range=1.0, size_average=True, channel=3)
         self.lpips = LearnedPerceptualImagePatchSimilarity(normalize=True)
@@ -368,16 +390,16 @@
         assert step == self.step
         # to save some training time, we no longer need to update those stats post refinement
         if self.step >= self.config.stop_split_at:
             return
         with torch.no_grad():
             # keep track of a moving average of grad norms
             visible_mask = (self.radii > 0).flatten()
-            assert self.xys.grad is not None
-            grads = self.xys.grad.detach().norm(dim=-1)
+            assert self.xys.absgrad is not None  # type: ignore
+            grads = self.xys.absgrad.detach().norm(dim=-1)  # type: ignore
             # print(f"grad norm min {grads.min().item()} max {grads.max().item()} mean {grads.mean().item()} size {grads.shape}")
             if self.xys_grad_norm is None:
                 self.xys_grad_norm = grads
                 self.vis_counts = torch.ones_like(self.xys_grad_norm)
             else:
                 assert self.vis_counts is not None
                 self.vis_counts[visible_mask] = self.vis_counts[visible_mask] + 1
@@ -605,36 +627,39 @@
     def get_param_groups(self) -> Dict[str, List[Parameter]]:
         """Obtain the parameter groups for the optimizers
 
         Returns:
             Mapping of different parameter groups
         """
         gps = self.get_gaussian_param_groups()
+        self.camera_optimizer.get_param_groups(param_groups=gps)
         return gps
 
     def _get_downscale_factor(self):
         if self.training:
             return 2 ** max(
                 (self.config.num_downscales - self.step // self.config.resolution_schedule),
                 0,
             )
         else:
             return 1
 
     def _downscale_if_required(self, image):
         d = self._get_downscale_factor()
         if d > 1:
-            newsize = [image.shape[0] // d, image.shape[1] // d]
-
-            # torchvision can be slow to import, so we do it lazily.
-            import torchvision.transforms.functional as TF
-
-            return TF.resize(image.permute(2, 0, 1), newsize, antialias=None).permute(1, 2, 0)
+            return resize_image(image, d)
         return image
 
+    @staticmethod
+    def get_empty_outputs(width: int, height: int, background: torch.Tensor) -> Dict[str, Union[torch.Tensor, List]]:
+        rgb = background.repeat(height, width, 1)
+        depth = background.new_ones(*rgb.shape[:2], 1) * 10
+        accumulation = background.new_zeros(*rgb.shape[:2], 1)
+        return {"rgb": rgb, "depth": depth, "accumulation": accumulation, "background": background}
+
     def get_outputs(self, camera: Cameras) -> Dict[str, Union[torch.Tensor, List]]:
         """Takes in a Ray Bundle and returns a dictionary of outputs.
 
         Args:
             ray_bundle: Input bundle of rays. This raybundle should have all the
             needed information to compute the outputs.
 
@@ -644,42 +669,44 @@
         if not isinstance(camera, Cameras):
             print("Called get_outputs with not a camera")
             return {}
         assert camera.shape[0] == 1, "Only one camera at a time"
 
         # get the background color
         if self.training:
+            optimized_camera_to_world = self.camera_optimizer.apply_to_camera(camera)[0, ...]
+
             if self.config.background_color == "random":
                 background = torch.rand(3, device=self.device)
             elif self.config.background_color == "white":
                 background = torch.ones(3, device=self.device)
             elif self.config.background_color == "black":
                 background = torch.zeros(3, device=self.device)
             else:
                 background = self.background_color.to(self.device)
         else:
+            optimized_camera_to_world = camera.camera_to_worlds[0, ...]
+
             if renderers.BACKGROUND_COLOR_OVERRIDE is not None:
                 background = renderers.BACKGROUND_COLOR_OVERRIDE.to(self.device)
             else:
                 background = self.background_color.to(self.device)
 
         if self.crop_box is not None and not self.training:
             crop_ids = self.crop_box.within(self.means).squeeze()
             if crop_ids.sum() == 0:
-                rgb = background.repeat(int(camera.height.item()), int(camera.width.item()), 1)
-                depth = background.new_ones(*rgb.shape[:2], 1) * 10
-                accumulation = background.new_zeros(*rgb.shape[:2], 1)
-                return {"rgb": rgb, "depth": depth, "accumulation": accumulation, "background": background}
+                return self.get_empty_outputs(int(camera.width.item()), int(camera.height.item()), background)
         else:
             crop_ids = None
         camera_downscale = self._get_downscale_factor()
         camera.rescale_output_resolution(1 / camera_downscale)
         # shift the camera to center of scene looking at center
-        R = camera.camera_to_worlds[0, :3, :3]  # 3 x 3
-        T = camera.camera_to_worlds[0, :3, 3:4]  # 3 x 1
+        R = optimized_camera_to_world[:3, :3]  # 3 x 3
+        T = optimized_camera_to_world[:3, 3:4]  # 3 x 1
+
         # flip the z and y axes to align with gsplat conventions
         R_edit = torch.diag(torch.tensor([1, -1, -1], device=self.device, dtype=R.dtype))
         R = R @ R_edit
         # analytic matrix inverse to get world2camera matrix
         R_inv = R.T
         T_inv = -R_inv @ T
         viewmat = torch.eye(4, device=R.device, dtype=R.dtype)
@@ -723,37 +750,27 @@
             BLOCK_WIDTH,
         )  # type: ignore
 
         # rescale the camera back to original dimensions before returning
         camera.rescale_output_resolution(camera_downscale)
 
         if (self.radii).sum() == 0:
-            rgb = background.repeat(H, W, 1)
-            depth = background.new_ones(*rgb.shape[:2], 1) * 10
-            accumulation = background.new_zeros(*rgb.shape[:2], 1)
-
-            return {"rgb": rgb, "depth": depth, "accumulation": accumulation, "background": background}
-
-        # Important to allow xys grads to populate properly
-        if self.training:
-            self.xys.retain_grad()
+            return self.get_empty_outputs(W, H, background)
 
         if self.config.sh_degree > 0:
-            viewdirs = means_crop.detach() - camera.camera_to_worlds.detach()[..., :3, 3]  # (N, 3)
-            viewdirs = viewdirs / viewdirs.norm(dim=-1, keepdim=True)
+            viewdirs = means_crop.detach() - optimized_camera_to_world.detach()[:3, 3]  # (N, 3)
             n = min(self.step // self.config.sh_degree_interval, self.config.sh_degree)
-            rgbs = spherical_harmonics(n, viewdirs, colors_crop)
+            rgbs = spherical_harmonics(n, viewdirs, colors_crop)  # input unnormalized viewdirs
             rgbs = torch.clamp(rgbs + 0.5, min=0.0)  # type: ignore
         else:
             rgbs = torch.sigmoid(colors_crop[:, 0, :])
 
         assert (num_tiles_hit > 0).any()  # type: ignore
 
         # apply the compensation of screen space blurring to gaussians
-        opacities = None
         if self.config.rasterize_mode == "antialiased":
             opacities = torch.sigmoid(opacities_crop) * comp[:, None]
         elif self.config.rasterize_mode == "classic":
             opacities = torch.sigmoid(opacities_crop)
         else:
             raise ValueError("Unknown rasterize_mode: %s", self.config.rasterize_mode)
 
@@ -825,14 +842,16 @@
         """
         gt_rgb = self.composite_with_background(self.get_gt_img(batch["image"]), outputs["background"])
         metrics_dict = {}
         predicted_rgb = outputs["rgb"]
         metrics_dict["psnr"] = self.psnr(predicted_rgb, gt_rgb)
 
         metrics_dict["gaussian_count"] = self.num_points
+
+        self.camera_optimizer.get_metrics_dict(metrics_dict)
         return metrics_dict
 
     def get_loss_dict(self, outputs, batch, metrics_dict=None) -> Dict[str, torch.Tensor]:
         """Computes and returns the losses dict.
 
         Args:
             outputs: the output to compute loss dict to
@@ -863,19 +882,25 @@
                 )
                 - self.config.max_gauss_ratio
             )
             scale_reg = 0.1 * scale_reg.mean()
         else:
             scale_reg = torch.tensor(0.0).to(self.device)
 
-        return {
+        loss_dict = {
             "main_loss": (1 - self.config.ssim_lambda) * Ll1 + self.config.ssim_lambda * simloss,
             "scale_reg": scale_reg,
         }
 
+        if self.training:
+            # Add loss from camera optimizer
+            self.camera_optimizer.get_loss_dict(loss_dict)
+
+        return loss_dict
+
     @torch.no_grad()
     def get_outputs_for_camera(self, camera: Cameras, obb_box: Optional[OrientedBox] = None) -> Dict[str, torch.Tensor]:
         """Takes in a camera, generates the raybundle, and computes the output of the model.
         Overridden for a camera-based gaussian model.
 
         Args:
             camera: generates raybundle
@@ -896,23 +921,15 @@
             batch: Batch of data.
             outputs: Outputs of the model.
 
         Returns:
             A dictionary of metrics.
         """
         gt_rgb = self.composite_with_background(self.get_gt_img(batch["image"]), outputs["background"])
-        d = self._get_downscale_factor()
-        if d > 1:
-            # torchvision can be slow to import, so we do it lazily.
-            import torchvision.transforms.functional as TF
-
-            newsize = [batch["image"].shape[0] // d, batch["image"].shape[1] // d]
-            predicted_rgb = TF.resize(outputs["rgb"].permute(2, 0, 1), newsize, antialias=None).permute(1, 2, 0)
-        else:
-            predicted_rgb = outputs["rgb"]
+        predicted_rgb = outputs["rgb"]
 
         combined_rgb = torch.cat([gt_rgb, predicted_rgb], dim=1)
 
         # Switch images from [H, W, C] to [1, C, H, W] for metrics computations
         gt_rgb = torch.moveaxis(gt_rgb, -1, 0)[None, ...]
         predicted_rgb = torch.moveaxis(predicted_rgb, -1, 0)[None, ...]
```

### Comparing `nerfstudio-1.0.3/nerfstudio/models/tensorf.py` & `nerfstudio-1.1.0/nerfstudio/models/tensorf.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/models/vanilla_nerf.py` & `nerfstudio-1.1.0/nerfstudio/models/vanilla_nerf.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/pipelines/__init__.py` & `nerfstudio-1.1.0/nerfstudio/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/pipelines/base_pipeline.py` & `nerfstudio-1.1.0/nerfstudio/pipelines/base_pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from dataclasses import dataclass, field
 from pathlib import Path
 from time import time
 from typing import Any, Dict, List, Literal, Mapping, Optional, Tuple, Type, Union, cast
 
 import torch
 import torch.distributed as dist
+import torchvision.utils as vutils
 from rich.progress import BarColumn, MofNCompleteColumn, Progress, TextColumn, TimeElapsedColumn
 from torch import nn
 from torch.cuda.amp.grad_scaler import GradScaler
 from torch.nn import Parameter
 from torch.nn.parallel import DistributedDataParallel as DDP
 
 from nerfstudio.configs.base_config import InstantiateConfig
@@ -357,39 +358,45 @@
         Returns:
             metrics_dict: dictionary of metrics
         """
         self.eval()
         metrics_dict_list = []
         assert isinstance(self.datamanager, (VanillaDataManager, ParallelDataManager, FullImageDatamanager))
         num_images = len(self.datamanager.fixed_indices_eval_dataloader)
+        if output_path is not None:
+            output_path.mkdir(exist_ok=True, parents=True)
         with Progress(
             TextColumn("[progress.description]{task.description}"),
             BarColumn(),
             TimeElapsedColumn(),
             MofNCompleteColumn(),
             transient=True,
         ) as progress:
             task = progress.add_task("[green]Evaluating all eval images...", total=num_images)
+            idx = 0
             for camera, batch in self.datamanager.fixed_indices_eval_dataloader:
                 # time this the following line
                 inner_start = time()
                 outputs = self.model.get_outputs_for_camera(camera=camera)
                 height, width = camera.height, camera.width
                 num_rays = height * width
-                metrics_dict, _ = self.model.get_image_metrics_and_images(outputs, batch)
+                metrics_dict, image_dict = self.model.get_image_metrics_and_images(outputs, batch)
                 if output_path is not None:
-                    raise NotImplementedError("Saving images is not implemented yet")
+                    for key in image_dict.keys():
+                        image = image_dict[key]  # [H, W, C] order
+                        vutils.save_image(image.permute(2, 0, 1).cpu(), output_path / f"eval_{key}_{idx:04d}.png")
 
                 assert "num_rays_per_sec" not in metrics_dict
                 metrics_dict["num_rays_per_sec"] = (num_rays / (time() - inner_start)).item()
                 fps_str = "fps"
                 assert fps_str not in metrics_dict
                 metrics_dict[fps_str] = (metrics_dict["num_rays_per_sec"] / (height * width)).item()
                 metrics_dict_list.append(metrics_dict)
                 progress.advance(task)
+                idx = idx + 1
         # average the metrics list
         metrics_dict = {}
         for key in metrics_dict_list[0].keys():
             if get_std:
                 key_std, key_mean = torch.std_mean(
                     torch.tensor([metrics_dict[key] for metrics_dict in metrics_dict_list])
                 )
```

### Comparing `nerfstudio-1.0.3/nerfstudio/pipelines/dynamic_batch.py` & `nerfstudio-1.1.0/nerfstudio/pipelines/dynamic_batch.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/plugins/__init__.py` & `nerfstudio-1.1.0/nerfstudio/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/plugins/registry.py` & `nerfstudio-1.1.0/nerfstudio/plugins/registry.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/plugins/registry_dataparser.py` & `nerfstudio-1.1.0/nerfstudio/plugins/registry_dataparser.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/plugins/types.py` & `nerfstudio-1.1.0/nerfstudio/plugins/types.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/process_data/__init__.py` & `nerfstudio-1.1.0/nerfstudio/process_data/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/process_data/base_converter_to_nerfstudio_dataset.py` & `nerfstudio-1.1.0/nerfstudio/process_data/base_converter_to_nerfstudio_dataset.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/process_data/colmap_converter_to_nerfstudio_dataset.py` & `nerfstudio-1.1.0/nerfstudio/process_data/colmap_converter_to_nerfstudio_dataset.py`

 * *Files 5% similar despite different names*

```diff
@@ -97,14 +97,17 @@
     """If True, use GPU."""
     use_sfm_depth: bool = False
     """If True, export and use depth maps induced from SfM points."""
     include_depth_debug: bool = False
     """If --use-sfm-depth and this flag is True, also export debug images showing Sf overlaid upon input images."""
     same_dimensions: bool = True
     """Whether to assume all images are same dimensions and so to use fast downscaling with no autorotation."""
+    use_single_camera_mode: bool = True
+    """Whether to assume all images taken with the same camera characteristics, set to False for multiple cameras in colmap (only works with hloc sfm_tool).
+    """
 
     @staticmethod
     def default_colmap_path() -> Path:
         return Path("colmap/sparse/0")
 
     @property
     def absolute_colmap_model_path(self) -> Path:
@@ -132,14 +135,15 @@
             with CONSOLE.status("[bold yellow]Saving results to transforms.json", spinner="balloon"):
                 num_matched_frames = colmap_utils.colmap_to_json(
                     recon_dir=self.absolute_colmap_model_path,
                     output_dir=self.output_dir,
                     image_id_to_depth_path=image_id_to_depth_path,
                     camera_mask_path=camera_mask_path,
                     image_rename_map=image_rename_map,
+                    use_single_camera_mode=self.use_single_camera_mode,
                 )
                 summary_log.append(f"Colmap matched {num_matched_frames} images")
             summary_log.append(colmap_utils.get_matching_summary(num_frames, num_matched_frames))
 
         else:
             CONSOLE.log(
                 "[bold yellow]Warning: Could not find existing COLMAP results. " "Not generating transforms.json"
@@ -190,14 +194,18 @@
         ) = process_data_utils.find_tool_feature_matcher_combination(
             self.sfm_tool, self.feature_type, self.matcher_type
         )
         # check that sfm_tool is hloc if using refine_pixsfm
         if self.refine_pixsfm:
             assert sfm_tool == "hloc", "refine_pixsfm only works with sfm_tool hloc"
 
+        # check that sfm_tool is hloc if using use_single_camera_mode
+        if not self.use_single_camera_mode:
+            assert sfm_tool == "hloc", "not_use_single_camera_mode only works with sfm_tool hloc"
+
         # set the image_dir if didn't copy
         if self.skip_image_processing:
             image_dir = self.data
         else:
             image_dir = self.image_dir
 
         if sfm_tool == "colmap":
@@ -224,14 +232,15 @@
                 colmap_dir=self.absolute_colmap_path,
                 camera_model=CAMERA_MODELS[self.camera_type],
                 verbose=self.verbose,
                 matching_method=self.matching_method,
                 feature_type=feature_type,
                 matcher_type=matcher_type,
                 refine_pixsfm=self.refine_pixsfm,
+                use_single_camera_mode=self.use_single_camera_mode,
             )
         else:
             raise RuntimeError("Invalid combination of sfm_tool, feature_type, and matcher_type, " "exiting")
 
     def __post_init__(self) -> None:
         super().__post_init__()
         install_checks.check_ffmpeg_installed()
```

### Comparing `nerfstudio-1.0.3/nerfstudio/process_data/colmap_utils.py` & `nerfstudio-1.1.0/nerfstudio/process_data/colmap_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -391,14 +391,15 @@
     recon_dir: Path,
     output_dir: Path,
     camera_mask_path: Optional[Path] = None,
     image_id_to_depth_path: Optional[Dict[int, Path]] = None,
     image_rename_map: Optional[Dict[str, str]] = None,
     ply_filename="sparse_pc.ply",
     keep_original_world_coordinate: bool = False,
+    use_single_camera_mode: bool = True,
 ) -> int:
     """Converts COLMAP's cameras.bin and images.bin to a JSON file.
 
     Args:
         recon_dir: Path to the reconstruction directory, e.g. "sparse/0"
         output_dir: Path to the output directory.
         camera_model: Camera model used.
@@ -414,14 +415,21 @@
 
     # TODO(1480) use pycolmap
     # recon = pycolmap.Reconstruction(recon_dir)
     # cam_id_to_camera = recon.cameras
     # im_id_to_image = recon.images
     cam_id_to_camera = read_cameras_binary(recon_dir / "cameras.bin")
     im_id_to_image = read_images_binary(recon_dir / "images.bin")
+    if set(cam_id_to_camera.keys()) != {1}:
+        CONSOLE.print(f"[bold yellow]Warning: More than one camera is found in {recon_dir}")
+        print(cam_id_to_camera)
+        use_single_camera_mode = False  # update bool: one camera per frame
+        out = {}  # out = {"camera_model": parse_colmap_camera_params(cam_id_to_camera[1])["camera_model"]}
+    else:  # one camera for all frames
+        out = parse_colmap_camera_params(cam_id_to_camera[1])
 
     frames = []
     for im_id, im_data in im_id_to_image.items():
         # NB: COLMAP uses Eigen / scalar-first quaternions
         # * https://colmap.github.io/format.html
         # * https://github.com/colmap/colmap/blob/bf3e19140f491c3042bfd85b7192ef7d249808ec/src/base/pose.cc#L75
         # the `rotation_matrix()` handles that format for us.
@@ -451,19 +459,20 @@
             "colmap_im_id": im_id,
         }
         if camera_mask_path is not None:
             frame["mask_path"] = camera_mask_path.relative_to(camera_mask_path.parent.parent).as_posix()
         if image_id_to_depth_path is not None:
             depth_path = image_id_to_depth_path[im_id]
             frame["depth_file_path"] = str(depth_path.relative_to(depth_path.parent.parent))
+
+        if not use_single_camera_mode:  # add the camera parameters for this frame
+            frame.update(parse_colmap_camera_params(cam_id_to_camera[im_data.camera_id]))
+
         frames.append(frame)
 
-    if set(cam_id_to_camera.keys()) != {1}:
-        raise RuntimeError("Only single camera shared for all images is supported.")
-    out = parse_colmap_camera_params(cam_id_to_camera[1])
     out["frames"] = frames
 
     applied_transform = None
     if not keep_original_world_coordinate:
         applied_transform = np.eye(4)[:3, :]
         applied_transform = applied_transform[np.array([0, 2, 1]), :]
         applied_transform[2, :] *= -1
```

### Comparing `nerfstudio-1.0.3/nerfstudio/process_data/equirect_utils.py` & `nerfstudio-1.1.0/nerfstudio/process_data/equirect_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/process_data/hloc_utils.py` & `nerfstudio-1.1.0/nerfstudio/process_data/hloc_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -67,28 +67,30 @@
         "NN-mutual",
         "adalam",
         "disk+lightglue",
         "superpoint+lightglue",
     ] = "superglue",
     num_matched: int = 50,
     refine_pixsfm: bool = False,
+    use_single_camera_mode: bool = True,
 ) -> None:
     """Runs hloc on the images.
 
     Args:
         image_dir: Path to the directory containing the images.
         colmap_dir: Path to the output directory.
         camera_model: Camera model to use.
         gpu: If True, use GPU.
         verbose: If True, logs the output of the command.
         matching_method: Method to use for matching images.
         feature_type: Type of visual features to use.
         matcher_type: Type of feature matcher to use.
         num_matched: Number of image pairs for loc.
         refine_pixsfm: If True, refine the reconstruction using pixel-perfect-sfm.
+        use_single_camera_mode: If True, uses one camera for all frames. Otherwise uses one camera per frame.
     """
     if not _HAS_HLOC:
         CONSOLE.print(
             f"[bold red]Error: To use this set of parameters ({feature_type}/{matcher_type}/hloc), "
             "you must install hloc toolbox!!"
         )
         sys.exit(1)
@@ -115,14 +117,20 @@
         retrieval_path = extract_features.main(retrieval_conf, image_dir, outputs)  # type: ignore
         if num_matched >= len(references):
             num_matched = len(references)
         pairs_from_retrieval.main(retrieval_path, sfm_pairs, num_matched=num_matched)  # type: ignore
     match_features.main(matcher_conf, sfm_pairs, features=features, matches=matches)  # type: ignore
 
     image_options = pycolmap.ImageReaderOptions(camera_model=camera_model.value)  # type: ignore
+
+    if use_single_camera_mode:  # one camera per all frames
+        camera_mode = pycolmap.CameraMode.SINGLE  # type: ignore
+    else:  # one camera per frame
+        camera_mode = pycolmap.CameraMode.PER_IMAGE  # type: ignore
+
     if refine_pixsfm:
         sfm = PixSfM(  # type: ignore
             conf={
                 "dense_features": {"use_cache": True},
                 "KA": {"dense_features": {"use_cache": True}, "max_kps_per_problem": 1000},
                 "BA": {"strategy": "costmaps"},
             }
@@ -130,24 +138,24 @@
         refined, _ = sfm.reconstruction(
             sfm_dir,
             image_dir,
             sfm_pairs,
             features,
             matches,
             image_list=references,
-            camera_mode=pycolmap.CameraMode.SINGLE,  # type: ignore
+            camera_mode=camera_mode,  # type: ignore
             image_options=image_options,
             verbose=verbose,
         )
         print("Refined", refined.summary())
 
     else:
         reconstruction.main(  # type: ignore
             sfm_dir,
             image_dir,
             sfm_pairs,
             features,
             matches,
-            camera_mode=pycolmap.CameraMode.SINGLE,  # type: ignore
+            camera_mode=camera_mode,  # type: ignore
             image_options=image_options,
             verbose=verbose,
         )
```

### Comparing `nerfstudio-1.0.3/nerfstudio/process_data/images_to_nerfstudio_dataset.py` & `nerfstudio-1.1.0/nerfstudio/process_data/images_to_nerfstudio_dataset.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/process_data/metashape_utils.py` & `nerfstudio-1.1.0/nerfstudio/process_data/metashape_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,17 +13,18 @@
 # limitations under the License.
 
 """Helper utils for processing metashape data into the nerfstudio format."""
 
 import json
 import xml.etree.ElementTree as ET
 from pathlib import Path
-from typing import Dict, List
+from typing import Dict, List, Optional
 
 import numpy as np
+import open3d as o3d
 
 from nerfstudio.process_data.process_data_utils import CAMERA_MODELS
 from nerfstudio.utils.rich_utils import CONSOLE
 
 
 def _find_param(calib_xml: ET.Element, param_name: str):
     param = calib_xml.find(param_name)
@@ -32,39 +33,40 @@
     return 0.0
 
 
 def metashape_to_json(
     image_filename_map: Dict[str, Path],
     xml_filename: Path,
     output_dir: Path,
+    ply_filename: Optional[Path] = None,  # type: ignore
     verbose: bool = False,
 ) -> List[str]:
     """Convert Metashape data into a nerfstudio dataset.
 
     Args:
         image_filename_map: Mapping of original image filenames to their saved locations.
         xml_filename: Path to the metashape cameras xml file.
         output_dir: Path to the output directory.
+        ply_filename: Path to the exported ply file.
         verbose: Whether to print verbose output.
 
     Returns:
         Summary of the conversion.
     """
 
     xml_tree = ET.parse(xml_filename)
     root = xml_tree.getroot()
     chunk = root[0]
     sensors = chunk.find("sensors")
 
-    # TODO Add support for per-frame intrinsics
     if sensors is None:
         raise ValueError("No sensors found")
 
     calibrated_sensors = [
-        sensor for sensor in sensors if sensor.get("type") == "spherical" or sensor.find("calibration")
+        sensor for sensor in sensors.iter("sensor") if sensor.get("type") == "spherical" or sensor.find("calibration")
     ]
     if not calibrated_sensors:
         raise ValueError("No calibrated sensor found in Metashape XML")
     sensor_type = [s.get("type") for s in calibrated_sensors]
     if sensor_type.count(sensor_type[0]) != len(sensor_type):
         raise ValueError(
             "All Metashape sensors do not have the same sensor type. "
@@ -112,15 +114,15 @@
             s["p2"] = _find_param(calib, "p2")
 
         sensor_dict[sensor.get("id")] = s
 
     components = chunk.find("components")
     component_dict = {}
     if components is not None:
-        for component in components:
+        for component in components.iter("component"):
             transform = component.find("transform")
             if transform is not None:
                 rotation = transform.find("rotation")
                 if rotation is None:
                     r = np.eye(3)
                 else:
                     assert isinstance(rotation.text, str)
@@ -143,23 +145,25 @@
                 m[:3, 3] = t / s
                 component_dict[component.get("id")] = m
 
     frames = []
     cameras = chunk.find("cameras")
     assert cameras is not None, "Cameras not found in Metashape xml"
     num_skipped = 0
-    for camera in cameras:
+    for camera in cameras.iter("camera"):
         frame = {}
         camera_label = camera.get("label")
         assert isinstance(camera_label, str)
         if camera_label not in image_filename_map:
             # Labels sometimes have a file extension. Try without the extension.
             # (maybe it's just a '.' in the image name)
             camera_label = camera_label.split(".")[0]  # type: ignore
             if camera_label not in image_filename_map:
+                if verbose:
+                    CONSOLE.print(f"Missing image for {camera.get('label')}, Skipping")
                 continue
         frame["file_path"] = image_filename_map[camera_label].as_posix()
 
         sensor_id = camera.get("sensor_id")
         if sensor_id not in sensor_dict:
             # this should only happen when we have a sensor that doesn't have calibration
             if verbose:
@@ -176,25 +180,42 @@
             continue
         transform = np.array([float(x) for x in camera.find("transform").text.split()]).reshape((4, 4))  # type: ignore
 
         component_id = camera.get("component_id")
         if component_id in component_dict:
             transform = component_dict[component_id] @ transform
 
+        # Metashape camera is looking towards -Z, +X is to the right and +Y is to the top/up of the first cam
+        # Rotate the scene according to nerfstudio convention
         transform = transform[[2, 0, 1, 3], :]
+        # Convert from Metashape's camera coordinate system (OpenCV) to ours (OpenGL)
         transform[:, 1:3] *= -1
         frame["transform_matrix"] = transform.tolist()
         frames.append(frame)
 
     data["frames"] = frames
+    applied_transform = np.eye(4)[:3, :]
+    applied_transform = applied_transform[np.array([2, 0, 1]), :]
+    data["applied_transform"] = applied_transform.tolist()
+
+    summary = []
+
+    if ply_filename is not None:
+        assert ply_filename.exists()
+        pc = o3d.io.read_point_cloud(str(ply_filename))
+        points3D = np.asarray(pc.points)
+        points3D = np.einsum("ij,bj->bi", applied_transform[:3, :3], points3D) + applied_transform[:3, 3]
+        pc.points = o3d.utility.Vector3dVector(points3D)
+        o3d.io.write_point_cloud(str(output_dir / "sparse_pc.ply"), pc)
+        data["ply_file_path"] = "sparse_pc.ply"
+        summary.append(f"Imported {ply_filename} as starting points")
 
     with open(output_dir / "transforms.json", "w", encoding="utf-8") as f:
         json.dump(data, f, indent=4)
 
-    summary = []
     if num_skipped == 1:
         summary.append(f"{num_skipped} image skipped because it was missing its camera pose.")
     if num_skipped > 1:
         summary.append(f"{num_skipped} images were skipped because they were missing camera poses.")
 
     summary.append(f"Final dataset is {len(data['frames'])} frames.")
```

### Comparing `nerfstudio-1.0.3/nerfstudio/process_data/odm_utils.py` & `nerfstudio-1.1.0/nerfstudio/process_data/odm_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,15 +132,15 @@
             s[p] = camera[p]
 
         sensor_dict[camera_id] = s
 
     shots_dict = {}
     reconstruction = None
 
-    if reconstruction_file.exists:
+    if reconstruction_file.exists():
         reconstruction = get_reconstruction(reconstruction_file)
         shots = reconstruction.get("shots", [])
         for filename in shots:
             shot = shots[filename]
             rotation = rodrigues_vec_to_rotation_mat(np.array(shot["rotation"]))
             translation = np.array(shot["translation"]).reshape(3, 1)
```

### Comparing `nerfstudio-1.0.3/nerfstudio/process_data/process_data_utils.py` & `nerfstudio-1.1.0/nerfstudio/process_data/process_data_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/process_data/realitycapture_utils.py` & `nerfstudio-1.1.0/nerfstudio/process_data/realitycapture_utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,31 +12,34 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Helper utils for processing reality capture data into the nerfstudio format."""
 
 import csv
 import json
+import shutil
 from pathlib import Path
-from typing import Dict, List
+from typing import Dict, List, Optional
 
 import numpy as np
 from PIL import Image
 
 from nerfstudio.process_data.process_data_utils import CAMERA_MODELS
 from nerfstudio.utils.rich_utils import CONSOLE
 
 
 def realitycapture_to_json(
     image_filename_map: Dict[str, Path],
     csv_filename: Path,
+    ply_filename: Optional[Path],
     output_dir: Path,
     verbose: bool = False,
 ) -> List[str]:
     """Convert RealityCapture data into a nerfstudio dataset.
+    See https://dev.epicgames.com/community/learning/knowledge-base/vzwB/capturing-reality-realitycapture-xmp-camera-math
 
     Args:
         image_filenames: List of paths to the original images.
         csv_filename: Path to the csv file containing the camera poses.
         output_dir: Path to the output directory.
         verbose: Whether to print verbose output.
 
@@ -69,38 +72,43 @@
 
         frame = {}
         img = np.array(Image.open(output_dir / image_filename_map[basename]))
         height, width, _ = img.shape
         frame["h"] = int(height)
         frame["w"] = int(width)
         frame["file_path"] = image_filename_map[basename].as_posix()
-        frame["fl_x"] = float(cameras["f"][i]) * max(width, height) / 36
-        frame["fl_y"] = float(cameras["f"][i]) * max(width, height) / 36
-        # TODO: Unclear how to get the principal point from RealityCapture, here a guess...
-        frame["cx"] = float(cameras["px"][i]) / 36.0 + width / 2.0
-        frame["cy"] = float(cameras["py"][i]) / 36.0 + height / 2.0
-        # TODO: Not sure if RealityCapture uses this distortion model
-        frame["k1"] = cameras["k1"][i]
-        frame["k2"] = cameras["k2"][i]
-        frame["k3"] = cameras["k3"][i]
-        frame["k4"] = cameras["k4"][i]
-        frame["p1"] = cameras["t1"][i]
-        frame["p2"] = cameras["t2"][i]
+        # reality capture uses the 35mm equivalent focal length
+        # See https://en.wikipedia.org/wiki/35_mm_equivalent_focal_length
+        scale = max(width, height)
+        frame["fl_x"] = float(cameras["f"][i]) * scale / 36.0
+        frame["fl_y"] = float(cameras["f"][i]) * scale / 36.0
+        frame["cx"] = float(cameras["px"][i]) * scale + width / 2.0
+        frame["cy"] = float(cameras["py"][i]) * scale + height / 2.0
+        frame["k1"] = float(cameras["k1"][i])
+        frame["k2"] = float(cameras["k2"][i])
+        frame["k3"] = float(cameras["k3"][i])
+        frame["k4"] = float(cameras["k4"][i])
+        frame["p1"] = float(cameras["t1"][i])
+        frame["p2"] = float(cameras["t2"][i])
 
         # Transform matrix to nerfstudio format. Please refer to the documentation for coordinate system conventions.
         rot = _get_rotation_matrix(-float(cameras["heading"][i]), float(cameras["pitch"][i]), float(cameras["roll"][i]))
 
         transform = np.eye(4)
         transform[:3, :3] = rot
         transform[:3, 3] = np.array([float(cameras["x"][i]), float(cameras["y"][i]), float(cameras["alt"][i])])
 
         frame["transform_matrix"] = transform.tolist()
         frames.append(frame)
     data["frames"] = frames
 
+    if ply_filename is not None:
+        shutil.copy(ply_filename, output_dir / "sparse_pc.ply")
+        data["ply_file_path"] = "sparse_pc.ply"
+
     with open(output_dir / "transforms.json", "w", encoding="utf-8") as f:
         json.dump(data, f, indent=4)
 
     summary = []
     if missing_image_data > 0:
         summary.append(f"Missing image data for {missing_image_data} cameras.")
     if len(frames) < len(image_filename_map):
```

### Comparing `nerfstudio-1.0.3/nerfstudio/process_data/record3d_utils.py` & `nerfstudio-1.1.0/nerfstudio/process_data/record3d_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/process_data/video_to_nerfstudio_dataset.py` & `nerfstudio-1.1.0/nerfstudio/process_data/video_to_nerfstudio_dataset.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/scripts/__init__.py` & `nerfstudio-1.1.0/nerfstudio/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/scripts/blender/__init__.py` & `nerfstudio-1.1.0/nerfstudio/scripts/blender/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/scripts/blender/nerfstudio_blender.py` & `nerfstudio-1.1.0/nerfstudio/scripts/blender/nerfstudio_blender.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/scripts/completions/__init__.py` & `nerfstudio-1.1.0/nerfstudio/scripts/completions/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/scripts/completions/install.py` & `nerfstudio-1.1.0/nerfstudio/scripts/completions/install.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/scripts/completions/setup.zsh` & `nerfstudio-1.1.0/nerfstudio/scripts/completions/setup.zsh`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/scripts/datasets/process_nuscenes_masks.py` & `nerfstudio-1.1.0/nerfstudio/scripts/datasets/process_nuscenes_masks.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/scripts/datasets/process_project_aria.py` & `nerfstudio-1.1.0/nerfstudio/scripts/datasets/process_project_aria.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/scripts/docs/__init__.py` & `nerfstudio-1.1.0/nerfstudio/scripts/docs/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/scripts/docs/add_nb_tags.py` & `nerfstudio-1.1.0/nerfstudio/scripts/docs/add_nb_tags.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/scripts/docs/build_docs.py` & `nerfstudio-1.1.0/nerfstudio/scripts/docs/build_docs.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/scripts/downloads/__init__.py` & `nerfstudio-1.1.0/nerfstudio/scripts/downloads/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/scripts/downloads/download_data.py` & `nerfstudio-1.1.0/nerfstudio/scripts/downloads/download_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
     "Giannini-Hall",
 ]
 nerfstudio_file_ids = {
     "bww_entrance": grab_file_id("https://drive.google.com/file/d/1ylkRHtfB3n3IRLf2wplpfxzPTq7nES9I/view?usp=sharing"),
     "campanile": grab_file_id("https://drive.google.com/file/d/13aOfGJRRH05pOOk9ikYGTwqFc2L1xskU/view?usp=sharing"),
     "desolation": grab_file_id("https://drive.google.com/file/d/14IzOOQm9KBJ3kPbunQbUTHPnXnmZus-f/view?usp=sharing"),
     "library": grab_file_id("https://drive.google.com/file/d/1Hjbh_-BuaWETQExn2x2qGD74UwrFugHx/view?usp=sharing"),
-    "poster": grab_file_id("https://drive.google.com/file/d/1dmjWGXlJnUxwosN6MVooCDQe970PkD-1/view?usp=sharing"),
+    "poster": grab_file_id("https://drive.google.com/file/d/1FceQ5DX7bbTbHeL26t0x6ku56cwsRs6t/view?usp=sharing"),
     "redwoods2": grab_file_id("https://drive.google.com/file/d/1rg-4NoXT8p6vkmbWxMOY6PSG4j3rfcJ8/view?usp=sharing"),
     "storefront": grab_file_id("https://drive.google.com/file/d/16b792AguPZWDA_YC4igKCwXJqW0Tb21o/view?usp=sharing"),
     "vegetation": grab_file_id("https://drive.google.com/file/d/1wBhLQ2odycrtU39y2akVurXEAt9SsVI3/view?usp=sharing"),
     "Egypt": grab_file_id("https://drive.google.com/file/d/1YktD85afw7uitC3nPamusk0vcBdAfjlF/view?view?usp=sharing"),
     "person": grab_file_id("https://drive.google.com/file/d/1HsGMwkPu-R7oU7ySMdoo6Eppq8pKhHF3/view?view?usp=sharing"),
     "kitchen": grab_file_id("https://drive.google.com/file/d/1IRmNyNZSNFidyj93Tt5DtaEU9h6eJdi1/view?view?usp=sharing"),
     "plane": grab_file_id("https://drive.google.com/file/d/1tnv2NC2Iwz4XRYNtziUWvLJjObkZNo2D/view?view?usp=sharing"),
```

### Comparing `nerfstudio-1.0.3/nerfstudio/scripts/downloads/eyeful_tower.py` & `nerfstudio-1.1.0/nerfstudio/scripts/downloads/eyeful_tower.py`

 * *Files 0% similar despite different names*

```diff
@@ -257,14 +257,15 @@
             frames.append(frame)
 
         frames = sorted(frames, key=lambda f: f["file_path"])
 
         output["frames"] = frames
         output["train_filenames"] = split_filenames["train"]
         output["val_filenames"] = split_filenames["test"]
+        output["test_filenames"] = []
         return output
 
     @staticmethod
     def subsample_nerfstudio_transforms(transforms: dict, n: int):
         """Uniformly samples n frames from a Nerfstudio transforms.json dict.
 
         Args:
```

### Comparing `nerfstudio-1.0.3/nerfstudio/scripts/downloads/utils.py` & `nerfstudio-1.1.0/nerfstudio/scripts/downloads/utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/scripts/eval.py` & `nerfstudio-1.1.0/nerfstudio/scripts/eval.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/scripts/exporter.py` & `nerfstudio-1.1.0/nerfstudio/scripts/exporter.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,28 +18,31 @@
 
 
 from __future__ import annotations
 
 import json
 import os
 import sys
+import typing
 from collections import OrderedDict
 from dataclasses import dataclass, field
 from pathlib import Path
 from typing import List, Optional, Tuple, Union, cast
 
 import numpy as np
 import open3d as o3d
 import torch
 import tyro
 from typing_extensions import Annotated, Literal
 
 from nerfstudio.cameras.rays import RayBundle
 from nerfstudio.data.datamanagers.base_datamanager import VanillaDataManager
+from nerfstudio.data.datamanagers.full_images_datamanager import FullImageDatamanager
 from nerfstudio.data.datamanagers.parallel_datamanager import ParallelDataManager
+from nerfstudio.data.datamanagers.random_cameras_datamanager import RandomCamerasDataManager
 from nerfstudio.data.scene_box import OrientedBox
 from nerfstudio.exporter import texture_utils, tsdf_utils
 from nerfstudio.exporter.exporter_utils import collect_camera_poses, generate_point_cloud, get_mesh_from_filename
 from nerfstudio.exporter.marching_cubes import generate_mesh_with_multires_marching_cubes
 from nerfstudio.fields.sdf_field import SDFField  # noqa
 from nerfstudio.models.splatfacto import SplatfactoModel
 from nerfstudio.pipelines.base_pipeline import Pipeline, VanillaPipeline
@@ -101,20 +104,14 @@
     """Method to estimate normals with."""
     normal_output_name: str = "normals"
     """Name of the normal output."""
     depth_output_name: str = "depth"
     """Name of the depth output."""
     rgb_output_name: str = "rgb"
     """Name of the RGB output."""
-    use_bounding_box: bool = True
-    """Only query points within the bounding box"""
-    bounding_box_min: Optional[Tuple[float, float, float]] = (-1, -1, -1)
-    """Minimum of the bounding box, used if use_bounding_box is True."""
-    bounding_box_max: Optional[Tuple[float, float, float]] = (1, 1, 1)
-    """Maximum of the bounding box, used if use_bounding_box is True."""
 
     obb_center: Optional[Tuple[float, float, float]] = None
     """Center of the oriented bounding box."""
     obb_rotation: Optional[Tuple[float, float, float]] = None
     """Rotation of the oriented bounding box. Expressed as RPY Euler angles in radians"""
     obb_scale: Optional[Tuple[float, float, float]] = None
     """Scale of the oriented bounding box along each axis."""
@@ -133,15 +130,18 @@
             self.output_dir.mkdir(parents=True)
 
         _, pipeline, _, _ = eval_setup(self.load_config)
 
         validate_pipeline(self.normal_method, self.normal_output_name, pipeline)
 
         # Increase the batchsize to speed up the evaluation.
-        assert isinstance(pipeline.datamanager, (VanillaDataManager, ParallelDataManager))
+        assert isinstance(
+            pipeline.datamanager,
+            (VanillaDataManager, ParallelDataManager, FullImageDatamanager, RandomCamerasDataManager),
+        )
         assert pipeline.datamanager.train_pixel_sampler is not None
         pipeline.datamanager.train_pixel_sampler.num_rays_per_batch = self.num_rays_per_batch
 
         # Whether the normals should be estimated based on the point cloud.
         estimate_normals = self.normal_method == "open3d"
         crop_obb = None
         if self.obb_center is not None and self.obb_rotation is not None and self.obb_scale is not None:
@@ -151,17 +151,14 @@
             num_points=self.num_points,
             remove_outliers=self.remove_outliers,
             reorient_normals=self.reorient_normals,
             estimate_normals=estimate_normals,
             rgb_output_name=self.rgb_output_name,
             depth_output_name=self.depth_output_name,
             normal_output_name=self.normal_output_name if self.normal_method == "model_output" else None,
-            use_bounding_box=self.use_bounding_box,
-            bounding_box_min=self.bounding_box_min,
-            bounding_box_max=self.bounding_box_max,
             crop_obb=crop_obb,
             std_ratio=self.std_ratio,
         )
         if self.save_world_frame:
             # apply the inverse dataparser transform to the point cloud
             points = np.asarray(pcd.points)
             poses = np.eye(4, dtype=np.float32)[None, ...].repeat(points.shape[0], axis=0)[:, :3, :]
@@ -314,15 +311,18 @@
             self.output_dir.mkdir(parents=True)
 
         _, pipeline, _, _ = eval_setup(self.load_config)
 
         validate_pipeline(self.normal_method, self.normal_output_name, pipeline)
 
         # Increase the batchsize to speed up the evaluation.
-        assert isinstance(pipeline.datamanager, (VanillaDataManager, ParallelDataManager))
+        assert isinstance(
+            pipeline.datamanager,
+            (VanillaDataManager, ParallelDataManager, FullImageDatamanager, RandomCamerasDataManager),
+        )
         assert pipeline.datamanager.train_pixel_sampler is not None
         pipeline.datamanager.train_pixel_sampler.num_rays_per_batch = self.num_rays_per_batch
 
         # Whether the normals should be estimated based on the point cloud.
         estimate_normals = self.normal_method == "open3d"
         if self.obb_center is not None and self.obb_rotation is not None and self.obb_scale is not None:
             crop_obb = OrientedBox.from_params(self.obb_center, self.obb_rotation, self.obb_scale)
@@ -334,17 +334,14 @@
             num_points=self.num_points,
             remove_outliers=self.remove_outliers,
             reorient_normals=self.reorient_normals,
             estimate_normals=estimate_normals,
             rgb_output_name=self.rgb_output_name,
             depth_output_name=self.depth_output_name,
             normal_output_name=self.normal_output_name if self.normal_method == "model_output" else None,
-            use_bounding_box=self.use_bounding_box,
-            bounding_box_min=self.bounding_box_min,
-            bounding_box_max=self.bounding_box_max,
             crop_obb=crop_obb,
             std_ratio=self.std_ratio,
         )
         torch.cuda.empty_cache()
         CONSOLE.print(f"[bold green]:white_check_mark: Generated {pcd}")
 
         if self.save_point_cloud:
@@ -479,57 +476,74 @@
 
 @dataclass
 class ExportGaussianSplat(Exporter):
     """
     Export 3D Gaussian Splatting model to a .ply
     """
 
+    obb_center: Optional[Tuple[float, float, float]] = None
+    """Center of the oriented bounding box."""
+    obb_rotation: Optional[Tuple[float, float, float]] = None
+    """Rotation of the oriented bounding box. Expressed as RPY Euler angles in radians"""
+    obb_scale: Optional[Tuple[float, float, float]] = None
+    """Scale of the oriented bounding box along each axis."""
+
     @staticmethod
-    def write_ply(filename: str, count: int, map_to_tensors: OrderedDict[str, np.ndarray]):
+    def write_ply(
+        filename: str,
+        count: int,
+        map_to_tensors: typing.OrderedDict[str, np.ndarray],
+    ):
         """
-        Writes a PLY file with given vertex properties and their float values in the order specified by the OrderedDict.
+        Writes a PLY file with given vertex properties and a tensor of float or uint8 values in the order specified by the OrderedDict.
         Note: All float values will be converted to float32 for writing.
 
         Parameters:
         filename (str): The name of the file to write.
         count (int): The number of vertices to write.
-        map_to_tensors (OrderedDict[str, np.ndarray]): An ordered dictionary mapping property names to numpy arrays of float values.
+        map_to_tensors (OrderedDict[str, np.ndarray]): An ordered dictionary mapping property names to numpy arrays of float or uint8 values.
             Each array should be 1-dimensional and of equal length matching 'count'. Arrays should not be empty.
         """
 
         # Ensure count matches the length of all tensors
         if not all(len(tensor) == count for tensor in map_to_tensors.values()):
             raise ValueError("Count does not match the length of all tensors")
 
-        # Type check for numpy arrays of type float and non-empty
+        # Type check for numpy arrays of type float or uint8 and non-empty
         if not all(
-            isinstance(tensor, np.ndarray) and tensor.dtype.kind in ["f", "d"] and tensor.size > 0
+            isinstance(tensor, np.ndarray)
+            and (tensor.dtype.kind == "f" or tensor.dtype == np.uint8)
+            and tensor.size > 0
             for tensor in map_to_tensors.values()
         ):
-            raise ValueError("All tensors must be numpy arrays of float type and not empty")
+            raise ValueError("All tensors must be numpy arrays of float or uint8 type and not empty")
 
         with open(filename, "wb") as ply_file:
             # Write PLY header
             ply_file.write(b"ply\n")
             ply_file.write(b"format binary_little_endian 1.0\n")
 
             ply_file.write(f"element vertex {count}\n".encode())
 
             # Write properties, in order due to OrderedDict
-            for key in map_to_tensors.keys():
-                ply_file.write(f"property float {key}\n".encode())
+            for key, tensor in map_to_tensors.items():
+                data_type = "float" if tensor.dtype.kind == "f" else "uchar"
+                ply_file.write(f"property {data_type} {key}\n".encode())
 
             ply_file.write(b"end_header\n")
 
             # Write binary data
-            # Note: If this is a perfromance bottleneck consider using numpy.hstack for efficiency improvement
+            # Note: If this is a performance bottleneck consider using numpy.hstack for efficiency improvement
             for i in range(count):
                 for tensor in map_to_tensors.values():
                     value = tensor[i]
-                    ply_file.write(np.float32(value).tobytes())
+                    if tensor.dtype.kind == "f":
+                        ply_file.write(np.float32(value).tobytes())
+                    elif tensor.dtype == np.uint8:
+                        ply_file.write(value.tobytes())
 
     def main(self) -> None:
         if not self.output_dir.exists():
             self.output_dir.mkdir(parents=True)
 
         _, pipeline, _, _ = eval_setup(self.load_config)
 
@@ -573,14 +587,24 @@
             for i in range(3):
                 map_to_tensors[f"scale_{i}"] = scales[:, i, None]
 
             quats = model.quats.data.cpu().numpy()
             for i in range(4):
                 map_to_tensors[f"rot_{i}"] = quats[:, i, None]
 
+            if self.obb_center is not None and self.obb_rotation is not None and self.obb_scale is not None:
+                crop_obb = OrientedBox.from_params(self.obb_center, self.obb_rotation, self.obb_scale)
+                assert crop_obb is not None
+                mask = crop_obb.within(torch.from_numpy(positions)).numpy()
+                for k, t in map_to_tensors.items():
+                    map_to_tensors[k] = map_to_tensors[k][mask]
+
+                n = map_to_tensors["x"].shape[0]
+                count = n
+
         # post optimization, it is possible have NaN/Inf values in some attributes
         # to ensure the exported ply file has finite values, we enforce finite filters.
         select = np.ones(n, dtype=bool)
         for k, t in map_to_tensors.items():
             n_before = np.sum(select)
             select = np.logical_and(select, np.isfinite(t).all(axis=-1))
             n_after = np.sum(select)
```

### Comparing `nerfstudio-1.0.3/nerfstudio/scripts/github/__init__.py` & `nerfstudio-1.1.0/nerfstudio/scripts/github/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/scripts/github/run_actions.py` & `nerfstudio-1.1.0/nerfstudio/scripts/github/run_actions.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     success = True
 
     for step in steps:
         if "name" in step and step["name"] in LOCAL_TESTS:
             curr_command = step["run"].replace("\n", ";").replace("\\", "")
             if curr_command.startswith("ruff"):
                 if "ruff check" in curr_command:
-                    curr_command = f"{curr_command} --fix"
+                    curr_command = curr_command.replace("ruff check", "ruff check --fix")
 
                 curr_command = curr_command.replace(" --check", "")
                 curr_command = curr_command.replace(" --diff", "")
                 curr_command = curr_command.replace(" --output-format=github", "")
 
             CONSOLE.line()
             CONSOLE.rule(f"[bold green]Running: {curr_command}")
```

### Comparing `nerfstudio-1.0.3/nerfstudio/scripts/process_data.py` & `nerfstudio-1.1.0/nerfstudio/scripts/process_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,20 +11,19 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 #!/usr/bin/env python
 """Processes a video or image sequence to a nerfstudio compatible dataset."""
 
-
 import sys
 import zipfile
 from dataclasses import dataclass
 from pathlib import Path
-from typing import Union
+from typing import Optional, Union
 
 import numpy as np
 import tyro
 from typing_extensions import Annotated
 
 from nerfstudio.process_data import (
     metashape_utils,
@@ -197,14 +196,15 @@
             )
             summary_log.extend(depth_processing_log)
 
         summary_log.extend(
             polycam_utils.polycam_to_json(
                 image_filenames=polycam_image_filenames,
                 depth_filenames=polycam_depth_filenames,
+                glb_filename=self.data / "raw.glb" if (self.data / "raw.glb").exists() else None,
                 cameras_dir=polycam_cameras_dir,
                 output_dir=self.output_dir,
                 min_blur_score=self.min_blur_score,
                 crop_border_pixels=self.crop_border_pixels,
             )
         )
 
@@ -226,37 +226,49 @@
 @dataclass
 class ProcessMetashape(BaseConverterToNerfstudioDataset, _NoDefaultProcessMetashape):
     """Process Metashape data into a nerfstudio dataset.
 
     This script assumes that cameras have been aligned using Metashape. After alignment, it is necessary to export the
     camera poses as a `.xml` file. This option can be found under `File > Export > Export Cameras`.
 
+    Additionally, the points can be exported as pointcloud under `File > Export > Export Point Cloud`. Make sure to
+    export the data in non-binary format and exclude the normals.
+
     This script does the following:
 
     1. Scales images to a specified size.
     2. Converts Metashape poses into the nerfstudio format.
     """
 
+    ply: Optional[Path] = None
+    """Path to the Metashape point export ply file."""
+
     num_downscales: int = 3
     """Number of times to downscale the images. Downscales by 2 each time. For example a value of 3
         will downscale the images by 2x, 4x, and 8x."""
     max_dataset_size: int = 600
     """Max number of images to train on. If the dataset has more, images will be sampled approximately evenly. If -1,
     use all images."""
 
     def main(self) -> None:
         """Process images into a nerfstudio dataset."""
 
         if self.xml.suffix != ".xml":
             raise ValueError(f"XML file {self.xml} must have a .xml extension")
-        if not self.xml.exists:
+        if not self.xml.exists():
             raise ValueError(f"XML file {self.xml} doesn't exist")
         if self.eval_data is not None:
             raise ValueError("Cannot use eval_data since cameras were already aligned with Metashape.")
 
+        if self.ply is not None:
+            if self.ply.suffix != ".ply":
+                raise ValueError(f"PLY file {self.ply} must have a .ply extension")
+            if not self.ply.exists():
+                raise ValueError(f"PLY file {self.ply} doesn't exist")
+
         self.output_dir.mkdir(parents=True, exist_ok=True)
         image_dir = self.output_dir / "images"
         image_dir.mkdir(parents=True, exist_ok=True)
 
         summary_log = []
 
         # Copy images to output directory
@@ -287,14 +299,15 @@
             CONSOLE.print("[bold red]No images found, exiting")
             sys.exit(1)
         summary_log.extend(
             metashape_utils.metashape_to_json(
                 image_filename_map=image_filename_map,
                 xml_filename=self.xml,
                 output_dir=self.output_dir,
+                ply_filename=self.ply,
                 verbose=self.verbose,
             )
         )
 
         CONSOLE.rule("[bold green]:tada: :tada: :tada: All DONE :tada: :tada: :tada:")
 
         for summary in summary_log:
@@ -319,31 +332,40 @@
 
     This script does the following:
 
     1. Scales images to a specified size.
     2. Converts RealityCapture poses into the nerfstudio format.
     """
 
+    ply: Optional[Path] = None
+    """Path to the RealityCapture exported ply file"""
+
     num_downscales: int = 3
     """Number of times to downscale the images. Downscales by 2 each time. For example a value of 3
         will downscale the images by 2x, 4x, and 8x."""
     max_dataset_size: int = 600
     """Max number of images to train on. If the dataset has more, images will be sampled approximately evenly. If -1,
     use all images."""
 
     def main(self) -> None:
         """Process images into a nerfstudio dataset."""
 
         if self.csv.suffix != ".csv":
             raise ValueError(f"CSV file {self.csv} must have a .csv extension")
-        if not self.csv.exists:
+        if not self.csv.exists():
             raise ValueError(f"CSV file {self.csv} doesn't exist")
         if self.eval_data is not None:
             raise ValueError("Cannot use eval_data since cameras were already aligned with RealityCapture.")
 
+        if self.ply is not None:
+            if self.ply.suffix != ".ply":
+                raise ValueError(f"PLY file {self.ply} must have a .ply extension")
+            if not self.ply.exists():
+                raise ValueError(f"PLY file {self.ply} doesn't exist")
+
         self.output_dir.mkdir(parents=True, exist_ok=True)
         image_dir = self.output_dir / "images"
         image_dir.mkdir(parents=True, exist_ok=True)
 
         summary_log = []
 
         # Copy images to output directory
@@ -373,15 +395,17 @@
         if num_frames == 0:
             CONSOLE.print("[bold red]No images found, exiting")
             sys.exit(1)
         summary_log.extend(
             realitycapture_utils.realitycapture_to_json(
                 image_filename_map=image_filename_map,
                 csv_filename=self.csv,
+                ply_filename=self.ply,
                 output_dir=self.output_dir,
+                verbose=self.verbose,
             )
         )
 
         CONSOLE.rule("[bold green]:tada: :tada: :tada: All DONE :tada: :tada: :tada:")
 
         for summary in summary_log:
             CONSOLE.print(summary, justify="center")
@@ -409,20 +433,20 @@
         """Process images into a nerfstudio dataset."""
 
         orig_images_dir = self.data / "images"
         cameras_file = self.data / "cameras.json"
         shots_file = self.data / "odm_report" / "shots.geojson"
         reconstruction_file = self.data / "opensfm" / "reconstruction.json"
 
-        if not shots_file.exists:
+        if not shots_file.exists():
             raise ValueError(f"shots file {shots_file} doesn't exist")
-        if not shots_file.exists:
+        if not shots_file.exists():
             raise ValueError(f"cameras file {cameras_file} doesn't exist")
 
-        if not orig_images_dir.exists:
+        if not orig_images_dir.exists():
             raise ValueError(f"Images dir {orig_images_dir} doesn't exist")
 
         if self.eval_data is not None:
             raise ValueError("Cannot use eval_data since cameras were already aligned with ODM.")
 
         self.output_dir.mkdir(parents=True, exist_ok=True)
         image_dir = self.output_dir / "images"
@@ -518,15 +542,15 @@
 
 
 def entrypoint():
     """Entrypoint for use with pyproject scripts."""
     tyro.extras.set_accent_color("bright_yellow")
     try:
         tyro.cli(Commands).main()
-    except RuntimeError as e:
+    except (RuntimeError, ValueError) as e:
         CONSOLE.log("[bold red]" + e.args[0])
 
 
 if __name__ == "__main__":
     entrypoint()
```

### Comparing `nerfstudio-1.0.3/nerfstudio/scripts/render.py` & `nerfstudio-1.1.0/nerfstudio/scripts/render.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/scripts/texture.py` & `nerfstudio-1.1.0/nerfstudio/scripts/texture.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/scripts/train.py` & `nerfstudio-1.1.0/nerfstudio/scripts/train.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/scripts/viewer/__init__.py` & `nerfstudio-1.1.0/nerfstudio/scripts/viewer/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/scripts/viewer/run_viewer.py` & `nerfstudio-1.1.0/nerfstudio/scripts/viewer/run_viewer.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,19 +12,21 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 #!/usr/bin/env python
 """
 Starts viewer in eval mode.
 """
+
 from __future__ import annotations
 
 import time
 from dataclasses import dataclass, field, fields
 from pathlib import Path
+from threading import Lock
 from typing import Literal
 
 import tyro
 
 from nerfstudio.configs.base_config import ViewerConfig
 from nerfstudio.engine.trainer import TrainerConfig
 from nerfstudio.pipelines.base_pipeline import Pipeline
@@ -85,29 +87,32 @@
         pipeline: Pipeline instance of which to load weights
         step: Step at which the pipeline was saved
     """
     base_dir = config.get_base_dir()
     viewer_log_path = base_dir / config.viewer.relative_log_filename
     banner_messages = None
     viewer_state = None
+    viewer_callback_lock = Lock()
     if config.vis == "viewer_legacy":
         viewer_state = ViewerLegacyState(
             config.viewer,
             log_filename=viewer_log_path,
             datapath=pipeline.datamanager.get_datapath(),
             pipeline=pipeline,
+            train_lock=viewer_callback_lock,
         )
         banner_messages = [f"Legacy viewer at: {viewer_state.viewer_url}"]
     if config.vis == "viewer":
         viewer_state = ViewerState(
             config.viewer,
             log_filename=viewer_log_path,
             datapath=pipeline.datamanager.get_datapath(),
             pipeline=pipeline,
             share=config.viewer.make_share_url,
+            train_lock=viewer_callback_lock,
         )
         banner_messages = viewer_state.viewer_info
 
     # We don't need logging, but writer.GLOBAL_BUFFER needs to be populated
     config.logging.local_writer.enable = False
     writer.setup_local_writer(config.logging, max_iter=config.max_num_iterations, banner_messages=banner_messages)
```

### Comparing `nerfstudio-1.0.3/nerfstudio/scripts/viewer/sync_viser_message_defs.py` & `nerfstudio-1.1.0/nerfstudio/scripts/viewer/sync_viser_message_defs.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/utils/__init__.py` & `nerfstudio-1.1.0/nerfstudio/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/utils/colormaps.py` & `nerfstudio-1.1.0/nerfstudio/utils/colormaps.py`

 * *Files 9% similar despite different names*

```diff
@@ -130,16 +130,16 @@
         far_plane: Furthest depth to consider. If None, use max image value.
         colormap: Colormap to apply.
 
     Returns:
         Colored depth image with colors in [0, 1]
     """
 
-    near_plane = near_plane or float(torch.min(depth))
-    far_plane = far_plane or float(torch.max(depth))
+    near_plane = near_plane if near_plane is not None else float(torch.min(depth))
+    far_plane = far_plane if far_plane is not None else float(torch.max(depth))
 
     depth = (depth - near_plane) / (far_plane - near_plane + 1e-10)
     depth = torch.clip(depth, 0, 1)
     # depth = torch.nan_to_num(depth, nan=0.0) # TODO(ethan): remove this
 
     colored_image = apply_colormap(depth, colormap_options=colormap_options)
 
@@ -167,43 +167,54 @@
 
     colored_image = torch.ones(image.shape[:-1] + (3,))
     colored_image[image[..., 0], :] = true_color
     colored_image[~image[..., 0], :] = false_color
     return colored_image
 
 
-def apply_pca_colormap(image: Float[Tensor, "*bs dim"]) -> Float[Tensor, "*bs rgb=3"]:
+def apply_pca_colormap(
+    image: Float[Tensor, "*bs dim"], pca_mat: Optional[Float[Tensor, "dim rgb=3"]] = None, ignore_zeros=True
+) -> Float[Tensor, "*bs rgb=3"]:
     """Convert feature image to 3-channel RGB via PCA. The first three principle
     components are used for the color channels, with outlier rejection per-channel
 
     Args:
         image: image of arbitrary vectors
+        pca_mat: an optional argument of the PCA matrix, shape (dim, 3)
+        ignore_zeros: whether to ignore zero values in the input image (they won't affect the PCA computation)
 
     Returns:
         Tensor: Colored image
     """
     original_shape = image.shape
     image = image.view(-1, image.shape[-1])
-    _, _, v = torch.pca_lowrank(image)
-    image = torch.matmul(image, v[..., :3])
-    d = torch.abs(image - torch.median(image, dim=0).values)
+    if ignore_zeros:
+        valids = (image.abs().amax(dim=-1)) > 0
+    else:
+        valids = torch.ones(image.shape[0], dtype=torch.bool)
+
+    if pca_mat is None:
+        _, _, pca_mat = torch.pca_lowrank(image[valids, :], q=3, niter=20)
+    assert pca_mat is not None
+    image = torch.matmul(image, pca_mat[..., :3])
+    d = torch.abs(image[valids, :] - torch.median(image[valids, :], dim=0).values)
     mdev = torch.median(d, dim=0).values
     s = d / mdev
-    m = 3.0  # this is a hyperparam controlling how many std dev outside for outliers
-    rins = image[s[:, 0] < m, 0]
-    gins = image[s[:, 1] < m, 1]
-    bins = image[s[:, 2] < m, 2]
-
-    image[:, 0] -= rins.min()
-    image[:, 1] -= gins.min()
-    image[:, 2] -= bins.min()
-
-    image[:, 0] /= rins.max() - rins.min()
-    image[:, 1] /= gins.max() - gins.min()
-    image[:, 2] /= bins.max() - bins.min()
+    m = 2.0  # this is a hyperparam controlling how many std dev outside for outliers
+    rins = image[valids, :][s[:, 0] < m, 0]
+    gins = image[valids, :][s[:, 1] < m, 1]
+    bins = image[valids, :][s[:, 2] < m, 2]
+
+    image[valids, 0] -= rins.min()
+    image[valids, 1] -= gins.min()
+    image[valids, 2] -= bins.min()
+
+    image[valids, 0] /= rins.max() - rins.min()
+    image[valids, 1] /= gins.max() - gins.min()
+    image[valids, 2] /= bins.max() - bins.min()
 
     image = torch.clamp(image, 0, 1)
     image_long = (image * 255).long()
     image_long_min = torch.min(image_long)
     image_long_max = torch.max(image_long)
     assert image_long_min >= 0, f"the min value is {image_long_min}"
     assert image_long_max <= 255, f"the max value is {image_long_max}"
```

### Comparing `nerfstudio-1.0.3/nerfstudio/utils/colors.py` & `nerfstudio-1.1.0/nerfstudio/utils/colors.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/utils/comms.py` & `nerfstudio-1.1.0/nerfstudio/utils/comms.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/utils/decorators.py` & `nerfstudio-1.1.0/nerfstudio/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/utils/eval_utils.py` & `nerfstudio-1.1.0/nerfstudio/utils/eval_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/utils/external.py` & `nerfstudio-1.1.0/nerfstudio/utils/external.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/utils/install_checks.py` & `nerfstudio-1.1.0/nerfstudio/utils/install_checks.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/utils/io.py` & `nerfstudio-1.1.0/nerfstudio/utils/io.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/utils/math.py` & `nerfstudio-1.1.0/nerfstudio/utils/math.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/utils/misc.py` & `nerfstudio-1.1.0/nerfstudio/utils/misc.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/utils/plotly_utils.py` & `nerfstudio-1.1.0/nerfstudio/utils/plotly_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/utils/poses.py` & `nerfstudio-1.1.0/nerfstudio/utils/poses.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/utils/printing.py` & `nerfstudio-1.1.0/nerfstudio/utils/printing.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/utils/profiler.py` & `nerfstudio-1.1.0/nerfstudio/utils/profiler.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/utils/rich_utils.py` & `nerfstudio-1.1.0/nerfstudio/utils/rich_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/utils/scripts.py` & `nerfstudio-1.1.0/nerfstudio/utils/scripts.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/utils/tensor_dataclass.py` & `nerfstudio-1.1.0/nerfstudio/utils/tensor_dataclass.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/utils/writer.py` & `nerfstudio-1.1.0/nerfstudio/utils/writer.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/viewer/__init__.py` & `nerfstudio-1.1.0/nerfstudio/viewer/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/viewer/control_panel.py` & `nerfstudio-1.1.0/nerfstudio/viewer/control_panel.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/viewer/export_panel.py` & `nerfstudio-1.1.0/nerfstudio/viewer/export_panel.py`

 * *Files 6% similar despite different names*

```diff
@@ -69,18 +69,20 @@
         close_button = client.add_gui_button("Close")
 
         @close_button.on_click
         def _(_) -> None:
             modal.close()
 
 
-def get_crop_string(obb: OrientedBox):
+def get_crop_string(obb: OrientedBox, crop_viewport: bool):
     """Takes in an oriented bounding box and returns a string of the form "--obb_{center,rotation,scale}
     and each arg formatted with spaces around it
     """
+    if not crop_viewport:
+        return ""
     rpy = vtf.SO3.from_matrix(obb.R.numpy(force=True)).as_rpy_radians()
     pos = obb.T.squeeze().tolist()
     scale = obb.S.squeeze().tolist()
     rpystring = " ".join([f"{x:.10f}" for x in rpy])
     posstring = " ".join([f"{x:.10f}" for x in pos])
     scalestring = " ".join([f"{x:.10f}" for x in scale])
     return f"--obb_center {posstring} --obb_rotation {rpystring} --obb_scale {scalestring}"
@@ -121,17 +123,16 @@
                 [
                     "ns-export pointcloud",
                     f"--load-config {config_path}",
                     f"--output-dir {output_dir.value}",
                     f"--num-points {num_points.value}",
                     f"--remove-outliers {remove_outliers.value}",
                     f"--normal-method {normals.value}",
-                    f"--use_bounding_box {control_panel.crop_viewport}",
                     f"--save-world-frame {world_frame.value}",
-                    get_crop_string(control_panel.crop_obb),
+                    get_crop_string(control_panel.crop_obb, control_panel.crop_viewport),
                 ]
             )
             show_command_modal(event.client, "point cloud", command)
 
     else:
         server.add_gui_markdown("<small>Point cloud export is not currently supported with Gaussian Splatting</small>")
 
@@ -170,16 +171,15 @@
                     f"--load-config {config_path}",
                     f"--output-dir {output_directory.value}",
                     f"--target-num-faces {num_faces.value}",
                     f"--num-pixels-per-side {texture_resolution.value}",
                     f"--num-points {num_points.value}",
                     f"--remove-outliers {remove_outliers.value}",
                     f"--normal-method {normals.value}",
-                    f"--use_bounding_box {control_panel.crop_viewport}",
-                    get_crop_string(control_panel.crop_obb),
+                    get_crop_string(control_panel.crop_obb, control_panel.crop_viewport),
                 ]
             )
             show_command_modal(event.client, "mesh", command)
 
     else:
         server.add_gui_markdown("<small>Mesh export is not currently supported with Gaussian Splatting</small>")
 
@@ -200,13 +200,14 @@
         def _(event: viser.GuiEvent) -> None:
             assert event.client is not None
             command = " ".join(
                 [
                     "ns-export gaussian-splat",
                     f"--load-config {config_path}",
                     f"--output-dir {output_directory.value}",
+                    get_crop_string(control_panel.crop_obb, control_panel.crop_viewport),
                 ]
             )
             show_command_modal(event.client, "splat", command)
 
     else:
         server.add_gui_markdown("<small>Splat export is only supported with Gaussian Splatting methods</small>")
```

### Comparing `nerfstudio-1.0.3/nerfstudio/viewer/render_panel.py` & `nerfstudio-1.1.0/nerfstudio/viewer/render_panel.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/viewer/render_state_machine.py` & `nerfstudio-1.1.0/nerfstudio/viewer/render_state_machine.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,15 +175,17 @@
                 if isinstance(self.viewer.get_model(), SplatfactoModel):
                     # Gaussians render much faster than we can send depth images, so we do some downsampling.
                     assert len(outputs["depth"].shape) == 3
                     assert outputs["depth"].shape[-1] == 1
 
                     desired_depth_pixels = {"low_move": 128, "low_static": 128, "high": 512}[self.state] ** 2
                     current_depth_pixels = outputs["depth"].shape[0] * outputs["depth"].shape[1]
-                    scale = min(desired_depth_pixels / current_depth_pixels, 1.0)
+
+                    # from the panel of ns-viewer, it is possible for user to enter zero resolution
+                    scale = min(desired_depth_pixels / max(1, current_depth_pixels), 1.0)
 
                     outputs["gl_z_buf_depth"] = F.interpolate(
                         outputs["depth"].squeeze(dim=-1)[None, None, ...],
                         size=(int(outputs["depth"].shape[0] * scale), int(outputs["depth"].shape[1] * scale)),
                         mode="bilinear",
                     )[0, 0, :, :, None]
                 else:
```

### Comparing `nerfstudio-1.0.3/nerfstudio/viewer/server/__init__.py` & `nerfstudio-1.1.0/nerfstudio/viewer/server/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/viewer/server/viewer_elements.py` & `nerfstudio-1.1.0/nerfstudio/viewer/server/viewer_elements.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/viewer/utils.py` & `nerfstudio-1.1.0/nerfstudio/viewer/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 from dataclasses import dataclass
-from typing import Any, List, Literal, Optional, Tuple, Union
+from functools import cached_property
+from typing import Any, List, Literal, Optional, Tuple, Type, Union
 
 import numpy as np
 import torch
 from jaxtyping import Float
 from torch import nn
 
 from nerfstudio.cameras.cameras import Cameras, CameraType
@@ -105,15 +106,15 @@
             model.render_aabb = SceneBox(aabb=torch.stack([crop_min_tensor, crop_max_tensor], dim=0))
     else:
         model.render_aabb = None
 
 
 def parse_object(
     obj: Any,
-    type_check,
+    type_check: Type[Any],
     tree_stub: str,
 ) -> List[Tuple[str, Any]]:
     """
     obj: the object to parse
     type_check: recursively adds instances of this type to the output
     tree_stub: the path down the object tree to this object
 
@@ -134,15 +135,16 @@
                 return
         ret.append((ts, v))
 
     if not hasattr(obj, "__dict__"):
         return []
     ret = []
     # get a list of the properties of the object, sorted by whether things are instances of type_check
-    obj_props = [(k, getattr(obj, k)) for k in dir(obj)]
+    # we skip cached properties, which can be expensive to call `getattr()` on!
+    obj_props = [(k, getattr(obj, k)) for k in dir(obj) if not isinstance(getattr(type(obj), k, None), cached_property)]
     for k, v in obj_props:
         if k[0] == "_":
             continue
         new_tree_stub = f"{tree_stub}/{k}"
         if isinstance(v, type_check):
             add(ret, new_tree_stub, v)
         elif isinstance(v, nn.Module):
```

### Comparing `nerfstudio-1.0.3/nerfstudio/viewer/viewer.py` & `nerfstudio-1.1.0/nerfstudio/viewer/viewer.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,17 +8,19 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-""" Manage the state of the viewer """
+"""Manage the state of the viewer"""
+
 from __future__ import annotations
 
+import contextlib
 import threading
 import time
 from pathlib import Path
 from typing import TYPE_CHECKING, Dict, List, Literal, Optional
 
 import numpy as np
 import torch
@@ -205,20 +207,30 @@
 
         with tabs.add_tab("Export", viser.Icon.PACKAGE_EXPORT):
             populate_export_tab(self.viser_server, self.control_panel, config_path, self.pipeline.model)
 
         # Keep track of the pointers to generated GUI folders, because each generated folder holds a unique ID.
         viewer_gui_folders = dict()
 
+        def prev_cb_wrapper(prev_cb):
+            # We wrap the callbacks in the train_lock so that the callbacks are thread-safe with the
+            # concurrently executing render thread. This may block rendering, however this can be necessary
+            # if the callback uses get_outputs internally.
+            def cb_lock(element):
+                with self.train_lock if self.train_lock is not None else contextlib.nullcontext():
+                    prev_cb(element)
+
+            return cb_lock
+
         def nested_folder_install(folder_labels: List[str], prev_labels: List[str], element: ViewerElement):
             if len(folder_labels) == 0:
                 element.install(self.viser_server)
                 # also rewire the hook to rerender
                 prev_cb = element.cb_hook
-                element.cb_hook = lambda element: [prev_cb(element), self._trigger_rerender()]
+                element.cb_hook = lambda element: [prev_cb_wrapper(prev_cb)(element), self._trigger_rerender()]
             else:
                 # recursively create folders
                 # If the folder name is "Custom Elements/a/b", then:
                 #   in the beginning: folder_path will be
                 #       "/".join([] + ["Custom Elements"]) --> "Custom Elements"
                 #   later, folder_path will be
                 #       "/".join(["Custom Elements"] + ["a"]) --> "Custom Elements/a"
```

### Comparing `nerfstudio-1.0.3/nerfstudio/viewer/viewer_elements.py` & `nerfstudio-1.1.0/nerfstudio/viewer/viewer_elements.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 
 from __future__ import annotations
 
 import warnings
 from abc import abstractmethod
 from dataclasses import dataclass
-from typing import TYPE_CHECKING, Any, Callable, Generic, List, Literal, Optional, Tuple, Union
+from typing import TYPE_CHECKING, Any, Callable, Generic, List, Literal, Optional, Tuple, Union, overload
 
 import numpy as np
 import torch
 import viser.transforms as vtf
 from typing_extensions import LiteralString, TypeVar
 from viser import (
     GuiButtonGroupHandle,
@@ -162,28 +162,50 @@
         return get_camera(camera_state, img_height, img_width)
 
     def register_click_cb(self, cb: Callable):
         """Deprecated, use register_pointer_cb instead."""
         CONSOLE.log("`register_click_cb` is deprecated, use `register_pointer_cb` instead.")
         self.register_pointer_cb("click", cb)
 
+    @overload
     def register_pointer_cb(
-        self, event_type: Literal["click", "rect-select"], cb: Callable, done_cb: Optional[Callable] = None
+        self,
+        event_type: Literal["click"],
+        cb: Callable[[ViewerClick], None],
+        removed_cb: Optional[Callable[[], None]] = None,
+    ):
+        ...
+
+    @overload
+    def register_pointer_cb(
+        self,
+        event_type: Literal["rect-select"],
+        cb: Callable[[ViewerRectSelect], None],
+        removed_cb: Optional[Callable[[], None]] = None,
+    ):
+        ...
+
+    def register_pointer_cb(
+        self,
+        event_type: Literal["click", "rect-select"],
+        cb: Callable[[ViewerClick], None] | Callable[[ViewerRectSelect], None],
+        removed_cb: Optional[Callable[[], None]] = None,
     ):
         """
         Add a callback which will be called when a scene pointer event is detected in the viewer.
         Scene pointer events include:
         - "click": A click event, which includes the origin and direction of the click
         - "rect-select": A rectangle selection event, which includes the screen bounds of the box selection
 
         The callback should take a ViewerClick object as an argument if the event type is "click",
         and a ViewerRectSelect object as an argument if the event type is "rect-select".
 
         Args:
             cb: The callback to call when a click or a rect-select is detected.
+            removed_cb: The callback to run when the pointer event is removed.
         """
         from nerfstudio.viewer.viewer import VISER_NERFSTUDIO_SCALE_RATIO
 
         def wrapped_cb(scene_pointer_msg: ScenePointerEvent):
             # Check that the event type is the same as the one we are interested in.
             if scene_pointer_msg.event_type != event_type:
                 raise ValueError(f"Expected event type {event_type}, got {scene_pointer_msg.event_type}")
@@ -199,15 +221,15 @@
                 assert len(origin) == 3
                 pointer_event = ViewerClick(origin, direction, screen_pos)
             elif scene_pointer_msg.event_type == "rect-select":
                 pointer_event = ViewerRectSelect(scene_pointer_msg.screen_pos[0], scene_pointer_msg.screen_pos[1])
             else:
                 raise ValueError(f"Unknown event type: {scene_pointer_msg.event_type}")
 
-            cb(pointer_event)
+            cb(pointer_event)  # type: ignore
 
         cb_overriden = False
         with warnings.catch_warnings(record=True) as w:
             # Register the callback with the viser server.
             self.viser_server.on_scene_pointer(event_type=event_type)(wrapped_cb)
             # If there exists a warning, it's because a callback was overriden.
             cb_overriden = len(w) > 0
@@ -215,16 +237,16 @@
         if cb_overriden:
             warnings.warn(
                 "A ScenePointer callback has already been registered for this event type. "
                 "The new callback will override the existing one."
             )
 
         # If there exists a cleanup callback after the pointer event is done, register it.
-        if done_cb:
-            self.viser_server.on_scene_pointer_done(done_cb)
+        if removed_cb is not None:
+            self.viser_server.on_scene_pointer_removed(removed_cb)
 
     def unregister_click_cb(self, cb: Optional[Callable] = None):
         """Deprecated, use unregister_pointer_cb instead. `cb` is ignored."""
         warnings.warn("`unregister_click_cb` is deprecated, use `unregister_pointer_cb` instead.")
         if cb is not None:
             # raise warning
             warnings.warn("cb argument is ignored in unregister_click_cb.")
```

### Comparing `nerfstudio-1.0.3/nerfstudio/viewer_legacy/__init__.py` & `nerfstudio-1.1.0/nerfstudio/viewer_legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/viewer_legacy/app/package.json` & `nerfstudio-1.1.0/nerfstudio/viewer_legacy/app/package.json`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/viewer_legacy/app/run_deploy.py` & `nerfstudio-1.1.0/nerfstudio/viewer_legacy/app/run_deploy.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/viewer_legacy/app/src/themes/leva_theme.json` & `nerfstudio-1.1.0/nerfstudio/viewer_legacy/app/src/themes/leva_theme.json`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/viewer_legacy/server/__init__.py` & `nerfstudio-1.1.0/nerfstudio/viewer_legacy/server/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/viewer_legacy/server/control_panel.py` & `nerfstudio-1.1.0/nerfstudio/viewer_legacy/server/control_panel.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/viewer_legacy/server/gui_utils.py` & `nerfstudio-1.1.0/nerfstudio/viewer_legacy/server/gui_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/viewer_legacy/server/path.py` & `nerfstudio-1.1.0/nerfstudio/viewer_legacy/server/path.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/viewer_legacy/server/render_state_machine.py` & `nerfstudio-1.1.0/nerfstudio/viewer_legacy/server/render_state_machine.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/viewer_legacy/server/state/node.py` & `nerfstudio-1.1.0/nerfstudio/viewer_legacy/server/state/node.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/viewer_legacy/server/state/state_node.py` & `nerfstudio-1.1.0/nerfstudio/viewer_legacy/server/state/state_node.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/viewer_legacy/server/utils.py` & `nerfstudio-1.1.0/nerfstudio/viewer_legacy/server/utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/viewer_legacy/server/viewer_elements.py` & `nerfstudio-1.1.0/nerfstudio/viewer_legacy/server/viewer_elements.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/viewer_legacy/server/viewer_state.py` & `nerfstudio-1.1.0/nerfstudio/viewer_legacy/server/viewer_state.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/viewer_legacy/server/viewer_utils.py` & `nerfstudio-1.1.0/nerfstudio/viewer_legacy/server/viewer_utils.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/viewer_legacy/viser/__init__.py` & `nerfstudio-1.1.0/nerfstudio/viewer_legacy/viser/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/viewer_legacy/viser/gui.py` & `nerfstudio-1.1.0/nerfstudio/viewer_legacy/viser/gui.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/viewer_legacy/viser/message_api.py` & `nerfstudio-1.1.0/nerfstudio/viewer_legacy/viser/message_api.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/viewer_legacy/viser/messages.py` & `nerfstudio-1.1.0/nerfstudio/viewer_legacy/viser/messages.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio/viewer_legacy/viser/server.py` & `nerfstudio-1.1.0/nerfstudio/viewer_legacy/viser/server.py`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio.egg-info/PKG-INFO` & `nerfstudio-1.1.0/nerfstudio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nerfstudio
-Version: 1.0.3
+Version: 1.1.0
 Summary: All-in-one repository for state-of-the-art NeRFs
 License: Apache 2.0
 Project-URL: Documentation, https://docs.nerf.studio
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
@@ -44,21 +44,21 @@
 Requires-Dist: scikit-image>=0.19.3
 Requires-Dist: splines==0.3.0
 Requires-Dist: tensorboard>=2.13.0
 Requires-Dist: torch>=1.13.1
 Requires-Dist: torchvision>=0.14.1
 Requires-Dist: torchmetrics[image]>=1.0.1
 Requires-Dist: typing_extensions>=4.4.0
-Requires-Dist: viser==0.1.26
+Requires-Dist: viser==0.1.27
 Requires-Dist: nuscenes-devkit>=1.1.1
 Requires-Dist: wandb>=0.13.3
 Requires-Dist: xatlas
 Requires-Dist: trimesh>=3.20.2
 Requires-Dist: timm==0.6.7
-Requires-Dist: gsplat>=0.1.9
+Requires-Dist: gsplat>=0.1.11
 Requires-Dist: pytorch-msssim
 Requires-Dist: pathos
 Requires-Dist: packaging
 Provides-Extra: gen
 Requires-Dist: diffusers==0.16.1; extra == "gen"
 Requires-Dist: transformers==4.29.2; extra == "gen"
 Requires-Dist: accelerate==0.19.0; extra == "gen"
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nerfstudio Version: 1.0.3 Summary: All-in-one
+Metadata-Version: 2.1 Name: nerfstudio Version: 1.1.0 Summary: All-in-one
 repository for state-of-the-art NeRFs License: Apache 2.0 Project-URL:
 Documentation, https://docs.nerf.studio Classifier: Development Status :: 3 -
 Alpha Classifier: Programming Language :: Python Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 appdirs>=1.4 Requires-Dist: av>=9.2.0 Requires-Dist: awscli>=1.31.10 Requires-
 Dist: comet_ml>=3.33.8 Requires-Dist: cryptography>=38 Requires-Dist:
 tyro>=0.6.6 Requires-Dist: gdown>=4.6.0 Requires-Dist: ninja>=1.10 Requires-
@@ -18,17 +18,17 @@
 "aarch64" Requires-Dist: pyngrok>=5.1.0 Requires-Dist: python-socketio>=5.7.1
 Requires-Dist: pyquaternion>=0.9.9 Requires-Dist: rawpy>=0.18.1;
 platform_machine != "arm64" Requires-Dist: newrawpy>=1.0.0b0; platform_machine
 == "arm64" Requires-Dist: requests Requires-Dist: rich>=12.5.1 Requires-Dist:
 scikit-image>=0.19.3 Requires-Dist: splines==0.3.0 Requires-Dist:
 tensorboard>=2.13.0 Requires-Dist: torch>=1.13.1 Requires-Dist:
 torchvision>=0.14.1 Requires-Dist: torchmetrics[image]>=1.0.1 Requires-Dist:
-typing_extensions>=4.4.0 Requires-Dist: viser==0.1.26 Requires-Dist: nuscenes-
+typing_extensions>=4.4.0 Requires-Dist: viser==0.1.27 Requires-Dist: nuscenes-
 devkit>=1.1.1 Requires-Dist: wandb>=0.13.3 Requires-Dist: xatlas Requires-Dist:
-trimesh>=3.20.2 Requires-Dist: timm==0.6.7 Requires-Dist: gsplat>=0.1.9
+trimesh>=3.20.2 Requires-Dist: timm==0.6.7 Requires-Dist: gsplat>=0.1.11
 Requires-Dist: pytorch-msssim Requires-Dist: pathos Requires-Dist: packaging
 Provides-Extra: gen Requires-Dist: diffusers==0.16.1; extra == "gen" Requires-
 Dist: transformers==4.29.2; extra == "gen" Requires-Dist: accelerate==0.19.0;
 extra == "gen" Requires-Dist: bitsandbytes==0.39.0; extra == "gen" Requires-
 Dist: sentencepiece==0.1.99; extra == "gen" Provides-Extra: dev Requires-Dist:
 pre-commit==3.3.2; extra == "dev" Requires-Dist: pytest==7.1.2; extra == "dev"
 Requires-Dist: pytest-xdist==2.5.0; extra == "dev" Requires-Dist:
```

### Comparing `nerfstudio-1.0.3/nerfstudio.egg-info/SOURCES.txt` & `nerfstudio-1.1.0/nerfstudio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio.egg-info/entry_points.txt` & `nerfstudio-1.1.0/nerfstudio.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `nerfstudio-1.0.3/nerfstudio.egg-info/requires.txt` & `nerfstudio-1.1.0/nerfstudio.egg-info/requires.txt`

 * *Files 5% similar despite different names*

```diff
@@ -29,21 +29,21 @@
 scikit-image>=0.19.3
 splines==0.3.0
 tensorboard>=2.13.0
 torch>=1.13.1
 torchvision>=0.14.1
 torchmetrics[image]>=1.0.1
 typing_extensions>=4.4.0
-viser==0.1.26
+viser==0.1.27
 nuscenes-devkit>=1.1.1
 wandb>=0.13.3
 xatlas
 trimesh>=3.20.2
 timm==0.6.7
-gsplat>=0.1.9
+gsplat>=0.1.11
 pytorch-msssim
 pathos
 packaging
 
 [:platform_machine != "arm64"]
 rawpy>=0.18.1
```

### Comparing `nerfstudio-1.0.3/pyproject.toml` & `nerfstudio-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nerfstudio"
-version = "1.0.3"
+version = "1.1.0"
 description = "All-in-one repository for state-of-the-art NeRFs"
 readme = "README.md"
 license = { text="Apache 2.0"}
 requires-python = ">=3.8.0"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python",
@@ -53,21 +53,21 @@
     "scikit-image>=0.19.3",
     "splines==0.3.0",
     "tensorboard>=2.13.0",
     "torch>=1.13.1",
     "torchvision>=0.14.1",
     "torchmetrics[image]>=1.0.1",
     "typing_extensions>=4.4.0",
-    "viser==0.1.26",
+    "viser==0.1.27",
     "nuscenes-devkit>=1.1.1",
     "wandb>=0.13.3",
     "xatlas",
     "trimesh>=3.20.2",
     "timm==0.6.7",
-    "gsplat>=0.1.9",
+    "gsplat>=0.1.11",
     "pytorch-msssim",
     "pathos",
     "packaging"
 ]
 
 [project.urls]
 "Documentation" = "https://docs.nerf.studio"
```

### Comparing `nerfstudio-1.0.3/tests/test_train.py` & `nerfstudio-1.1.0/tests/test_train.py`

 * *Files identical despite different names*

